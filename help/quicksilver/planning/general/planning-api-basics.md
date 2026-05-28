---
title: Adobe Workfront計画APIの基本
description: Adobe Workfront Planning APIの目標は、HTTP経由で動作するREST フルなアーキテクチャを導入することで、Planningとの統合を構築することを簡素化することです。 このドキュメントでは、RESTおよびJSON応答に精通していることを前提としており、Planning APIで実行されるアプローチについて説明します。
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: fdbe3945f59306fc26424d7e88b799d9dcaea4da
workflow-type: tm+mt
source-wordcount: '2206'
ht-degree: 4%

---


# Adobe Workfront Planning API の基本

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

Adobe Workfront Planning APIの目的は、HTTP経由で動作するRESTful アーキテクチャを導入することで、Planningとの統合を構築することを簡素化することです。 このドキュメントでは、RESTおよびJSON応答に精通していることを前提としています。

エンドポイントの完全なリファレンス、リクエスト/レスポンスのスキーマ、バージョン固有の詳細については、[Workfront Planning API開発者ドキュメント ](https://developer.adobe.com/wf-planning)を参照してください。

## 認証

Workfront Planning APIは、認証にOAuth 2.0を使用します。 資格情報は、Adobe Developer Consoleを使用して設定します。

統合タイプに応じて、次の2つのフローをサポートしています。

* **サーバー間認証（JWT）**：ユーザー操作のない自動統合およびバックエンドサービスの場合。 OAuth サーバー間の資格情報を使用します（クライアント資格情報の付与 – アプリケーションはクライアント IDと秘密鍵を使用して直接認証を行い、ユーザーのログインや同意手順を行わずにアクセストークンを取得します）。

  詳しくは、[ サーバー間の認証](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/)を参照してください。

* **ユーザー認証（認証コードフロー）**：特定のユーザーの代理で動作する統合用。 OAuth Web アプリまたはシングルページアプリの資格情報（認証コード付与 – ユーザーがログインして同意し、その後、アプリケーションがアクセストークンと交換する認証コードを受け取ります）を使用します。

  詳しくは、[ ユーザー認証](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/)を参照してください。

初めに、Adobe Developer Consoleでプロジェクトを作成し、Workfront Planning APIを追加して資格情報を取得します。

資格情報を設定するには、WorkfrontでOAuth2 アプリケーションを作成します。

詳しくは、[Workfront統合用のOAuth2 アプリケーションの作成](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

>[!NOTE]
>
>Workfront Planningでは、`/login` エンドポイントとAPI キー認証はサポートされていません。 `sessionID`または`apiKey`個のパラメーターは使用しないでください。


## API バージョン管理

Planning APIは、URL パスを使用してバージョン管理されます。

現在サポートされているバージョンは次のとおりです。

| バージョン | リリース日 |
|-----------|----------------|
| バージョン 1 | 2024年7月 |
| バージョン 2 | 2026年5月 |

<!--

(*****************add deprecation date column above, when we have one*****************)

-->


現在サポートされているバージョンについて詳しくは、[Workfront Planning API開発者ドキュメント ](https://developer.adobe.com/wf-planning)を参照してください。

すべての統合でバージョンを明示的にターゲットにすることをお勧めします。

```
https://{customer-domain}/maestro/api/v2/...
```

新しいメジャーバージョンがリリースされた場合、廃止日が通知されるまで、以前のバージョンは引き続き利用できます。

Workfront リリースノートに従って、APIの変更を常に把握します。


## URL構造と操作

オブジェクトは、一意の URI に HTTP リクエストを送信して操作します。 操作はHTTP メソッドで指定します。

| メソッド | 操作 |
|----------|----------------------------------------------------------------------|
| GET | IDによる単一のオブジェクトの取得、またはオブジェクトの検索/リスト |
| 投稿する | 新しいオブジェクトを作成 |
| PUT | 既存のオブジェクトの置き換え（完全更新） |
| PATCH | 既存のオブジェクトの部分的な更新（提供されたフィールドのみが変更されます） |
| DELETE | オブジェクトの削除 |

>[!NOTE]
>
>バージョン 1では、**Version1のメモ：** `PATCH`はサポートされていません。 すべての更新に`PUT`を使用します。


完全なエンドポイントパスとリクエスト/レスポンスの例については、[developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning)の&#x200B;**API リファレンス**&#x200B;を参照してください。

## HTTP ステータスコード

Planning APIは、標準のHTTP ステータスコードを返します。

| コード | 意味 |
|------------------------|-------------------------------------------------|
| 200 OK | 成功したGET、PUT、またはPATCH |
| 201作成 | 投稿が成功しました（リソースが作成されました） |
| 204 コンテンツなし | Adobe DELETEの成功 |
| 207 マルチステータス | 一括操作が完了し、結果が混在しました。一部の項目は成功し、一部の項目は失敗しました。 詳細については、個々のアイテムの応答を確認してください。 |
| 400不正なリクエスト | 無効なリクエスト – エラー応答を参照してください |
| 401未認証 | 認証トークンが見つからないか無効です |
| 403禁止 | 認証済みだが権限が不十分 |
| 404が見つかりません | リソースが存在しません |
| 409紛争 | 書き込み競合が発生しました。リソースは別のリクエストによって変更されました。 最新バージョンで再試行してください。 |
| 429要求が多すぎます | レート制限を超えました |

>[!NOTE]
>
>**バージョン 1のメモ：** バージョン 1では、POSTおよびDELETEを含むすべての正常な操作に対して`200 OK`が返されます。


## エラー処理

Planning APIは、一貫した形式でエラーを返します。 各エラー応答は、人間が読み取り可能なメッセージ、機械読み取り可能なエラーコード、およびサポートのエスカレーションのためのリクエスト IDを含む。

エラー応答の例：

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}
```

プログラムによるエラー処理を実行するには、`errorCode` （`status`ではなく）を使用してください。 失敗の最も具体的な分類を提供します。

>[!NOTE]
>
>**バージョン 1のメモ：** バージョン 1のエラー応答では、文字列`errorCode`の代わりに数値`type` フィールド （例：`40001`）を使用し、最上位`detail` フィールドではなく`report` オブジェクトに詳細をラップします。

## レコードのフィルタリング

レコード検索要求で`filter` パラメーターを使用して、特定の条件に一致するレコードのみを返します。 POST リクエストの場合、`filter`はリクエスト本文のJSON プロパティです。 GET リクエストの場合、`filter`はJSON エンコードされたフィルターグループを含むクエリパラメーターです。 フィルターは、明示的な論理演算子を含む型付き複合構造体を使用します。

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}
```

フィルターは、`AND` / `OR`演算子を使用してネストし、複合条件を構築できます。

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}
```

>[!NOTE]
>
>**バージョン 1注：** バージョン 1では、`filters` オブジェクトにMongo スタイルの型未入力演算子が使用されています。 演算子には`$`が先頭に付けられます（例：`$and`、`$or`、`$is`、`$contains`、`$isBetween`）。 ページネーション パラメーター（`offset`、`limit`）および`recordTypeId`は、URL パスおよびクエリパラメーターとしてではなく、リクエスト本文で渡されます。


## フィールドタイプと検索修飾子

フィールドで修飾子とフィルターを使用して、結果で返されるデータを制御できます。

例については、[Workfront Planning API開発者ドキュメント ](https://developer.adobe.com/wf-planning/)を参照してください。

### 検索修飾子の使用

Workfront Planningでは、次の検索修飾子がサポートされています。


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>修飾子</th>
      <th>例</th>
      <th>説明</th>
      <th>使用可能な値</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTAINS</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"CONTAINS","value":"product"}</td><td>フィールド値にフィルターが含まれているレコードを返します</td><td class="possible">"新製品のローンチ"</td></tr>
    <tr><td class="modifier">DOES_NOT_CONTAIN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"DOES_NOT_CONTAIN","value":"product"}</td><td>フィールド値にフィルターが含まれていないレコードを返します</td><td class="possible">「新しいローンチ」</td></tr>
    <tr><td class="modifier">IS</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS","value":"new product launch"}</td><td>フィールド値がフィルターと完全に一致するレコードを返します</td><td class="possible">"新製品のローンチ"</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT","value":"product"}</td><td>フィールド値がフィルターと完全に一致しないレコードを返します</td><td class="possible">"新製品のローンチ"</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EMPTY"}</td><td>フィールド値が空のレコードを返します</td><td class="possible">""またはnull</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_EMPTY"}</td><td>フィールド値が空でないレコードを返します</td><td class="possible">"新製品のローンチ"</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN","value":"10"}</td><td>フィールド値がフィルターより大きいレコードを返します</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"GREATER_THAN_OR_EQUAL","value":"10"}</td><td>フィールド値がフィルター以上のレコードを返します</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">LESS_THAN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN","value":"10"}</td><td>フィールド値がフィルターより小さいレコードを返します</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"LESS_THAN_OR_EQUAL","value":"10"}</td><td>フィールド値がフィルター以下のレコードを返します</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>フィールド値が2つのフィルター値の間にあるレコードを返します</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NOT_BETWEEN","value":["2024-01-01","2024-12-31"]}</td><td>2つのフィルター値の間にフィールド値が含まれていないレコードを返します</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_AFTER","value":"2024-01-01"}</td><td>フィルターの後に日付フィールド値があるレコードを返します</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_BEFORE","value":"2024-12-31"}</td><td>日付フィールド値がフィルターの前にあるレコードを返します</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_ANY_OF","value":["Active","Planned"]}</td><td>フィールド値がフィルターリストの任意の値と一致するレコードを返します</td><td class="possible">["Active","Planned","Complete"]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_NONE_OF","value":["Active","Planned"]}</td><td>フィールド値がフィルターリストの値のいずれとも一致しないレコードを返します</td><td class="possible">["Active","Planned"]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ANY_OF","value":["Tag1","Tag2"]}</td><td>複数の値フィールドにフィルター値のいずれかを含むレコードを返します</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_ALL_OF","value":["Tag1","Tag2"]}</td><td>複数の値フィールドにすべてのフィルター値が含まれているレコードを返します</td><td class="possible">["Tag1","Tag2"]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"IS_EXACTLY","value":["Tag1"]}</td><td>複数の値フィールドにフィルター値が正確に含まれ、他の値が含まれていないレコードを返します</td><td class="possible">["Tag1"]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{"fieldId":"&lt;id&gt;","condition":"HAS_NONE_OF","value":["Tag1"]}</td><td>複数値フィールドにフィルター値が含まれていないレコードを返します</td><td class="possible">["Tag1"]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>バージョン 1注：V1修飾子名には`$-prefixed camelCase`が使用されています（例：`$contains`、`$isNot`、`$isEmpty`、`$greaterThan`、`$greaterThanOrEqual`、`$lessThan`、`$lessThanOrEqual`、`$isBetween`、`$isNotBetween`、`$isAnyOf`、`$hasAllOf`）。 各修飾子の動作は同じです。


## フィールドタイプ別にサポートされるフィルター条件

| フィールドタイプ | サポートされる条件 |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| テキスト、長いテキスト | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| 数値、パーセント、通貨 | IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY |
| 日付 | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| 単一選択 | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| 複数選択，ユーザー | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| ブール値 | IS |
| 数式 | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| created-by | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF |
| updated-by | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| created-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN |
| updated-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY |
| 参照 | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| 参照 | リンクされたフィールドタイプによって異なります |

>[!NOTE]
>
>**バージョン 1注：** バージョン 1では、`$`接頭辞を付けた演算子名が使用されています（例：`$contains`、`$greaterThan`、`$isAnyOf`、`$hasAllOf`）。 フィールドタイプごとにサポートされる条件のセットは同じです。

## 人物フィールドによるフィルタリング

ユーザーフィールドフィルター（`user`、`created-by`、`updated-by`、`approved-by`）は、Adobe IMSユーザーIDとWorkfront ユーザーIDの両方を受け入れます。 プレーン文字列値は、Adobe IMSのユーザーIDとして解釈されます。

Workfront ユーザーIDを確認するために識別子の種類を設定するには、`id`および`idType` パラメーターを明示的に渡す必要があります。 `idType`でサポートされている値は、Workfront ユーザーIDの「`WF`」とAdobe IMSユーザーIDの「`IMS`」です。

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
> バージョン 1注：V1では、ユーザーのIMS IDによるフィルタリングのみがサポートされています。

## 外部IDによる外部参照フィールドのフィルタリング

外部参照フィールドは、レコードを他のAdobe システム（Workfront プロジェクトやAEM Assetsなど）のオブジェクトにリンクします。 内部的には、PlanningはPlanning レコード IDをこれらのオブジェクトに割り当てます。 これらのフィールドを元のオブジェクト IDで直接フィルターするには、フィルター条件に`"matchExternalId": true`を追加します。

このフラグは、`referenceOptions.isExternal`が`true`の参照フィールドに対してのみ有効です。外部参照フィールド以外では無視されます。 1つの文字列値を解決できない場合、リクエストは`400 Bad Request`で失敗します。 リスト値が指定された場合、未解決のエントリは変更されずに渡され、単純に一致しません。

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
>バージョン 1注：V1では、外部オブジェクト IDによるフィルタリングはサポートされていません。

## 外部接続フィールド

プランニングレコードタイプは、レコードを他のプランニングレコードタイプではなく、他のAdobe システムのオブジェクトにリンクする外部参照フィールドをホストできます。

APIを介して外部参照フィールドを作成するには、新しい`REFERENCE` フィールドの`referenceOptions.recordTypeId`を、目的の外部レコードタイプのIDに設定します。 サーバーは、ターゲット レコード タイプから`referenceOptions.isExternal=true`と接続メタデータ （`connectionName, objectName`）を自動的に取得します。

サポートされている外部オブジェクトタイプには、Workfront オブジェクト（プロジェクト、タスク、プログラム、ポートフォリオ、企業、グループ、チーム、ユーザー）およびAEM Assets（アセット、コンテンツフラグメント）が含まれます。

>[!NOTE]
>
>バージョン 1注：V1では、外部接続フィールドの作成はサポートされていません。


## 並べ替え

リクエストに`sort`配列を含めることで、任意のフィールドで結果を並べ替えます。

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

複数のソートフィールドが順番に評価されます。 ページ間で一貫性のある順序を確保するために、ページを分割するときは常に並べ替えを適用します。

結果をグループ化するには、並べ替えと一緒にグループ配列を含めます。

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>バージョン 1注：V1では、既存のビューの行の順序を適用するために、`sorting` （`sort`ではなく）、`groupingFieldIds` （フィールド IDの配列、`group` オブジェクトではない）および現在は非推奨の`rowOrderViewId`が使用されています。 これらのV1 パラメーターはいずれもバージョンでサポートされていません

## フィールド投影

応答で返されるフィールドを制限するには、コンマ区切りのリストを含む`fieldIds`または`fieldAliases` クエリパラメーターを使用します。 これにより、応答ペイロードのサイズが小さくなり、大量の統合や遅延が発生する可能性が高い統合に適しています。

>[!NOTE]
>
>**バージョン 1のメモ：** バージョン 1では、`?fieldIds=`や`?fieldAliases=`ではなく`?attributes=`を投影（例：`?attributes=data,createdBy`）に使用しています。

## ページネーション

Planning APIは、大きなデータセットを管理するためのページ分割された応答をサポートしています。

* **カーソルベースのページネーション**&#x200B;は、ワークスペース、レコードタイプ、フィールド、ビューに使用されます。 前の応答から`cursor`値を渡して、次のページを取得します。 カーソルに応じた応答には、ページ数が多いかどうかを示すhasMore フラグが含まれます。
* **ページベースのページネーション**&#x200B;は、レコード検索に使用されます。 `page`と`size`をクエリパラメーターとして使用します。 ページ間で一貫性のある順序を確保するために、ページを分割するときは常に並べ替えを適用します。 ページネーションは0から始まるので、2番目のページの結果を取得するには、パラメーターとして「`page=1`」を使用します。

例えば、次のリクエストを使用して、レコード検索から500 レコードの2番目のページを取得します。

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

ページ分割されたすべての応答には、より多くの結果が使用可能かどうかを示す構造化エンベロープが含まれます。 ページ間で一貫性のある順序を確保するために、ページを分割するときは常に並べ替えを適用します。

>[!NOTE]
>
> **バージョン 1のメモ：** V1では、リクエスト本文に渡された`offset`と`limit`が使用されています（デフォルトは500、最大は2,000）。 レコード 2001 ～ 4000を取得するには、リクエスト本文に「`offset`」:「`2000`」、「`limit`」:「`2000`」を設定します。 応答は、`totalCount` フィールドを持つフラットレコード配列を返します。

## 一括操作

Planning APIは、1回のリクエストでのレコードの一括作成、更新、パッチ適用、削除をサポートしています。 エンドポイントパス、リクエスト形式、操作ごとのレコードの制限については、[developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning)の&#x200B;**API リファレンス**&#x200B;を参照してください。

>[!NOTE]
>
>**バージョン 1のメモ：**&#x200B;一括操作は、バージョン 1では使用できません。


## 権限

エンティティへの権限は、リソースエンドポイント自体とは別に、専用の権限APIを使用して管理されます。 これにより、現在の権限を読み取り、共有リストを管理し、データ操作とは独立してアクセス要求を処理できます。 詳しくは、[Workfront Planning API](https://developer.adobe.com/wf-planning)の「API リファレンス」の節を参照してください。

>[!NOTE]
>
>**バージョン 1のメモ：** バージョン 1では、パブリック権限APIが公開されていません。 権限レベルは、リソース応答DTOに直接埋め込まれます。

## Workfront カスタムフォームでのPlanning APIの使用

Workfront カスタムフォームの外部ルックアップフィールドからPlanning APIを呼び出して、Workfront オブジェクト内に直接Planning データを表示できます。 詳細については、[ カスタムフォームの外部ルックアップフィールドの例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)を参照してください。

## 関連リソース

API関連の詳細なドキュメントについては、次の記事も参照してください。

* [Workfront Planning API](https://developer.adobe.com/wf-planning)開発者向けドキュメントとリファレンス
* [Adobe Workfront Planning の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning へのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)
* [Workfront 統合用の OAuth2 アプリケーションの作成](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->