---
content-type: api
navigation-topic: api-navigation-topic
title: カスタム OAuth 2 アプリケーションでの JWT フローの使用
description: カスタム OAuth 2 アプリケーションでの JWT フローの使用
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 100%

---

# JWT フローを使用した組織のカスタム OAuth 2 アプリケーションの設定と使用

Workfront と統合し、クライアントアプリがユーザーの代わりに Workfront と通信できるようにするには、次の操作が必要です。

* OAuth2 アプリケーションを作成
* 公開鍵証明書の作成
* JSON web トークン（JWT）の作成

## OAuth2 アプリケーションを作成

OAuth2 アプリケーションの作成手順については、[Workfront 統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)の[サーバー認証（JWT フロー）を使用した OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2)を参照してください。

## 公開鍵証明書の作成

JWT をアクセスリクエストに含めるには、署名し Base 64 でエンコードする必要があります。JWT ライブラリには、これらのタスクを実行する関数が用意されています。

トークンは、デジタル署名証明書の秘密鍵を使用して署名する必要があります。その場合は、関連付けられている任意の証明書の秘密鍵を使用して、JWT に署名することができます。

使用されるアルゴリズムは、RS256（SHA-256 を使用した RSA 署名）です。これは非対称アルゴリズムで、公開鍵と秘密鍵のペアを使用します。ID プロバイダーは署名の生成に使用される秘密（プライベート）鍵を持ち、JWT のコンシューマーは署名を検証するための公開鍵を取得します。

公開鍵を生成するには、次のうちの&#x200B;**いずれか一方**&#x200B;を行います。

* MacOS／Linux ターミナルを開いて次のコマンドを実行したあと、Workfront の OAuth2 アプリケーション設定で「**公開鍵を追加**」ボタンを使用して、`certificate_pub.crt` をアップロードします。

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Workfront での OAuth2 アプリケーション設定で「**公開鍵 / 秘密鍵のペアを生成**」ボタンを使用して、RSA を生成します。

## JSON web トークンの作成

サービスアカウント認証用の JSON web トークンは、特定の要求のセットを必要とします。また、有効なデジタル署名証明書を使用して署名する必要があります。JWT の作成には、公開されているライブラリまたはツールの 1 つを使用することをお勧めします。

JWT トークンの設定時に必要となる可能性のあるフィールドに関する情報を次の表に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>必須。有効期限パラメーターは、1970年1月1日 GMT 以降の絶対時間を測定する必須のパラメーターです。有効期限がイシューの発生日時よりも必ず後になるようにする必要があります。この時間が経過すると、JWT は無効になります。 </p> <p>メモ：アクセストークンと交換された後すぐに期限切れになるように、有効期間が非常に短いトークン（数分）を使用することをお勧めします。新しいアクセストークンが必要になるたびに、1 つの JWT が署名され、交換されます。これは、より安全なアプローチになります。必要に応じてアクセストークンを取得するために再利用される、有効期間の長いトークンはお勧めしません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">iss</td> 
   <td>必須。発行元は、OAuth2 アプリの詳細から得られる顧客 ID です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>必須。サブジェクトは、設定時に公開鍵を作成したユーザー ID です。</td> 
  </tr> 
 </tbody> 
</table>

## アクセストークンを取得するための JWT の交換

1. 以下に POST リクエストを送信します。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. リクエストの本文には、クライアント ID、クライアントシークレットおよび JWT を含む URL エンコードされたパラメーターが含まれている必要があります。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
