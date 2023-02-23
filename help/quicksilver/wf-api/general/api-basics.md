---
content-type: api
navigation-topic: general-api
title: API の基本
description: API の基本
author: John
feature: Workfront API
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: c1cec2c08c66c704385cde1abd0c019fd59702da
workflow-type: tm+mt
source-wordcount: '4405'
ht-degree: 0%

---


# API の基本

Adobe Workfront API の目的は、HTTP 経由で動作する REST フルアーキテクチャを導入することで、Workfrontとの統合の構築を簡略化することです。 このドキュメントでは、REST および JSON の応答に精通していることを前提とし、Workfront API がとるアプローチについて説明します。

Workfrontスキーマに精通していれば、統合のためにWorkfrontからデータを取り出すために使用できるデータベースの関係を理解するのに役立ちます。

## 制限とガイドライン

Workfront On-Demand システムのパフォーマンスを一貫させるために、各顧客は 10 個の同時 API スレッドに制限されています。 サンドボックス環境にも同じ制限があるので、顧客とパートナーは、コードを実稼動環境にリリースする前に API 呼び出しを正確にテストできます。

実稼動、プレビューおよびテストドライブ環境の場合、エンドユーザーリクエストはWorkfront CDN(Akamai) を介してルーティングされるので、URI の最大長は 8892 バイトです。 この制限は、CDN 経由でルーティングされる URI にのみ適用されます。

>[!NOTE]
>
>サンドボックス環境は CDN を通じてルーティングされないので、この制限はサンドボックス環境には適用されません。

### 免責事項

API の使用は、実稼動環境で実行する前に、Workfrontベータ環境でテストする必要があります。 お客様が、Workfrontがオンデマンドソフトウェアに対して負担が大きいと合理的に考えるプロセス（つまり、プロセスが他のお客様に対するソフトウェアの実行に重大な悪影響を与える）で API を使用している場合、Workfrontは、お客様に対し、そのプロセスを中止する権利を留保します。 お客様が遵守せず、問題が解決しない場合、Workfrontはプロセスを終了する権利を留保します。

## REST の基本

この節では、次の REST 原則に対するWorkfront REST API の操作方法の概要を説明します。

### オブジェクト URI

システム内の各オブジェクトには、オブジェクトタイプと ID で構成される一意の URI が提供されます。 次の例は、3 つの一意のオブジェクトを記述する URI を示しています。

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

オブジェクトタイプは大文字と小文字が区別されず、省略された ObjCode（proj など）または代替オブジェクト名（project など）を指定できます。

有効な ObjCode のリストについては、  [API エクスプローラ](../../wf-api/general/api-explorer.md).

### 操作

オブジェクトは、一意の URI に HTTP リクエストを送信することで操作されます。 実行する操作は HTTP メソッドで指定します。

標準の HTTP メソッドは、次の操作に対応しています。

* **GET** - ID でオブジェクトを取得し、クエリですべてのオブジェクトを検索し、レポートを実行し、名前付きクエリを実行します
* **POST**  — 新しいオブジェクトを挿入します
* **PUT**  — 既存のオブジェクトを編集します
* **DELETE**  — オブジェクトを削除します

クライアントに問題がある場合やプロトコルの長さ制限を回避するために、メソッドパラメーターを使用して HTTP の動作を上書きできます。 例えば、GET操作は、次の URI を投稿することで実装できます。
<pre>GET/attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET/attask/api/v15.0/project/4c78...54d0?method=get</pre>

### 応答

各リクエストには、JSON 形式での応答が提供されます。 リクエストが成功した場合はデータ属性、問題が発生した場合はエラー属性のいずれかが応答に含まれます。 例えば、リクエスト

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

は、次のような JSON 応答を返します。


<pre>{<br>    "data":[<br>        {<br>            "percentComplete":0,<br>            "status":「CUR」<br>            "priority":2,<br>            "name":「新規プロジェクトのブランド化」<br>            "ID":"4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>ブラウザーのアドレスバーからGETリクエストを実行する場合、sessionID をリクエストの一部に含める必要はありません。

PUT、POST、DELETEの各リクエストに対する特別なセキュリティが追加されました。 データベースへの書き込みまたはデータベースからの削除を引き起こすリクエストは、 **sessionID=abc123** が URI に含まれている。 次の例は、これがどのようにDELETE要求を探すかを示しています。
<pre>GET/attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET/attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### 認証

API は、リクエストごとに認証をおこない、リクエストされたオブジェクトを表示または変更するためのアクセス権をクライアントが持つようにします。

認証は、次のいずれかの方法で指定できるセッション ID を渡すことで実行されます。

#### リクエストヘッダー認証

推奨される認証方法は、セッショントークンを含む SessionID という名前のリクエストヘッダーを渡すことです。 これは安全に対して有利である [クロスサイトリクエストフォージェリ (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) 攻撃を受け、キャッシュ目的で URI に干渉しない。

リクエストヘッダーの例を次に示します。

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### リクエストパラメーター認証

次の例に示すように、sessionID という名前のリクエストパラメーターを渡すことで認証できます。 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Cookie ベースの認証

API は、Web UI でシステムに使用されるのと同じ cookie ベースの認証を使用します。 ここで、クライアントが Web UI を使用してWorkfrontにログインした場合、同じブラウザー内でおこなわれたAJAX呼び出しは同じ認証を使用します。

>[!NOTE]
>
>CSRF(Cross Site Request Forgery) 攻撃の可能性から保護するために、この認証方法は読み取り専用操作でのみ使用できます。

## ログイン

>[!IMPORTANT]
Workfrontでは、 `/login` エンドポイントまたは API キー。 代わりに、次のいずれかの認証方法を使用します。
* JWT を使用したサーバー認証
* OAuth2 を使用したユーザー認証
>
これらの認証方法の設定手順については、 [Workfront統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)
Workfrontでのサーバー認証の使用手順については、 [JWT フローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-jwt-flow.md)
Workfrontでのユーザー認証を使用する手順については、 [認証コードフローを使用して、組織のカスタム OAuth 2 アプリケーションを設定および使用する](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
この節で説明する手順は、まだAdobeビジネスプラットフォームに転送されていない組織にのみ適用されます。 組織がWorkfront Business Platform にオンボーディングされている場合、Adobe API を使用してWorkfrontにログインすることはできません。
組織がAdobeビジネスプラットフォームにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

有効なユーザー名とパスワードを使用して、次のリクエストを使用してセッション ID を取得できます。

```
POST /attask/api/v15.0/login?username=admin&password=user
```

これにより、今後のリクエストを認証する Cookie が設定され、新しく作成された sessionID、ログインしたユーザーの userID、その他のセッション属性を使用して JSON 応答が返されます。

>[!NOTE]
管理者でもある指定された API ユーザーがいる場合、Workfrontでは、ログインに API キーを使用することを強くお勧めします。

**API キーの生成**

次の例に示すように、API キーは、ユーザーとしてシステムにログインする際に生成できます。


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**以前に生成した API キーの取得**

また、getApiKey を実行すると、特定のユーザー用に以前に生成された API キーを取得することもできます。


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

その後、この結果を使用して、sessionID またはユーザー名とパスワードの代わりにこの値を使用するリクエストパラメーターとして「apiKey」を追加することで、API 呼び出しを認証できます。 これは、セキュリティの観点からは有益です。

以下に、 apiKey を使用してプロジェクトからデータを取得する例を示します。

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**API キーの無効化**

apiKey 値が侵害された場合は、次の例に示すように、「clearApiKey」を実行して、現在の API キーを無効化できます。

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

クリアすると、getApiKey を再度実行して新しい API キーを生成できます。

### ログアウト

セッションが完了したら、次の要求を使用してユーザーをログアウトし、sessionID へのアクセスを禁止できます。

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

ログアウトする sessionID は、cookie、リクエストヘッダーまたはリクエストパラメーターのいずれかとして指定できます。

ユーザーをログアウトするには：

1. ログイン画面に移動しますが、ログインはしません。
1. URL を/attask/api/v15.0/project/search に変更します。\
   ページが見つからないことに注意してください。
1. 置換 *検索* login?username=admin&amp;password=user を使用します。 *admin* および*ユーザ\
   *このセッションはブラウザーに cookie として保存され、後続のGETリクエストのたびに再開する必要はありません。

1. URL をに戻します。 **/attask/api/v15.0/project/search**.
1. 応答が提供されたことに注意してください。

PUT、POST、DELETEの各リクエストを実行する際は、ログイン後に提供される sessionID を必ず含める必要があります。

## GET動作

1 つ以上のオブジェクトを取得し、レポートを実行するには、HTTPGETメソッドを使用します。

### オブジェクトの取得

モディファイヤとフィルタを使用して、オブジェクトの検索を拡張できます。

#### オブジェクト ID を使用したオブジェクトの取得

オブジェクトの ID がわかっている場合は、一意の URI にアクセスしてオブジェクトを取得できます。 例えば、リクエスト

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

は、次のような応答を返します。

<pre>{<br>    "percentComplete":0,<br>    "status":「CUR」<br>    "priority":2,<br>    "name":「新規プロジェクトのブランド化」<br>    "ID":"4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


次の例に示すように、同じリクエストで複数のオブジェクトを取得するには、ID リクエストパラメーターを指定し、ID のコンマ区切りリストを指定します。


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

/attask/api/v15.0/project?id=...リクエストは `/attask/api/v15.0/project/...` リクエスト。

#### URI を使用したオブジェクトの取得

ID 以外の条件でオブジェクトを取得する場合は、URI を検索できます。

例えば、次のリクエストを使用して、システム内のすべてのプロジェクトのリストを返すことができます。

```
GET /attask/api/v15.0/project/search
```

要求パラメーターを名前と値のペアとして使用して、フィルターを指定できます。 例えば、次の例は、現在のすべてのプロジェクトを検索するリクエストを示しています。

```
GET /attask/api/v15.0/project/search?status=CUR
```

次のリクエストでは、まだ完了しておらず、John というユーザーに割り当てられているすべてのタスクを検索します。

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### 検索修飾子の使用

次の表に、Workfront API で使用できる修飾子の一部を示します。

| **修飾子** | **説明** | **例** |
|---|---|---|
| eq | 終了のステータスにある結果を返します | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | クローズ済みのステータスにない結果を返します | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | 完了の割合が 50 以上の結果を返します | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | 完了率が 50 以下の結果を返します | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | 説明が Null の結果を返します | <pre>...description_Mod=isnull...</pre> |
| notnull | 説明が Null でない結果を返します | <pre>...description_Mod=notnull...</pre> |
| 含む | 名前に「Workfront」が含まれる結果を返します | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| 間 | 過去 7 日間に入力日があった結果を返します | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
検索リクエストでは、大文字と小文字が区別されます。 エラーが発生した場合は、  **_Mod** および **範囲 (_R)** 大文字と小文字が正しい。

#### OR 文の使用

「OR」を含むパラメーターと数値を追加して検索を拡張し、フィルターまたは一連のフィルターのレベルを示すことができます。

OR ステートメントは、OR ステートメントのフィルタリング条件を満たす API 呼び出しのレコードのみを返します。 フィルターは、OR 文レベルで暗黙には含まれません。

例えば、をフィルタリングする場合は、

* 「Planning」を含む名前のタスク
* 「FixedAssets」という名前のポートフォリオ内のタスクで、「Steve」OR を含む名前の担当者に割り当てられています
* 「最終タスク」という親タスクを持つタスク

その後、次の API 呼び出しを複数の OR ステートメントと共に使用します。
<pre>GET/attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>OR(&amp;O):1:portfolio:name=FixedAssets<br>OR(&amp;O):1:portfolio:name_Mod=eq<br>OR(&amp;O):1:assignedTo:name=Steve<br>OR(&amp;O):1:assignedTo:name_Mod=cicontains<br>OR(&amp;O):2:parent:name=Final Task<br>OR(&amp;O):2:parent:name_Mod=eq
</pre>

#### フィルターパラメーターの使用

検索フィルターに URL パラメーターを使用する際に陥りそうな問題の 1 つは、Workfrontが特定のパラメーターを解析してから、様々な認証方法（ユーザー名、パスワード、apiKey、cookie）を確認することです。 この場合、パラメーターは呼び出しでフィルターとして使用されません。 

この問題を回避するには、JSON 形式のフィルターパラメーターにこれらの値を配置します。 例えば、を使用する代わりに、ユーザー名 testuser に対してフィルタリングを行う場合です。 
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>次の例に示すように、URL パラメーターをフィルターに渡します。
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### マップ要求パラメータの使用

デフォルトでは、検索から返されるデータは JSON 配列です。 使用例によっては、ID でインデックス付けされた JSON オブジェクトとして結果を取得するほうが効率的な場合があります。 これは、 map リクエストパラメーターを使用しておこなうことができます。 例えば、リクエスト 
<pre>/attask/api/v15.0/task/search?map=true</pre>次のような ID でインデックス付けされた応答を返します。
<pre>{<br>    "data":{<br>        "4c9a97db0000000f13ee446b9aead9b":{<br>            "percentComplete":0,<br>            "status":"NEW",<br>            "name":"最初のタスク"<br>            "ID":"4c9a97db0000000f13ee446b9aead9b",<br>            "taskNumber":1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601":{<br>            "percentComplete":0,<br>            "status":"INP:A",<br>            "name":「2 番目のタスク」<br>            "ID":"4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber":2 <br>        } <br>    } <br>}</pre>

#### Fields リクエストパラメーターの使用

デフォルトでは、オブジェクトを取得すると、最も一般的に使用されるフィールドのサブセットのみが返されます。

fields リクエストパラメーターを使用して、返されるフィールドのコンマ区切りリストを指定できます。 例えば、リクエスト
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>は、次のような応答を返します。
<pre>{<br>    "priority":2,<br>    "name":"最初のタスク"<br>    "ID":"4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate":"2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
これらのフィールド名では、大文字と小文字が区別されます。

使用可能なフィールド参照のリストについては、  [API エクスプローラ](../../wf-api/general/api-explorer.md)

#### ネストされたオブジェクトの検索

ネストされたオブジェクトを検索できます。 デフォルトでは、ネストされたオブジェクトは名前と ID のみを持って返されます。 例えば、すべての問題を所有者と共に取得するには、次のリクエストを使用します。
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>詳細な情報が必要な場合は、コロン構文を使用してネストされたフィールドを要求できます。 例えば、次のリクエストでは、所有者の名前、ID、タイトル、電話番号と共にすべての問題を検索します
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>を返します。 
<pre>{<br>    "name":「重要な問題だ」<br>    "ID":"4c78285f00000908ea8cfd66e084939f",<br>    "owner":{<br>        "title":「Operations Specialist」<br>        "phoneNumber":"555-1234",<br>        "name":"管理者ユーザー",<br>        "ID":"4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### ネストされたコレクションの取得

オブジェクトのネストされたコレクションを取得できます。 例えば、すべてのタスクを含むプロジェクトを取得するには、次のリクエストを使用します。
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>次のリクエストはタスクの割り当てを取得します。
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### 複数のネストされたフィールドの検索

デフォルトでは、各タスクの名前と ID のみが返されますが、コロン構文でネストされたフィールドを追加で指定することもできます。 関連するオブジェクトまたはコレクションの使用可能なすべてのフィールドを表示するには、単にコロンとアスタリスクをオブジェクトまたはコレクション参照に追加します。
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### カスタムデータの取得

プレフィックス「DE:」を使用して、カスタムデータフィールドを取得できます。 例えば、「CustomText」というパラメーターを持つプロジェクトをリクエストするには、次のリクエストを使用します。
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>それが戻る
<pre>{<br>    "name":"カスタムデータプロジェクト",<br>    "ID":"4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText":"task b" <br>}</pre>また、 parameterValues フィールドを要求することで、オブジェクトのすべてのカスタムデータを取得できます。 例： 
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>は、次のようなデータを返します。
<pre>{<br>    "name":"カスタムデータプロジェクト",<br>    "ID":"4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues:{ <br>        "DE:CustomText":"task b", <br>        "DE:CustomNumber":1.4, <br>        "DE:CustomCheckBoxes":["first", "second", "third"] <br>    } <br>}</pre>

#### 名前付きクエリの使用

一部のオブジェクトタイプには、一般的に実行される名前付き検索があり、クエリの名前をオブジェクトタイプ URI の末尾に追加することで使用できます。 例えば、次のリクエストでは、ユーザーに現在割り当てられている作業項目（タスクとタスク）を取得します。
<pre>/attask/api/v15.0/work/myWork</pre>名前付きクエリは、フィールドパラメーターに追加のフィールドを取得するリクエストをサポートします。 名前付きクエリの中には、追加のフィルターを受け付けるものもあります。 オブジェクトで使用可能な名前付きクエリのリストについては、[API エクスプローラー ](../../wf-api/general/api-explorer.md) のオブジェクトの「アクション」タブを参照してください。

#### カウントフィルターの使用

特定の検索結果から返される結果の数を指定できます。 これにより、サーバーはリクエストをより迅速に処理し、帯域幅を節約できます。 例えば、リクエスト
<pre>GET/attask/api/v15.0/project/count?status=CUR</pre>結果の数を次の形式で返します。
<pre>{<br>    "count":3 <br>}</pre>この結果は、完全なオブジェクトが送信される場合よりも、はるかに小さいダウンロードになります。 フィルター構文は search コマンドと同じです。

### レポートのリクエスト

1 つ以上のグループ化を使用して、一部のフィールドの集計のみが必要なレポートリクエストを実行できます。 次の例に示すように、レポートの構文は SOAP API の構文と同じです。
<pre>GET/attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>次の結果を返します。
<pre>{<br>    "最初のプロジェクト":{ <br>        "sum_hours":15 <br>    }, <br>     "2 つ目のプロジェクト":{ <br>        "sum_hours":30 <br>    } <br>}</pre>$$ROLLUP=true パラメーターを追加すると、各グループ化レベルでの合計が含まれます。
<pre>{<br>    "最初のプロジェクト":{ <br>        "sum_hours":15 <br>    }, <br>    "2 つ目のプロジェクト":{ <br>        "sum_hours":30 <br>    }, <br>    "$$ROLLUP":{ <br>        "sum_hours":45 <br>    } <br>}</pre>

### API でのクエリ結果の並べ替え

API 呼び出しに以下を追加すると、任意のフィールドで結果を並べ替えることができます。

&amp;entryDate_Sort=asc

たとえば、タスク「計画開始日」で並べ替える場合は、entryDate を削除し、「plannedCompletionDate」に置き換えます。

これは、Workfrontのほとんどのフィールドで機能します。

### クエリ制限の検討

オブジェクトを照会する場合は、関連オブジェクトの関係と検索制限に関して特に考慮する必要があります。 例えば、次の表に示すように、プロジェクトのクエリで返されるプロジェクト数は 2,000 以下です。 これら 2,000 件のプロジェクトが「主なオブジェクト」と見なされます。 プロジェクトの [ タスク ] フィールドに対してクエリを実行すると、[ タスク ] フィールド（コレクション）は、プライマリオブジェクト Project のセカンダリオブジェクトになります。 [ タスク ] フィールドのクエリには、プロジェクト上の何千ものタスクを含めることができます。 合計で、返されるオブジェクト（プロジェクトとタスク）の合計数は、最大 50,000 個を超えることはできません。

次の表に、最適なパフォーマンスを実現するために、検索リクエストに対しておこなわれた制限を示します。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>クエリ結果</th> 
   <th>制限事項</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">デフォルトの結果数</td> 
   <td>100</td> 
   <td> クエリフィルタで制限が指定されていない場合 ($$LIMIT)、結果に含めることができるプライマリオブジェクトは 100 個までです。 <br>詳しくは、 <a href="#using-paginated-responses" class="MCXref xref">ページ分割応答の使用</a> を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>結果の最大数</td> 
   <td>2,000</td> 
   <td>クエリフィルター ($$LIMIT) は、2000 件以下の結果を返すことができます。 詳しくは、「ページ分割された応答」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>最大フィールド深度</td> 
   <td>4</td> 
   <td>表示するフィールドを識別する場合、クエリ対象のオブジェクトから 4 レベル以上離れることはできません。</td> 
  </tr> 
  <tr> 
   <td>オブジェクトの最大数</td> 
   <td>50,000</td> 
   <td>結果セットには、プライマリオブジェクトとセカンダリオブジェクト50000を含めることはできません。</td> 
  </tr> 
  <tr> 
   <td>フィールドの最大数</td> 
   <td nowrap>1,000,000</td> 
   <td>結果セットが50000オブジェクトより少ない場合、結果に含まれるフィールドは最大 1,000,000 個です。</td> 
  </tr> 
  <tr> 
   <td>バッチ作成/更新の最大数</td> 
   <td>100</td> 
   <td>バッチの作成または更新の上限は 100 です。</td> 
  </tr> 
 </tbody> 
</table>

### ページ分割応答の使用 {#using-paginated-responses}

「デフォルトの結果数」クエリ制限を上書きし、200 件の結果を許可するには、次の例に示すように、クエリに$$LIMIT=200 フィルターを含めます。
<pre>GET/attask/api/v15.0/project/search?$$LIMIT=200</pre>システム内の他のテナントの信頼性とパフォーマンスを確保するために、1 つのクエリに許可される結果の上限は 2,000 個です。 より大きな制限を指定しようとすると、IllegalArgumentException エラーメッセージが表示されます。 

したがって、大きなデータセットに対して、ページ分割された応答の使用を検討することをお勧めします。 返される最初の結果を指定するには、$$FIRST フィルターを追加します。 例えば、次のリクエストは、クエリの結果 201-250 を返します。
<pre>GET/attask/api/v15.0/project/search?$$FIRST=201&amp;$$LIMIT=50</pre>

### アクセス規則の作成

アクセス規則を作成して、オブジェクトにアクセスできるユーザーを決定できます。 次に、設定できるアクセス規則の例を示します。

ID が「abc123」のユーザーとのみ共有されるようにプロジェクトを設定するには、次のリクエストを使用します。
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules:[ {accessorID:'abc123', accessorObjCode:'USER', coreAction:'表示'} ] }</pre>または、新しいユーザーとのみ共有し、既存の権限をそのまま維持するには、次の手順を実行します。
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>既存のアクセス・ルールを取得する手順は、次のとおりです。
<pre>GET/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST動作

POSTは、新しいオブジェクトを挿入します。 構文は「PUT」と同じですが、いくつかの例外があります。 新しいオブジェクトはまだ存在しないので、ID は付いていません。 このため、URI には ID が含まれません。

### オブジェクトの作成

次に、新しいプロジェクトを作成するリクエストの例を示します。
<pre>POST/attask/api/v15.0/project?name=新規プロジェクト</pre>応答には、新しく作成されたプロジェクトと、その新しい ID および指定されたその他のフィールドが含まれます。

### オブジェクトのコピー

一部のオブジェクトは、コピーをサポートしています。 これらのオブジェクトタイプでは、copySourceID パラメータを使用して投稿することで、新しいオブジェクトを作成できます。 例えば、次のリクエストは、指定されたプロジェクトをコピーし、新しい名前を付けます。

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### ドキュメントのアップロード

次の API URL を使用してドキュメントをアップロードできます。
<pre>POST/attask/api/v15.0/upload</pre>API では、コンテンツタイプが multipart/form-data である必要があります。 ファイルのパラメータ名は、uploadedFile にする必要があります。 サーバーが以下の JSON データを返します。
<pre>{<br>    "handle":"4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Workfrontドキュメントの作成時に、ハンドルを使用して次の URL に投稿できます。
<pre>POST/attask/api/v15.0/document?updates={<br>    名前：aFileName,<br>    ハンドル：abc...123, （ファイルのアップロードからの処理）<br>    docObjCode:PROJ、（または TASK、OPTASK など）<br>    objID:abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## PUT動作

PUTは、既存のオブジェクトの更新に使用されます。

PUTの応答はGETと同じです。 どちらの場合も、サーバーは更新後にオブジェクトの新しい状態を返します。 GETリクエストへの応答を変更するために使用されるすべてのルールは、PUTと連携しても機能します。例えば、返される追加のフィールドやカスタムデータを指定するなどです。

### オブジェクトの編集

オブジェクトの更新は、常に、オブジェクトの一意の URI を使用して ID でおこなわれます。 更新するフィールドは、リクエストパラメーターとして指定します。 例えば、プロジェクトの名前を変更するには、次のようなリクエストを送信します。
<pre>PUT/attask/api/v15.0/project/4c7...?name=新規プロジェクト名 <br>PUT/attask/api/v15.0/project?id=4c7...&amp;name=新規プロジェクト名</pre>更新には ID が必要なので、オブジェクトがサーバー上に存在しない場合、この操作は（挿入なしで）失敗します。

### JSON 編集の指定

次の例に示すように、updates リクエストパラメーターを使用して、JSON 構文を使用して更新するフィールドを指定できます。
<pre>PUT/attask/api/v15.0/project/4c7...?更新= <br>{<br>     名前："新規プロジェクト名", <br>     ステータス：「CUR」 <br>     ... <br>}</pre>

### ネストされた更新の作成

一部のオブジェクトには、非公開で所有するコレクションを更新できます。 例えば、次の例は、特定のタスクの既存の割り当てを上書きする方法を示しています。
<pre>PUT/attask/api/v15.0/task/4c7...?更新= <br>{<br>    割り当て：[ <br>        { <br>            assignedToID:"2222...54d0, <br>            assignmentPercent:50.0 <br>        },{ <br>            roleID:"1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
最上位レベルに対する更新は少ないものの、コレクションまたはネストされたオブジェクトに対する更新は既存のコレクションを完全に置き換えます。 オブジェクトに影響を与えずにタスクに対する 1 つの割り当てを編集するには、タスクに対してではなく、割り当てに対してPUTを使用します。

次の例では、プロジェクトをパブリックヘルプデスクキューにします。 既存のキューのプロパティは置き換えられます。
<pre>PUT/attask/api/v15.0/project/4c7...?更新= <br>{ <br>    queueDef :{ <br>        isPublic:1 <br>    } <br>}</pre>

### Action Request パラメーターの使用

一部のオブジェクトは、単純な編集に加えて、追加のアクションをサポートしています。 これらのアクションは、アクションリクエストパラメーターを使用して指定できます。 例えば、次のリクエストでは、指定されたプロジェクトのタイムラインが再計算されます。
<pre>PUT/attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>または<br><br>PUT/attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### オブジェクトの移動

次の例は、あるプロジェクトから別のプロジェクトにタスクを移動する際の構文を示しています。
<pre>PUT/attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>各アクションタイプの例を次に示します。(??)
<pre>PUT/attask/api/v15.0/project/1234/approveApproval<br><br>PUT/attask/api/v15.0/project/1234/calculateFinance<br><br>PUT/attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT/attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT/attask/api/v15.0/project/1234/recallApproval<br><br>PUT/attask/api/v15.0/project/1234/rejectApproval<br><br>PUT/attask/api/v15.0/task/1234/move<br><br>PUT/attask/api/v15.0/workitem/1234/markViewed</pre>作業項目を移動するプロジェクトを指定するには、移動アクションのみが追加の属性を指定する必要があります。

各アクションタイプの例を次に示します。 
<pre>PUT/attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID:'abc123', accessorObjCode:'USER', coreAction:'表示'}}</pre>

### オブジェクトの共有

次の例は、プロジェクトをチームと共有するための構文を示しています。
<pre>PUT/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxshare?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxaccessorObjCode=TEAMOB</pre>オブジェクトの編集時に、次の例のようなPUTを実行して更新を送信することで、オブジェクト上のすべてのアクセス規則を置き換えることができます。
<pre>PUT/attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxx',acessorObjCode:','TEAMOBcoreaction:'VIEW'}}</pre>次の例は、あるプロジェクトから別のプロジェクトにタスクを移動するための構文を示しています。
<pre>PUT/attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## DELETE動作

DELETEはオブジェクトを削除します。 いずれの場合も、URI にパラメータ force=true を含めると、サーバーは指定したデータとその依存関係を削除します。 次の例では、URI に対して HTTP タスクメソッドを実行してDELETEを削除します。
<pre>DELETE/attask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d0 <br>DELETE/attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE/attask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d0?force=true <br>DELETE/attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## 一括更新

一括更新ステートメントは、1 回の API 呼び出し内で複数のオブジェクトを同時に更新します。 一括作成 API 呼び出しは、次の例に示すように、通常の更新呼び出しと同様に作成されます。
<pre>PUT/attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=method&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>その結果、次のような戻り値が返されます。
<pre>データ：[{<br>    ID:"53ff8d3d003b438b57a8a784df38f6b3",<br>    名前："Test_Project_1",<br>    objCode:「PROJ」<br>    percentComplete:0,<br>    plannedCompletionDate:"2014-08-28T11:00:00:000-0400",<br>    plannedStartDate:"2014-08-28T11:00:00:000-0400",<br>    優先度：0,<br>    projectedCompletionDate:"2014-08-28T16:12:00:000-0400",<br>    ステータス："CUR"<br>},<br>{<br>    ID:"53ff8d49003b43a2562aa34eea3b6b10",<br>    名前："Test_Project_2",<br>    objCode:「PROJ」<br>    percentComplete:0usi<br>    plannedCompletionDate:"2014-08-28T11:00:00:000-0400",<br>    plannedStartDate:"2014-08-28T11:00:00:000-0400",<br>    優先度：0,<br>    projectedCompletionDate:"2014-08-28T16:12:00:000-0400",<br>    ステータス："CUR"<br>}]</pre>一括更新は、次のように実行することもできます。
<pre>PUT/attask/api/v15.0/proj?Umethod=PUT&amp;アップデート=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>その結果、次のような戻り値が返されます。
<pre>データ：[ {<br>     ID:"53ff8e15003b461d4560f7f65a440078",<br>     名前："Test_Project_1_Edit",<br>     objCode:「PROJ」<br>     percentComplete:0,<br>     plannedCompletionDate:"2014-08-28T11:00:00:000-0400",<br>     plannedStartDate:"2014-08-28T11:00:00:000-0400",<br>     優先度：0,<br>     projectedCompletionDate:"2014-08-28T16:16:00:000-0400",<br>     ステータス："CUR"<br>},<br>{<br>    ID:"53ff8e19003b46238a58d303608de502",<br>    名前："Test_Project_2_Edit",<br>    objCode:「PROJ」<br>    percentComplete:0,<br>    plannedCompletionDate:"2014-08-28T11:00:00:000-0400",<br>    plannedStartDate:"2014-08-28T11:00:00:000-0400",<br>    優先度：0,<br>    projectedCompletionDate:"2014-08-28T16:16:00:000-0400",<br>    ステータス："CUR"<br>}]</pre>すべての操作を同じトランザクションで発生させる場合は、リクエストパラメーターとしてバッチ API 呼び出しに「atomic=true」を追加します。 この方法で、いずれかの操作が失敗した場合、すべての操作がロールバックされます。

>[!NOTE]
アトミックバッチ操作は、「成功：true」またはエラーが返されます。
