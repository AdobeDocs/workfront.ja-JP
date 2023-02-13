---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhook 統合の登録
description: Webhook 統合の登録
author: John
feature: Workfront API
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 11%

---


# Webhook 統合の登録

Adobe Workfrontの管理者は、Workfront内でセットアップ/ドキュメント/カスタム統合に移動して、会社のカスタム Webhook 統合を追加できます。 管理者は、セットアップ内のカスタム統合ページから、既存のドキュメント Webhook 統合のリストを表示できます。 このページから、統合を追加、編集、有効、無効にすることができます。

統合を追加するには、 **カスタム統合の追加**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## 使用可能フィールド

統合を追加する際、管理者は次のフィールドに値を入力します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>フィールド名</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>名前</td> 
   <td>この統合の名前。</td> 
  </tr> 
  <tr> 
   <td>ベース API の URL</td> 
   <td> <p>コールバック API の場所。 外部システムを呼び出す場合、Workfrontはこのアドレスにエンドポイント名を追加するだけです。 例えば、管理者が Base API URL の「 https://www.mycompany.com/api/v1 」を入力した場合、Workfrontは次の URL を使用してドキュメントのメタデータを取得します。https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>リクエストパラメーター</td> 
   <td> <p>すべての API 呼び出しの文字列に追加されるオプションの値で、access_type </p> </td> 
  </tr> 
  <tr> 
   <td>認証タイプ</td> 
   <td>OAuth2 または ApiKey</td> 
  </tr> 
  <tr> 
   <td>認証 URL</td> 
   <td> <p>（OAuth2 のみ）ユーザー認証に使用される完全な URL。 Workfrontは、OAuth プロビジョニングプロセスの一環として、ユーザーをこのアドレスに移動します。 注意：Workfrontは、クエリ文字列に「state」パラメーターを追加します。 プロバイダーは、これをWorkfrontのリダイレクト URI に追加して、Workfrontに渡す必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td>トークン エンドポイント URL</td> 
   <td> <p>（OAuth2 のみ）OAuth2 トークンの取得に使用される完全な API URL。 これは、Webhook プロバイダーまたは外部ドキュメントプロバイダーによってホストされます</p> </td> 
  </tr> 
  <tr> 
   <td>クライアント ID</td> 
   <td>（OAuth2 のみ）この統合の OAuth2 クライアント ID。</td> 
  </tr> 
  <tr> 
   <td>クライアントシークレット</td> 
   <td> <p>（OAuth2 のみ）この統合の OAuth2 クライアント秘密鍵</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront リダイレクト URI</td> 
   <td>（OAuth2 のみ）これは読み取り専用のフィールドで、Workfrontによって生成されます。 この値は、この統合を外部のドキュメントプロバイダーに登録するために使用されます。 注意：認証 URL について前述したように、リダイレクトを実行する際には、プロバイダーは「state」パラメーターとその値をクエリ文字列に追加する必要があります。</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>（ApiKey のみ）Webhook プロバイダーに対する承認済み API 呼び出しをおこなうために使用されます。 Webhook プロバイダーによって発行された API キー。</p> </td> 
  </tr> 
 </tbody> 
</table>
