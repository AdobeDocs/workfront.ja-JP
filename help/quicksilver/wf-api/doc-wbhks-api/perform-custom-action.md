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
workflow-type: ht
source-wordcount: '191'
ht-degree: 100%

---


# カスタムアクションの実行（まだ実装されていません）

このエンドポイントを使用すると、Adobe Workfront ユーザー（または自動ワークフローイベント）が外部システムでアクションを実行できます。 /customAction エンドポイントは、「name」パラメーターを受け取ります。これにより、web フックプロバイダーは複数のカスタム操作を実装できます。

Web フックプロバイダーでは、カスタムアクションを /serviceInfo 応答の customActions 下に含めることで、Workfront に登録します。設定／ドキュメント／カスタム統合で web フックプロバイダーを設定または更新すると、Workfront がこのリストを読み込みます。

ユーザーは、「ドキュメントアクション」の下のセクションを選択することで、カスタムアクションをトリガーできます。

**URL**

GET /customAction

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
   <td> <p>名前</p> </td> 
   <td> <p>実行するアクションのタイプを指定する識別子。この値は、/serviceInfo エンドポイントから返される customAction 値のうちの 1 つに対応します。</p> </td> 
  </tr> 
  <tr> 
   <td>documentId </td> 
   <td>アクションの実行対象となる Workfront ドキュメントの ID。</td> 
  </tr> 
  <tr> 
   <td>documentVersionId</td> 
   <td>アクションの実行対象となる Workfront ドキュメントのバージョン ID。</td> 
  </tr> 
 </tbody> 
</table>

 

## 応答

成功または失敗を示す JSON 文字列（この後の「エラー処理」の節を参照）。失敗（status = &quot;failure&quot;）の場合、Workfront は、用意されているエラーメッセージをユーザーに表示します。

**例：**

```
https://sample.com/webhooks/customName?name=archive&documentId=5502082c003a4f30 ddec2fb2b739cb7c&documentVersionId=54b598a700e2342d6971597a5df1a8d3
```

応答

```
{
status: "success"
}
```
