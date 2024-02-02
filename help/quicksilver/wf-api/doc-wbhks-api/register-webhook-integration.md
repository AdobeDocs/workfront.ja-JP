---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Web フック統合の登録
description: Web フック統合の登録
author: Becky
feature: Workfront API
role: Developer
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '336'
ht-degree: 100%

---


# Web フック統合の登録

Adobe Workfront 管理者は、Workfront 内でセッ設定／ドキュメント／カスタム統合に移動して、会社のカスタム Web フック統合を追加することができます。設定内のカスタム統合ページから、管理者は既存のドキュメント web フック統合のリストを表示することができます。このページから、統合を追加、編集、有効化、無効化することができます。

統合を追加するには、「**カスタム統合の追加**」ボタンをクリックします。

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## 使用可能なフィールド

統合を追加する際、管理者は以下のフィールドに値を入力します。

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
   <td> <p>コールバック API の場所。外部システムを呼び出す場合、Workfront はこのアドレスにエンドポイント名を追加します。例えば、管理者が Base API URL の「https://www.mycompany.com/api/v1」を入力した場合、Workfront は次の URL を使用してドキュメントのメタデータを取得します：https://www.mycompany.com/api/v1/metadata?id=1234。</p> </td> 
  </tr> 
  <tr> 
   <td>パラメーターのリクエスト</td> 
   <td> <p>すべての API 呼び出しの文字列に追加されるオプションの値。例：access_type=offline </p> </td> 
  </tr> 
  <tr> 
   <td>認証タイプ</td> 
   <td>OAuth2 または ApiKey</td> 
  </tr> 
  <tr> 
   <td>認証 URL</td> 
   <td> <p>（OAuth2 のみ）ユーザー認証に使用される完全な URL。Workfront は、OAuth プロビジョニングプロセスの一環として、ユーザーをこのアドレスに移動させます。メモ：Workfront は、クエリ文字列に「状態」パラメーターを追加します。プロバイダーは、これを Workfront のリダイレクト URI に追加して、Workfront に返す必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td>トークンエンドポイント URL</td> 
   <td> <p>（OAuth2 のみ）OAuth2 トークンを取得するために使用される完全な API URL。これは、web フックプロバイダーまたは外部ドキュメントプロバイダーによってホストされます</p> </td> 
  </tr> 
  <tr> 
   <td>クライアント ID</td> 
   <td>（OAuth2 のみ）この統合に使用される OAuth2 クライアント ID</td> 
  </tr> 
  <tr> 
   <td>クライアントシークレット</td> 
   <td> <p>（OAuth2 のみ）この統合に使用される OAuth2 クライアントシークレット</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront リダイレクト URI</td> 
   <td>（OAuth2 のみ）これは読み取り専用のフィールドで、Workfront によって生成されます。この値は、この統合を外部のドキュメントプロバイダーに登録するために使用されます。メモ：前述の認証 URL と同様、リダイレクトを実行する際にプロバイダーは「state」パラメーターとその値をクエリ文字列に追加する必要があります。</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>（ApiKey のみ）web フックプロバイダーに対して承認済み API 呼び出しを行うために使用されます。Web フックプロバイダーで発行された API キー。</p> </td> 
  </tr> 
 </tbody> 
</table>
