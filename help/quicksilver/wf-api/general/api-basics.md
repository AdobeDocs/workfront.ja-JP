---
content-type: api
navigation-topic: general-api
title: API の基本
description: API の基本
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 362a14c2c25e995d06a26b77ab51448b033bc2ac
workflow-type: tm+mt
source-wordcount: '4361'
ht-degree: 98%

---


# API の基本

Adobe Workfront API の目的は、HTTP 経由で動作する REST フルアーキテクチャを導入することで、Workfront との統合の構築を簡略化することです。このドキュメントでは、REST および JSON の応答に精通していることを前提とし、Workfront API で採用されているアプローチについて説明します。

Workfront スキーマに精通していれば、統合のために Workfront からデータを取り出すときに使用できるデータベースの関係を理解できます。

## 制限とガイドライン

Workfront オンデマンドシステムのパフォーマンスを確保するため、各お客様が同時に実行できる API スレッドは 10 個に制限されています。サンドボックス環境にも同じ制限があるので、お客様とパートナーは、コードを実稼動環境にリリースする前に API 呼び出しを正確にテストできます。

実稼動、プレビューおよび体験版の環境では、エンドユーザーのリクエストは Workfront CDN（Akamai）を介してルーティングされるので、URI の最大長は 8892 バイトとなります。この制限は、CDN 経由でルーティングされる URI にのみ適用されます。

>[!NOTE]
>
>サンドボックス環境は CDN を通じてルーティングされないので、この制限はサンドボックス環境には適用されません。

### 免責事項

API の使用は、実稼動環境で実行する前に、Workfront ベータ環境でテストする必要があります。お客様がオンデマンドのソフトウェアに負担をかけると合理的に判断する処理で API を使用している場合（当該処理が他のお客様のソフトウェアのパフォーマンスに重大な悪影響を及ぼしている場合）、Workfront は当該処理の中止をお客様に求める権利を有します。お客様がこれに応じず問題が継続する場合、Workfront は当該処理を終了させる権利を有します。

## REST の基本

この節では、次の REST 原則に関して、Workfront REST API とやり取りを行う方法を詳しく説明します。

### オブジェクト URI

システム内の各オブジェクトには、オブジェクトタイプと ID で構成される一意の URI が与えられます。次の例は、3 つの一意のオブジェクトを記述する URI を示しています。

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

オブジェクトタイプは大文字と小文字が区別されず、省略形の ObjCode（proj など）、または代替オブジェクト名（project など）を指定できます。

有効な ObjCode のリストについては、[API エクスプローラー](../../wf-api/general/api-explorer.md)を参照してください。

### 操作

オブジェクトは、一意の URI に HTTP リクエストを送信して操作します。実行する操作は、HTTP メソッドで指定します。

標準の HTTP メソッドは、次の操作に対応しています。

* **GET** - ID でオブジェクトを取得、クエリですべてのオブジェクトを検索、レポートを実行、名前付きクエリを実行
* **POST** - 新しいオブジェクトを挿入
* **PUT** - 既存のオブジェクトを編集
* **DELETE** - オブジェクトを削除

クライアントの問題やプロトコルの長さ制限を回避するために、メソッドパラメーターを使用して HTTP の動作を上書きできます。例えば、GET 操作は、次の URI を送信することで実装できます。
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### 応答

各リクエストには、JSON 形式での応答が返されます。リクエストが成功した場合はデータ属性が応答に含まれ、問題が発生した場合はエラー属性が含まれます。例えば、次のリクエスト：

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

これは、次のような JSON 応答を返します。


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>ブラウザーのアドレスバーから GET リクエストを実行する場合、sessionID をリクエストの一部に含める必要はありません。

PUT、POST、DELETE の各リクエストに対する特別なセキュリティが追加されました。データベースへの書き込みまたはデータベースからの削除が発生するリクエストは、 **sessionID=abc123** が URI に含まれている場合のみ実行できます。次に示すのは、DELETE リクエストでの例です。
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### 認証

API はリクエストごとに認証を行い、リクエストされたオブジェクトを表示または変更するためのアクセス権をクライアントが持っていることを確認します。

認証は、次のいずれかの方法で与えられるセッション ID を渡すことで実行されます。

#### リクエストヘッダー認証

推奨される認証方法は、セッショントークンを含む SessionID という名前のリクエストヘッダーを渡すことです。[クロスサイトリクエストフォージェリー（CSRF）](https://en.wikipedia.org/wiki/Cross-site_request_forgery)攻撃に対して安全で、キャッシュ目的で URI に干渉することがありません。

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

API は、Web UI でシステムに使用されるのと同じ Cookie ベースの認証を使用します。ここで、クライアントが Web UI を使用して Workfront にログインした場合、同じブラウザー内で行われる AJAX 呼び出しに同じ認証を使用します。

>[!NOTE]
>
>CSRF（クロスサイトリクエストフォージェリー）攻撃の可能性から保護するために、この認証方法は読み取り専用操作でのみ使用できます。

## ログイン

>[!IMPORTANT]
>
Workfront では、`/login` エンドポイントまたは API キーの使用を推奨していません。代わりに、次のいずれかの認証方法を使用してください。
>
* JWT を使用したサーバー認証
* OAuth2 を使用したユーザー認証
>
これらの認証方法の設定手順については、[Workfront 統合用の OAuth2 アプリケーションの作成](../../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください
>
Workfront でのサーバー認証の使用手順については、[JWT フローを使用した組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-jwt-flow.md)を参照してください
>
Workfront でのユーザー認証を使用する手順については、[認証コードフローを使用した組織のカスタム OAuth 2 アプリケーションの設定および使用](../../wf-api/api/oauth-app-code-token-flow.md)を参照してください

>[!NOTE]
>
この節で説明する手順は、Adobe Business Platform にまだ登録されていない組織にのみ適用されます。組織が Adobe Business Platform にオンボーディングされている場合、Workfront API を介して Workfront にログインすることはできません。
>
組織が Adobe Business Platform にオンボーディングされているかどうかによって手順は異なります。手順のリストについては、[プラットフォームによる管理の違い（Adobe Workfront Fusion／Adobe Business Platform）](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

有効なユーザー名とパスワードを使用すると、次のリクエストを使用してセッション ID を取得できます。

```
POST /attask/api/v15.0/login?username=admin&password=user
```

これにより、今後のリクエストを認証する Cookie が設定され、新しく作成された sessionID、ログインしたユーザーの userID、その他のセッション属性を含む JSON 応答が返されます。

>[!NOTE]
>
管理者でもある API ユーザーが指定されている場合、Workfront では、ログインに API キーを使用することを強くお勧めします。

**API キーの生成**

次の例に示すユーザーとしてシステムにログインすると、API キーを生成できます。


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**以前に生成した API キーの取得**

また、getApiKey を実行すると、特定のユーザー用に以前に生成された API キーを取得することもできます。


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

その後、sessionID またはユーザー名とパスワードの代わりにこの値を含むリクエストパラメーターとして「apiKey」を追加することで、この結果を使用して API 呼び出しを認証できます。これは、セキュリティの観点から有益です。

次に、apiKey を使用してプロジェクトからデータを取得するリクエストの例を示します。

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**API キーの無効化**

apiKey 値が侵害された場合は、次の例に示すように、「clearApiKey」を実行して、現在の API キーを無効にすることができます。

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

クリアすると、getApiKey を再度実行して新しい API キーを生成できます。

### ログアウト

セッションが完了したら、次のリクエストを使用してユーザーをログアウトし、sessionID でのアクセスを防止します。

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

ログアウトする sessionID は、Cookie、リクエストヘッダーまたはリクエストパラメーターのいずれかとして指定できます。

ユーザーをログアウトするには、下記の手順に従います。

1. ログイン画面に移動しますが、ログインはしないでください。
1. URL を/attask/api/v15.0/project/search に変更します。\
   ページが見つからないことに注意してください。
1. *search* という単語を login?username=admin&amp;password=user に置き換え、*admin* と *user を自分のユーザー名とパスワードに置き換えます。\
   *このセッションはブラウザーに cookie として保存されるので、後続の GET リクエストのたびに再記述する必要はありません。

1. URL を **/attask/api/v15.0/project/search** に戻します。
1. 提供された応答に注意してください。

PUT、POST、DELETE の各リクエストを実行する際は、ログイン後に提供される sessionID を常に含める必要があります。

## GET 動作

1 つ以上のオブジェクトを取得し、レポートを実行するには、HTTP GET メソッドを使用します。

### オブジェクトの取得

修飾子とフィルターを使用すると、オブジェクトの検索を強化できます。

#### オブジェクト ID を使用したオブジェクトの取得

オブジェクトの ID がわかっている場合は、その一意の URI にアクセスしてオブジェクトを取得できます。例えば、次のリクエスト：

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

は、次のような応答を返します。

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


次の例に示すように、同じリクエストで複数のオブジェクトを取得するには、ID リクエストパラメーターを指定し、ID のコンマ区切りリストを指定します。


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

/attask/api/v15.0/project?id=...リクエストは `/attask/api/v15.0/project/...` リクエストと同じであることに留意してください。

#### URI を使用したオブジェクトの取得

ID 以外の条件でオブジェクトを取得する場合は、URI を検索できます。

例えば、次のリクエストを使用して、システム内のすべてのプロジェクトのリストを返すことができます。

```
GET /attask/api/v15.0/project/search
```

リクエストパラメーターを名前と値のペアとして使用して、フィルターを指定できます。例えば、次の例は、現在のすべてのプロジェクトを検索するリクエストを示しています。

```
GET /attask/api/v15.0/project/search?status=CUR
```

次のリクエストでは、John というユーザーに割り当てられているすべての未完了のタスクを検索します。

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### 検索修飾子の使用

次の表に、Workfront API で使用できる修飾子の一部を示します。

| **修飾子** | **説明** | **例** |
|---|---|---|
| eq | クローズ済みのステータスの結果を返す | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | クローズ済みのステータスではない結果を返す | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | 完了率が 50 以上の結果を返す | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | 完了率が 50 以下の結果を返す | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | 説明が Null の結果を返す | <pre>...description_Mod=isnull...</pre> |
| notnull | 説明が Null でない結果を返す | <pre>...description_Mod=notnull...</pre> |
| contains | 名前に「Workfront」が含まれる結果を返す | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| between | 過去 7 日以内のエントリ日を持つ結果を返す | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
検索リクエストでは、大文字と小文字が区別されます。エラーが発生した場合は、**_Mod** および **_Range** の大文字と小文字が正しいことを確認してください。

#### OR ステートメントの使用

「OR」を含むパラメーターと数値を追加して検索を拡張し、1 つのフィルターまたは一連のフィルターのレベルを示すことができます。

OR ステートメントは、OR ステートメントのフィルタリング条件を満たす API 呼び出しのレコードのみを返します。フィルターは、OR ステートメントのレベル全体に暗黙的に適用されません。

例えば、次のようなフィルターを実行する場合：

* 「Planning」を含む名前を持つタスク OR
* 「FixedAssets」という名前のポートフォリオ内のタスク AND 「Steve」を含む名前のユーザーに割り当てられている OR
* 「最終タスク」という名前の親タスクを持つタスク

次のように、複数の OR ステートメントを持つ API 呼び出しを使用します。
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### フィルターパラメーターの使用

検索フィルターに URL パラメーターを使用する際に陥りそうな問題の 1 つは、Workfront が特定のパラメーターを解析してから、様々な認証方法（ユーザー名、パスワード、apiKey、cookie）を確認することです。この場合、パラメーターは呼び出しでフィルターとして使用されません。 

この問題を回避するには、JSON 形式のフィルターパラメーターにこれらの値を配置します。例えば、以下を使用する代わりに、ユーザー名 testuser にフィルタリングを行う場合
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>次の例に示すように、URL パラメーターをフィルターに渡します。
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### マップリクエストパラメーターの使用

デフォルトでは、検索から返されるデータは JSON 配列です。ユースケースによっては、ID でインデックス付けされた JSON オブジェクトとして結果を取得するほうが効率的な場合があります。これは、map リクエストパラメーターを使用して行うことができます。例えば、次のリクエスト：
<pre>/attask/api/v15.0/task/search?map=true</pre>は、次のような ID でインデックス付けされた応答を返します。
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "first task",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "second task",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### フィールドリクエストパラメーターの使用

デフォルトでは、オブジェクトを取得すると、最も一般的に使用されるフィールドのサブセットのみが返されます。

フィールドリクエストパラメーターを使用して、特定のフィールドのカンマ区切りのリストが返されることを指定できます。例えば、次のリクエスト：
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>は、次のような応答を返します。
<pre>{<br>    "priority": 2,<br>    "name": "first task",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
これらのフィールド名では、大文字と小文字が区別されます。

使用可能なフィールド参照のリストについては、[API エクスプローラー](../../wf-api/general/api-explorer.md)を参照してください。

#### ネストされたオブジェクトの検索

ネストされたオブジェクトを検索できます。デフォルトでは、ネストされたオブジェクトは名前と ID のみで返されます。例えば、すべてのイシューを所有者とともに取得するには、次のリクエストを使用します。
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>詳細な情報が必要な場合は、コロン構文を使用してネストされたフィールドをリクエストできます。例えば、次のリクエストは、所有者の名前、ID、タイトル、電話番号とともにすべてのイシューを検索します。
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>そして、次を返します。
<pre>{<br>    "name": "an important issue",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "Operations Specialist",<br>        "phoneNumber": "555-1234",<br>        "name": "Admin User",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### ネストされたコレクションの取得

オブジェクトのネストされたコレクションを取得できます。例えば、すべてのタスクを含むプロジェクトを取得するには、次のリクエストを使用します。
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>次のリクエストはタスクの割り当てを取得します。
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### 複数のネストされたフィールドの検索

デフォルトでは、各タスクの名前と ID のみが返されますが、追加のネストされたフィールドはコロン構文で指定できます。関連するオブジェクトまたはコレクションの使用可能なすべてのフィールドを表示するには、単にコロンとアスタリスクをオブジェクトまたはコレクション参照に追加します。
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### カスタムデータの取得

接頭辞「DE:」を使用して、カスタムデータフィールドを取得できます。例えば、「CustomText」というパラメーターを持つプロジェクトをリクエストするには、次のリクエストを使用します。
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>これは、以下を戻します
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "task b" <br>}</pre>また、parameterValues フィールドをリクエストすることで、オブジェクトのすべてのカスタムデータを取得できます。例：
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>は、次のようなデータを返します。
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### 名前付きクエリの使用

一部のオブジェクトタイプには、一般的に実行される名前付き検索があり、クエリの名前をオブジェクトタイプ URI の末尾に追加することで使用できます。例えば、次のリクエストでは、ユーザーに現在割り当てられている作業アイテム（タスクとイシュー）を取得します。
<pre>/attask/api/v15.0/work/myWork</pre>名前付きクエリは、フィールドパラメーターに対する追加のフィールド取得のリクエストをサポートしています。名前付きクエリの中には、追加のフィルターを受け入れるものもあります。オブジェクトで使用可能な名前付きクエリのリストについては、[API Explorer]（../../wf-api/general/api-explorer.md）のオブジェクトで「アクション」タブを参照してください。

#### 使用 `Count`

以下を使用できます。 `count` をクリックして、クエリに一致する結果の数を返します。 これは、結果にデータが必要ない場合に役立ちます。 カウントのみを返すことで、サーバーはリクエストをより迅速に処理し、帯域幅を節約できます。 例えば、次のリクエスト：
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>の場合、結果の数を次の形式で返します。
<pre>{<br>    "count": 3 <br>}</pre>カウントを返す方が、完全なオブジェクトが返される場合よりも、データ転送ははるかに小さくなります。 構文は search コマンドと同じです。

### レポートのリクエスト

1 つ以上のグループ化がある場合、一部のフィールドの集計のみが必要なレポートリクエストを実行できます。次の例に示すように、レポートの構文は SOAP API の構文と同じです。
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>次の結果を返します。
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>     "Second Project": { <br>        "sum_hours": 30 <br>    } <br>}</pre>$$ROLLUP=true パラメーターを追加すると、各グループ化レベルでの合計が含まれます。
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>    "Second Project": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### API でのクエリ結果の並べ替え

API 呼び出しに以下を追加すると、任意のフィールド別に結果を並べ替えることができます。

&amp;entryDate_Sort=asc

たとえば、タスクの予定開始日で並べ替える場合は、entryDate を削除し、plannedCompletionDate に置き換えます。

これは、Workfront のほとんどのフィールドで使用できます。

### クエリ制限の検討

オブジェクトのクエリを実行する場合は、関連するオブジェクトの関係と検索制限に関して特に考慮する必要があります。例えば、次の表に示すように、プロジェクトのクエリで返されるプロジェクト数は 2,000 以下です。これら 2,000 個のプロジェクトが「プライマリオブジェクト」と見なされます。プロジェクトのタスクフィールドに対してクエリを実行すると、タスクフィールド（コレクション）は、プライマリオブジェクトであるプロジェクトのセカンダリオブジェクトになります。タスクフィールドのクエリには、プロジェクト上の何千ものタスクを含めることができます。返されるオブジェクト（プロジェクトとタスク）の合計数は、全体で最大値の 50,000 個を超えることはできません。

最適なパフォーマンスを実現するために検索リクエストに設けられた制限を、次の表に示します。 

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
   <td width="200">デフォルトの結果の数</td> 
   <td>100</td> 
   <td> クエリフィルター ($$LIMIT) で制限が指定されていない場合、結果に含めることができるプライマリオブジェクトは 100 個までです。<br>この制限を変更する方法について詳しくは、<a href="#using-paginated-responses" class="MCXref xref">ページ分割された応答の使用</a>を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>結果の最大数</td> 
   <td>2,000</td> 
   <td>クエリフィルター（例：$$LIMIT）は、2000 件までの結果を返すことができます。詳しくは、「ページ分割された応答」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>最大フィールド深度</td> 
   <td>4</td> 
   <td>表示するフィールドを識別する場合、クエリ対象のオブジェクトから離れられるのは 4 レベルまでです。</td> 
  </tr> 
  <tr> 
   <td>オブジェクトの最大数</td> 
   <td>50,000</td> 
   <td>結果セットには、プライマリオブジェクトとセカンダリオブジェクトを 50000 個含めることはできません。</td> 
  </tr> 
  <tr> 
   <td>フィールドの最大数</td> 
   <td nowrap>1,000,000</td> 
   <td>結果セットに含まれるオブジェクトが 50000 個未満の場合、結果に含まれるフィールドの数は最大 1,000,000 個です。</td> 
  </tr> 
  <tr> 
   <td>バッチの作成や更新の最大数</td> 
   <td>100</td> 
   <td>バッチの作成または更新の上限は 100 です。</td> 
  </tr> 
 </tbody> 
</table>

### ページ分割された応答の使用 {#using-paginated-responses}

デフォルトの結果数のクエリの制限を上書きし、200 個の結果を許可するには、次の例に示すように、クエリに `$$LIMIT=200` フィルターを指定します。
<pre>GET/attask/api/v15.0/project/search?$$LIMIT=200</pre>

システム内の他のテナントに対する信頼性とパフォーマンスを確保するために、1 つのクエリに許可される結果の最大数は 2,000 個のオブジェクトです。制限を大きく指定しようとすると、`IllegalArgumentException` エラーメッセージが表示されます。

したがって、大きなデータセットに対して、ページ分割された応答の使用を検討することをお勧めします。返される最初の結果を指定するには、`$$FIRST` フィルターを追加します。例えば、次のリクエストは、クエリの結果 201-250 を返します。
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

上記の例では、`$$FIRST=200` は 201 番目の結果を返します。`$$FIRST=0` は最初の結果を返します。$$FIRST の値は、結果を返す前にスキップする結果の数と考えると役立つ場合があります。

結果が正しくページ分割されるようにするには、並べ替えパラメーターを使用します。これにより、結果が同じ順序で返されるので、ページネーションは結果を繰り返したりスキップしたりしません。例えば、オブジェクト ID を使用して並べ替えるには、「`ID_Sort=asc`」を使用します。

### アクセスルールの作成

アクセスルールを作成して、オブジェクトにアクセスできるユーザーを決定できます。次に、設定できるアクセスルールの例を示します。

ID が「abc123」のユーザーとのみ共有されるようにプロジェクトを設定するには、次のリクエストを使用します。
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>または、新しいユーザーとのみ共有して既存の権限をそのまま維持するには、次を使用します。
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>既存のアクセスルールを取得するには、次を使用します。
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## POST 動作

POST は、新しいオブジェクトを挿入します。構文は「PUT」と同じですが、いくつかの例外があります。新しいオブジェクトはまだ存在しないので、ID は付いていません。このため、URI には ID が含まれません。

### オブジェクトの作成

次に、新しいプロジェクトを作成するリクエストの例を示します。
<pre>POST /attask/api/v15.0/project?name=New Project</pre>応答には、新しく作成されたプロジェクトと、その新しい ID および指定されたその他のフィールドが含まれます。

### オブジェクトのコピー

一部のオブジェクトは、コピーをサポートしています。これらのオブジェクトタイプでは、copySourceID パラメーターを使用して投稿することで、新しいオブジェクトを作成できます。例えば、次のリクエストは、指定されたプロジェクトをコピーし、新しい名前を付けます。

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### ドキュメントのアップロード

次の API URL を使用してドキュメントをアップロードできます。
<pre>POST /attask/api/v15.0/upload</pre>API では、コンテンツタイプが multipart/form-data である必要があります。ファイルのパラメーター名は、uploadedFile にする必要があります。サーバーが以下の JSON データを返します。
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Workfront ドキュメントの作成時に、ハンドルと次の URL への POST を使用できます。
<pre>POST /attask/api/v15.0/document?updates={<br>    name: aFileName,<br>    handle: abc...123, (handle from the file upload)<br>    docObjCode: PROJ, (or TASK, OPTASK, etc)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## PUT 動作

PUT は、既存のオブジェクトの更新に使用されます。

PUT に対する応答は GET と同じです。どちらの場合も、サーバーは更新後にオブジェクトの新しい状態を返します。GET リクエストへの応答を変更するために使用されるすべてのルールは、PUT と連携しても機能します。例えば、返される追加のフィールドやカスタムデータを指定するなどです。

### オブジェクトの編集

オブジェクトの更新は、常に、オブジェクトの一意の URI を使用して ID で行われます。更新するフィールドは、リクエストパラメーターとして指定します。例えば、プロジェクトの名前を変更するには、次のようなリクエストを送信します。
<pre>PUT /attask/api/v15.0/project/4c7...?name=New Project Name <br>PUT /attask/api/v15.0/project?id=4c7...&amp;name=New Project Name</pre>更新には ID が必要なので、オブジェクトがサーバー上に存在しない場合、この操作は（挿入なしで）失敗します。

### JSON 編集の指定

次の例に示すように、updates リクエストパラメーターを使用して、JSON 構文を使用して更新するフィールドを指定できます。
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{<br>     name: "New Project Name", <br>     status: "CUR", <br>     ... <br>}</pre>

### ネストされた更新の作成

一部のオブジェクトには、非公開で所有するコレクションを更新できます。例えば、次の例は、特定のタスクの既存の割り当てを上書きする方法を示しています。
<pre>PUT /attask/api/v15.0/task/4c7...?updates= <br>{<br>    assignments: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
最上位レベルに対する更新は少ないものの、コレクションまたはネストされたオブジェクトに対する更新は既存のコレクションを完全に置き換えます。オブジェクトに影響を与えずにタスクに対する 1 つの割り当てを編集するには、タスクに対する PUT ではなく、割り当てに対するタスクを使用します。

次の例では、プロジェクトをパブリックヘルプデスクキューにします。既存のキューのプロパティは置き換えられます。
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### アクションリクエストパラメーターの使用

一部のオブジェクトは、単純な編集に加えて、追加のアクションをサポートしています。これらのアクションは、アクションリクエストパラメーターを使用して指定できます。例えば、次のリクエストでは、指定されたプロジェクトのタイムラインが再計算されます。
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br> または <br><br>PUT /attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### オブジェクトの移動

次の例は、あるプロジェクトから別のプロジェクトにタスクを移動する際の構文を示しています。
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>各アクションタイプの例は、次の場所に示されています。（??）
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>作業項目を移動するプロジェクトを指定するには、移動アクションのみが追加の属性を指定する必要があります。

各アクションタイプの例を次に示します。 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### オブジェクトの共有

次の例は、プロジェクトをチームと共有するための構文を示しています。
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>オブジェクトの編集時に、次の例のような PUT を実行して更新を送信することで、オブジェクト上のすべてのアクセス規則を置き換えることができます。
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>次の例は、あるプロジェクトから別のプロジェクトにタスクを移動するための構文を示しています。
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## DELETE 動作

DELETE はオブジェクトを削除します。いずれの場合も、URI にパラメーター force=true を含めると、サーバーは指定したデータとその依存関係を削除します。次の例では、URI に対して HTTP DELETE メソッドを実行してタスクを削除します。
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## 一括更新

一括更新ステートメントは、1 回の API 呼び出し内で複数のオブジェクトを同時に更新します。一括作成 API 呼び出しは、次の例に示すように、通常の更新呼び出しと同様に作成されます。
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>その結果、次のような戻り値が返されます。
<pre>data: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>}]</pre>一括更新は、次のように実行することもできます。
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>その結果、次のような戻り値が返されます。
<pre>data: [ {<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>     priority: 0,<br>     projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    status: "CUR"<br>}]</pre>すべての操作を同じトランザクションで発生させる場合は、リクエストパラメーターとしてバッチ API 呼び出しに「atomic=true」を追加します。このようにすることで、いずれかの操作が失敗した場合にはすべての操作がロールバックされます。

>[!NOTE]
>
アトミックバッチ操作は、「success: true」またはエラーのみを返すことができます。
