---
content-type: api
navigation-topic: api-navigation-topic
title: OAuth 2 アプリケーションでの PKCE フローの使用
description: OAuth 2 アプリケーションでの PKCE フローの使用
author: Becky
feature: Workfront API
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# PKCE フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する

PKCE は、モバイルアプリケーションなどの動的に更新するアプリケーションで適切に機能する、安全な認証フローですが、すべての OAuth2 クライアントで役立ちます。 PKCE では、静的なクライアントシークレットの代わりに動的に生成された文字列を使用するので、クライアントシークレットの漏洩を防ぐことができます。

## PKCE の概要

PKCE フローには、次の手順が含まれます。 この節の手順は、詳細についてのみ説明しています。 これらの手順を実行するには、この記事の他の節を参照してください。

1. クライアントが `code_challenge` 変身させて `code_verifier` using `S256` 暗号化。

1. クライアントは、生成された `code_challenge`. OAuth2 が認証要求を受け入れられるように、アプリ（クライアント）を登録する必要があります。 登録後、アプリはブラウザーを OAuth2 にリダイレクトできます。

1. OAuth2 認証サーバーは、認証プロンプトをユーザーにリダイレクトします。

1. ユーザーが、設定済みのログインオプションの 1 つを使用して認証をおこなうと、OAuth2 がアプリケーションに付与する権限をリストする同意ページが表示される場合があります。

1. OAuth2 は、 `authorization code`.

1. アプリケーションは、このコードと共にを送信します。 `code_verifier`を OAuth2 に追加します。

1. OAuth2 認証サーバーが `code_verifier` の使用 `code_challenge_method` を最初の認証リクエストから削除し、結果を `code_challenge`. 両方の文字列の値が一致する場合、サーバーは、要求が同じクライアントから送信されたことを検証し、 `access token`.

1. OAuth2 は `access token`、およびオプションで `refresh token`.

1. これで、アプリケーションはこれらのトークンを使用して、ユーザーに代わって API などのリソースサーバーを呼び出すことができます。

1. リソースサーバーは、リクエストに応答する前にトークンを検証します。


## アプリケーションの設定

認証を実装する前に、Workfrontからアプリの統合を作成して、アプリを OAuth2 に登録する必要があります。

OAuth2 アプリケーションの作成手順については、 [PKCE を使用した OAuth2 シングルページ Web アプリケーションの作成 ](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Workfront統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)


## コード交換用の配達確認キーの作成

標準の認証コードフローと同様に、アプリは最初に、ユーザーのブラウザーを認証サーバーの `/authorize` endpoint. ただし、このインスタンスでは、コードチャレンジに沿ってを渡す必要もあります。

最初の手順は、コード検証者と課題を生成することです。

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">コード検証者</td>
        <td>
          <p>最小長が 43 文字のランダムな URL セーフ文字列</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">コードの課題</td>
        <td>
          <p>Base64 コード検証者の URL エンコードされた SHA-256 ハッシュ</p>
        </td>
      </tr>
    </tbody>
</table>


コード検証者とコードチャレンジを作成するには、クライアントアプリにコードを追加する必要があります。

PKCE ジェネレーターコードは、次のような出力を作成します。

>[!INFO]
>
>**例:**
>
>```
>{
>
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>
>}
>```

アプリが `code_verifier` の場合は後で、を `code_challenge` お使いの認証サーバーの `/authorize` URL。

## 認証コードのリクエスト

デフォルトのカスタム認証サーバーを使用している場合、リクエスト URL は次のようになります。

>[!INFO]
>
>**例:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

渡されるパラメーターに注意してください。

* `client_id` は、アプリケーションの設定時にで作成した OAuth2 アプリケーションのクライアント ID を照合します。

   手順については、「 Workfront統合用の OAuth2 アプリケーションの作成」の「 PKCE を使用した OAuth2 シングルページ Web アプリケーションの作成」を参照してください。

* `response_type` が `code`の場合は、アプリケーションが承認コード付与タイプを使用するので、

* `redirect_uri` は、ユーザーエージェントが `code`. OAuth2 アプリケーションの作成時に指定したリダイレクト URL の 1 つと一致する必要があります。

* `code_challenge_method` は、チャレンジの生成に使用するハッシュメソッドです。常に `S256` (PKCE を使用するWorkfront Oauth2 アプリケーションの場合 )

* `code_challenge` は、PKCE で使用されるコードチャレンジです。


## トークンのコードを交換する

アクセストークンの認証コードを交換するには、認証サーバーの `/token` エンドポイントと `code_verifier`.

>[!INFO]
>
>**例:**
>
>```
>/token \\
>
>  --header 'accept: application/json' \\
>
>  --header 'cache-control: no-cache' \\
>
>  --header 'content-type: application/x-www-form-urlencoded' \\
>
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> 通常の認証コードフローとは異なり、この呼び出しでは、クライアント ID とシークレットを含む Authorization ヘッダーは必要ありません。 そのため、このバージョンの認証コードフローは、バックエンドを持たないモバイルアプリケーションやシングルページアプリケーションなどのネイティブアプリに適しています。

渡されるパラメーターに注意してください。

* `grant_type` が `authorization_code`付与タイプは認証コードを使用するので、

* `redirect_uri` は、認証コードの取得に使用された URI と一致する必要があります。

* `code` は、/authorize エンドポイントから受け取った認証コードです。

* `code_verifier` は、アプリがで生成した PKCE コード検証ツールです。 [コード交換用の配達確認キーの作成](#Create).

* `client_id` はクライアントを識別し、OAuth2 で事前に登録されている値と一致する必要があります。


コードが引き続き有効で、コード検証が一致する場合は、アプリケーションがアクセストークンを受け取ります。

>[!INFO]
>
>**例:**
>
>```
>{
>
>    "access\_token": "eyJhd\[...\]Yozv",
>
>    "expires\_in": 3600,
>
>    "token\_type": "Bearer"
>
>}
>```

## アクセストークンの検証

アプリケーションがアクセストークンを使用して要求を渡す場合、リソースサーバーはその要求を検証する必要があります。

次のような API 呼び出しを使用して、アクセストークンを検証できます。

>[!INFO]
>
>**例:**
>
>```
>/attask/api/<api version>/proj/search \\
>
>  --header 'sessionID: <access\_token>' \\
>```

## 更新トークンのリクエスト

更新トークンをリクエストするには、次のように、API に対してPOST呼び出しを実行します。

>[!INFO]
>
>**例:**
>
>```
>/token \\
>
>  --header 'accept: application/json' \\
>
>  --header 'cache-control: no-cache' \\
>
>  --header 'content-type: application/x-www-form-urlencoded' \\
>
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
