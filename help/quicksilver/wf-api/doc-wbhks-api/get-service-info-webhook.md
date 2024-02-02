---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: サービスに関する情報を取得
description: サービスに関する情報を取得
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '266'
ht-degree: 100%

---


# サービスに関する情報の取得（まだ実装されていません）

>[!NOTE]
>
>この機能のリリース日は、まだ決定されていません。

特長や機能など、サービスに関する情報を返します。Adobe Workfront では、この情報を使用して Workfront のユーザーインターフェイスをカスタマイズします。例えば、web フックの実装にいくつかのカスタムアクションが含まれている場合、それらの操作は JSON でリストする必要があります。それにより、ユーザーは、これらのアクションを Workfront から呼び出すことができるようになります。

**URL**

GET /serviceInfo

## クエリパラメーター

なし。さらに、このエンドポイントへの呼び出しには、認証も必要ありません。

## 応答

このサービスに関する情報を含んだ JSON

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名前</th> 
   <th>タイプ </th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>文字列</td> 
   <td>このサービスで実装されている web フックのバージョン。この仕様の一番上にリストされているバージョン番号です。</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>文字列</td> 
   <td>このサービスの内部バージョン番号。この番号は web フックサービスプロバイダーが定め、情報提供の目的でのみ使用されます。<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher </td> 
   <td>文字列</td> 
   <td>Web フックの実装を提供する会社の名前。</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>文字列</td> 
   <td>このサービスで実装される API エンドポイントを含んだリスト。これは、Workfront のユーザーインターフェイスに、web フックプロバイダーから提供される機能が確実に反映されるようにするために使用されることがあります。リスト内の各項目には、エンドポイントの名前（「search」など）を含める必要があります。</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>文字列</td> 
   <td>  <p>この web フックで実装されているカスタム操作を含んだリストです。各リスト項目には、名前と表示名が含まれます。表示名は、Workfront の「ドキュメント アクション」ドロップダウンに表示されます。ドロップダウン内の項目をクリックすると、/customAction エンドポイントを呼び出すことで、web フック内のアクションが呼び出されます。</p></td> 
  </tr> 
 </tbody> 
</table>

**例：** `https://www.acme.com/api/serviceInfo`

戻り値

```
{
webhook version: "1.2", version: "1.0", publisher: "Acme, LLC", availableEndpoints: ["files", "metadata", "search", "download"
"thumbnail", "uploadInit", "upload" ], customActions [
{
name: "archive", displayName: "Archive" 
}, 
{name: "doSomethingElse", displayName: "Do Something" }, 
] 
}
```
