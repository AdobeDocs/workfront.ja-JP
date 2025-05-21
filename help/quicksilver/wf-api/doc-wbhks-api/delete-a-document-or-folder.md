---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントまたはフォルダーの削除
description: ドキュメントまたはフォルダーの削除
author: Becky
feature: Workfront API
role: Developer
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 48de4553478fc42d88d81ea953440337f6684e50
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 90%

---


# ドキュメントまたはフォルダーの削除（まだ実装されていません）

外部システム内の指定した ID を持つドキュメントまたはフォルダーを削除します。フォルダーを削除すると、その内容も削除されます。

## URL

PUT /delete

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| documentId  | 削除するドキュメントの ID |
| folderId  | 削除するフォルダーの ID |



## 応答

成功または失敗を示す JSON 文字列（この後の「エラー処理」の節を参照）。

### 例

PUT https://www.example.com/api/deleteid=1234 
* `status: "success"` を返します

* `status: "failure", error: "File not found"` を返します
