---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: http-modules
title: HTTP &gt;OAuth 2.0 リクエストモジュールを作成する
description: を作成するには、 [!DNL Adobe Workfront Fusion] OAuth 2.0 認証を必要とするサーバーに対する HTTP(S) リクエストを実行するには、まず OAuth 接続を作成する必要があります。 [!DNL Adobe Workfront Fusion] は、この接続でおこなわれたすべての呼び出しに適切な認証ヘッダーが付いていることを確認し、必要に応じて関連トークンを自動的に更新します。
author: Becky
feature: Workfront Fusion
exl-id: 6c68c9b9-9f74-44a7-94ed-3785081b8331
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2220'
ht-degree: 0%

---

# [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] にはが必要です [!DNL Adobe Workfront Fusion] に加えてライセンス [!DNL Adobe Workfront] ライセンス。

を作成するには、 [!DNL Adobe Workfront Fusion] OAuth 2.0 認証を必要とするサーバーに対する HTTP(S) リクエストを実行するには、まず OAuth 接続を作成する必要があります。 [!DNL Adobe Workfront Fusion] は、この接続でおこなわれたすべての呼び出しに適切な認証ヘッダーが付いていることを確認し、必要に応じて関連トークンを自動的に更新します。

[!DNL Workfront Fusion] は、次の OAuth 2.0 認証フローをサポートしています。

* 認証コードフロー
* 暗黙フロー

リソース所有者パスワード資格情報フローやクライアント資格情報フローなど、その他のフローは、このモジュールを通じて自動的にはサポートされません。

OAuth 2.0 認証について詳しくは、 [OAuth 2.0 承認フレームワーク](https://tools.ietf.org/html/rfc6749).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## の接続の作成 [!DNL OAuth] リクエスト

* [HTTP / OAuth 2.0 リクエストモジュールで接続を作成するための一般的な手順](#general-instructions-for-creating-a-connection-in-the-http--make-an-oauth-20-request-module)
* [HTTP でGoogleへの接続を作成する手順 >[!UICONTROL Make] OAuth 2.0 リクエストモジュール](#instructions-for-creating-a-connection-to-google-in-the-http-make-an-oauth-20-request-module)
* [HTTP / OAuth 2.0 リクエストモジュールを使用したMicrosoft Graph API への接続手順](#instructions-for-connecting-to-microsoft-graph-api-via-the-http--make-an-oauth-20-request-module)

### での接続の作成に関する一般的な手順 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール

1. で OAuth クライアントを作成します。 [!DNL target] 目的のサービス [!DNL Adobe Workfront Fusion] 通信する このオプションは、 [!UICONTROL 開発者] のセクションに含まれている必要があります。

   1. クライアントを作成する際に、適切な URL を `[!UICONTROL Redirect URL]` または `[!UICONTROL Callback URL]` フィールド：

      | 南北アメリカ/APAC | https://app.workfrontfusion.com/oauth/cb/oauth2 |
      |---|---|
      | EMEA | https://app-eu.workfrontfusion.com/oauth/cb/oauth2 |

   1. クライアントを作成すると、指定されたサービスは次の 2 つのキーを表示します。 `[!UICONTROL Client ID]` および `[!UICONTROL Client Secret]`. 一部のサービスでは、 `[!UICONTROL App Key]` および `[!UICONTROL App Secret]` . キーと秘密鍵を安全な場所に保存して、Workfront Fusion で接続を作成する際に指定できるようにします。

1. 次を検索： `[!UICONTROL Authorize URI]` および `[!UICONTROL Token URI]` （特定のサービスの API ドキュメント内）を参照してください。 URL アドレスを使用し、 [!DNL Workfront Fusion] が [!DNL target] サービス。 アドレスは OAuth 認証に使用されます。

   >[!NOTE]
   >
   >サービスで暗黙的なフローを使用する場合、 `[!UICONTROL Authorize URI]`.

   >[!INFO]
   >
   >**例：** Yahoo アドレス：
   >
   >* URI を許可：
   >
   >`https://api.login.yahoo.com/oauth2/request_auth`
   >
   >* トークン URI:
   >
   >`https://api.login.yahoo.com/oauth2/get_token`

1. （条件付き）ターゲットサービスでスコープ（アクセス権）を使用する場合、サービスで個々のスコープがどのように区切られるかを確認し、それに応じて詳細設定で区切り文字を設定してください。 区切り文字が正しく設定されていない場合、 [!DNL Workfront Fusion] 接続の作成に失敗し、無効なスコープエラーが発生しました。
1. 上記の手順を完了したら、で OAuth 接続の作成を開始できます。 [!DNL Workfront Fusion]. OAuth 2.0 HTTP(S) リクエストおよび応答処理モジュールをシナリオに追加します。
1. モジュールの「接続」フィールドで、 **[!UICONTROL 追加]**.

1. 次のフィールドに入力して、接続を作成します。

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 接続名 ] </td> 
      <td> <p>接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL フロータイプ ]</p> </td> 
      <td> <p>トークンを取得するフローを選択します。</p> 
       <ul> 
        <li><strong>[!UICONTROL 認証コード ]</strong>:次を入力します。 <code>[!UICONTROL Authorize URI]</code> および <code>[!UICONTROL Token URI]</code> を参照してください。</li> 
        <li><strong>[!UICONTROL 暗黙 ]</strong>:次を入力します。 <code>[!UICONTROL Authorize URI]</code> を参照してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL スコープ ] </td> 
      <td> <p>個々のスコープを追加します。 この情報は、特定のサービスの開発者向けドキュメント (API) に記載されています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL スコープ区切り文字 ] </td> 
      <td> <p>上に入力したスコープを区切る範囲を選択します。 この情報は、特定のサービスの開発者向けドキュメント (API) に記載されています。</p> <p>警告：区切り文字が正しく設定されていない場合、 [!DNL Workfront Fusion] 接続の作成に失敗し、無効なスコープエラーが表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント ID] </td> 
      <td> <p>クライアント ID を入力します。 クライアント ID は、接続するサービスで OAuth クライアントを作成したときに取得されました。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td> 
      <td> <p> クライアントの秘密鍵を入力します。 接続するサービスで OAuth クライアントを作成したときに、クライアントシークレットを取得しました。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL パラメーターを許可 ]</p> </td> 
      <td> <p>認証呼び出しに含めるパラメーターを追加します。 次の標準パラメーターは常に自動的に含まれ、追加する必要はありません。</p> <p>標準パラメーター：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL response_type]</strong> </p> <p> <code>code </code>([!UICONTROL 認証コードフロー ] および <code>token </code>（[!UICONTROL 暗黙的フロー ] の場合）</p> </li> 
        <li> <p><strong>[!UICONTROL redirect_uri]</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">南北アメリカ/APAC</td> 
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
      <td role="rowheader"> <p>[!UICONTROL アクセストークンパラメーター ]</p> </td> 
      <td> <p>トークン呼び出しに含めるパラメーターを追加します。 次の標準パラメーターは常に自動的に含まれ、追加する必要はありません。</p> <p>標準パラメーター：</p> 
       <ul> 
        <li><strong>[!UICONTROL grant_type]</strong>: <code>authorization_code</code></li> 
        <li> <p><strong>[!UICONTROL redirect_uri]:</strong> </p> 
         <table style="table-layout:auto">  
          <col> 
          <col> 
          <tbody> 
           <tr> 
            <td role="rowheader">南北アメリカ/APAC</td> 
            <td>https://app.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
           <tr> 
            <td role="rowheader">EMEA </td> 
            <td>https://app-eu.workfrontfusion.com/oauth/cb/oauth2</td> 
           </tr> 
          </tbody> 
         </table> </li> 
        <li><strong>[!UICONTROL client_id]</strong>:アカウントの作成時に受け取ったクライアント ID は、リクエスト本文に自動的に含まれます</li> 
        <li><strong>client_secret</strong>:アカウントの作成時に受け取ったクライアント秘密鍵は、リクエスト本文に自動的に含まれます</li> 
        <li><strong>コード</strong>:認証リクエストによって返されるコード</li> 
       </ul> <p>メモ:  <p>OAuth 2.0 標準は、この手順で少なくとも 2 つのクライアント認証方法 (<code>[!UICONTROL client_secret_basic]</code> および <code>[!UICONTROL client_secret_post]</code>) をクリックします。 [!DNL Workfront Fusion] は、 <code>[!UICONTROL client_secret_post]</code> メソッド。 したがって、これらのパラメーターは、トークンのリクエスト本文に自動的に含まれます。 </p> <p>OAuth 2.0 認証について詳しくは、 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 承認フレームワーク</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL トークンパラメーターを更新 ]</p> </td> 
      <td> <p>トークン呼び出しに含めるパラメーターを追加します。 次の標準パラメーターは常に自動的に含まれ、追加する必要はありません。</p> <p>標準パラメーター：</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL grant_type]</strong>: <code>refresh_token</code></p> </li> 
        <li> <p><strong>[!UICONTROL refresh_token]</strong>:接続しているサービスで取得された最新の更新トークン</p> </li> 
        <li> <p><strong>[!UICONTROL client_id]</strong>:アカウントの作成時に受け取ったクライアント ID は、リクエスト本文に自動的に含まれます</p> </li> 
        <li> <p><strong>[!UICONTROL client_secret]</strong>:アカウントの作成時に受け取ったクライアント秘密鍵は、リクエスト本文に自動的に含まれます</p> </li> 
       </ul> <p>メモ:  <p>OAuth 2.0 標準は、この手順で少なくとも 2 つのクライアント認証方法 (<code>[!UICONTROL client_secret_basic]</code> および <code>[!UICONTROL client_secret_post]</code>) をクリックします。 [!DNL Workfront Fusion] は、 <code>[!UICONTROL client_secret_post]</code> メソッド。 したがって、これらのパラメーターは、トークンのリクエスト本文に自動的に含まれます。 </p> <p>OAuth 2.0 認証について詳しくは、 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 承認フレームワーク</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL カスタムヘッダー ]</p> </td> 
      <td> <p>[!UICONTROL トークン ] および R[!UICONTROL 更新トークン ] の手順のヘッダーに含める追加のキーと値を指定します。</p> <p>メモ:  <p>OAuth 2.0 標準は、この手順で少なくとも 2 つのクライアント認証方法 (<code>[!UICONTROL client_secret_basic]</code> および <code>[!UICONTROL client_secret_post]</code>) をクリックします。 [!DNL Workfront Fusion] は自動的にはをサポートしません <code>[!UICONTROL client_secret_basic]</code> メソッド。 接続するサービスで、クライアント ID とクライアント秘密鍵が 1 つの文字列に結合され、Authorization ヘッダーに base64 がエンコードされると想定される場合は、そのヘッダーとキーの値をここに追加する必要があります。</p> <p> OAuth 2.0 認証について詳しくは、 <a href="https://tools.ietf.org/html/rfc6749">OAuth 2.0 承認フレームワーク</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL トークンの配置 ]</p> </td> 
      <td> <p>指定した URL に接続する際に、[!UICONTROL ヘッダー ]、[!UICONTROL クエリ文字列 ]、またはその両方でトークンを送信するかどうかを選択します。</p> <p>トークンは、最も一般的にリクエストヘッダーで送信されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ヘッダートークン名 ] </td> 
      <td> <p>ヘッダーに認証トークンの名前を入力します。 デフォルト: <code>[!UICONTROL Bearer]</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クエリー文字列パラメーター名 ] </td> 
      <td> <p>クエリ文字列に認証トークンの名前を入力します。 デフォルト: <code>[!UICONTROL access_token]</code>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]** 接続設定を保存します。
1. 続行 [OAuth 2.0 リクエストモジュールのセットアップ](#oauth-20-request-module-setup).

### への接続を作成する手順 [!DNL Google] 内 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 リクエストモジュールを作成する]

次の例は、 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 を作成する] 接続するモジュールを要求 [!DNL Google].

1. プロジェクトを作成し、OAuth 設定を指定し、資格情報を生成していることを確認します ( [接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントの使用](../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).
1. を開きます。 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 リクエストを作成] モジュール。
1. クリック **[!UICONTROL 追加]** をクリックします。
1. 次の値を入力します。

   <table style="table-layout:auto">  
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 接続名 ] </td> 
      <td> <p>接続の名前を入力します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL フロータイプ ]</p> </td> 
      <td> <p>[!UICONTROL 認証コード ]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URI を許可 ]</td> 
      <td><code>https://accounts.google.com/o/oauth2/v2/auth</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL トークン URI]</td> 
      <td><code>https://www.googleapis.com/oauth2/v4/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL スコープ ] </td> 
      <td> <p>個々のスコープを追加します。 スコープの詳細については、 <a href="https://developers.google.com/identity/protocols/oauth2/scopes">の OAuth 2.O スコープ [!DNL Google] API</a> 内 [!DNL Google] ドキュメント。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL スコープ区切り文字 ] </td> 
      <td> <p>[!UICONTROL スペース ]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント ID] </td> 
      <td> <p>を入力します。 [!DNL Google] クライアント ID。 </p> <p>クライアント ID を作成するには、 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth 資格情報を作成</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントの使用</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td> 
      <td> <p>を入力します。 [!DNL Google] クライアント秘密鍵。 </p> <p>クライアントシークレットを作成するには、 <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md#create2" class="MCXref xref">OAuth 資格情報を作成</a> in <a href="../../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md" class="MCXref xref">[!DNL Connect Adobe Workfront Fusion] から [!DNL Google] カスタム OAuth クライアントを使用するサービス</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL パラメーターを許可 ]</p> </td> 
      <td> <p>追加 <code>[!UICONTROL access_type]</code> - <code>[!UICONTROL offline] </code>キーと値のペアとして渡すことができます。</p> <p> <img src="assets/google-authentication-http.png"> </p> <p>注意：トークンの更新など、認証に関する問題が発生した場合は、 <code>[!UICONTROL prompt] </code>- <code>[!UICONTROL consent] </code>キーと値のペアとして渡すことができます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]** 接続設定を保存します。
1. 続行 [OAuth 2.0 リクエストモジュールのセットアップ](#oauth-20-request-module-setup).

### への接続手順 [!DNL Microsoft Graph API] 経由 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール

に関する手順については、 [!DNL Microsoft Graph API]を参照してください。 [を [!DNL MS Graph REST API] 経由 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール](../../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md).

## OAuth 2.0 リクエストモジュールのセットアップ

を設定し、 [!DNL Oauth 2].0 接続 ( [の接続の作成 [!DNL OAuth] リクエスト](#creating-a-connection-for-an-oauth-request)必要に応じて、モジュールの設定を続行します。 すべての認証トークンは、このリクエストと、同じ接続を使用する他のすべてのリクエストに自動的に含まれます。

次を設定する場合、 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 リクエストを作成] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<!--
<img src="assets/map-toggle-350x74.png" style="width: 350;height: 74;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続の設定について詳しくは、 <a href="#creating-a-connection-for-an-oauth-request" class="MCXref xref">OAuth 要求の接続の作成</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL すべての状態をエラーとして評価（2xx および 3xx を除く） </td> 
   <td> <p>エラー処理を設定するには、このオプションを使用します。</p> <p>詳しくは、 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">でのエラー処理 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>API エンドポイント、Web サイトなど、リクエストの送信先 URL を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。 以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> 目的のクエリのキーと値のペアを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 本文の種類 ]</p> </td> 
   <td> <p>HTTP Body は、使用するヘッダーがある場合、そのヘッダーの直後に HTTP トランザクションメッセージで送信されるデータバイトです。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Raw body タイプは、開発者向けドキュメントで送信するデータが指定されていない場合でも、通常、ほとんどの HTTP body リクエストに適しています。</p> <p>データを解析する形式を「[!UICONTROL コンテンツタイプ ]」フィールドに指定します。</p> <p>選択したコンテンツタイプにもかかわらず、デベロッパードキュメントで規定または必要な任意の形式でデータが入力されます。</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>この本文タイプは、 <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>の場合 <code>[!UICONTROL application/x-www-form-urlencoded]</code>を指定した場合、サーバーに送信される HTTP メッセージの本文は基本的に 1 つのクエリ文字列になります。 キーと値は、 <code>&amp;</code> そして <code>=</code> キーと値の間。 </p> <p>バイナリデータの場合、 <code>use [!UICONTROL multipart/form-data]</code> 代わりに、</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>例: </b></span></span> 
       <p>結果の HTTP リクエスト形式の例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] は、ファイルとデータの送信に使用される HTTP マルチパートリクエストです。 通常、ファイルをサーバーにアップロードする際に使用されます。</p> <p>リクエストで送信するフィールドを追加します。 各フィールドには、キーと値のペアを含める必要があります。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL テキスト ]</strong> </p> <p>リクエスト本文内で送信するキーと値を入力します。</p> </li> 
       <li> <p><strong>[!UICONTROL ファイル ]</strong> </p> <p>キーを入力し、リクエスト本文で送信するソースファイルを指定します。</p> <p>前のモジュールからアップロードするファイルをマッピングする ([!UICONTROL HTTP] &gt;[!UICONTROL ファイルを取得 ] または [!UICONTROL Google Drive] &gt;[!UICONTROL ファイルをダウンロード )) か、ファイル名とファイルデータを手動で入力します。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 応答を解析 ]</p> </td> 
   <td> <p>このオプションを有効にすると、応答を自動的に解析し、JSON および XML 応答を変換して、[!UICONTROL JSON] / [!UICONTROL JSON を解析 ] または [!UICONTROL XML] / [!UICONTROL XML] モジュールを使用する必要がなくなります。</p> <p>解析された JSON または XML コンテンツを使用する前に、モジュールを手動で 1 回実行して、モジュールが応答コンテンツを認識し、後続のモジュールにマッピングできるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タイムアウト ] </td> 
   <td> <p>リクエストのタイムアウト（秒単位）(1 ～ 300) を入力します。 デフォルトは 40 秒です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 他の HTTP モジュールとの Cookie の共有 ]</td> 
   <td> <p> このオプションを有効にすると、シナリオ内のすべての HTTP モジュールとサーバーから Cookie を共有できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 自己署名証明書 ]</td> 
   <td> <p> 自己署名証明書を使用して TLS を使用する場合は、証明書をアップロードします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 未検証（自己署名）証明書を使用している接続を拒否します ] </td> 
   <td> <p>未検証の TLS 証明書を使用している接続を拒否する場合は、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リダイレクトに従う ]</td> 
   <td> <p> このオプションを有効にすると、3xx 応答で URL リダイレクトに従います。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL すべてのリダイレクトに従う ] </td> 
   <td> <p>このオプションを有効にすると、すべての応答コードで URL リダイレクトに従います。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 配列と同じ複数のクエリ文字列キーのシリアル化を無効にする ]</p> </td> 
   <td> <p>デフォルトでは、 [!DNL Workfront Fusion] は、配列と同じ URL クエリー文字列パラメーターキーに対する複数の値を処理します。 例： <code>www.test.com?foo=bar&amp;foo=baz</code> が次に変換されます： <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. この機能を無効にするには、このオプションを有効にします。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 圧縮コンテンツをリクエスト ]</td> 
   <td> <p> Web サイトの圧縮バージョンを要求するには、このオプションを有効にします。</p> <p>これにより、 <code>[!UICONTROL Accept-Encoding]</code> 圧縮コンテンツをリクエストするヘッダー。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 相互 TLS を使用 ]</td> 
   <td> <p>HTTP リクエストで相互 TLS を使用するには、このオプションを有効にします。</p> <p>相互 TLS について詳しくは、 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">の HTTP モジュールでの相互 TLS の使用 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
