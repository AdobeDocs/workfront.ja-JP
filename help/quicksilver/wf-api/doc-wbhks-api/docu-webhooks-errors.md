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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 100%

---

# ドキュメント web フックのエラー処理

API リクエストを処理するときに問題が発生する可能性があります。その対応は、すべての API エンドポイントで一貫した方法で行う必要があります。エラーが発生した場合、web フックのプロバイダーはレスポンスヘッダーにエラーコードを含める必要があります。エラーコードの例は次のとおりです。

* 403 - Forbidden（禁止されている）リクエストトークンが見つからない、または無効であるか、トークンに関連付けられている資格情報に、指定されたリソースへのアクセス権がないことを示します。OAuth ベースの web フックプロバイダーに対しては、Adobe Workfront は新しいアクセストークンの取得を試みます。

* 404 - Not found（見つからない）指定したファイルまたはフォルダーが存在しないことを示します。

* 500 - Internal Server Error（内部サーバーエラー）その他の種類のエラーです。

* レスポンスボディのエラー説明で使用される形式は、次のとおりです。

  ```
  {status: "error"
   error: "Sample error message"}
  ```
