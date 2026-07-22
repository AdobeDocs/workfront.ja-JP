---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Data Connect クエリの例
description: 特定の種類のクエリの構文と構造を理解するために使用できるクエリの例。
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
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

このクエリは、Data Connectの変更イベント追跡機能を使用します。以前のイベントとは異なる新しいステータス値を持つイベントがトリガーされた日付を決定します。 

クエリを内側から調べる： 

1. 以前のステータスが異なるレコードを計算します。 
   * 変更イベントごとに、lag （）関数を使用して、以前のステータスの値を特定します。 

2. 変更されたレコードのみをフィルタリングします。 

   * 前のステータスが現在のステータスである場合は、手順1の計算からレコード！=選択します。 

3. 開始/終了の有効なタイムスタンプと期間を日数で計算します。 

   * `<status_begin_effective_timestamp>`: ステップ 2で計算されました。 

   * `<status_end_effective_timestamp>`：次の（リード（））に基づいて計算されます。 `<status_begin_effective_timestamp>`: `<status_begin_effective_timestamp>`がNULLでない場合にのみステータスを表示します。 
   * `<status_duration_days>`: `<status_begin_effective_timestamp>`と`<status_end_effective_timestamp>`のデータの違い。 

>[!NOTE]
>
>このクエリをPowerBIまたはTableauの独自の「ビュー」として使用することをお勧めします。`<object>_event view`から他のフィールドを取り込む場合は、このクエリの出力を`<object>_event view`に戻します。結合フィールドは次のとおりです。<br>
>projects_event: 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## 計画：単一レコードタイプのクエリ

この例では、Data Connect データレイクに保存されている1つのレコードタイプについて、Workfront Planning データをクエリする方法を示します。

### シナリオ

組織では、Workfront Planningを使用してキャンペーンを追跡しています。 各キャンペーンレコードには、名前、ステータス、開始日、終了日、所有者が含まれます。 ダッシュボードで使用する、アクティブなすべてのキャンペーンとその主要な詳細のリストを取得します。

* プランニング・レコード・タイプ・データは、PLANNINGRECORD_CURRENT ビューに格納されます。
* 各行は1つのレコードを表し、すべてのフィールド値はFIELD_VALUESという名前のJSON列に格納されます。
* レコードタイプは、RECORDTYPEID列で識別されます。
* レコードのワークスペースは、WORKSPACEID列（または人間が読み取り可能なフィルターのWORKSPACENAME列）によって識別されます。

### クエリ

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### 応答

上記のクエリは、次のデータを返します。

* **recordid**: キャンペーンの一意の計画レコード ID。
* **campaign_name**: FIELD_VALUES JSON オブジェクトから抽出されたキャンペーンの名前。
* **campaign_status**: キャンペーンの現在のステータス。
* **start_date**: キャンペーンの開始日。日付データタイプにキャストされます。
* **end_date**: キャンペーンの終了日。日付データタイプにキャストされます。
* **所有者**: キャンペーンオーナーとして割り当てられたユーザーまたはチームの名前。

### 説明

Data Connectのプランニングレコードは、レコードタイプに関係なく、単一のテーブル構造を共有します。 RECORDTYPEID列は、クエリを特定のレコードタイプ（この場合はCampaigns）にスコープするために使用されます。 `<your_campaign_record_type_id>`をクエリするレコードタイプのIDに置き換えます。このIDは、Workfront計画レコードタイプの設定またはRECORDTYPE_CURRENTをクエリすることによって見つけることができます。

フィールド値は、FIELD_VALUES列にJSON オブジェクトとして保存され、カスタムフォームデータに使用するのと同じコロン表記法を使用してアクセスされます。

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

フィールド名の参照は、大文字、間隔、絵文字など、プランニングレコードタイプのフィールド設定で定義されているフィールド名と完全に一致する必要があります。

>[!NOTE]
>
>Workfront Planningでレコードタイプを表示する際に、URLにプランニングレコードタイプ IDが表示されます。 「Rt...」で始まるURLのパスです。 レコードタイプは、Data Connect内の次のSQL呼び出しでも見つけることができます。
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## 計画：接続されたレコードタイプのクエリ

この例では、接続されている2つのPlanning レコード・タイプ（親レコード・タイプと接続されているレコード・タイプ）にわたってデータを問い合わせる方法を示します。

### シナリオ

Workfront Planningのキャンペーンレコードを戦術レコードに接続します。 関連する戦術の主要な詳細と共に、各キャンペーンを示すレポートを作成します。 経営陣が戦術別に整理されたキャンペーン活動を確認できるように、戦術名、戦略的優先順位、予算配分を示したいと考えています。

データ接続では、ネイティブのプランニング・レコード・タイプ間の接続は、PLANNINGRECORD_CURRENTのFIELD_VALUES_RAW列に直接保存されます。 「戦術」という名前の参照フィールドの場合、値は接続されたレコードオブジェクトのJSON配列で、接続されたレコードのRECORDIDを持つID プロパティを含みます。 SnowflakeのLATERAL FLATTENを使用して、この配列を行に展開し、接続されたレコードタイプに結合します。

### クエリ

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### 応答

上記のクエリは、次のデータを返します。

* **campaign_id**: キャンペーンの一意のプランニングレコード ID。
* **campaign_name**: キャンペーンレコードの名前。
* **campaign_status**: キャンペーンの現在のステータス。
* **tactic_name**：接続されている戦術レコードの名前。
* **strategic_priority**：接続された戦術レコードの戦略的優先度フィールド値。
* **budget_allocation**：接続された戦術レコードの予算配分フィールド値で、浮動小数点としてキャストされます。

### 説明 – 変更されたKP

ネイティブのプランニング・レコード・タイプ間の接続は、REFERENCE_CURRENT結合テーブルに格納されます。  REFERENCE_CURRENT結合テーブルは、RecordType間の結合に使用されます。   RecordType間で結合する場合は、TO_RECORDID フィールドを使用する必要があります。

PLANNINGRECORD ビューのREFERENCE_ID列には、その計画レコードに適用できるすべてのREFERENCEID フィールドのリストが含まれます。 field_valueと同じJSON表記法を使用して、IDにアクセスできます。

```
<reference_ids>:"<reference_name>"::text
```

REFERENCE_CURRENT ビューには、TO_RECORDIDがPLANNINGRECORD_* ビューの他の計画`recordId` フィールドを指す1つ以上のレコードが含まれています。

別の参照フィールドを追加の計画レコードに結合するには、REFERENCE_CURRENTとPLANNINGRECORDに結合する同じパターンを使用して_*ビューを上記のクエリに追加します。


## 計画：レコードタイプをWorkfront Workflow データクエリに結合

この例では、REFERENCE_CURRENT ビューに外部オブジェクト参照を保存するPlanningのネイティブ接続機能を使用して、Workfront PlanningのレコードタイプをWorkfrontのネイティブワークフローオブジェクト（この場合はプロジェクト）に結合する方法を示します。

### シナリオ

組織は、Planningのネイティブ接続機能を使用して、Workfront PlanningのCampaign レコードをWorkfront プロジェクトに接続します。 キャンペーンマネージャーがPlanning Workspaceのコンテキストから離れることなく、配信の進捗状況を追跡できるように、リンクされたプロジェクトのライブ実行データ（特に、プロジェクトの現在の完了率、予定完了日、割り当てられたプロジェクトオーナー）とキャンペーンの詳細を示す統合レポートを作成します。

### クエリ

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### 応答

上記のクエリは、次のデータを返します。

* **campaign_id**: キャンペーンの一意のプランニングレコード ID。
* **campaign_name**: キャンペーンレコードの名前。
* **campaign_status**: Planningからのキャンペーンの現在のステータス。
* **linked_project_id**：接続されているWorkfront プロジェクトを識別する、REFERENCE_CURRENT.TO_EXTERNALIDのWorkfront プロジェクト ID。
* **project_name**: PROJECTS_CURRENTのネイティブ Workfront プロジェクト名。
* **project_percent_complete**: プロジェクトの現在の完了率の値。
* **project_planned_completion**: リンクされたWorkfront プロジェクトの予定完了日。
* **project_owner_id**: プロジェクト所有者のWorkfront ユーザーID。
* **project_owner_name**: プロジェクト所有者の表示名。USERS_CURRENTに参加することで解決されます。

### 説明

プランニングレコードタイプからネイティブのWorkfront Workflow オブジェクトへの接続は、REFERENCE_CURRENTに保存されます。 このビューの各行は、1つの方向リンクを表します。TO_EXTERNALIDは、接続されたWorkfront オブジェクトのIDを保持します。 Workfront接続を表す行は、`TO_EXTERNALCONNECTIONNAME = 'workfront'`と、Workfront オブジェクトタイプのAPI コード（プロジェクトのPROJなど）に対応するTO_EXTERNALOBJECTNAME値によって識別されます。

PLANNINGRECORD テーブルのREFERENCE_ID列には、そのレコードに適用できるすべてのREFERENCEID フィールドのリストが含まれます。  field_valueと同じJSON表記法を使用して、IDにアクセスできます。\
PLANNINGRECORD_CURRENT内の1つのREFERENCE_IDには、REFERENCE_CURRENT テーブル内の1つ以上の参照リンクが含まれ、Workfront テーブル内の特定のオブジェクトタイプのオブジェクトにリンクする場合があります。

```
<reference_ids>:"<reference_name>"::text
```

プランニングビュー（PLANNINGRECORD_CURRENT、REFERENCE_CURRENT）はWORKFRONT.PLANNING スキーマに存在し、ネイティブのWorkfront ワークフロービュー（PROJECTS_CURRENT、USERS_CURRENTなど）は存在することに注意してください。 Workfront.WF スキーマに格納されます。 クロススキーマ結合には、完全修飾テーブル名が必要です。

クエリは3つの結合を実行します。

1. **参照テーブルへのレコードの計画：** REFERENCE_CURRENTは`TO_RECORDID = c.RECORDID`に結合され、各Campaign レコードから送信されたすべての接続を検索します。 `TO_EXTERNALCONNECTIONNAME = 'workfront'`および`TO_EXTERNALOBJECTNAME = 'PROJ'`のフィルターは、Workfront プロジェクトへの接続を具体的に表す行に結果を絞り込みます。
1. **Workfront プロジェクトへの参照テーブル：** TO_EXTERNALIDは、接続されたプロジェクトのネイティブ Workfront プロジェクト IDを保持します。 これは、ライブプロジェクトデータを取得するために`PROJECTS_CURRENT.projectid`に直接結合されます。
1. **ユーザーへのプロジェクト：** USERS_CURRENTへのLEFT JOINは、プロジェクトの所有者ID外部キーを人間が読み取り可能な名前に解決します。 ここではLEFT JOINが使用されるので、所有者が割り当てられていないプロジェクトも結果に含まれます。

>[!NOTE]
>
>Planningの外部のテーブルに結合する場合は、クエリでTO_RECORDID フィールドを使用しないでください。  外部テーブルに結合する場合は必要ありません。
>
>このパターンは、プロジェクト、ポートフォリオ、プログラムなど、Planningが接続をサポートするWorkfront Workflow オブジェクトに適用できます。TO_EXTERNALOBJECTNAME フィルターを適切なオブジェクト API コード（ポートフォリオのPORTやプログラムのPRGMなど）に変更し、対応するWORKFRONT.WF テーブルに結合します。 各オブジェクトタイプの正しいテーブル名とID列名については、Workfront Data Connect データディクショナリを参照してください。

別のREFERENCE フィールドを追加の外部レコードに結合するには、REFERENCE_CURRENTとWorkfrontのワークフロービューに結合する同じパターンを上記のクエリに追加します。

外部レコードとプランニングレコードの値は、REFERENCE_CURRENT テーブルに複数回結合し、適切な結合パターンを使用して、同じクエリで結合できます。


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
