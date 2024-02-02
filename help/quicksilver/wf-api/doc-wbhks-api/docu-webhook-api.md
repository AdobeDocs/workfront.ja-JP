---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメント Webhooks API
description: ドキュメント Webhooks API
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '3620'
ht-degree: 100%

---


# ドキュメント Webhooks API

Adobe Workfront のドキュメント Web フックは、Workfront が外部ドキュメントプロバイダーに対して認可された API 呼び出しを行う API エンドポイントのセットを定義します。これにより、誰でも任意のドキュメントストレージプロバイダー用のミドルウェアプラグインを作成できます。

Web フックベースの統合のユーザーエクスペリエンスは、Google Drive、Box、Dropboxなどの既存のドキュメント統合のユーザーエクスペリエンスに似ています。例えば、Workfront ユーザーは以下のアクションを実行できます。

* 外部ドキュメントプロバイダーのフォルダー構造をナビゲート
* ファイルを検索
* ファイルを Workfront にリンク
* 外部ドキュメントプロバイダーにファイルをアップロード
* ドキュメントのサムネールを表示

## 参照の実装

新しい web フック実装の開発をすぐに開始できるように、Workfront では参照の実装を提供しています。このためのコードは [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) にあります。この実装は Java ベースで、Workfront がネットワークファイルシステム上でドキュメントに接続できるようにします。

## Web フック統合の登録

Workfrontの 管理者は、Workfront 内で設定／ドキュメント／カスタム統合に移動して、会社のカスタム web フック統合を追加することができます。設定内のカスタム統合ページから、管理者は既存のドキュメント web フック統合のリストを表示することができます。このページから、統合を追加、編集、有効化、無効化することができます。統合を追加するには、「統合を追加」ボタンをクリックします。

### 使用可能なフィールド

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
   <td> <p>すべての API 呼び出しの文字列に追加されるオプションの値。例：access_type=offline</p> <p> </p> </td> 
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
   <td> <p>（OAuth2 のみ）OAuth2 トークンを取得するために使用される完全な API URL。これは、web フックプロバイダーまたは外部ドキュメントプロバイダーによってホストされます</p> <p> </p> </td> 
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
   <td>  <p>（OAuth2 のみ）これは読み取り専用のフィールドで、Workfront によって生成されます。この値は、この統合を外部のドキュメントプロバイダーに登録するために使用されます。メモ：前述の認証 URL と同様、リダイレクトを実行する際にプロバイダーは「state」パラメーターとその値をクエリ文字列に追加する必要があります。</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>（ApiKey のみ）web フックプロバイダーに対して承認済み API 呼び出しを行うために使用されます。Web フックプロバイダーで発行された API キー。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 認証

Workfront ドキュメント web フックでは、OAuth2 および ApiKey の 2 種類の認証形式をサポートしています。どちらの場合も、Workfront は API を呼び出す際に、認証トークンをヘッダーに入れて渡します。

### OAuth2

OAuth2 を使用すると、Workfront は、承認済み API 呼び出しをユーザーの代わりに web フックプロバイダーに対して行うことができます。その前に、ユーザーは外部ドキュメントプロバイダーアカウントを Workfront に接続し、Workfront への

アクセス権を付与して、ユーザーの代わりに操作できるようにする必要があります。このハンドシェイクプロセスは、ユーザーごとに 1 回だけ行われます。仕組みは次のとおりです。

1. まずユーザーが自分のアカウントに web フック統合を接続します。現在、これを行うには、「ドキュメントの追加」ドロップダウン／サービスを追加／カスタム統合名をクリックします。
1. Workfront により、ユーザーは認証 URL に移動します。ここでは、外部ドキュメントプロバイダーへのログインを求められる場合があります。このページは、web フックプロバイダーまたは外部ドキュメント管理システムによってホストされています。その際、Workfront は認証 URL に「state」パラメーターを追加します。同じ値を以下の手順で Workfront の戻り URI に追加することにより、この値を Workfront に返す必要があります。
1. 外部システムにログインしたら（またはユーザーが既にログインしている場合）、「認証」ページが表示され、ユーザーの代わりに一連のアクションを実行するためのアクセス権を Workfront が要求していることが説明されます。
1. ユーザーが「許可」ボタンをクリックすると、ブラウザーは Workfront リダイレクト URI にリダイレクトされ、その際にクエリ文字列に「code=`<code>`」が追加されます。OAuth2 仕様に従い、このトークンの有効期間は短く設定されています。クエリ文字列には「state=`<sent_by_workfront>`」も必要です。
1. Workfront はこのリクエストを処理し、認証コードを使用してトークンエンドポイント URL への API 呼び出しを行います。
1. トークンエンドポイント URL は、更新トークンとアクセストークンを返します。
1. Workfront はこれらのトークンを保存し、このユーザーに対して web フック統合を完全にプロビジョニングします。
1. これ以降、Workfront は web フックプロバイダーに対して、承認済み API 呼び出しを実行できるようになります。これらの呼び出しを行う際に、Workfront は、以下に示すように、アクセストークンを HTTP リクエストヘッダーに入れて送信します。

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. アクセストークンの有効期限が切れている場合、Workfront はトークンエンドポイント URL を呼び出して新しいアクセストークンを取得したあと、その新しいアクセストークンを使用して承認済み API 呼び出しを再度試みます。

### ApiKey

ApiKey を使用して web フックプロバイダーへの承認済み API 呼び出しを行う方が、OAuth2 よりもはるかに簡単です。API 呼び出しを行う際に、Workfront は ApiKey と Workfront ユーザー名を HTTP リクエストヘッダーに入れて渡すだけです。

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Web フックプロバイダーは、このユーザー名を使用して、ユーザー固有の権限を適用できます。この仕組みが最も効果を発揮するのは、両方のシステムがシングルサインオン（SSO）を使用して LDAP に接続している場合です。

### リクエストヘッダーの追加（オプション）

Workfront では、認証に OAuth2 トークンまたは ApiKey を使用する以外に、あらかじめ定義された一連のヘッダーを API 呼び出しごとに web フックプロバイダーに送信できます。前の節で説明したように、Workfront 管理者は web フック統合の登録または編集時にこれを設定できます。「Web フック統合の登録」を参照してください。

例えば、これは基本認証に使用できます。それには、Workfront 管理者がカスタム統合ダイアログで次のリクエストヘッダー情報を追加します。

   Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==

この QWxhZGRpbjpvcGVuIHNlc2FtZQ== は、「username:password」を Base64 でエンコードした文字列です。「基本認証」を参照してください。これが追加された場合、Workfront はこれを次のように、他のリクエストヘッダーに加えて、HTTP リクエストヘッダーに入れて渡します。

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API 仕様

ドキュメント web フックを機能させるために web フックプロバイダーが実装する必要がある API のリストを以下に示します。

### OAuth2 トークンの取得（OAuth2 認証のみ必要）

認証済みユーザーの OAuth2 更新トークンとアクセストークンを返します。この呼び出しは、ユーザーがドキュメント提供者をプロビジョニングするときに 1 回だけ実行されます。その後の呼び出しは、更新されたアクセストークンを取得するために行われます。

HTTP リクエスト POST [任意の URL]

この URL は設定可能で、カスタム統合設定ページのトークンエンドポイント URL 値に対応しています。

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
   <td> <p>値は「authorization_code」か「refresh_token」のいずれかです。指定した値は、この API 呼び出しに渡される 2 つのパラメーターのうち、code または refresh_token のいずれかを示します。</p> </td> 
  </tr> 
  <tr> 
   <td>コード</td> 
   <td>依存</td> 
   <td> <p>ユーザーが「付与」ボタンをクリックした直後に Workfront に送信される認証コード。これは、grant_type が「authorization_code」の場合にのみ必要です。認証コードは短期間のみ有効で、通常は 10 分以内に期限が切れます。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>依存</td> 
   <td> <p>これは、以前の access_token が期限切れである場合に、新しい access_token を取得するために後続の呼び出しを行う場合にのみ必要です。この値を送信する場合は、grant_type パラメーターを「refresh_token」に設定します。</p> </td> 
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
   <td>access_token.</td> 
   <td>文字列</td> 
   <td> <p>ユーザーに代わって認証済み API 呼び出しを行うために使用されるトークン。許可されていない API 呼び出しを防ぐために期限切れになります。</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token.</td> 
   <td>文字列</td> 
   <td> <p>この API メソッドを呼び出して新しい access_token を取得するのに使用される、長期間有効なトークン。</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in,</td> 
   <td>long</td> 
   <td>  <p>（オプション）access_token の有効期限が切れるまでの時間（秒単位）。通常は 3,600 です。</p></td> 
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

GET /metadata?id=[document or folder ID]

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
   <td>  <p>Web フックプロバイダーで参照される、ファイルまたはフォルダーの ID。これは、Workfront のドキュメント ID とは異なります。ルートディレクトリのメタデータを取得するには、値「/」を使用します。</p><p>メモ：ID の最大長は 255 文字です。</p></td> 
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
   <td>タイトル</td> 
   <td>文字列</td> 
   <td>ドキュメントまたはフォルダーの名前</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>文字列</td> 
   <td>この項目がファイルかフォルダーかを指定します（値は「file」か「folder」のどちらか）</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>文字列</td> 
   <td>ファイルまたはフォルダーの ID。</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>文字列</td> 
   <td> <p>ブラウザーウィンドウでドキュメントを表示するためにユーザーが使用する URL パス。この URL は、ドキュメントプロバイダーかネイティブ外部ストレージプロバイダーのどちらかでホストできます。</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>文字列</td> 
   <td> <p>ブラウザーウィンドウでドキュメントをダウンロードするためにユーザーが使用する URL パス。この URL は、ドキュメントプロバイダーかネイティブ外部ストレージプロバイダーのどちらかでホストできます。</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>文字列</td> 
   <td>ファイルの MIME タイプ（オプション）</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>文字列</td> 
   <td>このファイルが最後に変更された日時（RFC 3339 形式のタイムスタンプ）</td> 
  </tr> 
  <tr> 
   <td>サイズ</td> 
   <td>Long</td> 
   <td>バイト単位で表したファイルサイズ。（オプション）</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>ブール値</td> 
   <td>  <p>このファイルまたはフォルダーが認証済みユーザーに対して読み取り専用かどうかを示します。（オプション）</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**例：**`https://www.acme.com/api/metadata?id=12345`

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
>エラー処理は、すべての API 呼び出しで一貫している必要があります。詳しくは、以降の「エラー処理」の節を参照してください。

### フォルダーに含まれる項目のリストの取得

指定されたフォルダーのファイルおよびフォルダーのメタデータを返します。

**URL**

GET /files

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| parentId  | フォルダー ID。ルートディレクトリのメタデータを取得するには、値「/」を使用します。 |

{style="table-layout:auto"}

ドキュメント web フック API では、現在、ページネーションをサポートしていません。

**応答**

ファイルとフォルダーのリストを含んだ JSON。各項目のメタデータは、/metadata エンドポイントから返されるメタデータと同じです。

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

### 検索の実行

検索から返されたファイルやフォルダーのメタデータを返します。これは、全文検索としてまたは通常のデータベースクエリとして実行できます。ユーザーが外部ファイルブラウザーから検索を実行すると、Workfront が /search エンドポイントを呼び出します。

**URL**

GET /search

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
   <td>query</td> 
   <td>検索語または検索フレーズ</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>（オプション）検索の実行元フォルダーの ID。メモ：これは、Workfront の将来的な機能用のプレースホルダーです。現在、Workfront ではこのパラメーターを渡しません。 </p> </td> 
  </tr> 
  </tbody> 
</table>

ドキュメント web フック API では、現在、ページネーションをサポートしていません。

 

**応答**

クエリに一致するファイルやフォルダーのメタデータのリストを含んだ JSON。何をもって「一致」とするかは、web フックプロバイダーによって決まります。全文検索を行うのが理想です。ファイル名ベースの検索も有効です。

**例：**`https://www.acme.com/api/search?query=test-query`

**応答**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### ドキュメントのコンテンツの取得

ドキュメントの未加工のバイトデータを返します

**URL**

GET /download

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
   <td>ドキュメント ID</td> 
  </tr> 
 </tbody> 
</table>

 

**応答**

ドキュメントの未加工のバイトデータ。

**例：**`https://www.acme.com/api/download?id=123456`

### ドキュメントのサムネールの取得

ドキュメントのサムネールの未加工バイトデータを返します。

**URL**

GET /thumbnail

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| id  | ドキュメント ID |
| size  | サムネールの幅 |

{style="table-layout:auto"}

 

**応答**

サムネールの未加工のバイトデータです。

**例：**`https://www.acme.com/api/thumbnail?id=123456`

### ファイルのアップロード（前半）

ドキュメントストレージプロバイダーへのファイルのアップロードは、2 つの異なる API エンドポイントを必要とする 2 段階プロセスです。Workfront は、/uploadInit を呼び出して、アップロードプロセスを開始します。このエンドポイントはドキュメント ID を返します。この ID は、ドキュメントのバイトデータをアップロードする際に /upload に渡されます。基盤となるドキュメントストレージシステムによっては、長さ 0 のドキュメントを作成した後でドキュメントの内容を更新する必要がある場合があります。

ドキュメント ID とドキュメントバージョン ID を使用して、Workfront から追加の情報を取得できる機能が、この仕様のバージョン 1.1 に追加されました。例えば、ドキュメント管理システムがドキュメントに関する追加情報を必要とする場合に、web フックの実装コードでドキュメント ID を使用して、Workfront の RESTful API でその情報を取得するといったことができます。このような情報は、ドキュメントのカスタムデータフィールドから取得するのが優れたプラクティスです。また、情報にはタスク、イシューまたはプロジェクトを含めます。

**URL**

POST /uploadInit

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
   <td>Web フックプロバイダーで参照される親フォルダー ID。</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>ドキュメントの名前</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront ドキュメント ID（バージョン 1.1 で追加）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId</td> 
   <td>Workfront ドキュメントのバージョン ID（バージョン 1.1 で追加）</td> 
  </tr> 
 </tbody> 
</table>

 

**応答**

/metadata エンドポイントで定義した、ファイルのメタデータです。

**例：**`https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**応答**

`[file_metadata]` には、ドキュメントプロバイダーで使用される新しいドキュメント ID が含まれます。

### ファイルのアップロード（後半）

Web フックプロバイダーにドキュメントのバイトデータをアップロードします。

**URL**

PUT /upload

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| id  | 前半で作成されたドキュメント ID。 |


 

**リクエスト本文**

ドキュメントの Raw コンテンツのバイトデータです。

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

**例：**`https://www.acme.com/api/upload?id=1234` *[更新ストリームに含まれるドキュメントのバイトデータ]*

**応答**

```
{
"result":"success"
}
```

### サービスに関する情報の取得

（リリース日 - 未定）特長や機能など、サービスに関する情報を返します。Workfront では、この情報を使用して Workfront のユーザーインターフェイスをカスタマイズします。例えば、web フックの実装にいくつかのカスタムアクションが含まれている場合、それらの操作は JSON でリストする必要があります。それにより、ユーザーは、これらのアクションを Workfront から呼び出すことができるようになります。

**URL**

GET /serviceInfo

クエリパラメーター

なし。さらに、このエンドポイントへの呼び出しには、認証も必要ありません。

**応答**

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

### フォルダーを作成

（バージョン 1.2 で追加）特定のディレクトリにフォルダーを作成します。
URL

POST /createFolder

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| parentId  | フォルダーを作成するフォルダーの ID |
| 名前  | 新規フォルダーの名前 |

{style="table-layout:auto"}

 

**応答**

新しく作成されたフォルダーのメタデータ（/metadata エンドポイントで定義）。

**例：**`POST https://www.acme.com/api/createFolder`

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

### ドキュメントまたはフォルダーの削除

（リリース日 - 未定）外部システム内の特定の ID を持つドキュメントまたはフォルダーを削除します。フォルダーを削除すると、その内容も削除されます。

URL

PUT /delete

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| documentId  | 削除するドキュメントの ID |
| folderId  | 削除するフォルダーの ID |

{style="table-layout:auto"}

成功または失敗を示す応答 JSON 文字列（この後の「エラー処理」の節を参照）。

**例：** PUT https://www.acme.com/api/delete?documentId=1234

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


### ドキュメントまたはフォルダーの名前変更

（リリース日 - 未定）外部システム内の特定の ID を持つドキュメントまたはフォルダーの名前を変更します。

URL

PUT /rename

**クエリパラメーター**

| 名前  | 説明 |
|---|---|
| id | 名前を変更するドキュメントまたはフォルダーの ID |
| 名前  | ドキュメントまたはフォルダーの新しい名前 |

{style="table-layout:auto"}

 

応答

成功または失敗を示す JSON 文字列（この後の「エラー処理」の節を参照）。

**例：**

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

（リリース日 - 未定）このエンドポイントを使用すると、Workfront ユーザー（または自動化ワークフローイベント）が外部システムでアクションを実行できるようになります。/customAction エンドポイントは、「name」パラメーターを受け取ります。これにより、web フックプロバイダーは複数のカスタム操作を実装できます。

Web フックプロバイダーでは、カスタムアクションを /serviceInfo 応答の customActions 下に含めることで、Workfront に登録します。設定／ドキュメント／カスタム統合で web フックプロバイダーを設定または更新すると、Workfront がこのリストを読み込みます。\
![](assets/mceclip0-350x262.png)

ユーザーは、「ドキュメントアクション」の下のセクションを選択することで、カスタムアクションをトリガーできます。\
![](assets/mceclip1-350x95.png)

**URL**

GET /customAction

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
   <td><p>名前</p></td>
   <td><p>実行するアクションのタイプを指定する識別子。この値は、/serviceInfo エンドポイントから返される customAction 値のうちの 1 つに対応します。</p></td>
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

 

**応答**

成功または失敗を示す JSON 文字列（この後の「エラー処理」の節を参照）。失敗（status = &quot;failure&quot;）の場合、Workfront は、用意されているエラーメッセージをユーザーに表示します。

**例：** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

応答

```
{
"status": "success" 
}
```


## エラー処理

API リクエストを処理する際に問題が発生する場合があります。その対応は、すべての API エンドポイントで一貫した方法で行う必要があります。エラーが発生した場合は、web フックプロバイダーが以下を行います。

* 応答ヘッダーにエラーコードを含めます。エラーコードの例は次のとおりです。

   * 403 - Forbidden（禁止されている）リクエストトークンが見つからない、または無効であるか、トークンに関連付けられている資格情報に、指定されたリソースへのアクセス権がないことを示します。OAuth ベースの web フックプロバイダーの場合、Workfront は新しいアクセストークンの取得を試みます。
   * 404 - Not found（見つからない）指定したファイルまたはフォルダーが存在しないことを示します。
   * 500 - Internal Server Error（内部サーバーエラー）その他の種類のエラーです。

* 応答の本文に次の形式でエラーの説明を記述します。


```
{
"status": "error"
"error": "Sample error message" 
}
```


## テスト

ドキュメント web フックの実装が正しく動作することを確認するには、以下のテストを実行します。これらは、Workfront web インターフェイスを介して web フック実装のエンドポイントに間接的にヒットする手動のテストです。

### 前提条件

これらのテストを実行するには、以下が必要です。

* 高度文書管理（ADM）が有効になっている Workfront アカウント
* システム管理者権限を持つ、このアカウントの Workfront ユーザー 1 名
* Workfront から HTTP エンドポイントにアクセスできるドキュメント web フックインスタンス

またこれらのテストでは、Workfront の設定／ドキュメント／カスタム統合でドキュメント web フックインスタンスを既に登録していることも前提としています。

### テスト 1：ユーザーへのドキュメント web フックサービスのプロビジョニング

OAuth ベースの web フックプロバイダーの認証 URL とトークンエンドポイント URL をテストします。

1. Workfront で、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. ドキュメントを追加ドロップダウンをクリックし、「サービスを追加」でドキュメント web フックサービスを選択します。
1. （OAuth サービスのみ）前の手順を完了すると、サービスの OAuth2 認証ページがポップアップウィンドウに読み込まれて表示されます。（メモ：最初にサービスにログインするように求められる場合があります）。認証ページで、「信頼」ボタンまたは「許可」ボタンをクリックして、Workfront へのアクセス権をユーザーのアカウントに付与します。
1. ドキュメントを追加ドロップダウンにサービスが追加されたことを確認します。初めに表示されない場合は、ブラウザーを更新してみてください。

### テスト 2：Workfront へのドキュメントのリンク（/files および /metadata エンドポイントをテストします）

1. Workfront で、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. 「ドキュメントを追加」でドキュメント web フックサービスを選択します。
1. モーダルでフォルダー構造内を移動します。
1. フォルダー構造内を正しく移動できることを確認します。
1. ドキュメントを選択して Workfront にリンクします。

### テスト 3：コンテンツ管理システム内のドキュメントへの移動

/metadata エンドポイント（特に viewLink）をテストします。

1. Workfront にドキュメントをリンクします。
1. そのドキュメントを選択し、「開く」リンクをクリックします。
1. ドキュメントが新しいタブで開くことを確認します。

### テスト 4：コンテンツ管理システム内のドキュメントへの移動（ログインを使用）

/metadata エンドポイント（特に viewLink）をテストします。

1. コンテンツ管理システムからログアウトしていることを確認します。
1. Workfront にドキュメントをリンクします。
1. そのドキュメントを選択し、「開く」リンクをクリックします。
1. コンテンツ管理システムのログイン画面が新しいタブに読み込まれることを確認します。
1. ログインして、ドキュメントに移動したことを確認します。

### テスト 5：コンテンツ管理システムからのドキュメントのダウンロード

/metadata エンドポイント（特に downloadLink）をテストします。

1. Workfront にドキュメントをリンクします。
1. そのドキュメントを選択し、「ダウンロード」リンクをクリックします。
1. ダウンロードが開始されることを確認します。

### テスト 6：コンテンツの検索

/search エンドポイントをテストします。

1. Workfront で、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. 「ドキュメントを追加」でドキュメント web フックサービスを選択します。
1. モーダルで検索を実行します。
1. 検索結果が正しいことを確認します。

### テスト 7：Workfront からコンテンツ管理システムへのドキュメントの送信

/files、/uploadInit および /upload エンドポイントをテストします。

1. Workfront で、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. お使いのコンピューターから Workfront にドキュメントをアップロードします。
1. ドキュメントの詳細ページに移動します。
1. ドキュメント アクションドロップダウンから、「送信先」でドキュメント web フックサービスを選択します。
1. 目的の宛先フォルダーに移動し、「保存」ボタンをクリックします。
1. ドキュメントがコンテンツ管理システム内の正しい場所にアップロードされていることを確認します。

### テスト 8：Workfront でのサムネールの表示

/thumbnail エンドポイントをテストします。

1. Workfront にドキュメントをリンクします。
1. リストでドキュメントを選択します。
1. サムネールが右側のパネルに表示されることを確認します。

### テスト 9：コンテンツのバイトデータの取得

/download エンドポイントをテストします。

1. Workfront にドキュメントをリンクします。
1. ドキュメントの詳細ページに移動します。
1. ドキュメント アクション／送信先／Workfront を選択して、ドキュメントを Workfront に送信します。この結果、Workfront に新しいドキュメントバージョンが作成されます。
1. 「ダウンロード」リンクをクリックして、このドキュメントを Workfront からダウンロードします。

### テスト 10：アクセストークンの更新（OAuth2 web フックプロバイダーの場合のみ）

トークンエンドポイント URL のエンドポイントをテストします。

1. ドキュメント web フックサービスをユーザーにプロビジョニングします。
1. 1）タイムアウトまで待機する、2）外部システムで手動で無効にする、のいずれかの方法で、ユーザーのアクセストークンを無効にします。
1. Workfront でアクセストークンを更新します。それには、例えば、Workfront にドキュメントをリンクします。ドキュメントに移動してリンクできれば、アクセストークンが正常に更新されたことがわかります。

>[!NOTE]
>
>現在、リンクされたドキュメントの場合は「送信先」を使用できません。この機能は Workfront に追加される予定です。/download エンドポイントをテストするには、Postman などの REST クライアントを使用して、手動でエンドポイントにヒットさせます。または、デジタルプルーフを生成して、/download エンドポイントをテストすることもできます。デジタルプルーフを有効にするには、Workfront 管理者にお問い合わせください。

## バージョン

* バージョン 1.0（リリース日 - 2015年5月）

   * 初期仕様

* バージョン 1.1（リリース日 - 2015年6月）

   * /uploadInit の更新 - documentId と documentVersionId の追加

* バージョン 1.2（リリース日 - 2015年10月）

   * /createFolder の追加

