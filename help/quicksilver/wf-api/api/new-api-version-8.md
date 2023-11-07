---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 8 の新機能
description: これは、API バージョン 9 で初めて使用されるリソースのリストです。 バージョン 8 のリソースに対しておこなわれた更新のリストについては、 API バージョン 8 の更新を参照してください。
author: Becky
feature: Workfront API
role: Developer
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 26%

---

# API バージョン 8 の新機能

## 新しいリソース

これは、API バージョン 9 で初めて使用されるリソースのリストです。 バージョン 8 のリソースに対しておこなわれた更新のリストについては、 [API バージョン 8 の更新](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| backlogOrder | 顧客 |   |   | bulkCopy  |   | コピー |
| カラー | 反復  |   |   |   |   | カウント |
| customerID | lastUpdatedBy |   |   |   |   | 削除 |
| 見積 | opTask |   |   |   |   | 編集 |
| ID | プロジェクト |   |   |   |   | GET  |
| isReady | storyboardParent |   |   |   |   | レポート |
| iterationID | タスク |   |   |   |   | SEARCH |
| lastUpdateDate | チーム |   |   |   |   |   |
| lastUpdatedByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |
| opTaskID |   |   |   |   |   |   |
| parentStoryBoardOrder |   |   |   |   |   |   |
| projectID |   |   |   |   |   |   |
| storyBoardOrder |   |   |   |   |   |   |
| storyBoardParentID |   |   |   |   |   |   |
| taskID  |   |   |   |   |   |   |
| teamID |   |   |   |   |   |   |
| タイプ |   |   |   |   |   |   |
| uiObjCode |   |   |   |   |   |   |
| uiObjectID |   |   |   |   |   |   |

{style="table-layout:auto"}

### APIVersionMetadata

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | カウント  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**かんばんボード**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 追加 |
| name |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 削除 |
|   |   |   |   |   |   | 編集 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ProofApprovalStatus

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style="table-layout:auto"}

**ProofFileMetadata**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style="table-layout:auto"}

**ResourceBudgetedHour**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 追加 |
| budgetedHours |   |   |   |   |   | カウント |
| plannedBudgetedHours |   |   |   |   |   | 削除 |
| projectID |   |   |   |   |   | 編集 |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### ResourcePlannerFilter

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 追加 |
| name |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 削除 |
|   |   |   |   |   |   | 編集 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

**RichTextNote**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | カウント |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### 登録

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 購読者 | 追加 |
|   |   |   |   | removeSubscribers |   | カウント  |
|   |   |   |   | subscribes |   | 削除 |
|   |   |   |   | 配信停止 |   | GET |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style="table-layout:auto"}

### UserRole

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| roleID | 役割 |   |   |   |   |   |
| timePercentage | ユーザー |   |   |   |   |   |
| userID |   |   |   |   |   |   |
