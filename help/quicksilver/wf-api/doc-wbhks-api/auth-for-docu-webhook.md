---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメント web フックの認証
description: ドキュメント web フックの認証
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 100%

---

# ドキュメント web フックの認証

## 認証

Adobe Workfront ドキュメントの web フックでは、OAuth2 と ApiKey の 2 種類の認証形式をサポートしています。どちらの場合も、Workfront は API を呼び出す際に、認証トークンをヘッダーに入れて渡します。

### OAuth2

OAuth2 を使用すると、Workfront は、承認済み API 呼び出しをユーザーの代わりに web フックプロバイダーに対して行うことができます。その前に、ユーザーは外部ドキュメントプロバイダーアカウントを Workfront に接続し、Workfront への

アクセス権を付与して、ユーザーの代わりに操作できるようにする必要があります。このハンドシェイクプロセスは、ユーザーごとに 1 回だけ行われます。仕組みは次のとおりです。

1. まずユーザーが自分のアカウントに web フック統合を接続します。現在、これを行うには、「ドキュメントの追加」ドロップダウン／サービスを追加／カスタム統合名をクリックします。
1. Workfront により、ユーザーは認証 URL に移動します。ここでは、外部ドキュメントプロバイダーへのログインを求められる場合があります。このページは、web フックプロバイダーまたは外部ドキュメント管理システムによってホストされています。その際、Workfront は認証 URL に「state」パラメーターを追加します。同じ値を以下の手順で Workfront の戻り URI に追加することにより、この値を Workfront に返す必要があります。
1. 外部システムにログインしたら（またはユーザーが既にログインしている場合）、「認証」ページが表示され、ユーザーの代わりに一連のアクションを実行するためのアクセス権を Workfront が要求していることが説明されます。
1. ユーザーが「許可」ボタンをクリックすると、ブラウザーは Workfront リダイレクト URI にリダイレクトされ、その際にクエリ文字列に「code=`<code>`」が追加されます。OAuth2 仕様に従い、このトークンの有効期間は短く設定されています。クエリ文字列には「state=`<sent_by_workfront>`」も必要です。
1. Workfront はこのリクエストを処理し、認証コードを使用してトークンエンドポイント URL への API 呼び出しを行います。
1. トークンエンドポイント URL は、更新トークンとアクセストークンを返します。
1. Workfront はこれらのトークンを保存し、このユーザーに対して web フック統合を完全にプロビジョニングします。
1. これ以降、Workfront は web フックプロバイダーに対して、承認済み API 呼び出しを実行できるようになります。これらの呼び出しを行う際に、Workfront は、以下に示すように、アクセストークンを HTTP リクエストヘッダーに入れて送信します。

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. アクセストークンの有効期限が切れている場合、Workfront はトークンエンドポイント URL を呼び出して新しいアクセストークンを取得したあと、その新しいアクセストークンを使用して承認済み API 呼び出しを再度試みます。

### ApiKey

ApiKey を使用して web フックプロバイダーへの承認済み API 呼び出しを行う方が、OAuth2 よりもはるかに簡単です。API 呼び出しを行う際に、Workfront が ApiKey と Workfront ユーザー名を HTTP リクエストヘッダーに入れて渡すだけです。

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Web フックプロバイダーは、このユーザー名を使用して、ユーザー固有の権限を適用できます。この仕組みが最も効果を発揮するのは、両方のシステムがシングルサインオン（SSO）を使用して LDAP に接続している場合です。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
