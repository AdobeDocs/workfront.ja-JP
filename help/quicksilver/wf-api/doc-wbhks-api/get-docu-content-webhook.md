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
TQID: https://experienceleague.adobe.com/AIN65ofKDJA95iMpvNwoe3oQapmyxzDC16dpf5ehwH0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 43
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
   <td> ドキュメント ID</td> 
  </tr> 
 </tbody> 
</table>

## 応答

ドキュメントの未加工のバイトデータ。

**例**：`https://www.acme.com/api/download?id=123456`
