---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントの Web フックを使用した検索
description: ドキュメントの Web フックを使用した検索
author: Becky
feature: Workfront API, Digital Content and Documents
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# ドキュメントの Web フックを使用した検索

検索から返されたファイルおよびフォルダーのメタデータを返します。 これは、全文検索として、または通常のデータベースクエリとして実装できます。 Adobe Workfrontは、ユーザーが外部ファイルブラウザーから検索を実行するときに、/search エンドポイントを呼び出します。

## URL

GET/検索

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
   <td>クエリ</td> 
   <td>検索語句。</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（オプション）検索の実行元のフォルダー ID。 注意：これは、Workfrontの将来の機能のプレースホルダーです。 現在、workfront はこのパラメーターを渡しません。 </p> </td> 
  </tr> 
  <tr> 
   <td>最大</td> 
   <td>返す項目の最大数。 ページネーションに使用されます。</td> 
  </tr> 
  <tr> 
   <td>オフセット</td> 
   <td> ページオフセット。「max」と組み合わせて使用します。</td> 
  </tr> 
 </tbody> 
</table>

 

## 応答

クエリに一致するファイルおよびフォルダーのメタデータのリストを含む JSON。 「一致」を構成するものは、Webhook プロバイダーによって決定されます。 フルテキスト検索を行うのが理想です。 ファイル名ベースの検索も機能します。

**例:**

例:  `https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
