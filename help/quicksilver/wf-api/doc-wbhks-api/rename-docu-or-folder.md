---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントまたはフォルダーの名前の変更（まだ実装されていません）
description: ドキュメントまたはフォルダーの名前変更
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
TQID: https://experienceleague.adobe.com/-HmJkcMckTK6upblNcqX5LZkdYQxoWPDeuHkFjJarh4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 81
ht-degree: 100%

---

# ドキュメントまたはフォルダーの名前の変更（まだ実装されていません）

外部システム内の指定された ID を持つドキュメントやフォルダーの名前を変更します。

**URL**

PUT /rename

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| id | 名前を変更するドキュメントまたはフォルダーの ID |
| 名前  | ドキュメントまたはフォルダーの新しい名前 |


## 応答

成功または失敗を示す JSON 文字列（この後の「エラー処理」の節を参照）。

**例：** PUT https://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

戻り値

```
{status: "success"
 }returns
 {
 status: "failure", error: "Folder cannot be renamed because a folder with that name already exists."
 }
```
