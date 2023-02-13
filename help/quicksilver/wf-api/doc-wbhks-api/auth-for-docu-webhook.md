---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメント Web フックの認証
description: ドキュメント Web フックの認証
author: John
feature: Workfront API
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# ドキュメント Web フックの認証

## 認証

Adobe Workfront Document Webhook は、次の 2 種類の認証形式をサポートしています。OAuth2 および ApiKey。 どちらの場合も、Workfrontは API 呼び出しをおこなう際に、ヘッダーで認証トークンを渡します。

### OAuth2

OAuth2 を使用すると、Workfrontは、ユーザーに代わって Webhook プロバイダーに対して承認済みの API 呼び出しをおこなうことができます。 その前に、ユーザーは外部のドキュメントプロバイダーのアカウントをWorkfrontに接続し、Workfrontに付与する必要があります

自分の代理として行動するためのアクセス権 このハンドシェイクプロセスは、各ユーザーに対して 1 回だけ発生します。 仕組みは次のとおりです。

1. ユーザーが Webhook 統合のアカウントへの接続を開始します。 現在、これは「ドキュメントの追加」ドロップダウン/「サービスを追加」/「カスタム統合名」をクリックすることでおこなわれます。
1. Workfrontはユーザーに認証 URL を移動します。この URL は、ユーザーに外部のドキュメントプロバイダーへのログインを促す場合があります。 このページは、Webhook プロバイダーまたは外部ドキュメント管理システムによってホストされます。 その際、Workfrontは認証 URL に「state」パラメーターを追加します。 この値は、以下の手順で同じ値をWorkfrontの戻り URI に追加して、Workfrontに渡す必要があります。
1. 外部システムにログインした後（またはユーザーが既にログインしている場合）、「認証」ページが表示され、Workfrontがユーザーに代わって一連のアクションを実行するためのアクセスを要求していることを説明します。
1. ユーザーが「許可」ボタンをクリックすると、ブラウザーは、「code=`<code>`」をクエリ文字列に追加します。 OAuth2 仕様に従い、このトークンは短期間有効です。 クエリ文字列には、「state=`<sent_by_workfront>`&quot;.
1. Workfrontはこのリクエストを処理し、認証コードを使用してトークンエンドポイント URL への API 呼び出しをおこないます。
1. トークンエンドポイント URL は、更新トークンとアクセストークンを返します。
1. Workfrontはこれらのトークンを保存し、このユーザーに対して webhook 統合を完全にプロビジョニングします。
1. これ以降、Workfrontは Webhook プロバイダーに対して認証済みの API 呼び出しをおこなうことができます。 これらの呼び出しをおこなう場合、Workfrontは、次に示すように HTTP リクエストヘッダーでアクセストークンを送信します。

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. アクセストークンの有効期限が切れている場合、Workfrontはトークンエンドポイント URL を呼び出して新しいアクセストークンを取得し、新しいアクセストークンを使用して認証済み API 呼び出しを再試行します。

### ApiKey

ApiKey を使用して Webhook プロバイダーに対して承認された API 呼び出しをおこなう方が、OAuth2 よりもはるかに簡単です。 API 呼び出しをおこなう場合、Workfrontは HTTP リクエストヘッダーに ApiKey とWorkfrontのユーザー名を渡します。 

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook プロバイダーは、ユーザー名を使用して、ユーザー固有の権限を適用できます。 これは、両方のシステムがシングルサインオン (SSO) を使用して LDAP に接続する場合に最も適しています。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of “username:password”. See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
