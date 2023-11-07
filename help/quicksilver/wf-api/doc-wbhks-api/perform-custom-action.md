---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: カスタムアクションの実行
description: カスタムアクションの実行
author: Becky
feature: Workfront API
role: Developer
exl-id: a18b6b97-ee1e-4ad2-a4e1-00a644a0f4f2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 2%

---


# カスタムアクションの実行（未実装）

このエンドポイントを使用すると、Adobe Workfrontユーザー（または自動ワークフローイベント）が外部システムでアクションを実行できます。 /customAction エンドポイントは、「name」パラメーターを受け取ります。これにより、Webhook プロバイダーは複数のカスタム操作を実装できます。

Webhook プロバイダーは、カスタムアクションを customActions の下の/serviceInfo 応答に含めることで、Workfrontに登録します。 Workfrontは、設定/ドキュメント/カスタム統合で webhook プロバイダーを設定または更新すると、このリストを読み込みます。

ユーザーは、「ドキュメントのトリガー」の下のセクションを選択することで、カスタムのアクションを実行できます

**URL**

GET/customAction

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
   <td> <p>name</p> </td> 
   <td> <p>実行するアクションのタイプを指定する識別子。 この値は、 /serviceInfo エンドポイントから返される customAction 値の 1 つに対応します。</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>アクションを実行するワークフロントドキュメント ID。</td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td> アクションを実行するワークフロントドキュメントのバージョン ID。</td> 
  </tr> 
 </tbody> 
</table>

 

## 応答

以下のエラー処理の節で指定された、成功または失敗を示す JSON 文字列。 失敗した場合（例：status = &quot;failure&quot;）、Workfrontは提供されたエラーメッセージをユーザーに表示します。

**例:**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

応答

```
{
status: "success"
}
```
