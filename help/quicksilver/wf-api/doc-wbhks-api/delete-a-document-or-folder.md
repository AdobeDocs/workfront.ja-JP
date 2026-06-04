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
TQID: https://experienceleague.adobe.com/7-f8Z3qQQ2z7ZHHfSrGgJqIQCKdeqEoL96XlfCGzYSo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 75
ht-degree: 100%

---

# ドキュメントまたはフォルダーの削除（まだ実装されていません）

外部システム内の指定した ID を持つドキュメントまたはフォルダーを削除します。 フォルダーを削除すると、その内容も削除されます。

## URL

PUT /delete

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| documentId  | 削除するドキュメントの ID |
| folderId  |  削除するフォルダーの ID |



## 応答

成功または失敗を示す JSON 文字列（この後の「エラー処理」の節を参照）。

### 例

```
PUT https://www.example.com/api/deleteid=1234

* returns `status: "success"`

* returns `status: "failure", error: "File not found"`
```
