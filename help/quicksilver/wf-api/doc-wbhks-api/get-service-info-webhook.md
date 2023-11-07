---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: サービスに関する情報を取得します
description: サービスに関する情報を取得します
author: Becky
feature: Workfront API
role: Developer
exl-id: a3a423ff-29a6-466e-a568-f64e02dcb484
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 3%

---


# サービスに関する情報を取得します（まだ実装されていません）

>[!NOTE]
>
>この機能のリリース日は、まだ決定されていません。

機能など、サービスに関する情報を返します。 Adobe Workfrontは、この情報を使用してWorkfrontのユーザーインターフェイスをカスタマイズします。 例えば、Webhook の実装にいくつかのカスタムアクションが含まれている場合、JSON はそれらの操作を JSON でリストする必要があります。 その後、ユーザーは、Workfrontからこれらのアクションを呼び出すことができます。

**URL**

GET/serviceInfo

## クエリパラメーター

なし. また、このエンドポイントへの呼び出しに認証は必要ありません。

## 応答

このサービスに関する情報を含む JSON

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
   <td>String </td> 
   <td>このサービスで実装される Webhook のバージョン。 これは、この仕様の一番上にリストされているバージョン番号です。</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>String </td> 
   <td>このサービスの内部バージョン番号。 この番号は Webhook サービスプロバイダーによって決定され、情報提供の目的でのみ使用されます。<br><br></td> 
  </tr> 
  <tr> 
   <td>媒体社 </td> 
   <td>String </td> 
   <td>Webhook 実装を提供する会社の名前。</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>String </td> 
   <td>このサービスで実装される API エンドポイントを含むリスト。 これは、Workfrontのユーザーインターフェイスに、Webhook プロバイダーが提供する機能が確実に反映されるようにするために使用できます。 リスト内の各項目には、エンドポイントの名前（「search」など）を含める必要があります。</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>String</td> 
   <td>  <p>この Webhook によって実装されたカスタム操作を含むリストです。 各リスト項目には、名前と表示名が含まれます。 表示名は、Workfrontの「ドキュメントのアクション」ドロップダウンに表示されます。 ドロップダウン内の項目をクリックすると、/customAction エンドポイントを呼び出すことで、Webhook 内のアクションが呼び出されます。</p></td> 
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
