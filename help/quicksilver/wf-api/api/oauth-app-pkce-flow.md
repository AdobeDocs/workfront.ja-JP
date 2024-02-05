---
content-type: api
navigation-topic: api-navigation-topic
title: OAuth 2 アプリケーションでの PKCE フローの使用
description: OAuth 2 アプリケーションでの PKCE フローの使用
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 100%

---

# PKCE フローを使用した、組織のカスタム OAuth 2 アプリケーションの設定と使用

PKCE は、モバイルアプリなどの動的に更新するアプリケーションでうまく機能するセキュアな認証フローですが、すべての OAuth2 クライアントで役に立ちます。PKCE では、静的なクライアントシークレットではなく、動的に生成された文字列を使用するので、クライアントシークレットの漏洩のリスクを排除できます。

## PKCE の概要

PKCE フローには、以下の手順が含まれます。この節の手順は、情報についてのみ説明しています。これらの手順を実行するには、この記事の他の節を参照してください。

1. クライアントは、`S256` 暗号化を使用して `code_verifier` を変換することにより、`code_challenge` を作成します。

1. クライアントは、生成された `code_challenge` とともに、ブラウザーを OAuth2 サインインページに移動します。OAuth2 が認証要求を受け入れられるように、アプリ（クライアント）を登録する必要があります。登録後、アプリはブラウザーを OAuth2 にリダイレクトできます。

1. OAuth2 認証サーバーは、認証プロンプトをユーザーにリダイレクトします。

1. ユーザーは、設定されたログインオプションの 1 つを使用して認証すると、OAuth2 がアプリケーションに与える権限を一覧表示した同意ページが表示される場合があります。

1. OAuth2 は、`authorization code` を使用してアプリケーションにリダイレクトします。

1. アプリケーションは、`code_verifier` と併せて、このコードを OAuth2 に送信します。

1. OAuth2 認可サーバーは、最初の認可リクエストからの `code_challenge_method` を使用して `code_verifier` を変換し、その結果を `code_challenge` と照合します。両方の文字列の値が一致する場合、サーバーは、リクエストが同じクライアントから送信されたことを検証し、`access token` を発行します。

1. OAuth2 は `access token`、およびオプションとして `refresh token` を返します。

1. これで、アプリケーションはこれらのトークンを使用して、ユーザーに代わって API などのリソースサーバーを呼び出すことができます。

1. リソースサーバーは、リクエストに応答する前にトークンを検証します。


## アプリケーションの設定

認証を実装する前に、Workfront からアプリの統合を作成して、アプリを OAuth2 に登録する必要があります。

OAuth2 アプリケーションの作成手順については、[Workfront 統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)にある、[PKCE を使用した OAuth2 単一ページ web アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce)を参照してください。


## コード交換用のプルーフキーの作成

標準の認可コードフローと同様に、アプリはユーザーのブラウザーを認可サーバーの `/authorize` エンドポイントにリダイレクトすることから開始します。ただし、この場合はコードチャレンジも渡す必要があります。

最初の手順は、コードベリファイアおよびコードチャレンジを生成することです。

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">コードベリファイア</td>
        <td>
          <p>43 文字以上ののランダムな URL 対応文字列</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">コードチャレンジ</td>
        <td>
          <p>コードベリファイアの Base64 URL エンコードされた SHA-256 ハッシュ</p>
        </td>
      </tr>
    </tbody>
</table>


コードベリファイアおよびコードチャレンジを生成するには、クライアントアプリにコードを追加する必要があります。

PKCE ジェネレーターコードは、次のような出力を作成します。

>[!INFO]
>
>**例：**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

アプリは後で使用できるように `code_verifier` を保存し、`code_challenge` を認可リクエストとともに認可サーバーの `/authorize` URL に送信します。

## 認証コードのリクエスト

デフォルトのカスタム認証サーバーを使用している場合、リクエスト URL は以下のようになります。

>[!INFO]
>
>**例：**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

渡されるパラメーターに注意してください。

* `client_id` は、アプリケーションの設定時に作成した OAuth2 アプリケーションのクライアント ID と一致します。

  手順については、Workfront 統合用の OAuth2 アプリケーションの作成にある、PKCE を使用した OAuth2 単一ページ web アプリケーションの作成を参照してください。

* `response_type` は `code` です。これは、アプリケーションが認証コード付与タイプを使用するためです。

* `redirect_uri` は、ユーザーエージェントが `code` とともにリダイレクトされるコールバックの場所です。これは、OAuth2 アプリケーションの作成時に指定したリダイレクト URL の 1 つと一致する必要があります。

* `code_challenge_method` はチャレンジの生成に使用されるハッシュメソッドであり、PKCE を使用する Workfront Oauth2 アプリケーションの場合は常に `S256` です。

* `code_challenge` は、PKCE で使用されるコードチャレンジです。


## トークンのコードの交換

認証コードをアクセストークンと交換するには、認証コードを `code_verifier` とともに認証サーバーの `/token` エンドポイントに渡します。

>[!INFO]
>
>**例：**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> 通常の認証コードフローとは異なり、この呼び出しには、クライアント ID とクライアントシークレットを含む認証ヘッダーは必要ありません。そのため、このバージョンの認証コードフローは、バックエンドを持たないモバイルアプリケーションやシングルページアプリケーションなどのネイティブアプリケーションに適しています。

渡されるパラメーターに注意してください。

* `grant_type` は `authorization_code` です。これは、アプリが認証コード付与タイプを使用するためです。

* `redirect_uri` は、認証コードの取得に使用された URI と一致する必要があります。

* `code` は、/authorize エンドポイントから受け取った認証コードです。

* `code_verifier` は、[ コード交換用の証明キーを作成する ](#Create) でアプリが生成した PKCE コード検証ツールです。

* `client_id` はクライアントを識別し、OAuth2 で事前に登録されている値と一致する必要があります。


コードが引き続き有効で、コード検証が一致する場合は、アプリケーションがアクセストークンを受け取ります。

>[!INFO]
>
>**例：**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## アクセストークンの検証

アプリケーションがアクセストークンを使用してリクエストを渡す場合、リソースサーバーはそのリクエストを検証する必要があります。

次のような API 呼び出しを使用して、アクセストークンを検証できます。

>[!INFO]
>
>**例：**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## 更新トークンのリクエスト

更新トークンをリクエストするには、次のように、API に対して POST 呼び出しを実行します。

>[!INFO]
>
>**例：**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
