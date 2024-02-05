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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 94%

---

# ドキュメント Web フックを使用した検索

検索から返されたファイルやフォルダーのメタデータを返します。これは、全文検索としてまたは通常のデータベースクエリとして実行できます。Adobe Workfront は、ユーザーが外部ファイルブラウザーから検索を実行するときに、/search エンドポイントを呼び出します。

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
   <td> <p>（オプション）検索の実行元フォルダーの ID。メモ：これは、Workfront の将来的な機能用のプレースホルダーです。現在、Workfront ではこのパラメーターを渡しません。 </p> </td> 
  </tr> 
  <tr> 
   <td>最大</td> 
   <td>返す項目の最大数。ページネーションに使用されます。</td> 
  </tr> 
  <tr> 
   <td>オフセット</td> 
   <td> ページオフセット。「max」と組み合わせて使用します。</td> 
  </tr> 
 </tbody> 
</table>

 

## 応答

クエリに一致するファイルやフォルダーのメタデータのリストを含んだ JSON。何をもって「一致」とするかは、web フックプロバイダーによって決まります。全文検索を行うのが理想です。ファイル名ベースの検索も有効です。

**例：**

例：`https://www.acme.com/api/search?query=test-query`

```
[ 
{ File/Folder Metadata },
{ File/Folder Metadata } 
]
```
