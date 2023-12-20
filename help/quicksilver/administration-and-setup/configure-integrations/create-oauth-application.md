---
title: 用の OAuth2 アプリケーションの作成 [!DNL Workfront] 統合
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: As an [!DNL Adobe Workfront] 管理者は、のインスタンス用に OAuth2 アプリケーションを作成できます。 [!DNL Workfront]：他のアプリケーションがWorkfrontにアクセスできるようにします。 その後、ユーザーは、他のアプリケーションに対し、Workfrontデータへのアクセス権を付与できます。 この方法で、Workfrontを、独自の社内アプリケーションを含む、任意のアプリケーションと統合できます。
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: 762053edbf490532b96285a6d1edff2af49500a4
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 6%

---

# 用の OAuth2 アプリケーションの作成 [!DNL Workfront] 統合

As an [!DNL Adobe Workfront] 管理者は、のインスタンス用に OAuth2 アプリケーションを作成できます。 [!DNL Workfront]（他のアプリケーションがにアクセスできるようにする） [!DNL Workfront]. その後、ユーザーは他のアプリケーションに対し、そのアプリケーションへのアクセス権を付与できます [!DNL Workfront] データ。 この方法で、自社のアプリケーションを含む、任意のアプリケーションと統合できます。

以下を作成する場合、 [!UICONTROL OAuth2] アプリケーションで、クライアント ID とクライアント秘密鍵を生成します。 その後、ユーザーは API 呼び出しでクライアント ID を使用して、作成したアプリケーションと統合できます。

>[!NOTE]
>
>OAuth2 のコンテキストでは、「アプリの作成」とは、アプリとサーバーの間に、次のようなアクセスリンクを作成するプロセスを指します。 [!DNL Workfront].

* ユーザー資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、 [認証コードフローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-code-token-flow.md).
* サーバー認証（JWT フロー）を使用した OAuth2 アプリケーションの設定と使用の手順については、 [JWT フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE を使用して OAuth2 アプリケーションを設定および使用する手順については、 [PKCE フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-pkce-flow.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td><p>新規： [!UICONTROL Standard]</p>
   または
   <p>現在：[!UICONTROL プラン ]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> 次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## OAuth2 の概要

アプリケーションが、次から特定の情報を取り込む必要があると仮定します。 [!DNL Workfront]. 情報を要求するアプリケーションは、クライアントと呼ばれます。 この例では、クライアント名は ClientApp です。 ClientApp は特定のユーザーの情報にアクセスできる必要があるので、アクセスする必要があります [!DNL Workfront] を設定します。 ユーザーが ClientApp にユーザー名とパスワードを指定した場合、ClientApp はユーザーがアクセスできるすべてのデータにアクセスできます。 ClientApp は特定の情報の小さなセットのみを必要とするので、これはセキュリティ上のリスクとなります。

ClientApp 用の OAuth2 アプリを作成すると、基本的に次のように言います。 [!DNL Workfront] ClientApp がアクセスを許可されている [!DNL Workfront]が設定されますが、これは、アカウント ClientApp がにアクセスしているユーザーがアクセス権を付与している場合に限られます。

## OAuth2 アプリケーションの作成

OAuth2 アプリケーションを作成する場合、統合のニーズに最適なアプリケーションのタイプを選択します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アプリケーションタイプ</th> 
   <th>最適</th> 
   <th>認証方法</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>マシンツーマシンアプリケーション</p> </td> 
   <td> <p>お使いのサーバ上で実行する CLI、デーモン、またはスクリプトに最適</p> <p>例：</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>公開鍵 / 秘密鍵のペアのエンコーディングを使用した JSON web トークンによる認証。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>シングルページ Web アプリケーション</p> </td> 
   <td> <p>モバイルまたはシングルページ Web アプリケーションに最適</p> <p>例：</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>Proof Key for Code Exchange (PKCE) を使用した OAuth 2.0 認証コードフローによる認証。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Web アプリケーション</p> </td> 
   <td> <p>サーバー上の資格情報とトークンを処理するサーバー側アプリケーションに最適です。</p> <p>例：</p> 
    <ul> 
     <li> <p>[!DNL Go]</p> </li> 
     <li> <p>[!DNL Java]</p> </li> 
     <li> <p>[!DNL ASP.Net]</p> </li> 
     <li> <p>[!DNL Node.js]</p> </li> 
     <li> <p>[!DNL PHP]</p> </li> 
    </ul> </td> 
   <td> <p>OAuth 2.0 認証コードフローによる認証。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>一度に最大 10 個の OAuth2 アプリケーションを持つことができます。

* [サーバー認証を使用した OAuth2 アプリケーションの作成（JWT フロー）](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [ユーザー資格情報を使用した OAuth2 アプリケーションの作成（認証コードフロー）](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [PKCE を使用した OAuth2 シングルページ Web アプリケーションの作成](#create-an-oauth2-single-page-web-application-using-pkce)

### サーバー認証を使用した OAuth2 アプリケーションの作成（JWT フロー） {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth2 アプリケーション]**.
1. クリック **[!UICONTROL アプリ統合の作成]**.
The **新しい OAuth2 アプリケーション** ボックスが表示されます。
1. Adobe Analytics の **新しい OAuth2 アプリケーション** ボックス、選択 **[!UICONTROL サーバー認証]**.
1. 新しいアプリケーションの名前を入力します（例： ）。[!DNL Workfront] ClientApp の場合は。」
1. 「**[!UICONTROL 作成]**」をクリックします。
1. 新しいアプリのフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント ID]</td> 
      <td> <p>このフィールドは自動的に生成されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td> 
      <td> <p>このフィールドは自動的に生成されます</p> <p><b>重要</b>:  <p>このページを閉じる前に、このフィールドの内容を別のセキュリティで保護されたファイルにコピーしてください。 この秘密鍵は再び表示されなくなります。</p> <p>このキーが失われた場合は、そのキーを削除し、クライアントシークレットを作成します。</p> 
        <ol> 
         <li value="1"> <p>次をクリック： <b>[!UICONTROL 削除 ]</b> アイコン <img src="assets/delete.png"> をクリックして、現在のクライアントシークレットを削除します。</p> </li> 
         <li value="2"> <p>クリック <b>[!UICONTROL クライアント秘密鍵を追加 ]</b> をクリックして、新しいクライアントシークレットを生成します。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 公開鍵 ]</td> 
      <td> <p>サーバー間アプリは、認証に公開鍵と秘密鍵を使用します。 次のいずれかの操作を行います。</p> 
       <ul> 
        <li> <p>クリック <b>[!UICONTROL 公開鍵を追加 ]</b> 他のアプリケーションから公開鍵を入力します。</p> </li> 
        <li> <p>クリック <b>[!UICONTROL 公開鍵/秘密鍵のペアを生成 ]</b>をクリックし、他のアプリケーションと公開鍵を共有します。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名前 ]</td> 
      <td>これは、アプリに付けたのと同じ名前です。 このフィールドは空にできません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td>統合の説明を入力します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 保存]**」をクリックします。

ユーザー資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、 [JWT フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-jwt-flow.md).

### ユーザー資格情報を使用した OAuth2 アプリケーションの作成（認証コードフロー） {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth2 アプリケーション]**.
1. クリック **[!UICONTROL アプリ統合の作成]**.

   The **新しい OAuth2 アプリケーション** が表示されます。
1. Adobe Analytics の **新しい OAuth2 アプリケーション** ボックス、選択 **[!UICONTROL ユーザー認証]**.
1. 新しい OAuth2 アプリケーションの名前を入力します（例： ）。[!DNL Workfront] ClientApp の場合は。」
1. 「**[!UICONTROL 作成]**」をクリックします。
1. 新しいアプリのフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント ID]</td> 
      <td> <p>このフィールドは自動的に生成されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td> 
      <td> <p>このフィールドは自動的に生成されます</p> <p><b>重要</b>:  <p>このページを閉じる前に、このフィールドの内容を別のセキュリティで保護されたファイルにコピーしてください。 この秘密鍵は再び表示されなくなります。</p> <p>このキーが失われた場合は、そのキーを削除し、クライアントシークレットを作成します。</p> 
        <ol> 
         <li value="1"> <p>次をクリック： <b>[!UICONTROL 削除 ]</b> アイコン <img src="assets/delete.png"> をクリックして、現在のクライアントシークレットを削除します。</p> </li> 
         <li value="2"> <p>クリック <b>[!UICONTROL クライアント秘密鍵を追加 ]</b> をクリックして、新しいクライアントシークレットを生成します。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL リダイレクト URL]</td> 
      <td>ユーザーは、で認証された後、このパスにリダイレクトされます。 [!DNL Workfront].</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL トークンのローテーションを更新 ]</td> 
      <td>このオプションを有効にすると、更新トークンが使用されるたびに新しい更新トークンが発行されます。アプリケーションは、更新のたびに新しい更新トークンを格納する必要があります。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 更新トークンの絶対的な有効期限 ]</td> 
      <td> <p>更新トークンの有効期限が切れるまでの期間を選択します。 有効期限が切れたら、ユーザーは統合に再度ログインする必要があります。 更新トークンの有効期限を設定しない場合は、「[!UICONTROL 有効期限なし ]」を選択します。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">非アクティブリフレッシュトークンの有効期限</td> 
      <td> <p>ユーザーがシステム内でアクティブでない場合に、その更新トークンの有効期限を設定します。 </p> <p>例えば、無操作状態の更新トークンの有効期限が 6 か月で、ユーザーが 6 か月間ログインしない場合、更新トークンの絶対更新トークンの有効期限が 6 か月に設定されていても、更新トークンは有効期限が切れます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ロゴ ]</td> 
      <td>ロゴを追加して、このアプリをより識別しやすくすることができます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名前 ]</td> 
      <td>これは、アプリに付けたのと同じ名前です。 このフィールドは空にできません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td>統合の説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL アプリの説明 URL]</td> 
      <td>これには、「会社概要」ページへのリンクや、統合の詳細情報を含むページを指定できます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 保存]**」をクリックします。

ユーザー資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、 [認証コードフローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-code-token-flow.md).

### PKCE を使用した OAuth2 シングルページ Web アプリケーションの作成 {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth2 アプリケーション]**.
1. クリック **[!UICONTROL アプリ統合の作成]**.

   The **新しい OAuth2 アプリケーション** ボックスが表示されます。
1. Adobe Analytics の **新しい OAuth2 アプリケーション** ボックス、選択 **[!UICONTROL 単一ページ Web アプリケーション]**.
1. 新しい [!UICONTROL OAuth2] アプリケーション（例： ）[!DNL Workfront] ClientApp の場合は。」
1. 「**[!UICONTROL 作成]**」をクリックします。
1. 新しいアプリのフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント ID]</td> 
      <td> <p>このフィールドは自動的に生成されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL リダイレクト URL]</td> 
      <td>ユーザーは、Workfrontで認証された後、このパスにリダイレクトされます。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 更新トークンを使用するたびに回転 ]</td> 
      <td>このオプションを有効にすると、更新トークンが使用されるたびに新しい更新トークンが発行されます。アプリケーションは、更新のたびに新しい更新トークンを格納する必要があります。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 絶対的な有効期限 ]</td> 
      <td> <p>更新トークンの有効期限が切れるまでの期間を選択します。 有効期限が切れたら、ユーザーは統合に再度ログインする必要があります。 更新トークンの有効期限を設定しない場合は、「[!UICONTROL 有効期限なし ]」を選択します。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 無操作状態の有効期限 ]</td> 
      <td> <p>ユーザーがシステム内でアクティブでない場合に、その更新トークンの有効期限を設定します。 </p> <p>例えば、無操作状態の更新トークンの有効期限が 6 か月で、ユーザーが 6 か月間ログインしない場合、更新トークンの絶対更新トークンの有効期限が 6 か月に設定されていても、更新トークンは有効期限が切れます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ロゴ ]</td> 
      <td>ロゴを追加して、このアプリをより識別しやすくすることができます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名前 ]</td> 
      <td>これは、アプリに付けたのと同じ名前です。 このフィールドは空にできません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td>統合の説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 開発者名 ]</td> 
      <td>これは、OAuth2 アプリケーションを設定する開発者の名前です。</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL 開発者用電子メールアドレス ]</td> 
      <td>OAuth2 アプリケーションを設定している開発者の電子メールアドレスです。</td> 
     </tr> 
   <tr> 
      <td role="rowheader">[!UICONTROL プライバシーポリシー URL]</td> 
      <td>これは、組織がプライバシーポリシーを保存する場所へのリンクです。</td> 
     </tr>


   </tbody> 
   </table>

   <!-- removed this from the table, and added "Developer name" and following rows:
   [!UICONTROL App Description URL]</td> 
      <td>This can be a link to an "About us" page or a page with more information about the integration.> -->

1. 「**[!UICONTROL 保存]**」をクリックします。

## 作成した OAuth2 アプリケーションを設定して使用する

作成した OAuth2 アプリケーションをさらに設定して使用するには、API 呼び出しを含む技術的な知識が必要です。

* ユーザー資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、 [認証コードフローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-code-token-flow.md).
* サーバー認証（JWT フロー）を使用した OAuth2 アプリケーションの設定と使用の手順については、 [JWT フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-jwt-flow.md).
* PKCE を使用して OAuth2 アプリケーションを設定および使用する手順については、 [PKCE フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-pkce-flow.md).

## 認証コードフローの OAuth2 プロセス

>[!NOTE]
>
>ユーザーが [!UICONTROL OAuth2] API を介してアプリケーションを使用する。 この節では、一般的な用語での機能について説明し、情報提供のみを目的として提供されています。
>
>特定の API 呼び出しを含む、OAuth2 アプリケーションの使用に関する具体的な手順については、 [認証コードフローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-code-token-flow.md).

### 認証コードとアクセストークンを使用した認証 {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp には次の情報が必要です： [!DNL Workfront]を呼び出し、リクエストを [!DNL Workfront] API `/authorize` endpoint. リクエストには、 [!UICONTROL response_type] `code`：リクエストが認証コードを返す必要があることを示します。
1. このトリガー [!DNL Workfront] 認証プロンプトをユーザーに送信します。 ユーザーは、プロンプトに資格情報を入力し、 [!DNL Workfront] ClientApp と通信する権限。 ユーザーが既に [!DNL Workfront]の場合、この手順はスキップできます。
1. The [!DNL Workfront] API が認証コードを ClientApp に送信します。
1. ClientApp は、次の情報をリクエストでに送信します。 [!DNL Workfront] API `/token`   endpoint:

   * 手順 3 で ClientApp に送信した認証コード。 ユーザー権限の特定のインスタンスを識別します。
   * ClientApp OAuth2 アプリをで設定したときに生成されたクライアント秘密鍵 [!DNL Workfront]. これにより、 [!DNL Workfront] リクエストが ClientApp から送信されたことを知るために使用されます。

1. 認証コードとクライアントの秘密鍵が正しい場合、 [!DNL Workfront] はアクセストークンを ClientApp に送信します。 このアクセストークンは、 [!DNL Workfront] を ClientApp にコピーし、他のユーザーまたはクライアントアプリケーションで表示、コピー、使用することはできません。
1. ClientApp がアクセストークンをに送信する [!DNL Workfront] 特定の情報を求めるリクエストと共に
1. アクセストークンが正しいので、 [!DNL Workfront] は情報を ClientApp に送信します。

#### アクセストークンを更新しています

セキュリティのため、アクセストークンは短時間で期限切れになります。 資格情報を毎回入力しなくても新しいアクセストークンを取得するには、 [!DNL OAuth2] は更新トークンを使用します。 更新トークンはクライアントによって保存されます。

更新トークンの取得プロセスは、の節で説明した手順と同じです。 [認証コードとアクセストークンを使用した認証](#authorizing-with-an-authorization-code-and-access-token). 認証コードのリクエストには、スコープが含まれます `offline_access`：リクエストは、認証コードと共にリクエストトークンを返す必要があることを示します。
