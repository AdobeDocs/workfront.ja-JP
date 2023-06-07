---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Web フックを使用したドキュメントコンテンツの取得
description: ドキュメントの生のバイトを返します
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 0f0b5af7-f276-4856-852c-e976fa491f83
source-git-commit: 54d1753b9062b6d4910e4478c1f072b7fedc87eb
workflow-type: tm+mt
source-wordcount: '43'
ht-degree: 6%

---

# Web フックを使用したドキュメントコンテンツの取得

ドキュメントの生のバイトを返します

## URL

GET/ダウンロード

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
   <td> ドキュメント ID。</td> 
  </tr> 
 </tbody> 
</table>

## 応答

ドキュメントの生のバイト。

**例**:  `https://www.acme.com/api/download?id=123456`
