---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメント Web フックを使用した検索
description: ドキュメント Web フックを使用した検索
author: Becky
feature: Workfront API, Digital Content and Documents
role: Developer
exl-id: 8a3bf0c4-4a20-4311-8c05-15f4ef3a1d42
TQID: https://experienceleague.adobe.com/flRrmTOPVSGP83tVYfKG9AZOT7CNZN4IeWZNsVwcOO4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 139
ht-degree: 93%

---

# ドキュメント Web フックを使用した検索

検索から返されたファイルやフォルダーのメタデータを返します。 これは、全文検索としてまたは通常のデータベースクエリとして実行できます。 Adobe Workfront は、ユーザーが外部ファイルブラウザーから検索を実行するときに、/search エンドポイントを呼び出します。

## URL

GET /search

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
   <td>query</td> 
   <td>検索語または検索フレーズ</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（オプション）検索を実行したフォルダーID。メモ：これは、Workfrontの今後の機能のプレースホルダーです。現在、workfrontはこのパラメーターを渡しません。 </p> </td> 
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

クエリに一致するファイルやフォルダーのメタデータのリストを含んだ JSON。 何をもって「一致」とするかは、web フックプロバイダーによって決まります。 全文検索を行うのが理想です。 ファイル名ベースの検索も有効です。

**例：**

例：`https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
