---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 10 の新機能
description: アップデートされたリソース
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
TQID: https://experienceleague.adobe.com/7paMh3l4zsoBaafv6U6pp1M-SQjk-kdmSho9GYa15SU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 484
ht-degree: 100%

---

# API バージョン 10 の新機能

* [新しいリソース](#new-resources)
* [アップデートされたリソース](#updated-resources)
* [削除されたリソース](#removed-resources)

## 新しいリソース {#new-resources}

### ActivityLog

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | ADD |
|   |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | 検索 |

{style="table-layout:auto"}

### CalendarEntry

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
|   |   |   |   |   |   | COUNT  |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | EDIT  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | REPORT  |
|   |   |   |   |   |   | 検索 |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | REPORT  |
|   |   |   |   |   |   | 検索  |

{style="table-layout:auto"}

### ExternalAuthToken

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
|   |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | DELETE  |
|   |   |   |   |   |   | EDIT  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | REPORT  |
|   |   |   |   |   |   | 検索  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| customerID | 顧客 |   |   |   |   |   |
| groupID | グループ |   |   |   |   |   |
| planLimit |   |   |   |   |   |   |
| usedLicenses |   |   |   |   |   |   |
| worklimit |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserHomeCalendarPreference

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| customerID | 顧客 |   |   |   |   | ADD |
| edTime | ユーザー |   |   |   |   | COUNT |
| firstDayOfWeek |   |   |   |   |   | DELETE |
| ID |   |   |   |   |   | EDIT |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | レポート |
| userID |   |   |   |   |   | 検索 |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**アップデートされたリソース**

Workfront API のこのリリースでは、次の既存のリソースがアップデートされています。 リソースに対して行われた変更は、次のように示されます。

* 追加はシンプルにリスト表示されます
* 削除された内容は打ち消し線テキストで示されます
* 変更は、表の後で注記にリストされます。

### 承認

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval `<sup>1</sup>`   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |
| projectBudgetedCost  |   |   |   |   |   |   |
| projectNetValue  |   |   |   |   |   |   |
| projectRoi  |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost  |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup> Type changed from null to boolean`

### 割り当て

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`LESS_THAN_EQUAL を追加

### BudgetedHour

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### CustomerPreferences

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| 名前 `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> possibleValues の変更

### DocMetadataLinkGroup

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### ドキュメント

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> possibleValues の変更

費用

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### グループ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> possibleValues に変更

### OpTask

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> タイプを null からブール値に変更

### PortalSection

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### ポートフォリオ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### プロジェクト

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### ProofApproval

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approverDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### レート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>バリデーター CURRENCY を追加

### タスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### チーム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> バリデーター LESS_THAN を追加

### TeamAssignment

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TeamTask

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### タイムシート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### 更新

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup> possibleValues に変更

### ユーザー

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> を possibleValues に変更

### ワーク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> タイプを null からブール値に変更

## 削除されたリソース {#removed-resources}

### ResourceBudgetedHour

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | ADD  |
| budgetedHours |   |   |   |   |   | COUNT  |
| ID |   |   |   |   |   | 削除  |
| plannedBudgetedHours |   |   |   |   |   | 編集  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | レポート  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
