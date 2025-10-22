---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: データ接続クエリの例
description: クエリの例を使用すると、特定の種類のクエリの構文と構造を把握できます。
author: Nolan
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# Workfront Data Connect クエリの例

このページには、Workfront Data Connect データをより有効に活用するために、特定の種類のクエリの構文と構造を理解するために使用できる、基本的なクエリの例が含まれています。

## カスタムデータクエリ

この例では、カスタムフォームやカスタムフィールドなどのカスタムデータをWorkfrontで返すクエリを作成する方法を示しています。

### シナリオ

組織は、財務統合という名前のカスタムフォームを使用します。 このフォームは、すべてのプロジェクトに添付され、次のフィールドが含まれています。

* **ビジネスユニット**：文字列を含むカスタムフィールド。
* **ProjectID**：数値の文字列を含むカスタムフィールド。
* **拡張プロジェクト名**：事業部門、プロジェクト ID およびネイティブのWorkfront プロジェクト名の値を 1 つの文字列に連結する計算カスタムデータフィールド。

Data Connect に対するクエリの応答にこの情報を含める必要があります。 データレイク内のレコードのカスタムデータ値は、`parametervalues` という名前の列に含まれています。 この列は JSON オブジェクトとして保存されます。

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

* `projectid`：ネイティブ Workfront プロジェクト ID。
* `parametervalues`:JSON オブジェクトを格納する列。
* `name`: Workfrontのネイティブ プロジェクト名。
* `Business Unit`:`parametervalues` オブジェクトに含まれるカスタムデータ値。
* `Project ID`:`parametervalues` オブジェクトに含まれるカスタムデータ値。
* `Expanded Project Name`:`parametervalues` オブジェクトに含まれるカスタムデータ値。

### 説明

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

## ステータスクエリの時間

この例では、以前に割り当てられたステータスでプロジェクトが費やした時間を測定する方法を示します。 ステータスのタスクまたはイシューの時間を測定するように簡単に適応させることができます。または、オブジェクトに他の属性（カスタムデータ値を含む）が適用されていた時間を測定するように適応させることができます。

### シナリオ

組織のリーダーは、作業ライフサイクルの各段階で時間を費やしすぎていると考えています。 プロセスを改善するためのレコメンデーションを行う前に、プロジェクトのステータスが時間の経過と共に変化する頻度と、プロジェクトが特定のステータスにとどまる日数のベースライン測定を作成します。

PROJECTS_EVENT データビューを使用して、プロジェクトオブジェクトに対する各ステータス変更のリストを取り込みます。 新しいステータスを前のステータスと比較し、以前に割り当てられたステータスの有効な時間範囲を取得して、そのステータスで費やした日数を計算します。

このプロジェクトごとの各ステータスでの滞在時間の生の出力を使用すると、ビジュアライゼーションの作成を開始したり、データをさらに集計して、ステータス、プロジェクトタイプまたは年の時間別にステータス期間の平均を作成したりできます。 その後、このベースラインを使用して、リーダーシップの期待に応えるために測定できるベンチマークを設定します。

次のクエリでは、データ接続 PROJECTS_EVENTS データ ビューを使用して、各プロジェクトの状態変更イベントを比較し、状態に時間を表示します。

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

* `PROJECTID`：ステータス変更イベントに関連付けられたWorkfront プロジェクト ID。
* `PROJECT_NAME`:Workfrontのプロジェクト名。
* `PREVIOUS_STATUS`：変更直前のプロジェクトのステータス。
* `STATUS`：変更後のプロジェクトのステータス。
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`：以前のステータスが設定されたときの変更イベントのタイムスタンプ。
* `STATUS_END_EFFECTIVE_TIMESTAMP`：更新されたステータス値が設定されたときの変更イベントのタイムスタンプ。
* `STATUS_DURATION_DAYS`：有効なタイムスタンプの終了日と有効なタイムスタンプの開始日の差（日数）。

### 説明

クエリでは、Data Connect の変更イベントトラッキング機能を使用します。  以前のイベントとは異なる新しいステータス値を持つイベントがトリガーされた日付を特定します。 

クエリを内側から確認します。 

1. 前のステータスが異なるレコードを計算： 
   * すべての変更イベントに対して、lag （）関数を使用して status の以前の値を特定します。 

2. 変更されたレコードのみをフィルタリングします。 

   * ステップ 1 の計算（前のステータス）からレコードを選択します。=現在のステータス。 

3. 開始/終了有効タイムスタンプおよび期間を日数で計算します。 

   * `<status_begin_effective_timestamp>`：手順 2 で計算します。 

   * `<status_end_effective_timestamp>`：次の（lead （））に基づいて計算されます。 `<status_begin_effective_timestamp>`: ステータスが NULL でない場合 `<status_begin_effective_timestamp>` のみ表示されます。 
   * `<status_duration_days>`:`<status_begin_effective_timestamp>` と `<status_end_effective_timestamp>` のデータの違い 

>[!NOTE]
>
>PowerBI または Tableau では、このクエリを独自の「ビュー」として使用することをお勧めします。  `<object>_event view` から他のフィールドを取り込む場合は、このクエリからの出力を `<object>_event view` に結合し直します。  結合フィールドは次のようになります。<br>
>>projects_event の場合： 
>>`From projects_event p`
>>`Join <above query> c on c.projectid = p.projectid  `
>>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.-->
