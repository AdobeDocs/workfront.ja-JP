---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Web フックを使用したドキュメントコンテンツの取得
description: ドキュメントの未加工のバイトデータを返します
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '43'
ht-degree: 100%

---

# Web フックを使用したドキュメントコンテンツの取得

ドキュメントの未加工のバイトデータを返します

## URL

GET /download

## クエリパラメーター

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名前 </th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td>ドキュメント ID</td> 
  </tr> 
 </tbody> 
</table>

## 応答

ドキュメントの未加工のバイトデータ。

**例**：`https://www.acme.com/api/download?id=123456`
