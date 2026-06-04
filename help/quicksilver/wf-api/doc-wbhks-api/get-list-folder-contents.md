---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ファイルまたはフォルダーのメタデータを一覧表示する
description: ファイルまたはフォルダーのメタデータを一覧表示する
author: Becky
feature: Workfront API
role: Developer
exl-id: 9c9f9222-59ac-4643-8297-d4939bec7e64
TQID: https://experienceleague.adobe.com/nZv42xMbDRJbkwR-lFKI6dAbeszSzGWAwn--qkKhVVM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 101
ht-degree: 100%

---

# フォルダーコンテンツの項目リストを取得する

特定のフォルダーのファイルおよびフォルダーのメタデータを一覧表示します。

**URL**

GET /files

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| parentId  | フォルダー ID。 ルートディレクトリのメタデータを取得するには、値「/」を使用します。 |
| 最大  | 返す項目の最大数。 ページネーションに使用されます。 |
| オフセット  |  ページオフセット。「max」と組み合わせて使用します。 |


## 応答

ファイルとフォルダーのリストを含んだ JSON。 各項目のメタデータは、/metadata エンドポイントから返されるメタデータと同じです。

**例：** https://www.acme.com/api/files?parentId=123456

```
[ 
{
title:"Folder A",
kind:"folder"
id":"2lj23lkj",
viewLink:" https://www.acme.com/viewDocument?id=2lj23lkj ",
downloadLink:"https://www.acme.com/downloadDocument?id=2lj23lkj",
mimeType:"",
dateModified:"2014­06­05T17:39:45.251Z"
size: ""
},
{
title:"My Document",
kind:"file"
id":"da8cj234",
viewLink:" https://www.acme.com/viewDocument?id=da8cj234 ",
downloadLink:"https://www.acme.com/downloadDocument?id=da8cj234",
mimeType:"image/png",
dateModified:"2014­06­05T17:39:45.251Z"
size: "32554694"
}
]
```
