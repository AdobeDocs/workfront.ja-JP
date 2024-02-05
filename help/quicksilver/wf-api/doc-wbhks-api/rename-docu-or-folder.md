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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '78'
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
