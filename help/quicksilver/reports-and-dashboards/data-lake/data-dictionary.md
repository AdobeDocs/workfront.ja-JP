---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect データディクショナリ
description: ここでは、Workfront Data Connect のデータの構造と内容について説明します。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 6%

---

# Workfront Data Connect データディクショナリ

ここでは、Workfront Data Connect のデータの構造と内容について説明します。

>[!NOTE]
>
>データ接続のデータは 4 時間ごとに更新されるので、最近の変更がすぐには反映されない場合があります。

## テーブルタイプ

データ接続で使用して、最もインサイトを得られる方法でWorkfront データを表示できるテーブルタイプは多数あります。

* **現在のテーブル**

  「現在のテーブル」には、Workfrontの場合と同様に、すべてのオブジェクトのデータが表示され、データの現在のステータスが表示されます。 ただし、Workfront内よりもはるかに低い待ち時間でナビゲーションできます。

* **イベントテーブル**

  イベント テーブルは、Workfront内のすべての変更レコードを追跡します。つまり、オブジェクトのステータスが変わるたびに、変更がいつ行われたか、誰が変更を加えたか、および何が変更されたかを示すレコードが作成されます。 したがって、このテーブルはポイントインタイムの比較に役立ちます。 このテーブルには、過去 3 年間のレコードのみが含まれます。

* **日別履歴テーブル**

  「毎日の履歴」 テーブルには、「イベント」 テーブルの短縮バージョンが表示されます。このテーブルでは、各オブジェクトの状態が、個々のイベントが発生した時間ではなく日単位で表示されます。 したがって、このテーブルはトレンド分析に役立ちます。

<!-- Custom table -->

## エンティティ関係図

Workfront（およびデータ接続データレイク）のオブジェクトは、個々の値だけでなく、他のオブジェクトとの関係によって定義されます。 以下のエンティティ関係図は、データ接続のオブジェクト関係の高度なマッピングを提供します。 この図は、次のリンクを使用して表示およびダウンロードできます。

[データ接続エンティティ関係図](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>エンティティ関係ダイアグラムは処理中です。そのため、参照用にのみ使用され、変更される可能性があります。

## 日付タイプ

特定のイベントが発生するタイミングに関する情報を提供する日付オブジェクトが多数あります。

* `DL_LOAD_TIMESTAMP`：この日付は内部参照に使用され、データが現在、イベントまたは毎日の履歴テーブルに読み込まれた日時を反映します。 この日付は、データ分析には使用せず、Workfront Data Lake のベータ段階で削除される予定です。
* `CALENDAR_DATE`：この日付は、「日別の履歴」テーブルにのみ表示されます。 この表は、`CALENDAR_DATE` で指定された各日付に対して、UTC で 11:59 にどのようなデータが表示されたかを示しています。
* `BEGIN_EFFECTIVE_TIMESTAMP`：この日付は、イベント履歴テーブルと日別履歴テーブルの両方に存在し、現在の行にあるレコードの値が _to_ 変更されたタイミングで正確にレコードされます。
* `END_EFFECTIVE_TIMESTAMP`：この日付は、イベント履歴テーブルと日別履歴テーブルの両方に表示され、レコードが現在の行の値から別の行の値に _変更された_ ときにそのレコードが正確に表示されます。 `BEGIN_EFFECTIVE_TIMESTAMP` と `END_EFFECTIVE_TIMESTAMP` のクエリ間でを許可するには、新しい値がない場合でも、この値は null ではありません。 レコードがまだ有効な場合（つまり、値が変更されていない場合）、`END_EFFECTIVE_TIMESTAMP` の値は 2300-01-01 になります。

## 用語テーブル

次の表は、Workfrontのオブジェクト名（およびインターフェイスと API のオブジェクト名）と、Data Connect の同等の名前を関連付けています。

<table>
<thead>
  <tr>
    <th>Workfront エンティティ名</th>
    <th>インターフェイス参照</th>
    <th>API リファレンス | ラベル</th>
    <th>Data Lake テーブル</th>
    <th>メモ</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>割り当て</td>
    <td>割り当て</td>
    <td>割り当て |割り当て</td>
    <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>条件、優先度、重要度、ステータス</td>
    <td>システム | カスタム列挙</td>
    <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT</td>
    <td>レコードのタイプは、「enumClass」プロパティを使用して識別されます。 必要なタイプは次のとおりです。<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
  </tr>
  <tr>
    <td>ドキュメント</td>
    <td>ドキュメント</td>
    <td>DOCU | ドキュメント</td>
    <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br><br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>ドキュメントのバージョン</td>
    <td>DOCV | ドキュメント バージョン</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>グループ</td>
    <td>グループ</td>
    <td>GROUP | グループ</td>
    <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>時間</td>
    <td>時間</td>
    <td>時間 |時間</td>
    <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>時間タイプ</td>
    <td>時間タイプ</td>
    <td>時間 |時間タイプ</td>
    <td>HOURTYPES_CURRENT</td>
    <td></td>
  </tr>
  <tr>
    <td>マイルストーン</td>
    <td>マイルストーン</td>
    <td>マイル | マイルストーン</td>
    <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilestonePath</td>
    <td>マイルストーンパス</td>
    <td>MPATH | マイルストーン パス</td>
    <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>メモ</td>
    <td>メモ</td>
    <td>メモ |注意</td>
    <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>問題、要求</td>
    <td>OPTASK |問題</td>
    <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br><br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>ポートフォリオ</td>
    <td>ポートフォリオ</td>
    <td>ポート |Portfolio</td>
    <td>PORTFOLIO_現在 <br>PORTFOLIO_日別_履歴 <br>PORTFOLIO_イベント <br><br>PORTFOLIO_カスタム_値_現在 <br>PORTFOLIO_カスタム_値_日別_履歴 <br>PORTFOLIO_カスタム_値_イベント</td>
    <td></td>
  </tr>
  <tr>
    <td>プログラム</td>
    <td>プログラム</td>
    <td>PRGM | プログラム</td>
    <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br><br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>プロジェクト</td>
    <td>プロジェクト</td>
    <td>見込み | プロジェクト</td>
    <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br><br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>役割</td>
    <td>担当業務</td>
    <td>役割 |担当業務</td>
    <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>スケジュール</td>
    <td>スケジュール</td>
    <td>SCHED | スケジュール</td>
    <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>タスク</td>
    <td>タスク</td>
    <td>タスク | タスク</td>
    <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br><br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY_TASKS<br>CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>チーム</td>
    <td>チーム</td>
    <td>TEAMOB | チーム</td>
    <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>タイムシート</td>
    <td>タイムシート</td>
    <td>テスト | タイムシート</td>
    <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>ユーザー</td>
    <td>ユーザー</td>
    <td>ユーザー | ユーザー</td>
    <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br><br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
