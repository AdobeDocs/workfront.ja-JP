---
title: ' [!DNL Workfront]  統合用の OAuth2 アプリケーションを作成する'
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: ' [!DNL Adobe Workfront]  管理者は、 [!DNL Workfront] のインスタンス用に OAuth2 アプリケーションを作成できます。これにより、他のアプリケーションが Workfront にアクセスできるようになります。その後、ユーザーは他のアプリケーションに Workfront データへのアクセス権を付与できます。このようにして、Workfront を、独自の社内アプリケーションなど、選択したアプリケーションと統合できます。'
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: e13c7dda-8945-47ad-b6d3-4d6a62b368f5
source-git-commit: ff24fcc65791b6c18668a0dd3c58e033772a2def
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 87%

---

# [!DNL Workfront] 統合用の OAuth2 アプリケーションを作成する

[!DNL Adobe Workfront] 管理者は、[!DNL Workfront] のインスタンス用の OAuth2 アプリケーションを作成して、他のアプリケーションが [!DNL Workfront] にアクセスできるようにします。その後、ユーザーは他のアプリケーションに [!DNL Workfront] データへのアクセス権を付与できます。このようにして、独自の社内アプリケーションなど、選択したアプリケーションと統合できます。

[!UICONTROL OAuth2] アプリケーションを作成する場合、クライアント ID とクライアントシークレットを生成します。その後、ユーザーは API 呼び出しでクライアント ID を使用して、作成したアプリケーションと統合できます。

>[!NOTE]
>
>OAuth2 のコンテキストでは、「アプリの作成」とは、アプリと [!DNL Workfront] などのサーバーとの間にこの種のアクセスリンクを作成するプロセスを指します。

* ユーザーの資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、[認証コードフローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-code-token-flow.md)を参照してください。
* サーバー認証（JWT フロー）を使用した OAuth2 アプリケーションの設定と使用の手順については、[JWT フローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-jwt-flow.md)を参照してください。
* PKCE を使用して OAuth2 アプリケーションを設定および使用する手順については、[PKCE フローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-pkce-flow.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td><p>新規： [!UICONTROL Standard]</p>
   または
   <p>現在：[!UICONTROL プラン ]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> [!DNL Workfront] 管理者であることが必要です。 </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## OAuth2 の概要

アプリケーションが、次から特定の情報を取り込む必要があると仮定します。 [!DNL Workfront]. 情報を要求するアプリケーションは、クライアントと呼ばれます。この例では、クライアント名は ClientApp です。ClientApp は特定のユーザーの情報にアクセスできる必要があるので、アクセスする必要があります [!DNL Workfront] を設定します。 ユーザーが ClientApp にユーザー名とパスワードを付与した場合、ClientApp はユーザーがアクセスできるすべてのデータにアクセスできます。ClientApp は少数の特定の情報セットのみを必要とするため、これはセキュリティ上のリスクとなります。

ClientApp 用の OAuth2 アプリを作成すると、基本的に、ClientApp が [!DNL Workfront] にアクセスできることを [!DNL Workfront] に伝えることになりますが、これは ClientApp がアクセスしているアカウントのユーザーがアクセス許可を与えた場合に限ります。

## OAuth2 アプリケーションを作成

OAuth2 アプリケーションを作成する場合、統合のニーズに最適なアプリケーションのタイプを選択します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アプリケーションタイプ</th> 
   <th>以下に最適</th> 
   <th>認証方法</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>マシン間アプリケーション</p> </td> 
   <td> <p>サーバー上で実行する CLI、デーモン、またはスクリプトに最適</p> <p>例：</p> 
    <ul> 
     <li> <p>[!DNL Shell] </p> </li> 
     <li> <p>[!DNL Python]</p> </li> 
    </ul> </td> 
   <td> <p>公開鍵 / 秘密鍵ペアのエンコーディングを使用した JSON Web トークンによる認証。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>シングルページ Web アプリケーション</p> </td> 
   <td> <p>モバイルまたはシングルページ web アプリケーションに最適</p> <p>例：</p> 
    <ul> 
     <li> <p>[!DNL Javascript]</p> </li> 
     <li> <p>[!DNL Angular]</p> </li> 
     <li> <p>[!DNL React]</p> </li> 
     <li> <p>[!DNL Vue]</p> </li> 
    </ul> </td> 
   <td> <p>Proof Key for Code Exchange（PKCE）を使用した OAuth 2.0 認証コードフローによる認証。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Web アプリケーション</p> </td> 
   <td> <p>サーバー上の資格情報とトークンを処理するサーバー側アプリケーションに最適</p> <p>例：</p> 
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

* [サーバー認証を使用した OAuth2 アプリケーションを作成する（JWT フロー）](#create-an-oauth2-application-using-server-authentication-jwt-flow)
* [ユーザー資格情報を使用した OAuth2 アプリケーションの作成（認証コードフロー）](#create-an-oauth2-application-using-user-credentials-authorization-code-flow)
* [PKCE を使用した OAuth2 シングルページ Web アプリケーションの作成](#create-an-oauth2-single-page-web-application-using-pkce)

### サーバー認証を使用した OAuth2 アプリケーションを作成する（JWT フロー） {#create-an-oauth2-application-using-server-authentication-jwt-flow}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth2 アプリケーション]**.
1. クリック **[!UICONTROL アプリ統合の作成]**.
The **新しい OAuth2 アプリケーション** ボックスが表示されます。
1. Adobe Analytics の **新しい OAuth2 アプリケーション** ボックス、選択 **[!UICONTROL 機械 — 機械アプリケーション]**.
1. 「[!DNL Workfront] for ClientApp」などの、新しいアプリケーションの名前を入力します。
1. 「**[!UICONTROL 作成]**」をクリックします。
1. 新しいアプリのフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>このフィールドは自動的に生成されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>このフィールドは自動的に生成されます</p> <p><b>重要</b>：  <p>このページを閉じる前に、このフィールドの内容を別の安全なファイルにコピーしてください。この秘密鍵は再び表示されなくなります。</p> <p>このキーが失われた場合は、そのキーを削除し、クライアントシークレットを作成します。</p> 
        <ol> 
         <li value="1"> <p><b>[!UICONTROL Delete]</b> アイコン <img src="assets/delete.png"> をクリックして、現在のクライアントシークレットを削除します。</p> </li> 
         <li value="2"> <p>「<b>[!UICONTROL Add client secret]</b>」をクリックして、新しいクライアントシークレットを生成します。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public Keys]</td> 
      <td> <p>サーバー間アプリは、認証に公開鍵と秘密鍵を使用します。次のいずれかの操作を行います。</p> 
       <ul> 
        <li> <p>「<b>[!UICONTROL Add a public key]</b>」をクリックして、他のアプリケーションから公開鍵を入力します。</p> </li> 
        <li> <p>「<b>[!UICONTROL Generate a public/private keypair]</b>」をクリックして、他のアプリケーションと公開鍵を共有します。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>これは、アプリに付けたのと同じ名前です。このフィールドを空白にすることはできません.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>統合の説明を入力します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 保存]**」をクリックします。

ユーザー資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、[JWT フローを使用した組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-jwt-flow.md)を参照してください。

### ユーザー資格情報を使用した OAuth2 アプリケーションの作成（認証コードフロー） {#create-an-oauth2-application-using-user-credentials-authorization-code-flow}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth2 アプリケーション]**.
1. 「**[!UICONTROL アプリ統合を作成]**」をクリックします。

   The **新しい OAuth2 アプリケーション** が表示されます。
1. Adobe Analytics の **新しい OAuth2 アプリケーション** ボックス、選択 **[!UICONTROL Web アプリケーション]**.
1. 「[!DNL Workfront] for ClientApp」などの、新しい OAuth2 アプリケーションの名前を入力します。
1. 「**[!UICONTROL 作成]**」をクリックします。
1. 新しいアプリのフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>このフィールドは自動的に生成されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client secret]</td> 
      <td> <p>このフィールドは自動的に生成されます</p> <p><b>重要</b>：  <p>このページを閉じる前に、このフィールドの内容を別の安全なファイルにコピーしてください。この秘密鍵は再び表示されなくなります。</p> <p>このキーが失われた場合は、そのキーを削除し、クライアントシークレットを作成します。</p> 
        <ol> 
         <li value="1"> <p><b>[!UICONTROL Delete]</b> アイコン <img src="assets/delete.png"> をクリックして、現在のクライアントシークレットを削除します。</p> </li> 
         <li value="2"> <p>「<b>[!UICONTROL Add client secret]</b>」をクリックして、新しいクライアントシークレットを生成します。</p> </li> 
        </ol> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirect URLs]</td> 
      <td>[!DNL Workfront]で認証されたユーザーは、このパスにリダイレクトされます。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Refresh token rotation]</td> 
      <td>このオプションを有効にすると、更新トークンが使用されるたびに新しい更新トークンが発行されます。アプリケーションは、更新のたびに新しい更新トークンを格納する必要があります。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Absolute refresh token expiration]</td> 
      <td> <p>更新トークンの有効期限が切れるまでの期間を選択します。 有効期限が切れたら、ユーザーは統合に再度ログインする必要があります。更新トークンの有効期限を設定しない場合は、「[!UICONTROL No expiration]」を選択します。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">非アクティブ更新トークンの有効期限</td> 
      <td> <p>ユーザーがシステム内でアクティブでない場合に、その更新トークンの有効期限を設定します。 </p> <p>例えば、非アクティブ更新トークンの有効期限が 6 か月で、ユーザーが 6 か月間ログインしなかった場合、絶対期限が 6 か月より長く設定されていても、更新トークンは期限切れとなります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>ロゴを追加して、このアプリをより識別しやすくすることができます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>これは、アプリに付けたのと同じ名前です。このフィールドを空白にすることはできません.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>統合の説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL App Description URL]</td> 
      <td>ここでは、会社概要のページや統合の詳細情報を含むページへのリンクを指定できます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 保存]**」をクリックします。

ユーザー資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、[認証コードフローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-code-token-flow.md)を参照してください。

### PKCE を使用した OAuth2 シングルページ Web アプリケーションの作成 {#create-an-oauth2-single-page-web-application-using-pkce}

{{step-1-to-setup}}

1. 左側のナビゲーションパネルで、 **[!UICONTROL システム]**&#x200B;を選択し、「 **[!UICONTROL OAuth2 アプリケーション]**.
1. 「**[!UICONTROL アプリ統合を作成]**」をクリックします。

   The **新しい OAuth2 アプリケーション** ボックスが表示されます。
1. Adobe Analytics の **新しい OAuth2 アプリケーション** ボックス、選択 **[!UICONTROL 単一ページ Web アプリケーション]**.
1. 「[!DNL Workfront] for ClientApp」など、[!UICONTROL OAuth2] アプリケーションの新しい名前を入力します。
1. 「**[!UICONTROL 作成]**」をクリックします。
1. 新しいアプリのフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td> <p>このフィールドは自動的に生成されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Redirect URLs]</td> 
      <td>Workfront で認証されたユーザーは、このパスにリダイレクトされます。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 更新トークンを使用するたびに回転 ]</td> 
      <td>このオプションを有効にすると、更新トークンが使用されるたびに新しい更新トークンが発行されます。アプリケーションは、更新のたびに新しい更新トークンを格納する必要があります。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 絶対的な有効期限 ]</td> 
      <td> <p>更新トークンの有効期限が切れるまでの期間を選択します。有効期限が切れたら、ユーザーは統合に再度ログインする必要があります。更新トークンの有効期限を設定しない場合は、「[!UICONTROL No expiration]」を選択します。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL 無操作状態の有効期限 ]</td> 
      <td> <p>ユーザーがシステム内でアクティブでない場合に、その更新トークンの有効期限を設定します。 </p> <p>例えば、非アクティブ更新トークンの有効期限が 6 か月で、ユーザーが 6 か月間ログインしなかった場合、絶対期限が 6 か月より長く設定されていても、更新トークンは期限切れとなります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Logo]</td> 
      <td>ロゴを追加して、このアプリをより識別しやすくすることができます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>これは、アプリに付けたのと同じ名前です。このフィールドを空白にすることはできません.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
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

## 作成した OAuth2 アプリケーションの設定および使用

作成した OAuth2 アプリケーションをさらに設定して使用するには、API 呼び出しを含む技術的な知識が必要です。

* ユーザー資格情報を使用して OAuth2 アプリケーションを設定および使用する手順（認証コードフロー）については、[認証コードフローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用](../../wf-api/api/oauth-app-code-token-flow.md)を参照してください。
* サーバー認証（JWT フロー）を使用した OAuth2 アプリケーションの設定と使用の手順については、[JWT フローを使用した、組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-jwt-flow.md)を参照してください。
* PKCE を使用して OAuth2 アプリケーションを設定および使用する手順については、[PKCE フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用](../../wf-api/api/oauth-app-pkce-flow.md)を参照してください。

## 認証コードフローの OAuth2 プロセス

>[!NOTE]
>
>ユーザーは API を通じて [!UICONTROL OAuth2] アプリケーションにアクセスします。この節は一般的な用語での機能について説明し、情報提供のみを目的としています。
>
>特定の API 呼び出しを含む、OAuth2 アプリケーションの使用に関する具体的な手順については、[認証コードフローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用](../../wf-api/api/oauth-app-code-token-flow.md)を参照してください。

### 認証コードとアクセストークンを使用した認証 {#authorizing-with-an-authorization-code-and-access-token}

1. ClientApp は [!DNL Workfront] からの情報を必要とするため、[!DNL Workfront] API `/authorize`エンドポイントにリクエストを送信します。リクエストには、[!UICONTROL response_type]`code` が含まれます。これは、リクエストが認証コードを返す必要があることを示します。
1. これにより、[!DNL Workfront] がトリガーされ、ユーザーに認証プロンプトが送信されます。ユーザーは、プロンプトに資格情報を入力すると、[!DNL Workfront] に ClientApp と通信するためのアクセス許可が付与されます。ユーザーが既に [!DNL Workfront] にログインしている場合、この手順をスキップできます。
1. [!DNL Workfront] API が認証コードを ClientApp に送信します。
1. ClientApp は、リクエストで次の情報を [!DNL Workfront] API `/token`エンドポイントに送信します。

   * 手順 3 で ClientApp に送信した認証コード。これは、ユーザー権限の特定のインスタンスを識別します。
   * [!DNL Workfront] でClientApp OAuth2 アプリを設定したときに生成されたクライアントシークレット。これにより、[!DNL Workfront] はリクエストが ClientApp から送信されていることを認識できるようになります。

1. 認証コードとクライアントシークレットが正しい場合、[!DNL Workfront] はアクセストークンを ClientApp に送信します。このアクセストークンは [!DNL Workfront] から ClientApp に直接送信され、他のユーザーやクライアントアプリケーションが表示、コピー、使用することはできません。
1. ClientApp は、特定情報のリクエストとともにアクセストークンを [!DNL Workfront] に送信します。
1. アクセストークンが正しいので、[!DNL Workfront] は情報を ClientApp に送信します。

#### アクセストークンの更新

セキュリティのため、アクセストークンは短時間で期限切れになります。資格情報を毎回入力せずに新しいアクセストークンを取得するには、[!DNL OAuth2] は更新トークンを使用します。更新トークンはクライアントによって保存されます。

更新トークンの取得プロセスは、[認証コードとアクセストークンを使用した認証](#authorizing-with-an-authorization-code-and-access-token)の節で説明した手順と同じです。認証コードのリクエストには、リクエストが認証コードとともにリクエストトークンを返す必要があることを示す、スコープ `offline_access` が含まれています。
