---
title: Adobe Workfront計画APIの基本
description: Adobe Workfront Planning APIの目標は、HTTP経由で動作するREST フルなアーキテクチャを導入することで、Planningとの統合を構築することを簡素化することです。 このドキュメントでは、RESTおよびJSON応答に精通していることを前提としており、Planning APIで実行されるアプローチについて説明します。
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: c3d34c4b33164f5fe5b4420f3ddc81f3390abbf1
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 14%

---


# Adobe Workfront Planning API の基本

{{planning-important-intro}}

<!--
Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 
-->

<!--
To comment out when we release V2: 

# Adobe Workfront Planning API Basics

The goal of the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a RESTful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses.

For complete endpoint reference, request/ response schemas, and version-specific details, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>When using the Planning API, all user-related information is returned using the Adobe Identity Management System (IMS) user ID, not the Workfront user ID. (*************checking with Lilit because this changed in V2**************)


## Authentication

The Workfront Planning API uses the same authentication model as the Workfront API. All organizations on the Adobe Business Platform authenticate via OAuth2.

We support the following two flows:

* **Server-to-server authentication (JWT)**: For automated integrations and backend services. 

    For information, see [Configure and use your organization's custom OAuth 2 applications using JWT flow](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md).

* **User authentication (Authorization Code flow)**: For integrations acting on behalf of a specific user. 

    For information, see [Configure and use your organization's custom OAuth 2 applications using JWT flow](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md).

To set up credentials, create an OAuth2 application in Workfront. 

For information, see [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md). 

>[!NOTE]
>
>The `/login` endpoint and API key authentication are not supported for Workfront Planning. Do not use `sessionID` or `apiKey` parameters.


## API versioning

The Planning API is versioned via the URL path. 

The following are current supported versions: 

| Version   | Release date   |
|-----------|----------------|
| Version 1 | July 2024 |
| Version 2 | May 2026   |

(*****************add deprecation date column above, when we have one*****************)


For more information about the current supported versions, see the article [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning).

We recommend explicitly targeting a version in all integrations:

```
https://{customer-domain}/maestro/api/v2/...

```

When a new major version is released, the previous version will continue to be available until a deprecation date is communicated.

Follow the Workfront release notes to stay informed of API changes.


## URL structure and operations

Objects are manipulated by sending an HTTP request to their unique URI. The operation is specified by the HTTP method.

| Method   | Operation                                                            |
|----------|----------------------------------------------------------------------|
| GET      | Retrieve a single object by ID, or search/list objects               |
| POST     | Create a new object                                                  |
| PUT      | Replace an existing object (full update)                             |
| PATCH    | Partially update an existing object (only provided fields are modified) |
| DELETE   | Delete an object                                                     |

>[!NOTE]
>
>**V1 note:** `PATCH` is not supported in Version 1. Use `PUT` for all updates.


For full endpoint paths and request/response examples, see the **API reference** at [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## HTTP status codes

The Planning API returns standard HTTP status codes:

| Code                   | Meaning                                         |
|------------------------|-------------------------------------------------|
| 200 OK                 | Successful GET, PUT, or PATCH                   |
| 201 Created            | Successful POST (resource created)              |
| 204 No Content         | Successful DELETE                               |
| 400 Bad Request        | Invalid request — see error response for details |
| 401 Unauthorized       | Missing or invalid authentication token         |
| 403 Forbidden          | Authenticated but insufficient permissions      |
| 404 Not Found          | Resource does not exist                         |
| 429 Too Many Requests  | Rate limit exceeded                             |

>[!NOTE]
>
>**V1 note:** Version 1 returns `200 OK` for all successful operations, including POST and DELETE.


## Error handling

The Planning API returns errors in a consistent format. Each error response includes a human-readable message, a machine-readable error code, and a request ID for support escalation.

Example error response:

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

Use `errorCode` (not `status`) to drive programmatic error handling. It provides the most specific classification of the failure.

>[!NOTE]
>
>**V1 note:** Version 1 error responses use a numeric `type` field (e.g. `40001`) instead of a string `errorCode`, and wrap detail in a `report` object rather than a top-level `detail` field.

## Filtering records

Use the `filter` parameter in record search requests to return only records matching specific criteria. Filters use a typed composite structure with explicit logical operators:

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

Filters can be nested using `AND` / `OR` operators to build compound conditions:

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
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}

```

>[!NOTE]
>
>**V1 note:** Version 1 uses Mongo-style untyped operators in a `filters` object. Operators are prefixed with `$` (e.g. `$and`, `$or`, `$is`, `$contains`, `$isBetween`). Pagination parameters (`offset`, `limit`) and `recordTypeId` are passed in the request body rather than as URL path and query parameters.


## Field types and search modifiers

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Using search modifiers 

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
 
### Field types 

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

## Supported filter conditions by field type

| Field Type                  | Supported Conditions                                                                                         |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| text, long-text             | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY                                              |
| number, percentage, currency| IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY      |
| date                        | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY                         |
| single-select               | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                                   |
| multi-select, user          | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                    |
| boolean                     | IS                                                                                                           |
| formula, url                | CONTAINS, DOES_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY                                              |
| created-by, updated-by      | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF                                                                            |
| created-at, updated-at      | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN                                                 |
| reference                   | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY                                    |
| lookup                      | Depends on the linked field type                                                                             |

>[!NOTE]
>
>**V1 note:** Version 1 uses `$`-prefixed operator names (e.g. `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). The set of supported conditions per field type is the same.

## Sorting

Sort results by any field by including a `sort` array in your request:

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}

```

Multiple sort fields are evaluated in order. Always apply a sort when paginating to ensure consistent ordering across pages.

>[!NOTE]
>
>**V1 note:** The array key is `sorting` in Version 1, not `sort`.


---

## Field projection

To limit which fields are returned in a response, use the `fieldIds` or `fieldAliases` query parameters with a comma-separated list. This reduces response payload size and is recommended for high-volume or latency-sensitive integrations.

>[!NOTE]
>
>**V1 note:** Version 1 uses `?attributes=` for projection (e.g. `?attributes=data,createdBy`) rather than `?fieldIds=` or `?fieldAliases=`.

## Pagination

The Planning API supports paginated responses to manage large datasets.

* **Cursor-based pagination** is used for workspace and record type listings. Pass a cursor value from the previous response to retrieve the next page.
* **Page-based pagination** is used for record search. Use `page` and `size` as query parameters.

All paginated responses include a structured envelope indicating whether more results are available. Always apply a sort when paginating to ensure consistent ordering across pages.

>[!NOTE]
>
> **V1 note:** Version 1 uses `offset` and `limit` passed in the request body, with a default of 500 results and a maximum of 2,000. The response is a flat array with a `totalCount` field rather than a structured envelope.

## Bulk operations

The Planning API supports bulk create, update, patch, and delete of records in a single request. Refer to the **API reference** at [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning) for endpoint paths, request formats, and per-operation record limits.

>[!NOTE]
>
>**V1 note:** Bulk operations are not available in Version 1.


## Permissions

Resource permissions are managed through a dedicated Permissions API, separate from the resource endpoints themselves. This allows you to read current permissions, manage workspace or record type members, and handle access requests independently of data operations. For more information, see the "API references" section in the article [Workfront Planning API](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**V1 note:** Version 1 does not expose a public Permissions API. Permission level is embedded directly in resource response DTOs.

## Using the Planning API with Workfront custom forms

You can call the Planning API from an External lookup field in a Workfront custom form to surface Planning data directly within Workfront objects. For more information, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Related resources

For more API-related documentation, also see the following articles:

* [Workfront Planning API](https://developer.adobe.com/wf-planning) developer documentation and reference
* [Get started with Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md)
* [Create OAuth2 applications for Workfront integrations](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

-->

Adobe Workfront Planning APIの目標は、HTTP経由で動作するREST フルなアーキテクチャを導入することで、Planningとの統合を構築することを簡素化することです。 このドキュメントでは、RESTおよびJSON応答に精通していることを前提としており、Planning APIで実行されるアプローチについて説明します。

Workfront計画スキーマを理解すると、統合のためにWorkfront計画からデータを取り出すために使用できるデータベースの関係を理解するのに役立ちます。

Workfront カスタムフォームの外部参照フィールドから計画APIを呼び出すことができます。

外部参照フィールドについて詳しくは、[&#x200B; カスタムフォームの外部参照フィールドの例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)を参照してください。

>[!NOTE]
>
>Planning APIを使用する場合、Workfront ユーザーIDではなく、Adobe Identity Management System （IMS）ユーザーIDを使用してすべてのユーザー関連情報が返されます。
>
>詳しくは、[Adobe Admin Consoleでのユーザーの管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください。

## Workfront Planning APIのバージョン

* バージョン 1 - 2024年7月にリリース

  詳しくは、この記事の「[Workfront Planning API Version 1](#workfront-planning-api-version-1)」の節を参照してください。
  <!--
    Maybe retitle the "Workfront Planning API" section below to "Workfront Planning API Version 1" when Version 2 releases
    -->

<!--
* Version 2 - released in May 2026

    For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.
-->

## Workfront Planning API バージョン 1

Workfront Planning API バージョン 1は、2024年7月にリリースされました。

次の節では、Workfront API バージョン 1で使用可能になった機能について説明します。

特に指定されていない限り、今後のすべてのAPI バージョンには同じ機能が含まれます。

<!--
Becky had put the title of this article as"Workfront Planning API URL", but she did not document what that URL is; asking dev and hiding it for now
-->

<!--
For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).
-->

### 操作

オブジェクトは、一意の URI に HTTP リクエストを送信して操作します。 実行する操作は、HTTP メソッドで指定します。

標準の HTTP メソッドは、次の操作に対応しています。

* **GET** - IDでオブジェクトを取得し、クエリですべてのオブジェクトを検索します
* **POST** - 新しいオブジェクトを挿入
* **PUT** - 既存のオブジェクトを編集
* **DELETE** - オブジェクトを削除

各操作の詳細と例については、[Workfront Planning API開発者ドキュメント &#x200B;](https://developer.adobe.com/wf-planning/)を参照してください。

### フィールドタイプとそれらに使用される検索修飾子

フィールドで修飾子とフィルターを使用して、結果で返されるデータを制御できます。

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### 検索修飾子の使用

Workfront Planningでは、次の検索修飾子がサポートされています。

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
        <td>フィールド値にフィルターが含まれているレコードを返します  </td>
        <td>"新製品のローンチ"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>フィールド値にフィルターが含まれていないレコードを返します  </td>
        <td>「新しいローンチ」  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>フィールド値がフィルターと完全に一致するレコードを返します  </td>
        <td>"新製品のローンチ"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>フィールド値がフィルターと正確に一致しないレコードを返します  </td>
        <td>"新製品のローンチ"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>フィールド値が空のレコードを返します  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>フィールド値が空でないレコードを返します  </td>
        <td>"新製品のローンチ"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>フィールド値がフィルターより大きいレコードを返します  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>フィールド値がフィルター以上のレコードを返します  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>フィールド値がフィルターより小さいレコードを返します  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>フィールド値がフィルター以下のレコードを返します </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>フィールド値がフィルターの後にあるレコードを返します  </td>
        <td>「2024-05-15T20:00:00.000Z」  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>フィールド値がフィルターの前にあるレコードを返します </td>
        <td>「2024-05-12T20:00:00.000Z」 </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>フィールド値がフィルター間にあるレコードを返します  </td>
        <td><ul><li>「2024-05-12T20:00:00.000Z」 </li><li>「2024-05-14T20:00:00.000Z」 </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>フィールド値がフィルター間にないレコードを返します  </td>
        <td><ul><li>「2024-05-09T20:00:00.000Z」  </li><li>「2024-05-17T20:00:00.000Z」  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>フィールド値がフィルターのいずれかであるレコードを返します  </td>
        <td><ul><li>「アクティブ」 </li><li>「完了」 </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>フィールド値がフィルターのどれでもないレコードを返します </td>
        <td><ul><li>「完了」  </li><li>「固定」  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>フィールド値にフィルターのいずれかを持つレコードを返します  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>フィールド値にすべてのフィルターが含まれているレコードを返します  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>フィールド値にフィルターが含まれていないレコードを返します </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>フィールド値が正確にフィルターであるレコードを返します  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>

#### フィールドタイプ

次に、サポートされるフィールドタイプのリストと、それらのフィールドタイプごとに使用できる検索修飾子のリストを示します

| フィールドタイプ | サポートされている検索修飾子 |
|---|---|
| テキスト | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| ロングテキスト | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| 数値 | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| 割合 | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| 通貨 | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| 日付 | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| 単一選択 | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| 複数選択 | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| ブール値 | $is |
| ユーザー | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| 数式 | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| 参照 | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| 参照 | リンクされたフィールドによって異なります |

### 「And」ステートメントと「Or」ステートメントの使用

API呼び出しでは、$and文と&quot;$or&quot;文を組み合わせた複数の条件に基づくフィルターを使用できます

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

### fields リクエストパラメーターの使用

fields リクエストパラメーターを使用して、返す特定のフィールドのコンマ区切りリストを指定できます。 これらのフィールド名では、大文字と小文字が区別されます。

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
..
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

### クエリ制限とページ分割された応答

デフォルトでは、Planning API リクエストは、リストの先頭から500件の結果を返します。 結果数のデフォルト制限を上書きするには、リクエストで`limit` パラメーターを使用し、2000件まで別の数値に設定します。

リクエストに`offset` パラメーターを追加して、大規模なデータセットに対してページ分割された応答を使用することをお勧めします。 ページ分割された応答を使用すると、返す必要がある最初の結果の場所を指定できます。

例えば、2001-4000の結果を返す場合は、次のリクエストを使用できます。 次の例では、2001番目の結果から開始して、アクティブなステータスにある2000件のレコードを返します。

`POST /v1/records/search`



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

結果が正しくページ分割されるようにするには、並べ替えパラメーターを使用します。 これにより、結果が同じ順序で返されるので、ページネーションは結果を繰り返したりスキップしたりしません。

並べ替えについて詳しくは、この記事の「[API](#sorting-query-results-in-the-api)でのクエリ結果の並べ替え」を参照してください。

<!--

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