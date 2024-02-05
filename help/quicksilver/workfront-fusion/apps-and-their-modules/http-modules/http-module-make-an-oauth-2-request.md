---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: http-modules
title: HTTP &gt; OAuth 2.0 リクエストモジュールを作成
description: OAuth 2.0 認証を必要とするサーバーに対する  [!DNL Adobe Workfront Fusion]  HTTP(S) リクエストを実行するには、まず OAuth 接続を作成する必要があります。 [!DNL Adobe Workfront Fusion]  は、この接続で行われたすべての呼び出しに適切な認証ヘッダーが付いていることを確認し、必要に応じて関連トークンを自動的に更新します。
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '2220'
ht-degree: 100%

---

# [!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 リクエスト作成]モジュール

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] には [!DNL Adobe Workfront] ライセンスに加えて [!DNL Adobe Workfront Fusion] ライセンスが必要です。

OAuth 2.0 認証を必要とするサーバーに対する [!DNL Adobe Workfront Fusion] HTTP(S) リクエストを実行するには、まず OAuth 接続を作成する必要があります。[!DNL Adobe Workfront Fusion] は、この接続で行われたすべての呼び出しに適切な認証ヘッダーが付いていることを確認し、必要に応じて関連トークンを自動的に更新します。

[!DNL Workfront Fusion] は、次の OAuth 2.0 認証フローをサポートしています。

* 認証コードフロー
* 暗黙フロー

リソース所有者パスワード資格情報フローやクライアント資格情報フローなど、その他のフローは、このモジュールを通じて自動的にはサポートされません。

OAuth 2.0 認証について詳しくは、[OAuth 2.0 承認フレームワーク](https://tools.ietf.org/html/rfc6749)を参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL OAuth] リクエストへの接続を作成

* [HTTPで接続を作成するための一般的な手順／OAuth 2.0 リクエスト作成モジュール](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [HTTPで Google への接続を作成するための手順／OAuth 2.0 リクエスト[!UICONTROL 作成]モジュール](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [HTTP 経由で Microsoft Graph API への接続を作成するための手順／OAuth 2.0 リクエスト作成モジュール](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### [!UICONTROL HTTP] で接続を作成するための一般的な手順／[!UICONTROL OAuth 2.0 リクエスト作成]モジュール

1. [!DNL Adobe Workfront Fusion] と通信する [!DNL target] サービスに OAuth クライアントを作成します。このオプションは、所定のサービスの[!UICONTROL 開発者]セクションに含まれていることが多いです。

   1. クライアントを作成する際に、適切な URL を `[!UICONTROL Redirect URL]` または `[!UICONTROL Callback URL]` フィールドに入力します：

      | 南北アメリカ／APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. クライアントを作成すると、指定されたサービスは次の 2 つのキー（`[!UICONTROL Client ID]` と `[!UICONTROL Client Secret]`）が表示されます。これらの `[!UICONTROL App Key]` および `[!UICONTROL App Secret]` を呼び出すサービスもあります。キーと秘密鍵を安全な場所に保存して、Workfront Fusion で接続を作成する際に指定できるようにします。

1. `[!UICONTROL Authorize URI]` および `[!UICONTROL Token URI]` を特定のサービスの API ドキュメント内で探します。これらの URL アドレスを使用して [!DNL Workfront Fusion] は [!DNL target] サービスと通信します。アドレスは OAuth 認証に使用されます。

   >[!NOTE]
   >
   >サービスで暗黙的なフローを使用する場合、`[!UICONTROL Authorize URI]` のみが必要です。

   >[!INFO]
   >
   >**例：** Yahoo アドレス：
   >
   >* URI を許可：
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* トークン URI：
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. （条件付き）ターゲットサービスでスコープ（アクセス権）を使用する場合、サービスで個々のスコープがどのように区切られるかを確認し、それに応じて詳細設定で区切り文字を設定してください。区切り文字が正しく設定されていない場合、[!DNL Workfront Fusion] は接続の作成に失敗し、範囲無効エラーが表示されます。
1. 上記の手順を完了したら、[!DNL Workfront Fusion] で OAuth 接続の作成を開始できます。OAuth 2.0 HTTP(S) リクエストおよび応答処理モジュールをシナリオに追加します。
1. モジュールの「接続」フィールドで、「**[!UICONTROL 追加]**」をクリックします。

1. 次のフィールドに入力して、接続を作成します。

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>トークンを取得するフローを選択します。</p> 
       <ul> 
        <li><strong>[!UICONTROL Authorization Code]</strong>：サービスの API ドキュメントにある <code>[!UICONTROL Authorize URI]</code> と <code>[!UICONTROL Token URI]</code> を入力します。</li> 
        <li><strong>[!UICONTROL Implicit]</strong>：サービスの API ドキュメントにある <code>[!UICONTROL Authorize URI]</code> を入力してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>個々のスコープを追加します。この情報は、特定のサービスの開発者向けドキュメント（API）に記載されています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>上記で入力したスコープを区切る範囲を選択します。この情報は、特定のサービスの開発者向けドキュメント（API）に記載されています。</p> <p>警告：区切り文字が正しく設定されていない場合、[!DNL Workfront Fusion] は接続の作成に失敗し、無効なスコープエラーが表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>クライアント ID を入力します。クライアント ID は、接続するサービスで OAuth クライアントを作成したときに取得されました。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p> クライアントの秘密鍵を入力します。接続するサービスで OAuth クライアントを作成したときに、クライアントシークレットを取得しました。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorize parameters]</p> </td> 
      <td> <p>認証呼び出しに含めるパラメーターを追加します。次の標準パラメーターは常に自動的に含まれるため、追加する必要はありません。</p> <p>標準パラメーター：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> [!UICONTROL Authorization Code flow] 用の <code>code </code> および [!UICONTROL Implicit flow] 用の <code>token </code> の場合</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">南北アメリカ／APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong> </p> <p> アカウントの作成時に受け取ったクライアント ID</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Access token parameters]</p> </td> 
      <td> <p>トークン呼び出しに含めるパラメーターを追加します。次の標準パラメーターは常に自動的に含まれるため、追加する必要はありません。</p> <p>標準パラメーター：</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>： <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]：</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">南北アメリカ／APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>：アカウントの作成時に受け取ったクライアント ID は、リクエスト本文に自動的に含まれます</li> 
        <li><strong>client_secret</strong>：アカウントの作成時に受け取ったクライアントシークレットが、リクエスト本文に自動的に含まれます</li> 
        <li><strong>コード</strong>：認証リクエストによって返されるコード</li> 
       </ul> <p>メモ：  <p>OAuth 2.0 標準は、この手順で少なくとも 2 つのクライアント認証方法（<code>[!UICONTROL client_secret_basic]</code> および <code>[!UICONTROL client_secret_post]</code>）をサポートします。[!DNL Workfront Fusion] は、指定したクライアント ID と暗号鍵を <code>[!UICONTROL client_secret_post]</code> メソッドで自動送信します。したがって、これらのパラメーターは、トークンのリクエスト本文に自動的に含まれます。 </p> <p>OAuth 2.0 認証について詳しくは、<a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 承認フレームワーク</a>を参照してください。</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Refresh token parameters]</p> </td> 
      <td> <p>トークン呼び出しに含めるパラメーターを追加します。次の標準パラメーターは常に自動的に含まれるため、追加する必要はありません。</p> <p>標準パラメーター：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>：接続しているサービスで取得された最新の更新トークン。</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>：アカウントの作成時に受け取ったクライアント ID は、リクエスト本文に自動的に含まれます</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>：アカウントの作成時に受け取ったクライアント秘密鍵は、リクエスト本文に自動的に含まれます</p> </li> 
       </ul> <p>メモ：  <p>OAuth 2.0 標準は、この手順で少なくとも 2 つのクライアント認証方法（<code>[!UICONTROL client_secret_basic]</code> および <code>[!UICONTROL client_secret_post]</code>）をサポートします。[!DNL Workfront Fusion] は、指定したクライアント ID と暗号鍵を <code>[!UICONTROL client_secret_post]</code> メソッドで自動送信します。したがって、これらのパラメーターは、トークンのリクエスト本文に自動的に含まれます。 </p> <p>OAuth 2.0 認証について詳しくは、<a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 認証フレームワーク</a>を参照してください。</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Custom Headers]</p> </td> 
      <td> <p>[!UICONTROL Token] および R[!UICONTROL efresh Token] の手順のヘッダーに含める追加のキーと値を指定します。</p> <p>メモ：  <p>OAuth 2.0 標準は、この手順で少なくとも 2 つのクライアント認証方法（<code>[!UICONTROL client_secret_basic]</code> および <code>[!UICONTROL client_secret_post]</code>）をサポートします。[!DNL Workfront Fusion] は自動的には <code>[!UICONTROL client_secret_basic]</code> メソッドをサポートしません。接続しているサービスで、クライアント ID とクライアント秘密鍵が 1 つの文字列に結合され、Authorization ヘッダーに base64 がエンコードされると想定される場合は、そのヘッダーとキーの値をここに追加する必要があります。</p> <p> OAuth 2.0 認証について詳しくは、<a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 承認フレームワーク</a>を参照してください。</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Token placement]</p> </td> 
      <td> <p>指定した URL に接続する際に、[!UICONTROL header]、[!UICONTROL query string]、またはその両方でトークンを送信するかどうかを選択します。</p> <p>トークンは、最も一般的にリクエストヘッダーで送信されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Header token name] </td> 
      <td> <p>ヘッダーに認証トークンの名前を入力します。デフォルト：<code>[!UICONTROL Bearer]</code>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Query string parameter name] </td> 
      <td> <p>クエリ文字列に認証トークンの名前を入力します。デフォルト：<code>[!UICONTROL access_token]</code>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続設定を保存します。
1. [OAuth 2.0 リクエストモジュールのセットアップ](#oauth-20-request-module-setup)に継続します。

### [!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 リクエスト作成モジュール]で [!DNL Google] への接続を作成する手順

次の例は、[!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 実行]リクエストモジュールを使用して [!DNL Google] に接続する方法を示しています。

1. [カスタム OAuth クライアントを使用して  [!DNL Adobe Workfront Fusion]  を  [!DNL Google Services]  に接続する](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)に説明されているように、プロジェクトを作成、OAuth 設定を行い、資格情報が生成されていることを確認します。
1. [!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 実行リクエスト]モジュールを開きます。
1. 接続ボックスの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 次の値を入力します。

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name] </td> 
      <td> <p>接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Flow type]</p> </td> 
      <td> <p>[!UICONTROL Authorization Code]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope] </td> 
      <td> <p>個々のスコープを追加します。スコープについて詳しくは、[!DNL Google] ドキュメントにある<a href="https://developers.google.com/identity/protocols/oauth2/scopes"> [!DNL Google] API</a>向け OAuth 2.0 スコープを参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator] </td> 
      <td> <p>[!UICONTROL SPACE]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID] </td> 
      <td> <p>[!DNL Google] クライアント ID を入力します。 </p> <p>クライアント ID を作成するには、「カスタム OAuth クライアントを使用して <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] を [!DNL Google Services] に接続</a>」の <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth 資格情報を作成</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td> <p>[!DNL Google] クライアント秘密鍵を入力します。 </p> <p>クライアント秘密鍵を作成するには、「OAuth クライアントを使用して <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] を [!DNL Google] サービスに接続</a>」の <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth 資格情報を作成</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Authorize parameters]</p> </td> 
      <td> <p><code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code> キーと値のペアを追加します。</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>メモ：トークンの更新など、認証に関する問題が発生した場合は、<code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code> キーと値のペアを試してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続設定を保存します。
1. [OAuth 2.0 リクエストモジュールのセットアップ](#oauth-20-request-module-setup)に継続します。

### [!DNL Microsoft Graph API] に [!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 リクエストを作成] モジュール経由で接続する手順

[!DNL Microsoft Graph API] に関する手順については、[ [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] 経由で [!DNL MS Graph REST API] を呼び出す／[!UICONTROL OAuth 2.0 リクエストを作成]モジュール](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md)を参照してください。

## OAuth 2.0 リクエストモジュールの設定

[ [!DNL OAuth]  リクエストのための接続を作成](#creating-a-connection-for-an-oauth-request)の説明に従って [!DNL Oauth 2].0 接続を確立したら、必要に応じてモジュールの設定を続けます。すべての認証トークンは、このリクエストと、同じ接続を使用する他のリクエストに自動的に含まれます。

[!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 リクエストを作成]モジュールを構成すると、[!DNL Workfront Fusion] に以下のフィールドが表示されます。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>接続の設定の詳細については、この記事の <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">OAuth リクエスト用の接続を作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evaluate all states as errors (except for 2xx and 3xx]) </td> 
   <td> <p>エラー処理を設定するには、このオプションを使用します。</p> <p>詳しくは、<a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref"> [!DNL Adobe Workfront Fusion]</a> でのエラー処理 を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>API エンドポイント、ウェブサイトなど、リクエストの送信先 URL を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref"> [!DNL Adobe Workfront Fusion]</a> での HTTP リクエスト方法を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。例： <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> 目的のクエリのキーと値のペアを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Body type]</p> </td> 
   <td> <p>HTTP 本文は、使用するヘッダーがある場合、そのヘッダーの直後に HTTP トランザクションメッセージで送信されるデータバイトです。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Raw 本文タイプは、開発者向けドキュメントで送信するデータが指定されていない場合でも、通常、ほとんどの HTTP 本文リクエストに適しています。</p> <p>データを解析する形式を [!UICONTROL Content type] フィールドに指定します。</p> <p>選択したコンテンツタイプに関係なく、データは開発者ドキュメントで規定または必須されている形式で入力されます。</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>この本文タイプは、<code>[!UICONTROL application/x-www-form-urlencoded]</code> を使用したデータの投稿です。</p> <p><code>[!UICONTROL application/x-www-form-urlencoded]</code> の場合、サーバーに送信される HTTP メッセージの本文は基本的に 1 つのクエリ文字列になります。キーと値はキーと値のペアでエンコードされます。ペア同士は <code>&amp;</code> で区切られ、各ペアのキーと値の間には <code>=</code> が入ります。 </p> <p>バイナリデータの場合は、代わりに <code>use [!UICONTROL multipart/form-data]</code>。</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>例：</b></span></span> 
       <p>結果の HTTP リクエスト形式の例は、次のようになります。</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] は、ファイルとデータの送信に使用される HTTP マルチパートリクエストです。通常、ファイルをサーバーにアップロードする際に使用されます。</p> <p>リクエストで送信するフィールドを追加します。各フィールドには、キーと値のペアが含まれている必要があります。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Text]</strong> </p> <p>リクエスト本文内で送信するキーと値を入力します。</p> </li> 
       <li> <p><strong>[!UICONTROL File]</strong> </p> <p>キーを入力し、リクエスト本文で送信するソースファイルを指定します。</p> <p>前のモジュールからアップロードするファイルをマッピングするか（[!UICONTROL HTTP]／&lbrack;[!UICONTROL Get a File] または [!UICONTROL Google Drive]／[!UICONTROL Download a File]）、またはファイル名とファイルデータを手動で入力します。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse response]</p> </td> 
   <td> <p>このオプションを有効にすると、応答を自動的に解析し、JSON および XML 応答を変換するので、[!UICONTROL JSON]／[!UICONTROL Parse JSON] または [!UICONTROL XML]／[!UICONTROL Parse XML] モジュールを使用する必要がなくなります。</p> <p>解析された JSON または XML コンテンツを使用する前に、モジュールを手動で 1 回実行して、モジュールが応答コンテンツを認識し、後続のモジュールにマッピングできるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timeout] </td> 
   <td> <p>リクエストのタイムアウトを秒単位で入力します（1～300）。デフォルトは 40 秒です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Share cookies with other HTTP modules]</td> 
   <td> <p> このオプションを有効にすると、シナリオ内のすべての HTTP モジュールとサーバーから Cookie を共有できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-signed certificate]</td> 
   <td> <p> 自己署名証明書を使用して TLS を使用する場合は、証明書をアップロードします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reject connections that are using unverified (self-signed) certificates] </td> 
   <td> <p>このオプションを有効にすると、未検証の TLS 証明書を使用している接続を拒否できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow redirect]</td> 
   <td> <p> このオプションを有効にすると、3xx 応答で URL リダイレクトに従います。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Follow all redirects] </td> 
   <td> <p>このオプションを有効にすると、すべての応答コードで URL リダイレクトに従います。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Disable serialization of multiple same query string keys as arrays]</p> </td> 
   <td> <p>デフォルトでは、[!DNL Workfront Fusion] は、同じ URL クエリ文字列パラメーターキーの複数の値を配列として処理します。例えば、<code>www.test.com?foo=bar&amp;foo=baz</code> は <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code> に変換されます。このオプションをアクティブ化すると、この機能は無効になります。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Request compressed content]</td> 
   <td> <p> このオプションを有効にすると、web サイトの圧縮バージョンを要求できます。</p> <p>これにより、圧縮コンテンツを要求する <code>[!UICONTROL Accept-Encoding]</code> ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Use Mutual TLS]</td> 
   <td> <p>このオプションを有効にすると、HTTP リクエストで相互 TLS を使用できます。</p> <p>相互 TLS について詳しくは、<a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">HTTP モジュールでの相互 TLS の使用：[!DNL Adobe Workfront Fusion]</a> を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>
