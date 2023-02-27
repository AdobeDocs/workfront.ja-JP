---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Document Webhook API
description: Document Webhook API
author: Becky
feature: Workfront API
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '3661'
ht-degree: 3%

---


# Document Webhook API

Adobe Workfront Document Webhook は、Workfrontが外部ドキュメントプロバイダーに対して承認済みの API 呼び出しをおこなう API エンドポイントのセットを定義します。 これにより、誰でも任意のドキュメントストレージプロバイダー用のミドルウェアプラグインを作成できます。

Webhook ベースの統合のユーザーエクスペリエンスは、Google Drive、Box、Dropboxなどの既存のドキュメント統合のユーザーエクスペリエンスと似ています。 例えば、Workfrontユーザーは次の操作を実行できます。

* 外部ドキュメントプロバイダーのフォルダー構造に移動する
* ファイルを検索
* ファイルをWorkfrontにリンク
* 外部ドキュメントプロバイダーにファイルをアップロード
* ドキュメントのサムネールを表示

## 参照実装

新しい Web フック実装の開発をすぐに開始できるように、Workfrontでは参照実装を提供しています。 これを行うコードは、で確認できます。 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). この実装は Java ベースで、Workfrontはネットワークファイルシステム上でドキュメントに接続できます。

## Webhook 統合の登録

Workfrontの管理者は、Workfront内でセットアップ/ドキュメント/カスタム統合に移動して、会社のカスタム Webhook 統合を追加できます。 管理者は、セットアップ内のカスタム統合ページから、既存のドキュメント Webhook 統合のリストを表示できます。 このページから、統合を追加、編集、有効、無効にすることができます。 統合を追加するには、「統合を追加」ボタンをクリックします。

### 使用可能フィールド

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
   <td> <p>すべての API 呼び出しの文字列に追加されるオプションの値で、access_type</p> <p> </p> </td> 
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
   <td> <p>（OAuth2 のみ）OAuth2 トークンの取得に使用される完全な API URL。 これは、Webhook プロバイダーまたは外部ドキュメントプロバイダーによってホストされます</p> <p> </p> </td> 
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
   <td>  <p>（OAuth2 のみ）これは読み取り専用のフィールドで、Workfrontによって生成されます。 この値は、この統合を外部のドキュメントプロバイダーに登録するために使用されます。 注意：認証 URL について前述したように、リダイレクトを実行する際には、プロバイダーは「state」パラメーターとその値をクエリ文字列に追加する必要があります。</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>（ApiKey のみ）Webhook プロバイダーに対する承認済み API 呼び出しをおこなうために使用されます。 Webhook プロバイダーによって発行された API キー。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 認証

Workfront Document Webhook は、次の 2 種類の認証形式をサポートしています。OAuth2 および ApiKey。 どちらの場合も、Workfrontは API 呼び出しをおこなう際に、ヘッダーで認証トークンを渡します。

### OAuth2

OAuth2 を使用すると、Workfrontは、ユーザーに代わって Webhook プロバイダーに対して承認済みの API 呼び出しをおこなうことができます。 その前に、ユーザーは外部のドキュメントプロバイダーのアカウントをWorkfrontに接続し、Workfrontに付与する必要があります

自分の代理として行動するためのアクセス権 このハンドシェイクプロセスは、各ユーザーに対して 1 回だけ発生します。 仕組みは次のとおりです。

1. ユーザーが Webhook 統合のアカウントへの接続を開始します。 現在、これは「ドキュメントの追加」ドロップダウン/「サービスを追加」/「カスタム統合名」をクリックすることでおこなわれます。
1. Workfrontはユーザーに認証 URL を移動します。この URL は、ユーザーに外部のドキュメントプロバイダーへのログインを促す場合があります。 このページは、Webhook プロバイダーまたは外部ドキュメント管理システムによってホストされます。 その際、Workfrontは認証 URL に「state」パラメーターを追加します。 この値は、以下の手順で同じ値をWorkfrontの戻り URI に追加して、Workfrontに渡す必要があります。
1. 外部システムにログインした後（またはユーザーが既にログインしている場合）、「認証」ページが表示され、Workfrontがユーザーに代わって一連のアクションを実行するためのアクセスを要求していることを説明します。
1. ユーザーが「許可」ボタンをクリックすると、ブラウザーは、「code=`<code>`」をクエリ文字列に追加します。 OAuth2 仕様に従い、このトークンは短期間有効です。 クエリ文字列には、「state=`<sent_by_workfront>`&quot;.
1. Workfrontはこのリクエストを処理し、認証コードを使用してトークンエンドポイント URL への API 呼び出しをおこないます。
1. トークンエンドポイント URL は、更新トークンとアクセストークンを返します。
1. Workfrontはこれらのトークンを保存し、このユーザーに対して webhook 統合を完全にプロビジョニングします。
1. これ以降、Workfrontは Webhook プロバイダーに対して認証済みの API 呼び出しをおこなうことができます。 これらの呼び出しをおこなう場合、Workfrontは、次に示すように HTTP リクエストヘッダーでアクセストークンを送信します。

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. アクセストークンの有効期限が切れている場合、Workfrontはトークンエンドポイント URL を呼び出して新しいアクセストークンを取得し、新しいアクセストークンを使用して認証済み API 呼び出しを再試行します。

### ApiKey

ApiKey を使用して Webhook プロバイダーに対して承認された API 呼び出しをおこなう方が、OAuth2 よりもはるかに簡単です。 API 呼び出しをおこなう場合、Workfrontは HTTP リクエストヘッダーに ApiKey とWorkfrontのユーザー名を渡します。

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Webhook プロバイダーは、ユーザー名を使用して、ユーザー固有の権限を適用できます。 これは、両方のシステムがシングルサインオン (SSO) を使用して LDAP に接続する場合に最も適しています。

### リクエストヘッダーの追加（オプション）

Workfrontでは、認証に OAuth2 トークンまたは ApiKey を使用する以外に、あらかじめ定義された一連のヘッダーを API 呼び出しごとに Webhook プロバイダーに送信できます。 上記の節で説明したように、Workfrontの管理者が Webook 統合の登録または編集時に設定できます。 「Webhook 統合の登録」を参照してください。

例えば、これは基本認証に使用できます。 これをおこなうには、Workfront管理者がカスタム統合ダイアログに次のリクエストヘッダー情報を追加します。

   認証基本 QWxhZGRpbjpvcGVuIHNlc2FtZQ==

ここで、QWxhZGRpbjpvcGVuIHNlc2FtZQ==は、&quot;username:password&quot;の base-64 エンコードされた文字列です。 基本認証を参照してください。 これが追加された場合、Workfrontは他のリクエストヘッダーに加えて、HTTP リクエストヘッダーにこれを渡します。

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API 仕様

ドキュメントの Web フックを機能させるために Webhook プロバイダーが実装する必要がある API のリストを以下に示します。

### OAuth2 トークンの取得（OAuth2 認証のみ必要）

認証済みユーザーの OAuth2 更新トークンとアクセストークンを返します。 この呼び出しは、ユーザーがドキュメントプロバイダーをプロビジョニングするときに 1 回だけ実行されます。 その後の呼び出しは、更新されたアクセストークンを取得するためにおこなわれます。

HTTP リクエストPOST/any/url

この URL は設定可能で、カスタム統合設定ページの「トークンエンドポイント URL 」値に対応しています。

**クエリパラメーター**

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
   <td> <p>値には、「authorization_code」または「refresh_token」が含まれます。 指定された値は、この API 呼び出しに渡される 2 つのパラメーターのうちの 1 つを示します。コードまたは refresh_token。</p> </td> 
  </tr> 
  <tr> 
   <td>コード</td> 
   <td>依存</td> 
   <td> <p>ユーザーが「付与」ボタンをクリックした直後にWorkfrontに送信された認証コード。 これは、付与タイプが「authorization_code」の場合にのみ必要です。 認証コードは短期間のみ有効で、通常は 10 分以内に期限が切れます。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>依存</td> 
   <td> <p>これは、以前の access_token が期限切れである場合に、新しい access_token を取得するために後続の呼び出しを行う場合にのみ必要です。 この値を送信する際に、 grant_type パラメータを「refresh_token」に設定します。</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>はい</td> 
   <td>このカスタム統合用にWorkfrontで設定されたクライアント ID。</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>はい</td> 
   <td> このカスタム統合用にWorkfrontで設定されたクライアントシークレット。</td> 
  </tr> 
 </tbody> 
</table>

 

**応答**

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
   <td>access_token </td> 
   <td>String</td> 
   <td> <p>ユーザーに代わって認証済み API 呼び出しをおこなうために使用されるトークン。 この期限は、許可されていない API 呼び出しを防ぐために期限切れになります。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>String</td> 
   <td> <p>この API メソッドを呼び出して新しい access_token を取得するのに使用される、長期間有効なトークン。</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>（オプション） access_token の有効期限が切れるまでの時間（秒単位）です。通常は 3,600 です。</p></td> 
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


**応答**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### ファイルまたはフォルダーのメタデータの取得

指定されたファイルまたはフォルダーのメタデータを返します。

**URL**

GET/metadata?id=[ドキュメントまたはフォルダー ID]

**クエリパラメーター**

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
   <td>id</td> 
   <td>  <p>Webhook プロバイダーによって参照されるファイルまたはフォルダーの ID。 これは、Workfrontのドキュメント ID とは異なります。 ルートディレクトリのメタデータを取得するには、値「/」を使用します。</p><p>注意：ID の最大長は 255 文字です。</p></td> 
  </tr> 
 </tbody> 
</table>

 

**応答**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名前 </th> 
   <th>タイプ </th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>String </td> 
   <td>ドキュメントまたはフォルダーの名前</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>String </td> 
   <td>この項目がファイルかフォルダーかを指定します（「ファイル」または「フォルダー」）</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>String </td> 
   <td>ファイルまたはフォルダーの ID。</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>String </td> 
   <td> <p>ユーザーがブラウザーウィンドウでドキュメントを表示するために使用する URL パス。 この URL は、ドキュメントプロバイダーまたはネイティブの外部ストレージプロバイダーによってホストされます。</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>String </td> 
   <td> <p>ブラウザーウィンドウでドキュメントをダウンロードするためにユーザーが使用する URL パス。 この URL は、ドキュメントプロバイダーまたはネイティブの外部ストレージプロバイダーによってホストされます。</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>String </td> 
   <td>ファイルの MIME タイプ。 (オプション)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>String </td> 
   <td>このファイルが最後に変更された時刻（RFC 3339 形式のタイムスタンプ）</td> 
  </tr> 
  <tr> 
   <td>サイズ</td> 
   <td>Long</td> 
   <td>  ファイルのサイズ（バイト単位）。 (オプション)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>ブール値</td> 
   <td>  <p> このファイルまたはフォルダーが認証済みユーザーに対して読み取り専用かどうかを示します。(オプション)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**例：** `https://www.acme.com/api/metadata?id=12345`

**応答**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>エラー処理は、すべての API 呼び出しで一貫している必要があります。 詳しくは、以下の「エラー処理」の節を参照してください。

### フォルダ内の項目のリストを取得する

指定されたフォルダーのファイルおよびフォルダーのメタデータを返します。

**URL**

GET/ファイル

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| parentId  | フォルダー ID。 ルートディレクトリのメタデータを取得するには、値「/」を使用します。 |

{style=&quot;table-layout:auto&quot;}

Document Webhooks API は、現在、ページネーションをサポートしていません。

**応答**

ファイルとフォルダーのリストを含む JSON。 各項目のメタデータは、/metadata エンドポイントから返されるメタデータと同じです。

**例：** `https://www.acme.com/api/files?parentId=123456`

**応答**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### 検索を実行

検索から返されたファイルおよびフォルダーのメタデータを返します。 これは、全文検索として、または通常のデータベースクエリとして実装できます。 Workfrontは、ユーザーが外部ファイルブラウザーから検索を実行するときに、/search エンドポイントを呼び出します。

**URL**

GET/検索

**クエリパラメーター**

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
   <td>クエリ</td> 
   <td>検索語句。</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（オプション）検索の実行元のフォルダー ID。 注意：これは、Workfrontの将来の機能のプレースホルダーです。 現在、workfront はこのパラメーターを渡しません。 </p> </td> 
  </tr> 
  </tbody> 
</table>

Document Webhooks API は、現在、ページネーションをサポートしていません。

 

**応答**

クエリに一致するファイルおよびフォルダーのメタデータのリストを含む JSON。 「一致」を構成するものは、Webhook プロバイダーによって決定されます。 フルテキスト検索を行うのが理想です。 ファイル名ベースの検索も機能します。

**例：** `https://www.acme.com/api/search?query=test-query`

**応答**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### ドキュメントのコンテンツを取得する

ドキュメントの生のバイトを返します

**URL**

GET/ダウンロード

**クエリパラメーター**

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
   <td> <p>id</p> </td> 
   <td> ドキュメント ID。</td> 
  </tr> 
 </tbody> 
</table>

 

**応答**

ドキュメントの生のバイト。

**例：** `https://www.acme.com/api/download?id=123456`

### ドキュメントのサムネールを取得する

ドキュメントの生のサムネールのバイト数を返します。

**URL**

GET/サムネール

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| id  | ドキュメント ID。 |
| サイズ  |  サムネールの幅 |

{style=&quot;table-layout:auto&quot;}

 

**応答**

生のサムネールのバイト数です。

**例：** `https://www.acme.com/api/thumbnail?id=123456`

### ファイルのアップロード — パート 1 / 2

ファイルをドキュメントストレージプロバイダーにアップロードするプロセスは、2 つの異なる API エンドポイントを必要とする 2 つの手順です。 Workfrontは、 /uploadInit を呼び出して、アップロードプロセスを開始します。 このエンドポイントはドキュメント ID を返し、ドキュメントのバイトをアップロードする際に/upload に渡されます。 基になるドキュメントストレージシステムに応じて、長さ 0 のドキュメントを作成し、後でドキュメントの内容を更新する必要が生じる場合があります。

この仕様のバージョン 1.1 に追加されたドキュメント ID とドキュメントバージョン ID を使用して、Workfrontから追加の情報を取得できます。 例えば、ドキュメント管理システムがドキュメントに関する追加情報を必要とする場合、Webhook 実装コードはドキュメント ID を使用して、Workfrontの RESTful API を使用してその情報を取得できます。 ベストプラクティスとして、この情報は、ドキュメント上のカスタムデータフィールドから取得され、タスク、問題、またはプロジェクトが含まれている場合があります。

**URL**

POST/uploadInit

**クエリパラメーター**

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
   <td>parentId </td> 
   <td>Webhook プロバイダーによって参照される親フォルダー ID。</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>ドキュメントの名前</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfrontドキュメント ID （バージョン 1.1 で追加）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfrontドキュメントのバージョン ID（バージョン 1.1 で追加）</td> 
  </tr> 
 </tbody> 
</table>

 

**応答**

ファイルのメタデータ（/metadata エンドポイントで定義）。

**例：** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**応答**

`[file_metadata]` には、ドキュメントプロバイダーが使用する新しいドキュメント ID が含まれます。

### ファイルのアップロード — パート 2 / 2

Webhook プロバイダーにドキュメントのバイトをアップロードします。

**URL**

PUT/upload

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| id  |  作成されたドキュメント ID。 |


 

**リクエスト本文**

ドキュメントの生の内容のバイト。

**応答**

```
{
"result": "success"
}
```

または

```
{
"result": "fail"
}
```

**例：** `https://www.acme.com/api/upload?id=1234` *[更新ストリームに含まれるドキュメントのバイト数]*

**応答**

```
{
"result":"success"
}
```

### サービスに関する情報を取得します 

（リリース日 — TBD）機能など、サービスに関する情報を返します。 Workfrontは、この情報を使用してWorkfrontのユーザーインターフェイスをカスタマイズします。 例えば、Webhook の実装にいくつかのカスタムアクションが含まれている場合、JSON はそれらの操作を JSON でリストする必要があります。 その後、ユーザーは、Workfrontからこれらのアクションを呼び出すことができます。

**URL**

GET/serviceInfo

クエリパラメーター

なし. また、このエンドポイントへの呼び出しに認証は必要ありません。

**応答**

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

**例：** https://www.acme.com/api/serviceInfo

**戻り値**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### フォルダーの作成

（バージョン 1.2 で追加）特定のディレクトリにフォルダーを作成します。
URL

POST/createFolder

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| parentId  | フォルダーが作成されるフォルダー ID |
| name  | 新しいフォルダーの名前 |

{style=&quot;table-layout:auto&quot;}

 

**応答**

新しく作成されたフォルダーのメタデータ（/metadata エンドポイントで定義）。

**例：** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

戻り値

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### ドキュメントまたはフォルダの削除

（リリース日 — TBD）外部システム内の指定した ID を持つドキュメントまたはフォルダを削除します。 フォルダーを削除すると、その内容も削除されます。

URL

PUT/delete

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| documentId  | 削除するドキュメント ID |
| folderId  |  削除するフォルダー ID |

{style=&quot;table-layout:auto&quot;}

応答：以下のエラー処理の節で指定された、成功または失敗を示す JSON 文字列。

**例：** PUThttps://www.acme.com/api/delete id=1234

戻り値

```
{
"status": "success" 
}
```

戻り値

```
{
"status": "failure", "error": "File not found"
}
```


### ドキュメントまたはフォルダの名前を変更する

（リリース日 — TBD）外部システムで指定した ID を持つドキュメントまたはフォルダーの名前を変更します。

URL

PUT/rename

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| id | 名前を変更するドキュメントまたはフォルダー ID |
| name  | ドキュメントまたはフォルダの新しい名前 |

{style=&quot;table-layout:auto&quot;}

 

応答

以下のエラー処理の節で指定された、成功または失敗を示す JSON 文字列。

**例:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### カスタムアクションの実行

（リリース日 — 未定）このエンドポイントを使用すると、Workfrontユーザー（または自動ワークフローイベント）が外部システムでアクションを実行できるようになります。 /customAction エンドポイントは、「name」パラメーターを受け取ります。これにより、Webhook プロバイダーは複数のカスタム操作を実装できます。

Webhook プロバイダーは、カスタムアクションを customActions の下の/serviceInfo 応答に含めることで、Workfrontに登録します。 Workfrontは、設定/ドキュメント/カスタム統合で webhook プロバイダーを設定または更新すると、このリストを読み込みます。\
![](assets/mceclip0-350x262.png)

ユーザーは、「ドキュメントのトリガー」の下のセクションを選択することで、カスタムのアクションを実行できます\
![](assets/mceclip1-350x95.png)

**URL**

GET/customAction

**クエリパラメーター**

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
   <td><p>name</p></td>
   <td><p>実行するアクションのタイプを指定する識別子。 この値は、 /serviceInfo エンドポイントから返される customAction 値の 1 つに対応します。</p></td>
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

 

**応答**

以下のエラー処理の節で指定された、成功または失敗を示す JSON 文字列。 失敗した場合（例：status = &quot;failure&quot;）、Workfrontは提供されたエラーメッセージをユーザーに表示します。

**例：** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

応答

```
{
"status": "success" 
}
```


## エラー処理

API リクエストを処理する際に問題が発生する場合があります。 これは、すべての API エンドポイントをまたいで一貫した方法で処理する必要があります。 エラーが発生した場合は、Webhook プロバイダーが次の操作をおこないます。

* 応答ヘッダーにエラーコードを含めます。 次のエラーコードが含まれます。

   * 403 — 禁止。 リクエストトークンが見つからないか無効であるか、トークンに関連付けられている資格情報に指定されたリソースへのアクセス権がないことを示します。 OAuth ベースの Webhook プロバイダーの場合、Workfrontは新しいアクセストークンの取得を試みます。
   * 404 — 見つかりません。 指定したファイルまたはフォルダが存在しないことを示します。
   * 500 — 内部サーバーエラー。 その他のタイプのエラー。

* 次の形式を使用して、応答の本文にエラーの説明を記述します。


```
{
"status": "error"
"error": "Sample error message" 
}
```


## テスト

ドキュメントの Webhook の実装が正しく動作することを確認するには、次のテストを実行します。 これらは、Workfront Web インターフェイスを介して Webhook 実装のエンドポイントに間接的にヒットする手動のテストです。

### 前提条件

これらのテストを実行するには、以下が必要です。

* Advanced Document Management (ADM) が有効なWorkfrontアカウント
* このアカウントのWorkfrontユーザーがシステム管理者権限を持つ
* Workfrontから HTTP エンドポイントにアクセスできるドキュメント Webhook インスタンス

また、これらのテストでは、セットアップ/ドキュメント/カスタム統合で、Workfrontで Document Webhook インスタンスを既に登録していることを前提としています。

### テスト 1:ユーザー用のドキュメント Webhook サービスのプロビジョニング

OAuth ベースの Webhook プロバイダーの認証 URL およびトークンエンドポイント URL をテストします。

1. Workfrontで、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. 「ドキュメントを追加」ドロップダウンをクリックし、「サービスを追加」で Document Webhook サービスを選択します。
1. （OAuth サービスのみ）前の手順を完了すると、サービスの OAuth2 認証ページ読み込みがポップアップウィンドウに表示されます。 ( 注意：最初にサービスにログインするよう求められる場合があります )。 認証ページで、「信頼」または「許可」ボタンをクリックして、Workfrontにユーザーのアカウントへのアクセス権を付与します。
1. サービスが「ドキュメントの追加」ドロップダウンに追加されたことを確認します。 最初に表示されない場合は、ブラウザーを更新してみてください。

### テスト 2:ドキュメントをWorkfrontにリンクする次のエンドポイントをテストします。/files, /metadata

1. Workfrontで、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. 「ドキュメントの追加」で Document Webhook サービスを選択します。
1. モーダルから、フォルダー構造内を移動します。
1. フォルダー構造を正しくナビゲートできることを確認します。
1. ドキュメントを選択してWorkfrontにリンク

### テスト 3:コンテンツ管理システム内のドキュメントに移動します

次のエンドポイントをテストします。/metadata （具体的には viewLink）

1. ドキュメントをWorkfrontにリンク
1. ドキュメントを選択し、「開く」リンクをクリックします。
1. ドキュメントが新しいタブで開いていることを確認します。

### テスト 4:コンテンツ管理システム内のドキュメント（ログインを使用）に移動します

次のエンドポイントをテストします。/metadata （具体的には viewLink）

1. コンテンツ管理システムからログアウトしていることを確認します。
1. ドキュメントをWorkfrontにリンクします。
1. ドキュメントを選択し、「開く」リンクをクリックします。
1. 新しいタブで、コンテンツ管理システムのログイン画面が読み込まれることを確認します。
1. ログインして、ドキュメントに移動したことを確認します

### テスト 5:コンテンツ管理システムからドキュメントをダウンロードします

次のエンドポイントをテストします。/metadata （特に downloadLink）

1. ドキュメントをWorkfrontにリンクします。
1. ドキュメントを選択し、「ダウンロード」リンクをクリックします。
1. ダウンロードが開始されることを確認します。

### テスト 6:コンテンツを検索

次のエンドポイントをテストします。/search

1. Workfrontで、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. 「ドキュメントの追加」で Document Webhook サービスを選択します。
1. モーダルから検索を実行します。
1. 検索結果が正しいことを確認します。

### テスト 7:Workfrontからコンテンツ管理システムにドキュメントを送信

次のエンドポイントをテストします。/files, /uploadInit, /upload

1. Workfrontで、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. お使いのコンピューターからWorkfrontにドキュメントをアップロード
1. ドキュメントの詳細ページに移動します。
1. 「ドキュメントアクション」ドロップダウンから、「送信先… 」の下で Document Webhook サービスを選択します。
1. 目的の宛先フォルダーに移動し、「保存」ボタンをクリックします。
1. コンテンツ管理システムでドキュメントが正しい場所にアップロードされていることを確認します。

### テスト 8:Workfrontでのサムネールの表示

次のエンドポイントをテストします。/thumbnail

1. ドキュメントをWorkfrontにリンクします。
1. リストからドキュメントを選択します。
1. サムネールが右側のパネルに表示されることを確認します。

### テスト 9:コンテンツのバイト数を取得します

次のエンドポイントをテストします。/download

1. ドキュメントをWorkfrontにリンクします。
1. ドキュメントの詳細ページに移動します。
1. ドキュメントアクション/送信先/Workfrontを選択して、ドキュメントをWorkfrontに送信します。 これにより、Workfrontに新しいドキュメントバージョンが作成されます。
1. 「ダウンロード」リンクをクリックして、Workfrontからドキュメントをダウンロードします。

### テスト 10:アクセストークンを更新（OAuth2 Webhook プロバイダーのみ）

次のエンドポイントをテストします。トークンエンドポイント URL

1. ユーザー用のドキュメント Webhook サービスのプロビジョニング
1. 1 ) タイムアウトを待機しているか、2) 外部システムで手動で無効にして、ユーザーのアクセストークンを無効にします。
1. Workfrontでアクセストークンを更新します。 例えば、ドキュメントをWorkfrontにリンクすることで、これを実行できます。 に移動してドキュメントをリンクできる場合は、アクセストークンが正常に更新されたことがわかります。

>[!NOTE]
>
>現在、リンクされたドキュメントには [ 送信先 ] を使用できません。 これはWorkfrontによって追加されます。 Postmanなどの REST クライアントを使用してエンドポイントを手動でヒットし、/download エンドポイントをテストできます。 または、デジタル配達確認を生成して、/download エンドポイントをテストすることもできます。 デジタル校正を有効にするには、Workfrontにお問い合わせください。

## バージョン

* バージョン 1.0（リリース日 — 2015 年 5 月）

   * 初期仕様

* バージョン 1.1（リリース日 — 2015 年 6 月）

   * /uploadInit の更新 — documentId と documentVersionId の追加

* バージョン 1.2（リリース日 — 2015 年 10 月）

   * /createFolder を追加しました

