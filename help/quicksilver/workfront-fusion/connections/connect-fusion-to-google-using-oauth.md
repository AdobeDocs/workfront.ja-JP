---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: カスタム OAuth クライアントを使用して  [!DNL Adobe Workfront Fusion]  を  [!DNL Google Services]  に接続
description: カスタム OAuth クライアントを使用し、 [!DNL Adobe Workfront Fusion]  を使用して  [!DNL Google Services]  に接続できます。この手順には、既存の  [!DNL Google]  アカウントが必要です。
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 89%

---

# カスタム OAuth クライアントを使用して [!DNL Adobe Workfront Fusion] を [!DNL Google Services] に接続

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p><p>または</p><p>現在：[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>レガシー：任意 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>新規：</p> <ul><li>[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Workfront] プラン：組織は [!DNL Adobe Workfront Fusion] を購入する必要があります。</li><li>[!UICONTROL Ultimate] [!DNL Workfront] プラン：[!DNL Workfront Fusion] が含まれています。</li></ul>
   <p>または</p>
   <p>現在：[!DNL Adobe Workfront Fusion] を購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

この接続を作成するには、既存の [!DNL Google] アカウントが必要です。

## カスタム OAuth クライアントを使用して Fusion をGoogle サービスに接続する

この連携を作成するには、Google Cloud Platform でプロジェクトを作成して設定し、そのプロジェクトに基づいて Fusion で連携を設定する必要があります。

* [ [!DNL Google Cloud Platform] にプロジェクトを作成します。](#create-a-project-on-google-cloud-platform)
* [[!UICONTROL OAuth 同意 ] 設定の指定 ](#configure-oauth-consent-settings)
* [OAuth 資格情報を作成](#create-oauth-credentials)
* [ [!DNL Google]  接続  [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion)

>[!NOTE]
>
>この手順の目的は次のとおりです。
>
>* 個人用（[!DNL `@gmail.com`] および [!DNL `@googlemail.com`] ユーザー）
>* 内部使用（カスタム OAuth クライアントの使用を希望する [!DNL Google Workspace] ユーザー）

### [!DNL Google Cloud Platform] でプロジェクトを作成

[!DNL Google Cloud] プラットフォームでプロジェクトを作成するには、以下のように行います。

1. [!DNL Google] 認証情報を使用して、[[!DNL Google Cloud] プラットフォーム](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project)にログインします。
1. 左側のパネルで、**[!UICONTROL ダッシュボード]**&#x200B;をクリックします。
1. 画面の右上隅にある「**[!UICONTROL プロジェクトを作成]**」をクリックします。
1. **[!UICONTROL プロジェクト名]**&#x200B;を入力し、続いて「**[!UICONTROL 作成]**」をクリックします。

1. 画面上部の近くの「**[!UICONTROL API とサービスを有効にする]**」タブをクリックします。
1. 画面上部の「**[!UICONTROL API とサービスを検索]**」フィールドに、使用するサービスの名前（[!DNL Gmail] API または [!DNL Google Drive] AP）を入力します。
1. 表示されたら、[!DNL Workfront Fusion] に接続する API またはサービスをクリックします。
1. 「**[!UICONTROL 有効にする]**」をクリックして、選択した API を有効にします。
1. 有効にする API ごとに、手順 6～8 を繰り返します。

   >[!NOTE]
   >
   >[!DNL Google Drive] API と、使用するすべての [!DNL Google] アプリの API（[!DNL Google Sheets] API など）を有効にする必要があります。

1. 表示される画面で、右上隅にある「**[!UICONTROL 資格情報を作成]**」をクリックします。
1. この記事にある [OAuth の同意設定を指定](#configure-oauth-consent-settings)の節に進みます。

### [!UICONTROL OAuth 同意]の設定を指定

1. 左側のパネルで、「**[!UICONTROL OAuth 同意画面]**」をクリックします。
1. **[!UICONTROL 外部]**&#x200B;を選択し、続いて「**[!UICONTROL 作成]**」をクリックします。

   >[!NOTE]
   >
   >このオプションを選択すると、課金されなくなります。詳しくは、[!DNL Google] の検証要件の例外に関する情報を参照してください。

1. 必須フィールドに次のように入力します。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App name]</p> </td> 
      <td> <p>同意を要求するアプリの名前を入力します。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL User support email]</td> 
      <td>ユーザーがこのアプリに接続する際の同意に関する質問を連絡するためのメールアドレスを入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Email addresses]</td> 
      <td>Google がプロジェクトに対する変更を通知する際に使用できるメールアドレスを 1 つ以上入力します。</td> 
     </tr> 
    </tbody> 
   </table>

1. [!UICONTROL 認証済みドメイン]の下で、「**[!UICONTROL ドメインを追加]**」をクリックし、`workfrontfusion.com` と入力します。

1. 「**[!UICONTROL 保存して続行]**」をクリックします。
1. 「**[!UICONTROL スコープを追加または削除]**」をクリックします。
1. 右側のパネルで、次のスコープを有効にします。

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>サービス／API</th> 
      <th>必須スコープ</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

リストを展開するか、リストの次のページに移動して、すべてを表示する必要が生じる場合があります。

1. 「**[!UICONTROL 更新]**」をクリックします。
1. 「**[!UICONTROL 保存して続行]**」をクリックします。
1. （オプション）テストユーザーをプロジェクトに追加します。
1. 「**[!UICONTROL 保存して続行]**」をクリックします。
1. 情報の正確性を確認し、「**[!UICONTROL ダッシュボードに戻る]**」をクリックします。

   >[!NOTE]
   >
   >[!DNL Google] による検証のために同意画面や申請を送信する必要はありません。

1. [OAuth 資格情報を作成](#create-oauth-credentials)に進みます。

### OAuth 資格情報を作成

1. 左側のパネルで、「**[!UICONTROL 資格情報]**」をクリックします。

   >[!NOTE]
   >
   >これが最初に有効にした API またはサービス（[!DNL Gmail] または [!DNL Google Drive]）ではない場合は、新しい資格情報を作成する必要はありません。

1. 画面の上部付近にある「**[!UICONTROL 資格情報を作成]**」をクリックし、ドロップダウンメニューから「**[!UICONTROL OAuth クライアント ID]**」を選択します。

1. 必須フィールドに次のように入力します。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Application type]</td> 
      <td> <p> [!UICONTROL Web application]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. [!UICONTROL 承認済みリダイレクト URI] の下で、「**[!UICONTROL URI を追加]**」をクリックし、次のうち **1 つ**&#x200B;を入力します。

   * [!DNL Gmail] または [!DNL Google Drive] の場合：`https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * その他の [!DNL Google] アプリの場合：`https://app.workfrontfusion.com/oauth/cb/google`

1. 「**[!UICONTROL 作成]**」をクリックします。

   [!UICONTROL クライアント ID] および[!UICONTROL クライアントシークレット]が表示されます。

1. [!UICONTROL クライアント ID] および[!UICONTROL クライアントシークレット]を、安全な場所にコピーします。これらを使用して、[!DNL Workfront Fusion] で接続を作成します。
1. [ [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion) で  [!DNL Google]  に接続に進みます。

### [!DNL Workfront Fusion] で [!DNL Google] に接続

[!DNL Google] への接続を作成するプロセスは、[!DNL Google] サービス（[!DNL Google Sheets] や [!DNL Google Docs] など）のモジュールを使用しているか、[!UICONTROL HTTP]／[!UICONTROL OAuth2.0 を作成]リクエストモジュール経由で [!DNL Google] に接続しているかで異なります。

* [ [!DNL Google]  サービスで  [!DNL Google]  に接続](#connect-to-google-in-a-google-service)
* [[!UICONTROL HTTP]／[!UICONTROL OAuth2.0 リクエストを作成]モジュールで  [!DNL Google]  に接続](#connect-to-google-in-the-http--make-an-oauth20-request-module)

#### [!DNL Google] サービスで [!DNL Google] に接続

1. [!DNL Workfront Fusion] で、接続を作成する必要がある [!DNL Google] モジュールを見つけます。
1. 「**[!UICONTROL 接続を作成]**」をクリックしてから、「**[!UICONTROL 詳細設定を表示]**」をクリックします。

1. 「[[!UICONTROL OAuth 認証情報を作成]](#create-oauth-credentials)」で取得した「[!UICONTROL クライアント ID]」と「[!UICONTROL クライアントシークレット]」をそれぞれのフィールドに入力し、「**[!UICONTROL 続行]**」をクリックします。

1. [!DNL Google] アカウントにログインします。

   **[!UICONTROL このアプリは検証されていません]**&#x200B;ウィンドウが表示されます。ウィンドウのタイトルに表示される「アプリ」は、前述で作成した OAuth クライアントです。

1. カスタム OAuth クライアントを使用したアクセスを許可するには、「**[!UICONTROL 詳細]**」をクリックしてから「**[!UICONTROL [!DNL Workfront Fusion] に移動（安全でない）]**」をクリックします。

1. 「**[!UICONTROL 許可]**」をクリックして [!DNL Workfront Fusion] 権限を付与します。
1. 表示されるウィンドウで、「**[!UICONTROL 許可]**」を再度クリックして、選択内容を確認します。

   カスタム OAuth クライアントを使用して、目的の [!DNL Google] サービスへの接続が確立されます。

#### [!UICONTROL HTTP]／[!UICONTROL OAuth2.0 リクエストを作成]モジュールで [!DNL Google] に接続します {#connect-to-google-in-the-http--make-an-oauth20-request-module}

[!UICONTROL HTTP]／[!UICONTROL OAuth2.0 リクエストを作成]モジュールで [!DNL Google] に接続する手順については、[[[!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 リクエストを作成]モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)で [!UICONTROL HTTP] での  [!DNL Google]  への接続の作成手順／[!UICONTROL OAuth 2.0 リクエストを作成]モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)を参照してください。

## 考えられるエラーメッセージ：[!UICONTROL [403] アクセスが設定されていません]

[!UICONTROL `403 Access Not Configured`] エラーメッセージが表示された場合は、Google Cloud Platform で対応する API を有効にする必要があります。 API を有効にするには、この記事の「[ [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) でプロジェクトを作成」の節の手順に従います。
