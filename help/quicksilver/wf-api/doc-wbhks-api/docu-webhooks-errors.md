---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Document Webhooks エラー処理
description: Document Webhooks エラー処理
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 0%

---

# Document Webhooks エラー処理

問題は、API リクエストを処理する際に発生する可能性があります。 これは、すべての API エンドポイントで一貫した方法で処理する必要があります。 エラーが発生した場合、Webhook プロバイダーは応答ヘッダーにエラーコードを含める必要があります。 次のエラーコードが含まれます。

* 403 — 禁止。 リクエストトークンが見つからないか無効であるか、トークンに関連付けられている資格情報に指定されたリソースへのアクセス権がないことを示します。 OAuth ベースの Webhook プロバイダーの場合、Adobe Workfrontは新しいアクセストークンの取得を試みます。

* 404 — 見つかりません。 指定したファイルまたはフォルダが存在しないことを示します。

* 500 — 内部サーバーエラー。 その他のタイプのエラー。

* 次の形式を使用した、応答本文のエラーの説明。

  ```
  {status: "error"
   error: "Sample error message"}
  ```
