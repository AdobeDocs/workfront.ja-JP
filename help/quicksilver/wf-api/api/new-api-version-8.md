---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 8 の新機能
description: これは、API バージョン 9 で初めて使用されるリソースのリストです。 バージョン 8 のリソースに対しておこなわれた更新のリストについては、 API バージョン 8 の更新を参照してください。
author: Becky
feature: Workfront API
exl-id: 90fefaa6-d387-4cdb-8aea-9a939fe2ac26
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 32%

---

# API バージョン 8 の新機能

## 新しいリソース

これは、API バージョン 9 で初めて使用されるリソースのリストです。 バージョン 8 のリソースに対しておこなわれた更新のリストについては、 [API バージョン 8 の更新](../../wf-api/api/new-api-version-8-updates.md)

**AgileWork**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| backlogOrder | 顧客 |   |   | bulkCopy  |   | コピー |
| カラー | 反復  |   |   |   |   | カウント |
| customerID | lastUpdatedBy |   |   |   |   | 削除 |
| 見積もり | opTask |   |   |   |   | 編集 |
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

{style=&quot;table-layout:auto&quot;}

### APIVersionMetadata

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| deprecationRelease |   |   |   |   |   | カウント  |
| removalRelease |   |   |   |   |   | GET |
| versionName |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**かんばんボード**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 追加 |
| name |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 削除 |
|   |   |   |   |   |   | 編集 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ProofApprovalStatus

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   |   |
| proofApprovalStatusID |   |   |   |   |   |   |
| proofApprovalStatusLabel |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ProofFileMetadata**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| documentVersionID | documentVersion |   |   |   |   |   |
| fileIndex |   |   |   |   |   |   |
| fileName |   |   |   |   |   |   |
| ID |   |   |   |   |   |   |
| isURL |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

**ResourceBudgetedHour**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| allocationDate |   |   |   |   |   | 追加 |
| budgetedHours |   |   |   |   |   | カウント |
| plannedBudgetedHours |   |   |   |   |   | 削除 |
| projectID |   |   |   |   |   | 編集 |
| roleID |   |   |   |   |   | GET |
| userID |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### ResourcePlannerFilter

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 追加 |
| name |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 削除 |
|   |   |   |   |   |   | 編集 |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

**RichTextNote**

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | カウント |
|   |   |   |   |   |   | GET |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### 登録

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|  ID |   |   |   | addSubscribers | 購読者 | 追加 |
|   |   |   |   | removeSubscribers |   | カウント  |
|   |   |   |   | subscribes |   | 削除 |
|   |   |   |   | 配信停止 |   | GET |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | SEARCH |

{style=&quot;table-layout:auto&quot;}

### UserRole

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| roleID | 役割 |   |   |   |   |   |
| timePercentage | ユーザー |   |   |   |   |   |
| userID |   |   |   |   |   |   |
