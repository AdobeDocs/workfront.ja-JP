---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 8 の新機能
description: これは、API バージョン 9 で初めて使用されるリソースのリストです。バージョン 8 のリソースに対して行われた更新のリストについては、API バージョン 8 の更新を参照してください。
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 100%

---

# API バージョン 8 の新機能

## 新しいリソース

これは、API バージョン 9 で初めて使用されるリソースのリストです。バージョン 8 のリソースに対して行われた更新のリストについては、[API バージョン 8 の更新](../../wf-api/api/new-api-version-8-updates.md)を参照してください。

**AgileWork**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| backlogOrder | 顧客 |   |   | bulkCopy |   | コピー |
| 色 | イテレーション |   |   |   |   | COUNT |
| customerID | lastUpdatedBy |   |   |   |   | 削除 |
| 見積り | opTask |   |   |   |   | EDIT |
| ID | プロジェクト |   |   |   |   | GET |
| isReady | storyboardParent |   |   |   |   | REPORT |
| iterationID | タスク |   |   |   |   | SEARCH |
| lastUpdateDate | チーム |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| 名前 |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| タイプ |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | COUNT |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**かんばんボード**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | EDIT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | 検索 |

{style="table-layout:auto"}

### ProofApprovalStatus

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | ADD |
| budgetedHours |   |   |   |   |   | COUNT |
| plannedBudgetedHours |   |   |   |   |   | DELETE |
| projectID |   |   |   |   |   | EDIT |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | 検索 |

{style="table-layout:auto"}

### ResourcePlannerFilter

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | ADD |
| name |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | DELETE |
|   |   |   |   |   |   | EDIT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | COUNT |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 登録

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   | addSubscribers | サブスクライバー | ADD |
|   |   |   |   | removeSubscribers |   | COUNT  |
|   |   |   |   | subscribes |   | DELETE |
|   |   |   |   | unsubscribes |   | GET |
|   |   |   |   |   |   | REPORT |
|   |   |   |   |   |   | 検索 |

{style="table-layout:auto"}

### UserRole

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| roleID | 役割 |   |   |   |   |   |
| timePercentage | ユーザー |   |   |   |   |   |
| userID |   |   |   |   |   |   |
