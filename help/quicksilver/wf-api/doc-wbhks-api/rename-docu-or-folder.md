---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントまたはフォルダーの名前を変更する（まだ実装されていません）
description: ドキュメントまたはフォルダの名前を変更する
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 5b1a4a02-a7fd-41f2-9adb-74b40606270b
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '81'
ht-degree: 4%

---


# ドキュメントまたはフォルダーの名前を変更する（まだ実装されていません）

外部システムで指定した ID を持つドキュメントまたはフォルダの名前を変更します。

**URL**

PUT/rename

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| id | 名前を変更するドキュメントまたはフォルダー ID |
| name  | ドキュメントまたはフォルダの新しい名前 |


## 応答

以下のエラー処理の節で指定された、成功または失敗を示す JSON 文字列。

**例：** PUThttps://www.acme.com/api/rename

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

戻り値

```
{status: “success”
 }returns
 {
 status: “failure”, error: “Folder cannot be renamed because a folder with that name already exists.”
 }
```
