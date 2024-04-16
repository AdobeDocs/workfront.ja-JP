---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Data Lake データディクショナリ
description: このページでは、Workfront Data Lake のデータの構造と内容について説明します。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 912f46c87170d6b678d885ccc1fb0170526578df
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 9%

---

# Workfront Data Lake のデータディクショナリ

このページでは、Workfront Data Lake のデータの構造と内容について説明します。

>[!NOTE]
>
>Workfront Data Lake のデータは 4 時間ごとに更新されるので、最近の変更が直ちに反映されない場合があります。

## テーブルタイプ

最も多くのインサイトを提供する方法でWorkfront データを表示するために使用できるテーブルタイプは多数あります。

### 現在のテーブル

「現在のテーブル」には、Workfrontの場合と同様に、すべてのオブジェクトのデータが表示され、データの現在のステータスが表示されます。 ただし、Workfront内よりもはるかに低い待ち時間でナビゲーションできます。

### イベントテーブル

イベント テーブルは、Workfront内のすべての変更レコードを追跡します。つまり、オブジェクトのステータスが変わるたびに、変更がいつ行われたか、誰が変更を加えたか、および何が変更されたかを示すレコードが作成されます。 したがって、このテーブルはポイントインタイムの比較に役立ちます。 このテーブルには、過去 3 年間のレコードのみが含まれます。

### 日別履歴テーブル

「毎日の履歴」 テーブルには、「イベント」 テーブルの短縮バージョンが表示されます。このテーブルでは、各オブジェクトの状態が、個々のイベントが発生した時間ではなく日単位で表示されます。 したがって、このテーブルはトレンド分析に役立ちます。

<!-- Custom table -->

## 用語テーブル

次の表は、Workfrontのオブジェクト名（およびインターフェイスと API のオブジェクト名）と、データレイクの同等の名前を関連付けたものです。

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
    <td>ASSIGNMENTS_CURRENT<br>     ASSIGNMENTS_DAILY_HISTORY<br>     ASSIGNMENTS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>CustomEnum</td>
    <td>条件、優先度、重要度、ステータス</td>
    <td>システム | カスタム列挙</td>
    <td>CUSTOMENUMS_CURRENT<br>     CUSTOMENUMS_DAILY_HISTORY<br>     CUSTOMENUMS_EVENT</td>
    <td>レコードのタイプは、「enumClass」プロパティを使用して識別されます。 想定されるタイプは次のとおりです。<br>     CONDITION_OPTASK<br>     CONDITION_PROJ<br>     CONDITION_TASK<br>     PRIORITY_OPTASK<br>     PRIORITY_PROJ<br>     PRIORITY_TASK<br>     SEVERITY_OPTASK<br>     STATUS_OPTASK<br>     STATUS_PROJ<br>     STATUS_TASK</td>
  </tr>
  <tr>
    <td>ドキュメント</td>
    <td>ドキュメント</td>
    <td>DOCU | ドキュメント</td>
    <td>DOCUMENTS_CURRENT<br>     DOCUMENTS_DAILY_HISTORY<br>     DOCUMENTS_EVENT<br>     <br>     DOCUMENTS_CUSTOM_VALUE_CURRENT<br>     DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>     DOCUMENTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>DocumentVersion</td>
    <td>ドキュメントのバージョン</td>
    <td>DOCV | ドキュメント バージョン</td>
    <td>DOCUMENTVERSIONS_CURRENT<br>     DOCUMENTVERSIONS_DAILY_HISTORY<br>     DOCUMENTVERSIONS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>グループ</td>
    <td>グループ</td>
    <td>GROUP | グループ</td>
    <td>GROUPS_CURRENT<br>     GROUPS_DAILY_HISTORY<br>     GROUPS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>時間</td>
    <td>時間</td>
    <td>時間 |時間</td>
    <td>HOURS_CURRENT<br>     HOURS_DAILY_HISTORY<br>     HOURS_EVENT</td>
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
    <td>MILESTONES_CURRENT<br>     MILESTONES_DAILY_HISTORY<br>     MILESTONES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>MilestonePath</td>
    <td>マイルストーンパス</td>
    <td>MPATH | マイルストーン パス</td>
    <td>MILESTONEPATHS_CURRENT<br>     MILESTONEPATHS_DAILY_HISTORY<br>     MILESTONEPATHS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>メモ</td>
    <td>メモ</td>
    <td>メモ |注意</td>
    <td>NOTES_CURRENT<br>     NOTES_DAILY_HISTORY<br>     NOTES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>OpTask</td>
    <td>問題、要求</td>
    <td>OPTASK |問題</td>
    <td>OPTASKS_CURRENT<br>     OPTASKS_DAILY_HISTORY<br>     OPTASKS_EVENT<br>     <br>     OPTASKS_CUSTOM_VALUE_CURRENT<br>     OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>     OPTASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>ポートフォリオ</td>
    <td>ポートフォリオ</td>
    <td>ポート |Portfolio</td>
    <td>PORTFOLIO_現在<br>     PORTFOLIO_DAILY_HISTORY<br>     PORTFOLIO_イベント<br>     <br>     PORTFOLIO_カスタム_値_現在<br>     PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>     PORTFOLIO_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>プログラム</td>
    <td>プログラム</td>
    <td>PRGM | プログラム</td>
    <td>PROGRAMS_CURRENT<br>     PROGRAMS_DAILY_HISTORY<br>     PROGRAMS_EVENT<br>     <br>     PROGRAMS_CUSTOM_VALUE_CURRENT<br>     PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>     PROGRAMS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>プロジェクト</td>
    <td>プロジェクト</td>
    <td>見込み | プロジェクト</td>
    <td>プロジェクト_現在<br>     PROJECTS_DAILY_HISTORY<br>     PROJECTS_EVENT<br>     <br>     PROJECTS_CUSTOM_VALUE_CURRENT<br>     PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>     PROJECTS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>役割</td>
    <td>担当業務</td>
    <td>役割 |担当業務</td>
    <td>ROLES_CURRENT<br>     ROLES_DAILY_HISTORY<br>     ROLES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>スケジュール</td>
    <td>スケジュール</td>
    <td>SCHED | スケジュール</td>
    <td>SCHEDULES_CURRENT<br>     SCHEDULES_DAILY_HISTORY<br>     SCHEDULES_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>タスク</td>
    <td>タスク</td>
    <td>タスク | タスク</td>
    <td>タスク_現在<br>     TASKS_DAILY_HISTORY<br>     TASKS_EVENT<br>     <br>     TASKS_CUSTOM_VALUE_CURRENT<br>     TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>     TASKS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>チーム</td>
    <td>チーム</td>
    <td>TEAMOB | チーム</td>
    <td>TEAMS_CURRENT<br>     TEAMS_DAILY_HISTORY<br>     TEAMS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>タイムシート</td>
    <td>タイムシート</td>
    <td>テスト | タイムシート</td>
    <td>TIMESHEETS_CURRENT<br>     TIMESHEETS_DAILY_HISTORY<br>     TIMESHEETS_EVENT</td>
    <td></td>
  </tr>
  <tr>
    <td>ユーザー</td>
    <td>ユーザー</td>
    <td>ユーザー | ユーザー</td>
    <td>USERS_CURRENT<br>     USERS_DAILY_HISTORY<br>     USERS_EVENT<br>     <br>     USERS_CUSTOM_VALUE_CURRENT<br>     USERS_CUSTOM_VALUE_DAILY_HISTORY<br>     USERS_CUSTOM_VALUE_EVENT</td>
    <td></td>
  </tr>
</tbody>
</table>
