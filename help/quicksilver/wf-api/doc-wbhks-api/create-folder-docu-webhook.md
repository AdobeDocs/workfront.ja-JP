---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントの Web フックを含むフォルダーの作成
description: ドキュメントの Web フックを含むフォルダーの作成
author: John
feature: Workfront API
exl-id: 50905915-58c9-4b50-b8a1-133833884a88
source-git-commit: 1b11a4c5f0fdf1987e9f02f7aa06ec6ec36426d3
workflow-type: tm+mt
source-wordcount: '66'
ht-degree: 7%

---


# ドキュメントの Web フックを含むフォルダーの作成

指定されたディレクトリにフォルダーを作成します。

## URL

POST/createFolder

## クエリパラメーター

| **名前** | **説明** |
|---|---|
| parentId  | フォルダーが作成されるフォルダー ID |
| name  | 新しいフォルダーの名前 |




**応答**

新しく作成されたフォルダーのメタデータ（/metadata エンドポイントで定義）。

## 例

```
POST https://www.acme.com/api/createFolder
­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------
parentId=1234
name=New Folder 
-------------------------------
```

戻り値

```
{title:"New Folder",br /> kind:"folder"
 id":"5678",
 viewLink:"”,
 downloadLink:"",
 mimeType:"",
 dateModified:"2014­06­05T17:39:45.251Z"
 size: ""
 }
```
