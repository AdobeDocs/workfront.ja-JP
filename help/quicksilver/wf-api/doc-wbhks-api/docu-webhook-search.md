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
TQID: 'https://experienceleague.adobe.com/flRrmTOPVSGP83tVYfKG9AZOT7CNZN4IeWZNsVwcOO4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 100%
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
   <td> <p>（オプション）検索の実行元フォルダーの ID。 メモ：これは、Workfront の将来的な機能用のプレースホルダーです。 現在、Workfront ではこのパラメーターを渡しません。 </p> </td> 
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
