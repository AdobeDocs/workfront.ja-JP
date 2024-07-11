---
title: 'Adobe Workfront計画 API の基本'
description: Adobe Workfront Planning API の目標は、HTTP 経由で動作する REST-ful アーキテクチャを導入することで、Planning との統合を簡単に構築することです。 このドキュメントは、REST 応答と JSON 応答に精通していることを前提としており、Planning API によるアプローチについて説明しています。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ebdcb8ee2a6efe96c77f863e85f8911d20ab1dd4
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 13%

---


# Adobe Workfront計画 API の基本

Adobe Workfront Planning API の目標は、HTTP 経由で動作する REST-ful アーキテクチャを導入することで、Planning との統合を簡単に構築することです。 このドキュメントは、REST 応答と JSON 応答に精通していることを前提としており、Planning API によるアプローチについて説明しています。

Workfront Planning スキーマをよく理解しておくと、統合を目的としてWorkfront Planning からデータを取り出す際に利用できるデータベースの関係を理解しやすくなります。

## Workfront計画 API の URL

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### 操作

オブジェクトは、一意の URI に HTTP リクエストを送信して操作します。実行する操作は、HTTP メソッドで指定します。

標準の HTTP メソッドは、次の操作に対応しています。

* **GET** - ID でオブジェクトを取得し、クエリですべてのオブジェクトを検索します
* **POST** - 新しいオブジェクトを挿入
* **PUT** - 既存のオブジェクトを編集
* **DELETE** - オブジェクトを削除

各操作の詳細と例については、を参照してください [Workfront Planning API 開発者向けドキュメント](https://developer.adobe.com/wf-planning/).

### フィールドタイプと、それらで使用される検索修飾子

フィールドに修飾子とフィルターを使用して、結果で返されるデータを制御できます。

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### 検索修飾子の使用

Workfront Planning では、次の検索修飾子をサポートしています。

<table>
    <tr>
        <td><b>修飾子</b></td>
        <td><b>例</b></td>
        <td><b>説明</b></td>
        <td><b>可能な値</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>フィールド値にフィルターが含まれるレコードを返します  </td>
        <td>「新製品の発売」  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>フィールド値にフィルターが含まれていないレコードを返します  </td>
        <td>"新しいローンチ"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>フィールド値がフィルターと完全に一致するレコードを返します  </td>
        <td>「新製品の発売」  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>フィールド値がフィルターと完全には一致しないレコードを返します  </td>
        <td>「新製品の発売」  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>フィールド値が空でないレコードを返します  </td>
        <td><ul><li>"" </li><li>ヌル </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>フィールド値が空でないレコードを返します  </td>
        <td>「新製品の発売」  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>フィールド値がフィルターよりも大きいレコードを返します  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>フィールドの値がフィルターよりも大きいか等しいレコードを返します  </td>
        <td><ul><li>10</li><li>20</li><ul><li>25</li> </td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>フィールド値がフィルターよりも小さいレコードを返します  </td>
        <td><ul><li>5</li><li>9</li><ul> </td>
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>フィールド値がフィルター値以下のレコードを返します </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>フィールド値がフィルターの後のレコードを返します  </td>
        <td>"2024-05-15T20:00:00.000Z ”  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>フィールド値がフィルターの前にあるレコードを返します </td>
        <td>"2024-05-12T20:00:00.000Z ” </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>フィールド値がフィルターの範囲内にあるレコードを返します  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z ” </li><li>"2024-05-14T20:00:00.000Z ” </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>フィールド値がフィルターの範囲外にあるレコードを返します  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z ”  </li><li>"2024-05-17T20:00:00.000Z ”  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>フィールド値がフィルターのいずれかであるレコードを返します  </td>
        <td><ul><li>"アクティブ" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>フィールド値がフィルターのいずれでもないレコードを返します </td>
        <td><ul><li>"完了"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>フィールド値にフィルターのいずれかが含まれているレコードを返します  </td>
        <td><ul><li>["アクティブ", "固定"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>フィールド値にすべてのフィルターが含まれるレコードを返します  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>フィールド値にフィルターがないレコードを返します </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>フィールド値が完全にフィルターであるレコードを返します  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>

#### フィールドタイプ

サポートされているフィールドタイプのリストと、それらの各フィールドタイプで使用できる検索修飾子は次のとおりです

| フィールドタイプ | サポートされる検索修飾子 |
|---|---|
| テキスト | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| 長テキスト | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| 数値 | $is、$isNot、$greaterThan、$greaterThanOrEqual、$lessThan、$lessThanOrEqual、$isEmpty、$isNotEmpty |
| 割合 | $is、$isNot、$greaterThan、$greaterThanOrEqual、$lessThan、$lessThanOrEqual、$isEmpty、$isNotEmpty |
| 通貨 | $is、$isNot、$greaterThan、$greaterThanOrEqual、$lessThan、$lessThanOrEqual、$isEmpty、$isNotEmpty |
| 日付 | $is、$isNot、$isAfter、$isBefore、$isBetween、$isNotBetween、$isEmpty、$isNotEmpty |
| 単一選択 | $is、$isNot、$isAnyOf、$isNoneOf、$isEmpty、$isNotEmpty |
| 複数選択 | $hasAnyOf、$hasAllOf、$isExactly、$hasNoneOf、$isEmpty、$isNotEmpty |
| ブール値 | $is |
| ユーザー | $hasAnyOf、$hasAllOf、$isExactly、$hasNoneOf、$isEmpty、$isNotEmpty |
| 数式 | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| 作成者 | $is, $isNot, $isAnyOf, $isNoneOf |
| 作成日 | $is、$isNot、$isAfter、$isBefore、$isBetween、$isNotBetween |
| 更新者 | $is、$isNot、$isAnyOf、$isNoneOf、$isEmpty、$isNotEmpty |
| 更新日時 | $is、$isNot、$isAfter、$isBefore、$isBetween、$isNotBetween、$isEmpty、$isNotEmpty |
| 参照 | $hasAnyOf、$hasAllOf、$isExactly、$hasNoneOf、$isEmpty、$isNotEmpty |
| 参照 | リンクされたフィールドに依存 |

### 「And」ステートメントと「Or」ステートメントの使用

API 呼び出しでは、$and&quot; ステートメントと「$or」 ステートメントで組み合わせた、複数の条件に基づくフィルターを使用できます

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

### フィールドリクエストパラメーターの使用

フィールドリクエストパラメーターを使用して、返す必要がある特定のフィールドのコンマ区切りリストを指定できます。 これらのフィールド名では、大文字と小文字が区別されます。

例えば、次のリクエスト：

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
....
```

は、次のような応答を返します。


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### API でのクエリ結果の並べ替え

API 呼び出しに以下を追加すると、任意のフィールド別に結果を並べ替えることができます。


`/v1/records/search`

リクエスト本文：

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

### クエリの制限とページ分割された応答

デフォルトでは、Planning API リクエストは、リストの先頭から 500 件の結果を返します。 結果数のデフォルトの制限を上書きするには、を使用できます `limit` リクエストでをパラメーターし、別の数、最大 2000 件の結果に設定します。

大規模なデータセットに対しては、を追加することで、ページ分割された応答の使用を検討することをお勧めします。 `offset` あなたの要求に対するパラメーター。 ページ分割された応答では、返される最初の結果の場所を指定できます。

例えば、2001～4000 の範囲で結果を返す場合は、次のリクエストを使用できます。 次の例では、2001 番目の結果から、アクティブ・ステータスの 2000 件のレコードが戻されます：

`POST /v1/records/search `



リクエスト本文：

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

結果が正しくページ分割されるようにするには、並べ替えパラメーターを使用します。これにより、結果が同じ順序で返されるので、ページネーションで結果が繰り返されたりスキップされたりすることはありません。

並べ替えについて詳しくは、 [API でのクエリ結果の並べ替え](#sorting-query-results-in-the-api) この記事の内容です。



