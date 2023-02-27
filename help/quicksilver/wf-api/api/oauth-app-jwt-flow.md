---
content-type: api
navigation-topic: api-navigation-topic
title: カスタム OAuth 2 アプリケーションでの JWT フローの使用
description: カスタム OAuth 2 アプリケーションでの JWT フローの使用
author: Becky
feature: Workfront API
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# JWT フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する

Workfrontと統合し、クライアントアプリがユーザーの代わりにWorkfrontと通信できるようにするには、次の操作が必要です。

* OAuth2 アプリケーションの作成
* 公開鍵証明書の作成
* JSON Web トークン (JWT) の作成

## OAuth2 アプリケーションの作成

OAuth2 アプリケーションの作成手順については、 [サーバー認証を使用した OAuth2 アプリケーションの作成（JWT フロー）](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [Workfront統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## 公開鍵証明書の作成

JWT は、アクセス要求に含めるために署名され、base-64 エンコードされている必要があります。 JWT ライブラリは、これらのタスクを実行する関数を提供します。

トークンは、電子署名証明書の秘密鍵を使用して署名する必要があります。 その場合は、関連付けられている証明書の秘密鍵を使用して、JWT に署名できます。

使用されるアルゴリズムは、RS256（SHA-256 を使用した RSA Signature）です。 これは非対称のアルゴリズムで、公開鍵と秘密鍵のペアを使用します。 ID プロバイダーは、署名の生成に使用する秘密鍵を持ち、JWT のコンシューマーは、署名を検証するための公開鍵を取得します。

公開鍵を生成するには、次の操作を行います。 **1 つ** 以下のうちの 1 つ。

* MacOS/Linux ターミナルを開き、次のコマンドを実行してから、アップロードします。 `certificate_pub.crt` の使用 **公開鍵を追加** ボタン ( Workfrontの OAuth2 アプリケーション設定 )

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* 以下を使用： **公開鍵/秘密鍵のペアを生成** ボタン ( Workfrontでの OAuth2 アプリケーション設定 ) をクリックして、RSA を生成します。

## JSON Web トークンの作成

サービスアカウント認証用の JSON Web トークンには、特定の要求のセットが必要です。また、有効なデジタル署名証明書を使用して署名する必要があります。 JWT の構築には、公開されているライブラリまたはツールの 1 つを使用することをお勧めします。

次の表に、JWT トークンの設定時に必要となるフィールドに関する情報を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>必須. expiration パラメーターは、01/01/1970 GMT からの絶対時間を測定する必須のパラメーターです。 有効期限は、問題が発生した時刻よりも後にする必要があります。 この時間が経過すると、JWT は無効になります。 </p> <p>注意：非常に短い有効なトークン（数分）を持つことをお勧めします。その場合、アクセストークンと交換した後すぐに期限が切れます。 新しいアクセストークンが必要になるたびに、1 つの JWT が署名および交換されます。 これは、より安全なアプローチです。 必要に応じて、アクセストークンの取得に再利用する、長期間有効なトークンはお勧めしません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">is</td> 
   <td>必須. 発行者は、OAuth2 アプリの詳細からの顧客 ID です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>必須. 件名は、設定で公開鍵を作成したユーザー ID です。</td> 
  </tr> 
 </tbody> 
</table>

## JWT を交換してアクセストークンを取得する

1. POSTリクエストの送信先：

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. リクエストの本文には、クライアント ID、クライアントの秘密鍵、JWT を含む URL エンコードされたパラメーターを含める必要があります。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
