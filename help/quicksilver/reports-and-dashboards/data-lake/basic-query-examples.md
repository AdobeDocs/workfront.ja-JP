---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: データ接続クエリの例
description: クエリの例を使用すると、特定の種類のクエリの構文と構造を把握できます。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Workfront Data Connect クエリの例

このページには、Workfront Data Connect データをより有効に活用するために、特定の種類のクエリの構文と構造を理解するために使用できる、基本的なクエリの例が含まれています。

## カスタムデータクエリ

この例では、カスタムフォームやカスタムフィールドなどのカスタムデータをWorkfrontで返すクエリを作成する方法を示しています。

### シナリオ：

組織の PeopleSoft は、Finance Integration という名前のカスタムフォームを使用します。 このフォームは、すべてのプロジェクトに添付され、次のフィールドが含まれています。

* **PeopleSoft ビジネスユニット** – 文字列を含むカスタムフィールド。
* **PeopleSoft ProjectID** – 数値の文字列を含むカスタムフィールド。
* **拡張プロジェクト名** - PeopleSoft ビジネスユニット、PeopleSoft プロジェクト ID およびネイティブのWorkfront プロジェクト名の値を 1 つの文字列に連結する計算カスタムデータフィールド。

Data Connect に対するクエリの応答にこの情報を含める必要があります。 データレイク内のレコードのカスタムデータ値は、`parameterValues` という名前の列に含まれています。 この列は JSON オブジェクトとして保存されます。

### クエリ :

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:PeopleSoft Business Unit" :: int as PeopleSoftBusinessUnit,
    parametervalues:"DE:PeopleSoft Project ID" :: int as PeopleSoftProjectID,
    parametervalues:"DE:Expanded Project Name" :: text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### 応答

上記のクエリは、次のデータを返します。

* `projectid` - ネイティブ Workfront プロジェクト ID
* `parametervalues` - JSON オブジェクトを格納する列
* `name` - Workfrontのネイティブ プロジェクト名。
* `PeopleSoft Business Unit` - `parametervalues` オブジェクトに含まれるカスタムデータ値
* `PeopleSoft Project ID` - `parametervalues` オブジェクトに含まれるカスタムデータ値
* `Expanded Project Name` - `parametervalues` オブジェクトに含まれるカスタムデータ値

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
