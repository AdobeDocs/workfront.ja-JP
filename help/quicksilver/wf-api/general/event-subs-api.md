---
content-type: api
navigation-topic: general-api
title: イベント購読 API
description: イベント購読 API
author: John
feature: Workfront API
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c52f1839d3d00c71c6d567084dafd586d161d8fb
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 3%

---


# イベント購読 API

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

イベントの購読でサポートされているAdobe Workfrontオブジェクトでアクションが発生した場合、Workfrontが目的のエンドポイントに応答を送信するように設定できます。 つまり、サードパーティアプリケーションは、発生後すぐに、Workfront API を介してWorkfrontとのやり取りから更新を受け取ることができます。 一般に、ログに記録されるデータ変更から 5 秒未満で Webhook 通知を受け取ることが想定されます。 平均的に、お客様は、ログに記録されるデータ変更から 1 秒未満で Webhook 通知を受け取ります。  

ファイアウォールを通じてイベント購読ペイロードを受け取るには、次の IP アドレスをイベントに追加する必要があ許可リストります。

**ヨーロッパのお客様の場合：**

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

次のトピックでは、イベント購読 API をサポートしています。

## イベント購読でサポートされるオブジェクト

次のWorkfrontオブジェクトは、イベント購読でサポートされています。

* 割り当て
* 会社
* ダッシュボード
* ドキュメント
* 費用
* 時間
* 問題
* メモ
* ポートフォリオ
* プログラム
* プロジェクト
* レポート
* タスク
* テンプレート
* タイムシート
* ユーザー

イベント購読オブジェクトでサポートされるフィールドのリストについては、 [イベント購読リソースフィールド](../../wf-api/api/event-sub-resource-fields.md).

## イベント購読認証

イベント購読を作成、クエリ、または削除するには、Workfrontユーザーが次の条件を満たす必要があります。

* 「システム管理者」のアクセスレベル
* API キー

   >[!NOTE]
   >
   >ユーザーが既にWorkfront API を使用している場合は、既に apiKey を持っている必要があります。 次の HTTP リクエストを使用して apiKey を取得できます。

**リクエスト URL:**

```
PUT https://<HOSTNAME>/attask/api/v7.0/USER?action=getApiKey&username=<USERNAME>&password=<PASSWORD>
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
   <td> <p>Content-type</p> </td> 
   <td> <p>text/html</p> </td> 
  </tr> 
 </tbody> 
</table>

**応答コード：**

| 応答コード | 説明 |
|---|---|
| 200(OK) | リクエストは正常に処理され、ユーザーの既存の apiKey が応答本文に返されます。 |
| 401 （未認証） | サーバーはリクエストを確認しましたが、リクエスト apiKey/user がこのリクエストを行うためのアクセス権を持っていないので、リクエストを処理できませんでした。 |

{style=&quot;table-layout:auto&quot;}

**応答本文の例：**

```
{
               "data"{
               "result": "rekxqndrw9783j4v79yhdsakl56bu1jn"
               }
      }
```

>[!NOTE]
>
> Workfront API を初めて使用する場合は、次のリンクから実行できる apiKey を生成する必要があります。


```
PUT https://<HOSTNAME>/attask/api/v7.0/USER/generateApiKey?username=<USERNAME>&password=<PASSWORD>
```

## 購読リソースの作成

購読リソースには、次のフィールドが含まれます。

* objId （オプション）

   * **文字列**  — イベントが発生する、指定した objCode のオブジェクトの ID。 このフィールドを指定しない場合、ユーザーは指定したタイプのすべてのオブジェクトに対するイベントを受け取ります。

* objCode（必須）

   * **文字列**  — 変更をサブスクライブするオブジェクトの objCode。 objCode に指定できる値を次の表に示します。

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
        <td scope="col"><p>割り当て</p></td> 
       </tr> 
       <tr> 
        <td scope="col">会社 </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">ダッシュボード</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>ドキュメント</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>費用</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>時間</p></td> 
        <td scope="col">HOUR</td> 
       </tr> 
       <tr> 
        <td scope="col">問題</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">メモ</td> 
        <td scope="col">メモ</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>ポートフォリオ</p></td> 
        <td scope="col"><p>ポート</p></td> 
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
      </tbody> 
     </table>

* eventType（必須）

   * **文字列**  — オブジェクトがサブスクライブされているイベントのタイプを表す値。 使用可能なイベントタイプは次のとおりです。

      * 作成
      * 削除 
      * 更新

* url （必須）

   * **文字列**  — サブスクリプションイベントペイロードが HTTP 経由で送信されるエンドポイントの URL。

* authToken （必須）

   * **文字列** - 「URL」フィールドに指定された URL での認証に使用される OAuth2 bearer トークン。 

## イベント購読 API リクエストの作成

ユーザーに管理者アクセス権が付与され、購読リソースが作成されたことを確認したら、イベント購読を作成する準備が整いました。

次の構文を使用して、URL を構築します。

**リクエスト URL:**


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
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>認証</p> </td> 
   <td> <p>apiKey 値</p> </td> 
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
| 201 （作成済み） | イベント配信登録が正常に作成されました。 |
| 400（無効なリクエスト） | サブスクリプションリソースの URL フィールドが無効と見なされました。 |
| 401 （未認証） | 提供された apiKey は空であったか、無効と見なされました。 |
| 403 （禁止） | 指定された apiKey と一致するユーザーには、管理者アクセス権がありません。 |

サブスクリプションリソースをリクエストの本文として渡すと（content-type は「application/json」）、指定されたオブジェクトに対してイベントサブスクリプションが作成されます。 応答コード 201 （作成済み）は、購読が作成されたことを示します。 201 以外の応答コードは、サブスクリプションが **NOT** 作成済み

>[!NOTE]
 「Location」応答ヘッダーには、新しく作成されたイベント購読の URI が含まれます。

**応答ヘッダーの例：**

| 応答ヘッダー | 例 |
|---|---|
| Content-Length | `→0` |
| 日付 | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| 場所 | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| サーバー | `→Apache-Coyote/1.1` |

## イベント購読のクエリ

HTTP を使用してWorkfrontに問い合わせる場合は、GETメソッドを使用します。 イベント購読をクエリするには、2 つの方法があります。購読 ID（以下を参照）でクエリを実行するか、すべてのイベント購読をクエリします。

### すべてのイベント購読をクエリ

apiKey 値で指定された顧客のすべてのイベント購読をクエリできます。 また、次のオプションを使用して応答を管理することもできます。

* **ページ**:返すページ数を指定するクエリパラメーターオプション。 デフォルトは 1 です。
* **制限**:クエリーパラメーターオプションを使用して、1 ページあたりに返す結果の数を指定します。 デフォルトは 100 で、最大は 1000 です。

特定の顧客に関するすべてのイベント購読を一覧表示するためのリクエスト構文は次のとおりです。

**リクエスト URL:**

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
   <td> <p>認証</p> </td> 
   <td> <p>apiKey 値</p> </td> 
  </tr> 
 </tbody> 
</table>

**応答コード：**

| 応答コード | 説明 |
|---|---|
| 200(OK) | 指定された apiKey に一致する顧客に対して見つかったすべてのイベント購読で返されたリクエスト。 |
| 401 （未認証） | 提供された apiKey は空でした。 |
| 403 （禁止） | 指定された apiKey と一致するユーザーには、管理者アクセス権がありません。 |


**応答ヘッダーの例：**

| 応答ヘッダー | 例 |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| 日付 | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| サーバー | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


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

* **ページ** および **制限** は、リクエストで指定された値です。値が指定されていない場合はデフォルトです。
* **page_count** は、クエリを実行できるページの合計数です。
* **total_count** は、クエリに一致する購読の合計数です。

### イベント購読 ID によるクエリ

イベント購読の ID で、イベント購読をクエリできます。 イベント購読をリストするためのリクエスト構文は次のとおりです。

**リクエスト URL:**

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
   <td> <p>認証</p> </td> 
   <td> <p>apiKey 値</p> </td> 
  </tr> 
 </tbody> 
</table>

**応答コード：**

| 応答コード | 説明 |
|---|---|
| 200(OK) | 指定された購読 ID と一致するイベント購読が返されたリクエスト。 |
| 401 （未認証） | 提供された apiKey は空でした。 |
| 403 （禁止） | 指定された apiKey と一致するユーザーには、管理者アクセス権がありません。 |


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

## イベント購読のフィルタリング

イベント購読のフィルタリングを使用して、関連するメッセージのみを確実に受け取るようにできます。 購読のフィルターを作成すると、エンドポイントで使用する必要のあるメッセージの数が大幅に減る場合があります。

例： **更新 — タスク** イベント購読は、 **newState** イベントペイロードので、 **taskStatus** as **現在**.

>[!IMPORTANT]
イベント購読のフィルタリングには、次の属性が適用されます

* フィルターフィールドに空でない値が含まれる場合、 **newState** フィルターのキーと値が含まれている場合、購読された URL に送信されます
* フィルターは、 **newState** AND/OR **oldState**&#x200B;オブジェクトの
* フィルターは、特定の値と等しいかどうかに基づいてのみ評価されます
* フィルターの構文が正しくないか、 **newState** ペイロードの場合、エラーが発生したことを示す検証メッセージは返されません
* 現在存在する配信登録では、フィルターを更新できません。新しいフィルターパラメーターを使用して新しい購読を作成する必要があります。
* 1 つの購読に複数のフィルターを適用できます。購読は、すべてのフィルター条件が満たされた場合にのみ配信されます。
* 1 つの購読に複数のフィルターを適用する方法は、 **および** 論理演算子。
* 1 つ以上のイベント購読フィールドパラメーターが各イベント購読で異なる限り、複数のイベント購読を 1 つのオブジェクトに適用できます。
* 1 つのオブジェクトに複数のイベントサブスクリプションが割り当てられている場合、そのオブジェクトに関連付けられているすべてのイベントサブスクリプションを 1 つのエンドポイントに返すことができます。 この方法は、論理演算子の同等の代替として使用できます **または** フィルターパラメーターを使用して設定できない

### 比較演算子の使用

比較フィールドは、フィルターフィールドと共に指定できます。 比較結果をフィルタリングするには、このフィールドで比較演算子を使用します。 例えば、タスクのステータスが現在と異なる場合にのみペイロードを送信する UPDATE - TASK サブスクリプションを作成できます。 次の比較演算子を使用できます。

#### eq:次と等しい

このフィルターを使用すると、発生した変更が一致する場合にメッセージを表示できます `fieldValue` をフィルターに正確に含めます。 この `fieldValue` 値では大文字と小文字が区別されます。

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

#### ne:等しくない

このフィルターを使用すると、発生した変更が一致しない場合にメッセージを表示できます `fieldValue` をフィルターに正確に含めます。 この `fieldValue` 値では大文字と小文字が区別されます。

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

#### gt:より大きい

このフィルターを使用すると、指定した `fieldName` が `fieldValue`.

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

#### gte:次よりも大きいか等しい

このフィルターを使用すると、指定した `fieldName` 次の値以上 `fieldValue`.

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

#### lt:より小さい

このフィルターを使用すると、指定した `fieldName` が `fieldValue`.

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

#### lte:次よりも小さいか等しい

このフィルターを使用すると、指定した `fieldName` 次の値以下 `fieldValue`.

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

#### 含む

このフィルターを使用すると、発生した変更に `fieldValue` 」と入力します。 この `fieldValue` 値は大文字と小文字を区別します

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

#### 変更

このフィルターを使用すると、指定したフィールド (`fieldName`) の値が oldstate と newstate で異なる。 指定したフィールド (`fieldName`) はその変更を返しません。

>[!NOTE]
`fieldValue` のフィルター配列では、効果はありません。

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

#### state

このコネクタは、作成または更新されたオブジェクトの新しい状態または古い状態にフィルターを適用します。 これは、何かから別のものに変更が加えられた場所を知りたい場合に役立ちます。
`oldState` は、CREATE では使用できません `eventTypes`.

>[!NOTE]
指定されたフィルターを含む以下のサブスクリプションは、タスクの名前にが含まれるメッセージのみを返します `again` の `oldState`：タスクに対して更新がおこなわれる前の内容。
この場合、1 つのメッセージから別のメッセージに変更された objCode メッセージを見つけるのが使用例です。 例えば、「Research Some name」から「Research TeamName Some name」に変更されたタスクをすべて検索するには、次のようにします。

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

この `filterConnector` 購読ペイロードのフィールドを使用すると、フィルターの適用方法を選択できます。 デフォルトは「AND」です。ここで、フィルターはすべて `true` 購読メッセージが表示されるまで 「OR」が指定されている場合、購読メッセージが受け取るには、1 つのフィルターのみが一致する必要があります。

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

## イベント購読の削除

HTTP を使用してWorkfrontを削除する場合は、DELETEメソッドを使用します。 サブスクリプション ID で単一のイベントサブスクリプションを削除するリクエスト構文は次のとおりです。

**リクエスト URL:**

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
   <td> <p>認証</p> </td> 
   <td> <p> ユーザーの apiKey </p> </td> 
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
   <th> 説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 （コンテンツなし）</td> 
   <td>サーバーは、指定された subscriptionID に一致するイベント購読を正常に削除しました。</td> 
  </tr> 
  <tr> 
   <td>401 （未認証）</td> 
   <td>提供された apiKey は空でした。</td> 
  </tr> 
  <tr> 
   <td>403 （禁止）</td> 
   <td>指定された apiKey と一致するユーザーには、管理者アクセス権がありません。</td> 
  </tr> 
  <tr> 
   <td>404 （見つかりません）</td> 
   <td>サーバーは、削除用に提供された subscriptionID に一致するイベント配信登録を見つけられませんでした。</td> 
  </tr> 
 </tbody> 
</table>

**応答ヘッダーの例：**

| 応答ヘッダー | 例 |
|---|---|
| 日付 | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| サーバー | `→Apache-Coyote/1.1` |


**応答本文の例：** 該当なし

## イベントペイロードの例

ユーザーが受け取るペイロードは、オブジェクトのタイプによって異なりますが、様々なペイロードが配信される一貫した形式があります。

例えば、次のプロパティは、すべてのイベントペイロードで一貫性を保ちます。

* eventType
* subscriptionId
* oldState
* newState
* eventTime

形式は一貫していますが、プロパティ内に含まれる値は、オブジェクトやオブジェクトの種類によって異なります。

UPDATE イベントと CREATE イベントのペイロードの例を以下に示します。 UPDATE の例では、oldState オブジェクトと newState オブジェクトは同じですが、CREATE の例では、oldState オブジェクトが空（NULL ではない）です。

次に、UPDATE イベントのペイロードの例を示します。

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

イベント購読に含まれる特殊文字とネットワーク設定との競合が原因でイベント購読が拒否された場合は、Base64 エンコードを使用してイベント購読を渡すことができます。 Base64 は、任意のデータを ASCII 文字列形式に変換できる一連のエンコーディングスキームです。 Base64 はセキュリティ暗号化の一種ではないことに注意する必要があります。

### Base 64 エンコーディングフィールド

base64Encoding フィールドは、イベント購読ペイロードの Base64 エンコーディングを有効にするために使用されるオプションのフィールドです。 デフォルト値は false で、指定可能な値は次のとおりです。true、false および&quot; &quot; （空白）。

### base64Encoding フィールドを使用したリクエストの例

base64Encoding フィールドを true に設定してリクエストをおこなうと、 **newState** および **oldState** ペイロード内のオブジェクトは、基本 64 エンコーディング文字列として配信されます。 base64Encoding フィールドが false に設定されている場合、空白のままの場合、またはリクエストに含まれていない場合、返されるペイロードは base 64 でエンコードされません。

次に、 base64Encoding フィールドを使用するリクエストの例を示します。

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

### 基本 64 エンコーディングの応答ペイロードの例

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

## すべてのイベント購読を問い合わせる廃止されたメソッド

次の API エンドポイントは非推奨（廃止予定）となっており、新しい実装では使用しないでください。 また、古い実装を **イベント購読のクエリ** 上記の節を参照してください。

apiKey 値で指定された顧客のすべてのイベント購読をクエリできます。 特定の顧客に関するすべてのイベント購読を一覧表示するためのリクエスト構文は、次の URL です。

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
   <td> <p>認証</p> </td> 
   <td> <p> ユーザーの apiKey </p> </td> 
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
   <th> 説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 （コンテンツなし）</td> 
   <td>リクエストは、ユーザーに対して見つかったすべてのイベント購読を正常に返しました。</td> 
  </tr> 
  <tr> 
   <td>401 （未認証）</td> 
   <td>提供された apiKey は空でした。</td> 
  </tr> 
  <tr> 
   <td>403 （禁止）</td> 
   <td>指定された apiKey と一致するユーザーには、管理者アクセス権がありません。</td> 
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
