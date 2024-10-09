---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: データ接続クエリの例
description: クエリの例を使用すると、特定の種類のクエリの構文と構造を把握できます。
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Workfront Data Connect クエリの例

このページには、Workfront Data Connect データをより有効に活用するために、特定の種類のクエリの構文と構造を理解するために使用できる、基本的なクエリの例が含まれています。

## カスタムデータクエリ

この例では、カスタムフォームやカスタムフィールドなどのカスタムデータをWorkfrontで返すクエリを作成する方法を示しています。

### シナリオ：

組織は、財務統合という名前のカスタムフォームを使用します。 このフォームは、すべてのプロジェクトに添付され、次のフィールドが含まれています。

* **ビジネスユニット** – 文字列を含むカスタムフィールド。
* **ProjectID** – 数値の文字列を含むカスタムフィールド。
* **拡張プロジェクト名** - ビジネスユニット、プロジェクト ID およびネイティブのWorkfront プロジェクト名の値を 1 つの文字列に連結する計算カスタムデータフィールド。

Data Connect に対するクエリの応答にこの情報を含める必要があります。 データレイク内のレコードのカスタムデータ値は、`parametervalues` という名前の列に含まれています。 この列は JSON オブジェクトとして保存されます。

### クエリ :

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### 応答：

上記のクエリは、次のデータを返します。

* `projectid` - ネイティブ Workfront プロジェクト ID
* `parametervalues` - JSON オブジェクトを格納する列
* `name` - Workfrontのネイティブ プロジェクト名。
* `Business Unit` - `parametervalues` オブジェクトに含まれるカスタムデータ値
* `Project ID` - `parametervalues` オブジェクトに含まれるカスタムデータ値
* `Expanded Project Name` - `parametervalues` オブジェクトに含まれるカスタムデータ値

### 説明：

`parametervalues` の JSON オブジェクトに対してクエリを実行する場合、次のコードを使用して、各カスタムデータフィールドに列としてアクセスできます。

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` は、クエリ対象のテーブル内の JSON オブジェクトの名前です。 カスタムデータの場合、これは常に `parametervalues` になります。
* `<parameter_name>` はフォーム設定ツールで見つかった `parametername` 文字列ですが、この値と一致しない場合もあります。

>[!NOTE]
>
>Workfront フォーム設定ツールでパラメーターの名前が変更された場合、JSON オブジェクト内の新しい列として表されます。 そのため、フォーム設定ツールで作成した列の名前は変更しないことをお勧めします。 ただし、ラベルを変更しても JSON オブジェクトには影響しません。
>
>パラメーター名のテキスト文字列が正しくない場合、列はエラーではなく NULL 値を返します。

* `<data_type>` は、JSON オブジェクトから返される値を、フィールドに適したデータタイプに変換します。 返される値に互換性のないデータタイプを選択すると、データタイプ不一致エラーが発生します。 使用可能なデータタイプは次のとおりです。

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` （例：`Number(32,4)` は 1234.0987 を返します）
   * `date`
   * `timestamp`

* `<column_name>` は、カスタムデータ列ごとに作成するラベルです。

>[!NOTE]
>
>フォームで値が割り当てられているパラメーターのみが JSON オブジェクトに含まれます。 フォーム上のカスタムデータフィールドが空の場合は、表示されません。

<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
