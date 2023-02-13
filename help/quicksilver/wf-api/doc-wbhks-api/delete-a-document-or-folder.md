---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントまたはフォルダーの削除
description: ドキュメントまたはフォルダーの削除
author: John
feature: Workfront API
exl-id: b56ec13a-1ee1-4bef-b39b-e625d00e4952
source-git-commit: 9de8ee7fad2a3cb67c4fc6bfdff4d6ce50f15afd
workflow-type: tm+mt
source-wordcount: '82'
ht-degree: 4%

---


# ドキュメントまたはフォルダーの削除（未実装）

外部システム内の指定された ID を持つドキュメントまたはフォルダを削除します。 フォルダーを削除すると、フォルダーの内容も削除されます。

## URL

PUT/delete

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| documentId  | 削除するドキュメント ID |
| folderId  |  削除するフォルダー ID |



## 応答

以下のエラー処理の節で指定された、成功または失敗を示す JSON 文字列。

### 例

PUThttps://www.example.com/api/deleteid=1234
* 戻り値 `status: “success”`

* 戻り値 `status: “failure”, error: “File not found”`
