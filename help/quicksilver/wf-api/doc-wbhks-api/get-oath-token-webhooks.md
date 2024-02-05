---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: OAuth2 トークンを取得
description: OAuth2 トークンを取得
author: Becky
feature: Workfront API
role: Developer
exl-id: f3a2630d-d34e-4d36-b2bb-707ba0d3258e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 94%

---


# OAuth2 トークンを取得

## OAuth2 トークンの取得

認証済みユーザーの OAuth2 更新トークンとアクセストークンを返します。この呼び出しは、ユーザーがドキュメント提供者をプロビジョニングするときに 1 回だけ実行されます。その後の呼び出しは、更新されたアクセストークンを取得するために行われます。

**URL**

POST/any/url

この URL は設定可能で、カスタム統合設定ページのトークンエンドポイント URL 値に対応しています。

### クエリパラメーター

<table style="table-layout:auto">
 <col>
 <col>
 <col>
 <thead>
  <tr>
   <th>名前</th>
   <th>必須</th>
   <th>説明</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>grant_type</td>
   <td>はい</td>
   <td><p>値は「authorization_code」か「refresh_token」のいずれかです。指定した値は、この API 呼び出しに渡される 2 つのパラメーターのうち、code または refresh_token のいずれかを示します。</p></td>
  </tr>
  <tr>
   <td>コード</td>
   <td>依存</td>
   <td><p>ユーザーが「付与」ボタンをクリックした直後にAdobe Workfrontに送信された認証コード。 これは、grant_type が「authorization_code」の場合にのみ必要です。認証コードは短期間のみ有効で、通常は 10 分以内に期限が切れます。</p></td>
  </tr>
  <tr>
   <td>refresh_token</td>
   <td>依存</td>
   <td><p>これは、以前の access_token が期限切れである場合に、新しい access_token を取得するために後続の呼び出しを行う場合にのみ必要です。この値を送信する場合は、grant_type パラメーターを「refresh_token」に設定します。</p></td>
  </tr>
  <tr>
   <td>client_id</td>
   <td>はい</td>
   <td>このカスタム統合用に Workfront で設定されたクライアント ID。</td>
  </tr>
  <tr>
   <td>client_secret</td>
   <td>はい</td>
   <td>このカスタム統合用に Workfront で設定されたクライアントの秘密鍵。</td>
  </tr>
 </tbody>
</table>

 

## 応答

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
   <td>access_token.</td>
   <td>文字列</td>
   <td><p>ユーザーに代わって認証済み API 呼び出しを行うために使用されるトークン。許可されていない API 呼び出しを防ぐために期限切れになります。</p></td>
  </tr>
  <tr>
   <td>refresh_token.</td>
   <td>文字列</td>
   <td><p>この API メソッドを呼び出して新しい access_token を取得するのに使用される、長期間有効なトークン。</p></td>
  </tr>
  <tr>
   <td>expires_in,</td>
   <td>long</td>
   <td><p>（オプション）access_token の有効期限が切れるまでの時間（秒単位）。通常は 3,600 です。</p></td>
  </tr>
 </tbody>
</table>

**例**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```

## 応答

```
{
access_token:"ad8af5ad5ads759",
refresh_token:"9a0h5d87d808ads",
expires_id:3600
}
```
