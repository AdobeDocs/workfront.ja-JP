---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 10 の新機能
description: 更新されたリソース
author: Becky
feature: Workfront API
role: Developer
exl-id: 8ac384ae-5d65-4c0e-98c1-cf38cfbff460
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 35%

---

# API バージョン 10 の新機能

* [新しいリソース](#new-resources)
* [更新されたリソース](#updated-resources)
* [削除されたリソース](#removed-resources)

## 新しいリソース {#new-resources}

### ActivityLog

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | 追加 |
|   |   |   |   |   |   | カウント |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntry

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 追加 |
|   |   |   |   |   |   | カウント  |
|   |   |   |   |   |   | 削除  |
|   |   |   |   |   |   | 編集  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | レポート  |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### CalendarEntryExternalReference

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | カウント |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | レポート  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### ExternalAuthToken

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 追加 |
|   |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 削除  |
|   |   |   |   |   |   | 編集  |
|   |   |   |   |   |   | GET  |
|   |   |   |   |   |   | レポート  |
|   |   |   |   |   |   | SEARCH  |

{style="table-layout:auto"}

### LicenseTypeGroupLimit

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
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

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| customerID | 顧客 |   |   |   |   | 追加 |
| edTime | ユーザー |   |   |   |   | カウント |
| firstDayOfWeek |   |   |   |   |   | 削除 |
| ID |   |   |   |   |   | 編集 |
| showPTO |   |   |   |   |   | GET |
| startTime |   |   |   |   |   | レポート |
| userID |   |   |   |   |   | SEARCH |
| workDate |   |   |   |   |   |   |

{style="table-layout:auto"}

**更新されたリソース**

このリリースのWorkfront API では、次の既存のリソースが更新されています。 リソースに対して行われた変更は、次のように示されます。

* 追加は単にリストに表示されます
* 削除は取り消し線テキストで示されます
* 変更は、注記の表の後にリストされます。

### 承認

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
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

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| assignmentPercent `<sup>1</sup>` |   |   |   |   |   |   |
| viewedByAssignedToUser |   |   |   |   |   |   |

{style="table-layout:auto"}

`<sup>1</sup>`LESS_THAN_EQUAL を追加しました。

### BudgetedHour

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### CustomerPreferences

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| name `<sup>1</sup>` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> possibleValues の変更

### DocMetadataLinkGroup

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   | getMetadataForDocument |   |   |

{style="table-layout:auto"}

### ドキュメント

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `masterTaskID` |  |   |   |   |   |   |

{style="table-layout:auto"}

### DocumentRequest

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

DocumentVersion

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| externalIntegrationType <sup>1</sup> |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> possibleValues の変更

費用

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### グループ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   | licenseTypeLimit |   |   | addRemoveLicenseTypeLimits  |   |   |
|   |   |   |   | setLicenseTypeLimit |   |   |

{style="table-layout:auto"}

### LinkedFolder

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| externalIntegrationType<sup>1</sup> |  |  |  |  |   |   |

{style="table-layout:auto"}

<sup>1</sup> possibleValues の変更

### Opタスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| priorityColor |   |  | pendingApproval<sup>1</sup> |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 型が null から boolean に変更されました

### PortalSection

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |  |   | groupIDs |   |   |   |

{style="table-layout:auto"}

### ポートフォリオ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| portfolioNetValue |   |   |   |  |  |   |
| portfolioRoi |   |   |   |   |   |   |

{style="table-layout:auto"}

### プロジェクト

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| projectBudgetedCost  |   |   |   | linkExternalObject  |   |   |
| projectNetValue |   |   |   | unlinkExternalObject |   |   |
| projectRoi |   |   |   |   |   |   |
| resourcePlannerBudgetedLaborCost |   |   |   |   |   |   |

{style="table-layout:auto"}

### ProofApproval

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| approverDecision |   |   |   |   |   |   |

{style="table-layout:auto"}

### レート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| rateValue <sup>1</sup> |  |  |  |  |  |   |

{style="table-layout:auto"}

<sup>1</sup>バリデーター CURRENCY を追加しました。

### タスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| kanbanFlag |   |   |   |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### チーム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| hoursPerPoint <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> LESS_THAN バリデーターを追加しました。

### TeamAssignment

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TeamTask

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `masterTaskID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### タイムシート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   |   |

{style="table-layout:auto"}

### 更新

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| updateType `<sup>1</sup>` |   |   |   |   |   | objectUpdatesWithNoteAndJournalEntryIndex  |

{style="table-layout:auto"}

<sup>1</sup> possibleValues の変更

### ユーザー

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   | accessLevel  |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| eventType <sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> possibleValues の変更

### 作業

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| kanbanFlag |  |  | pendingApproval <sup>1</sup>  |   |   |   |
| `masterTaskID` |   |   |   |   |   |   |
| priorityColor  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 型が null から boolean に変更されました

## 削除されたリソース {#removed-resources}

### ResourceBudgetedHour

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 追加  |
| budgetedHours |   |   |   |   |   | カウント  |
| ID |   |   |   |   |   | 削除  |
| plannedBudgetedHours |   |   |   |   |   | 編集  |
| projectID |   |   |   |   |   | GET  |
| roleID |   |   |   |   |   | レポート  |
| userID |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

 

 

 
