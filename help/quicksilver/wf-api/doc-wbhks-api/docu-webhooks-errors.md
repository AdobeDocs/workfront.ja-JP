---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメント web フックのエラー処理
description: ドキュメント web フックのエラー処理
author: Becky
feature: Workfront API
role: Developer
exl-id: 6e0f3be7-5321-44bd-a404-d5bef1462d82
TQID: https://experienceleague.adobe.com/KoMJXXZbDdywLGIwYTu7o8GigPxQ5RG6sNQpOTMHWY0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 123
ht-degree: 100%

---

# ドキュメント web フックのエラー処理

API リクエストを処理するときに問題が発生する可能性があります。 その対応は、すべての API エンドポイントで一貫した方法で行う必要があります。 エラーが発生した場合、web フックのプロバイダーはレスポンスヘッダーにエラーコードを含める必要があります。 エラーコードの例は次のとおりです。

* 403 - Forbidden（禁止されている） リクエストトークンが見つからない、または無効であるか、トークンに関連付けられている資格情報に、指定されたリソースへのアクセス権がないことを示します。 OAuth ベースの web フックプロバイダーに対しては、Adobe Workfront は新しいアクセストークンの取得を試みます。

* 404 - Not found（見つからない） 指定したファイルまたはフォルダーが存在しないことを示します。

* 500 - Internal Server Error（内部サーバーエラー） その他の種類のエラーです。

* レスポンスボディのエラー説明で使用される形式は、次のとおりです。

  ```
  {status: "error"
   error: "Sample error message"}
  ```
