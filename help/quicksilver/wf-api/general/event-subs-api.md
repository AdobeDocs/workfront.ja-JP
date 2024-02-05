---
content-type: api
navigation-topic: general-api
title: Event Subscription API
description: Event Subscription API
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c08bd3311892d24a9bd40af138169957f5ea2ca4
workflow-type: tm+mt
source-wordcount: '2147'
ht-degree: 99%

---


# Event Subscription API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

イベント登録でサポートされている Adobe Workfront オブジェクトでアクションが発生した場合、目的のエンドポイントに応答を送信するように Workfront を設定できます。つまり、サードパーティアプリケーションは、発生後すぐに、Workfront API を介して Workfront とのやり取りから更新を受け取ることができます。一般に、ログに記録されるデータ変更から 5 秒未満で web フック通知を受信すると予想できます。平均的に、顧客は、ログに記録されるデータ変更から 1 秒未満で web フック通知を受け取ります。  

ファイアウォール経由でイベント登録ペイロードを受け取るには、次の IP アドレスを許可リストに追加する必要があります。

**ヨーロッパの顧客の場合：**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**ヨーロッパ以外の場所の顧客の場合：**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

次のトピックでは、Event Subscription API がサポートされています。

## イベント登録でサポートされるオブジェクト

次の Workfront オブジェクトは、イベント登録でサポートされています。

* 割り当て
* 会社
* ダッシュボード
* ドキュメント
* 費用
* フィールド
* 時間
* イシュー
* メモ
* ポートフォリオ
* プログラム
* プロジェクト
* レコード
* レコードタイプ
* レポート
* タスク
* テンプレート
* タイムシート
* ユーザー
* ワークスペース

イベント登録オブジェクトでサポートされるフィールドのリストについては、[イベント登録リソースフィールド](../../wf-api/api/event-sub-resource-fields.md)を参照してください。

## イベント登録認証

イベント登録を作成、クエリ、削除するには、Workfront ユーザーが次の条件を満たす必要があります。

* イベント登録を使用するには、「システム管理者」のアクセスレベルが必要です。
* イベント登録 API を使用するには `sessionID` ヘッダーが必要です

  詳しくは、[API の基本](api-basics.md)の[認証](api-basics.md#authentication)を参照してください。

## 登録リソースを作成

登録リソースには、次のフィールドが含まれます。

* objId（オプション）

   * **文字列** - イベントが発生したオブジェクト（指定された objCode のオブジェクト）の ID。このフィールドを指定しない場合、ユーザーは、指定されたタイプのすべてのオブジェクトのイベントを受け取ります。

* objCode（必須）

   * **文字列** - 変更に登録されるオブジェクトの objCode。objCode に指定できる値を次の表に示します。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>オブジェクト</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">割り当て</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">会社</td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">ダッシュボード</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>ドキュメント</p></td> 
        <td scope="col">DOCU</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>費用</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>フィールド</p></td> 
        <td scope="col"><p>フィールド</p></td> 
       </tr> 
      <tr> 
        <td scope="col"><p>時間</p></td> 
        <td scope="col">時間</td> 
       </tr> 
       <tr> 
        <td scope="col">イシュー</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">メモ</td> 
        <td scope="col">メモ</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>ポートフォリオ</p></td> 
        <td scope="col"><p>PORT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>プログラム</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>プロジェクト</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>レコード</p></td> 
        <td scope="col"><p>レコード</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>レコードタイプ</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>レポート</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>タスク</p></td> 
        <td scope="col"><p>タスク</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>テンプレート</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">タイムシート</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">ユーザー</td> 
        <td scope="col">ユーザー</td> 
       </tr> 
       <tr> 
        <td scope="col">ワークスペース</td> 
        <td scope="col">WORKSPACE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType（必須）

   * **文字列** - オブジェクトが登録されているイベントのタイプを表す値。使用可能なイベントタイプは次のとおりです。

      * 作成
      * DELETE
      * UPDATE

* url（必須）

   * **文字列** - 登録イベントペイロードが HTTP で送信されるエンドポイントの URL。

* authToken（必須）

   * **文字列** - 「URL」フィールドで指定された URL での認証に使用される OAuth2 ベアラートークン。

## イベント登録 API リクエストの作成

ユーザーに管理者アクセス権を確実に付与し、登録リソースを作成したら、イベント登録を作成する準備が整います。

次の構文を使用して、URL を作成します。

**リクエスト URL：**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**リクエストヘッダー：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>ヘッダー名</p> </th> 
   <th> <p>ヘッダー値</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>コンテンツタイプ</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID 値</p> </td> 
  </tr> 
 </tbody> 
</table>

**リクエスト本文の例：**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| 応答コード | 説明 |
|---|---|
| 201（作成済み） | イベント登録が正常に作成されました。 |
| 400（無効なリクエスト） | 登録リソースの URL フィールドが無効と見なされました。 |
| 401（未認証） | 指定された sessionID が空か、無効と見なされました。 |
| 403（禁止） | 指定された sessionID と一致するユーザーには、管理者アクセス権がありません。 |

登録リソースをリクエストの本文として渡すと（content-type は「application/json」）、指定されたオブジェクトのイベント登録が作成されます。応答コード 201（作成済み）は、登録が作成されたことを示します。201 以外の応答コードは、登録が作成&#x200B;**されなかった**&#x200B;ことを意味します。

>[!NOTE]
>
>「Location」応答ヘッダーには、新しく作成されたイベント登録の URI が含まれています。

**応答ヘッダーの例：**

| 応答ヘッダー | 例 |
|---|---|
| Content-Length | `→0` |
| 日付 | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Location | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| サーバー | `→Apache-Coyote/1.1` |

## イベント登録のクエリ

Workfront の HTTP をクエリする場合は、GET メソッドを使用します。イベント登録をクエリするには、2 とおりの方法があります。つまり、登録 ID でクエリする方法（以下を参照）と、すべてのイベント登録をクエリする方法です。

### すべてのイベント登録をクエリする方法

ある顧客のイベント登録をすべてクエリすることができます。また、次のオプションを使用して応答を管理することもできます。

* **page**：返すページ数を指定するクエリパラメーターオプション。デフォルトは 1 です。
* **limit**：1 ページあたりに返す結果の数を指定するクエリパラメーターオプション。デフォルトは 100 で、最大値は 1000 です。

特定の顧客のイベント登録をすべてリストするためのリクエスト構文は、次のとおりです。

**リクエスト URL：**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**リクエストヘッダー：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>ヘッダー名</p> </th> 
   <th> <p>ヘッダー値</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID 値</p> </td> 
  </tr> 
 </tbody> 
</table>

**応答コード：**

| 応答コード | 説明 |
|---|---|
| 200（OK） | 指定された sessionID と一致する顧客に対して見つかったすべてのイベント登録で返されたリクエスト。 |
| 401（未認証） | 提供された sessionID は空でした。 |
| 403（禁止） | 指定された sessionID と一致するユーザーには、管理者アクセス権がありません。 |


**応答ヘッダーの例：**

| 応答ヘッダー | 例 |
|---|---|
| コンテンツタイプ | `→application/json;charset=UTF-8` |
| 日付 | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| サーバー | `→Apache-Coyote/1.1` |
| 転送コード化 | `→chunked` |


**応答本文の例：**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

ここで

* **page** と **limit** は、リクエストで指定された値、または値が指定されていない場合はデフォルトです。
* **page_count** は、クエリを実行できるページの合計数です。
* **total_count** は、クエリに一致するサブスクリプションの合計数です。

### イベント登録 IDによるクエリ

イベント登録 IDで、イベント登録をクエリできます。イベント登録をリストするためのリクエスト構文は次のとおりです。

**リクエストURL：**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**リクエストヘッダー：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>ヘッダー名</p> </th> 
   <th> <p>ヘッダー値</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>sessionID 値</p> </td> 
  </tr> 
 </tbody> 
</table>

**応答コード：**

| 応答コード | 説明 |
|---|---|
| 200（OK） | 指定されたサブスクリプションIDと一致するイベント登録が返されたリクエスト。 |
| 401（未認証） | 提供された sessionID は空でした。 |
| 403（禁止） | 指定された sessionID と一致するユーザーには、管理者アクセス権がありません。 |


**応答本文の例：**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## イベント登録のフィルタリング

イベント登録のフィルタリングを使用して、関連するメッセージのみを確実に受け取るようにできます。サブスクリプションのフィルターを作成すると、エンドポイントで使用する必要のあるメッセージの数が大幅に減る場合があります。

例えば、**更新 - タスク**&#x200B;イベント登録は、イベントペイロードの **newState** が、**taskStatus** を **current** として定義する場合にのみトリガーするように設定できます。

>[!IMPORTANT]
>
イベント登録のフィルタリングには、次の属性が適用されます

* フィルターフィールドに空でない値が含まれる場合、フィルターキーと値を含む **newState** のメッセージだけが購読されたURLに送信されます。
* オブジェクトの&#x200B;**newState** AND/OR **oldState**&#x200B;に含まれるカスタムデータによってのみフィルタリングできます
* フィルターは、特定の値と等しいかどうかに基づいてのみ評価されます
* フィルターの構文が正しくないか、ペイロードの **newState** に含まれるデータに一致しない場合、エラーが発生したことを示す検証メッセージは返されません。
* 現在存在するサブスクリプションでは、フィルターを更新できません。新しいサブスクリプションは、新しいフィルターパラメーターを使用して作成する必要があります。
* 1 つの登録に複数のフィルターを適用でき、その登録は、すべてのフィルター条件が満たされた場合にのみ対応されます。
* 1 つの登録に複数のフィルターを適用する方法は、**AND** 論理演算子を使用する場合と同等です。
* 1 つ以上のイベント登録フィールドパラメーターがイベント登録ごとに異なる限り、複数のイベント登録を 1 つのオブジェクトに適用できます。
* 1 つのオブジェクトに複数のイベント登録が割り当てられている場合、そのオブジェクトに関連付けられているすべてのイベント登録を 1 つのエンドポイントに返すことができます。この方法は、フィルターパラメーターを使用する場合には設定できない論理演算子 **OR** の同等の代替手段として使用できます。

### 比較演算子の使用

フィルターフィールドと一緒に比較フィールドを指定できます。比較結果をフィルタリングするには、このフィールドで比較演算子を使用します。例えば、タスクのステータスが現在と異なる場合にのみペイロードを送信する UPDATE - TASK 登録を作成できます。次の比較演算子を使用できます。

#### eq：次と等しい

このフィルターを使用すると、発生した変更がフィルター内の `fieldValue` と正確に一致する場合に、メッセージが届きます。`fieldValue` 値では大文字と小文字が区別されます。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne：次と等しくない

このフィルターを使用すると、発生した変更がフィルター内の `fieldValue` と正確に一致しない場合に、メッセージが届きます。`fieldValue` 値では大文字と小文字が区別されます。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt：次よりも大きい

このフィルターを使用すると、指定された `fieldName` に対する更新が `fieldValue` の値よりも大きい場合に、メッセージが届きます。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### gte：次よりも大きいか等しい

このフィルターを使用すると、指定された `fieldName` に対する更新が `fieldValue` の値よりも大きいか等しい場合に、メッセージが届きます。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt：次よりも小さい

このフィルターを使用すると、指定された `fieldName` に対する更新が `fieldValue` の値よりも小さい場合に、メッセージが届きます。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte：次よりも小さいか等しい

このフィルターを使用すると、指定された `fieldName` に対する更新が `fieldValue` の値よりも小さいか等しい場合に、メッセージが届きます。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### が次を含む

このフィルターを使用すると、発生した変更がフィルター内の `fieldValue` を含んでいる場合に、メッセージが届きます。`fieldValue` 値では大文字と小文字が区別されます

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### changed：変更

このフィルターを使用すると、指定されたフィールド（`fieldName`）で oldState と newState の値が異なる場合にのみ、メッセージが届きます。指定されたフィールド（`fieldName`）以外のフィールドを更新しても、その変更は返されません。

>[!NOTE]
>
以下の filters 配列内の `fieldValue` による影響はありません。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### 状態

このコネクタを使用すると、作成または更新されたオブジェクトの新しい状態または古い状態にフィルターが適用されます。これは、状態が変化した場所を把握する場合に役立ちます。
`oldState` は、CREATE `eventTypes` では使用できません。

>[!NOTE]
>
フィルターが指定された以下の登録では、`oldState`（タスクが更新される前の状態）でタスク名に `again` が含まれているメッセージのみを返します。
この場合のユースケースは、状態が変化した objCode メッセージを見つけることです。例えば、「Research Some name」から「Research TeamName Some name」に変更されたタスクをすべて検索するには、次のように指定します。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### コネクタフィールドの使用

登録ペイロードの `filterConnector` フィールドを使用すると、フィルターの適用方法を選択できます。デフォルトは「AND」です。この場合、登録メッセージが届くためには、フィルターがすべて `true` である必要があります。「OR」が指定されている場合、登録メッセージが届くためには、1 つのフィルターのみが一致する必要があります。

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## イベント登録の削除

Workfront の HTTP を削除する場合は、DELETE メソッドを使用します。登録 ID で 1 つのイベント登録を削除するためのリクエスト構文は、次のとおりです。

**リクエスト URL：**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**リクエストヘッダー：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>ヘッダー名</p> </th> 
   <th> <p>ヘッダー値</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID 値 </p> </td> 
  </tr> 
 </tbody> 
</table>

**応答コード：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>応答コード</p> </th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200（コンテンツなし）</td> 
   <td>サーバーは、指定された subscriptionID に一致するイベント登録を正常に削除しました。</td> 
  </tr> 
  <tr> 
   <td>401（未認証）</td> 
   <td>提供された sessionID は空でした。</td> 
  </tr> 
  <tr> 
   <td>403（禁止）</td> 
   <td>指定された sessionID と一致するユーザーには、管理者アクセス権がありません。</td> 
  </tr> 
  <tr> 
   <td>404（見つかりません）</td> 
   <td>サーバーは、削除用に指定された subscriptionID に一致するイベント登録を見つけることができませんでした。</td> 
  </tr> 
 </tbody> 
</table>

**応答ヘッダーの例：**

| 応答ヘッダー | 例 |
|---|---|
| 日付 | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| サーバー | `→Apache-Coyote/1.1` |


**応答本文の例：**&#x200B;該当なし

## イベントペイロードの例

ユーザーが受信するペイロードは、オブジェクトの種類によって異なりますが、様々なペイロードが配信される一貫した形式があります。

例えば、次のプロパティは、すべてのイベントペイロードで一貫性を保ちます。

* eventType
* subscriptionId
* oldState
* newState
* eventTime

形式は一貫していますが、プロパティ内に含まれる値は、オブジェクトやオブジェクトの種類によって異なります。

UPDATE イベントと CREATE イベントのペイロードの例を以下に示します。UPDATE の例では、oldState オブジェクトと newState オブジェクトは同じですが、CREATE の例では、oldState オブジェクトは空です（NULL ではありません）。

次は、UPDATE イベントのペイロードの例です。

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

次に、CREATE イベントのペイロードの例を示します。

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Base 64 エンコーディング

イベント登録に含まれる特殊文字とネットワーク設定との競合が原因でイベント購読が拒否された場合は、Base64 エンコードを使用してイベント登録を渡すことができます。Base64 は、任意のデータを ASCII 文字列形式に変換できる一連のエンコーディングスキームです。Base64 はセキュリティ暗号化の一種ではないことに注意する必要があります。

### Base 64 エンコーディングフィールド

base64Encoding フィールドは、イベント登録ペイロードの Base64 エンコーディングを有効にするために使用されるオプションのフィールドです。デフォルト値は false で、指定可能な値は true、false および「 」（空白）です。

### base64Encoding フィールドを使用したリクエストの例

base64Encoding フィールドを true に設定してリクエストを行うと、ペイロード内の **newState** および **oldState** オブジェクトは、Base 64 エンコーディング文字列として配信されます。base64Encoding フィールドが false に設定されている場合、空白のままの場合、またはリクエストに含まれていない場合、返されるペイロードは Base 64 でエンコードされません。

次に、base64Encoding フィールドを使用するリクエストの例を示します。

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Base64 エンコーディングの応答ペイロードの例

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## すべてのイベント登録をクエリする非推奨メソッド

次の API エンドポイントは非推奨（廃止予定）となっており、新しい実装では使用しないでください。また、古い実装を上記の「**イベント登録をクエリ**」セクションで説明されているメソッドに移行させることもお勧めします。

sessionID 値で指定された顧客のすべてのイベント登録をクエリできます。特定の顧客に関するすべてのイベント登録を一覧表示するためのリクエスト構文は、次の URL です。

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**リクエストヘッダー：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>ヘッダー名</p> </th> 
   <th> <p>ヘッダー値</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> sessionID 値 </p> </td> 
  </tr> 
 </tbody> 
</table>

**応答コード：**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>応答コード</p> </th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200（コンテンツなし）</td> 
   <td>リクエストは、ユーザーに対して見つかったすべてのイベント登録を正常に返しました。</td> 
  </tr> 
  <tr> 
   <td>401（未認証）</td> 
   <td>提供された sessionID は空でした。</td> 
  </tr> 
  <tr> 
   <td>403（禁止）</td> 
   <td>指定されたセッション ID と一致するユーザーには、管理者アクセス権がありません。</td> 
  </tr> 
 </tbody> 
</table>

 

### 応答本文の例

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
