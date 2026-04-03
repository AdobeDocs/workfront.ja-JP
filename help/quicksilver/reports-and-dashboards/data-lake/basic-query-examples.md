---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect クエリの例
description: 特定の種類のクエリの構文と構造を理解するために使用できるクエリの例。
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 1%

---

# Workfront Data Connect クエリの例

このページでは、Workfront Data Connect データをより効果的に活用するために、特定の種類のクエリの構文と構造を理解するために使用できる基本的なクエリの例を示します。

## カスタムデータクエリ

この例では、カスタムフォームやカスタムフィールドなど、Workfrontでカスタムデータを返すクエリを作成する方法を示します。

### シナリオ

組織では、Finance Integrationという名前のカスタムフォームを使用します。 フォームは各プロジェクトに添付され、次のフィールドが含まれます。

* **事業部**：文字列を含むカスタムフィールド。
* **ProjectID**：数値文字列を含むカスタムフィールド。
* **拡張プロジェクト名**: Business Unit、ProjectID、およびネイティブ Workfront プロジェクト名の値を1つの文字列に連結する、計算されたカスタム データ フィールド。

Data Connectに対するクエリの応答にこの情報を含める必要があります。 データレイク内のレコードのカスタムデータ値は、`parametervalues`というタイトルの列に含まれています。 この列はJSON オブジェクトとして保存されます。

### クエリ

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

### 応答

上記のクエリは、次のデータを返します。

* `projectid`: ネイティブ Workfront プロジェクト ID。
* `parametervalues`: JSON オブジェクトを格納する列。
* `name`: ネイティブ Workfront プロジェクト名。
* `Business Unit`: `parametervalues` オブジェクトに含まれるカスタムデータ値。
* `Project ID`: `parametervalues` オブジェクトに含まれるカスタムデータ値。
* `Expanded Project Name`: `parametervalues` オブジェクトに含まれるカスタムデータ値。

### 説明

`parametervalues` JSON オブジェクトをクエリする場合、各カスタムデータフィールドに列としてアクセスするには、次を使用します。

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>`は、クエリ中のテーブル内のJSON オブジェクトの名前です。 カスタムデータの場合、これは常に`parametervalues`になります。
* `<parameter_name>`は、フォーム設定ツールで見つかった`parametername`文字列ですが、必ずしもこの値と一致しない場合があります。

>[!NOTE]
>
>Workfront フォーム設定ツールでパラメーターの名前が変更された場合、JSON オブジェクトの新しい列として表されます。 そのため、フォーム設定ツールで作成した列の名前は変更しないことをお勧めします。 ただし、JSON オブジェクトに影響を与えずにラベルを変更できます。
>
>パラメーター名のテキスト文字列が正しくない場合、列はエラーではなくNULL値を返します。

* `<data_type>`は、JSON オブジェクトから返される値を、フィールドに適したデータ型に変換します。 返される値に互換性のないデータタイプを選択すると、データタイプの不一致エラーが発生します。 使用可能なデータタイプは次のとおりです。

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` （例：`Number(32,4)`は1234.0987を返します）
   * `date`
   * `timestamp`

* `<column_name>`は、カスタムデータ列ごとに作成するラベルです。

>[!NOTE]
>
>フォームで値が割り当てられたパラメーターのみがJSON オブジェクトに含まれます。 カスタムデータフィールドがフォーム上で空の場合、そのフィールドは表示されません。

## ステータスクエリの時間

この例では、以前に割り当てられたステータスでプロジェクトが費やした時間を測定する方法を示します。 ステータス内のタスクやイシューの時間を測定するように簡単に調整したり、オブジェクトに他の属性（カスタムデータ値を含む）が適用された時間を測定するように調整したりできます。

### シナリオ

組織のリーダーは、作業ライフサイクルの各段階で多くの時間を費やしていると考えています。 プロセスを改善するための推奨事項を提案する前に、プロジェクトステータスが時間の経過とともに変更される頻度と、プロジェクトが特定のステータスを維持する日数をベースラインで測定する必要があります。

PROJECTS_EVENT データビューを使用して、プロジェクトオブジェクトに対する各ステータス変更のリストを取得します。 新しいステータスと前のステータスを比較し、以前に割り当てられたステータスの有効時間範囲を取得し、そのステータスに費やした日数を計算します。

プロジェクトごとに各ステータスに費やされた時間のこの生の出力を使用して、ビジュアライゼーションを構築したり、データをさらに集計したりして、ステータス、プロジェクトのタイプ、または年の時間ごとにステータス期間の平均値を構築することができます。 この基準値は、経営陣の期待に応えるためのベンチマークを設定するために使用されます。

次のクエリでは、Data Connect PROJECTS_EVENTS データビューを使用して、各プロジェクトステータス変更イベントを比較し、ステータスの時間を表示します。

### クエリ

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### 応答

上記のクエリは、次のデータを返します。

* `PROJECTID`: ステータス変更イベントに関連付けられているWorkfront プロジェクト ID。
* `PROJECT_NAME`: Workfront プロジェクト名。
* `PREVIOUS_STATUS`：変更の直前のプロジェクトのステータス。
* `STATUS`：変更後のプロジェクトのステータス。
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`：前のステータスが設定されたときの変更イベントのタイムスタンプ。
* `STATUS_END_EFFECTIVE_TIMESTAMP`：更新されたステータス値が設定されたときの変更イベントタイムスタンプ。
* `STATUS_DURATION_DAYS`：有効な終了タイムスタンプと有効な開始タイムスタンプの違い（日数）。

### 説明

クエリは、Data Connectの変更イベント追跡機能を使用します。  以前のイベントとは異なる新しいステータス値を持つイベントがトリガーされた日付を決定します。 

クエリを内側から調べる： 

1. 以前のステータスが異なるレコードを計算します。 
   * 変更イベントごとに、lag （）関数を使用して、以前のステータスの値を特定します。 

2. 変更されたレコードのみをフィルタリングします。 

   * 前のステータスのステップ 1の計算からレコードを選択します。=現在のステータス。 

3. 開始/終了の有効なタイムスタンプと期間を日数で計算します。 

   * `<status_begin_effective_timestamp>`: ステップ 2で計算されました。 

   * `<status_end_effective_timestamp>`：次の（リード（））に基づいて計算されます。 `<status_begin_effective_timestamp>`: `<status_begin_effective_timestamp>`がNULLでない場合にのみステータスを表示します。 
   * `<status_duration_days>`: `<status_begin_effective_timestamp>`と`<status_end_effective_timestamp>`のデータの違い。 

>[!NOTE]
>
>このクエリをPowerBIまたはTableauの独自の「ビュー」として使用することをお勧めします。  `<object>_event view`から他のフィールドを取り込む場合は、このクエリの出力を`<object>_event view`に戻します。  結合フィールドは次のとおりです：<br>
>projects_eventの場合： 
>`From projects_event p`
>`Join <above query> c on c.projectid = p.projectid  `
>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
