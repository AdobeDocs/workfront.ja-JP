---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 8 のアップデート
description: API バージョン 8 のアップデートを参照してください。
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 68%

---

# API バージョン 8 のアップデート

## アップデートされたリソース

Adobe Workfront API のこのリリースでは、次の既存のリソースがアップデートされています。バージョン 8 で初めて使用されるリソースを表示するには、[API バージョン 8 の新機能](../../wf-api/api/new-api-version-8.md)を参照してください。リソースに対して行われた変更は、次の方法で示されます。

* 追加はシンプルにリスト表示されます
* 削除された内容は打ち消し線テキストで示されます
* 表の後にメモに変更内容が記載されます

### AccessRequest

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| アクション<sup>1</sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値の変更

### AccessRule<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>  |   |   |   |   |   |   |
| forbiddenActions<sup>2</sup> |   |   |   |   |   |   |
| secondaryActions<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 削除されたフラグ： REPORTABLE\
<sup>2</sup> 可能な値の変更

### 承認

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  | resourcePools |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更\
<sup>2</sup>追加されたフラグ：DYNAMIC、LAZY_READ、NOT_GROUPABLE

### 割り当て

|   |   |   |   | フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### 顧客

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   | getPackagingOptionValue |   |   |
| proofPlan<sup>1</sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### CustomerPreferences

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| 名前<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### DocumentApproval

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>追加されたフラグ： NOT_FILTERABLE

### DocumentVersion

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style="table-layout:auto"}

### グループ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   | 所有者 |   |   |   |   |

{style="table-layout:auto"}

### HourType

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>追加されたフラグ： NOT_FILTERABLE

### イテレーション

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style="table-layout:auto"}

### いいね!

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### メモ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### OpTask

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | イテレーション |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| 見積り |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### ポートフォリオ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### プログラム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### プロジェクト

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### ProofApproval

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approverID | 承認者 |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID<sup>1</sup> |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>追加されたフラグ： NOT_FILTERABLE

### QueueDef

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| requestorCoreAction<sup>1</sup> |   |   |   |   |   |   |
| requestorForbiddenActions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### レート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| 名前 |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### ReservedTime

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style="table-layout:auto"}

### ResourceManager

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style="table-layout:auto"}

### タスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### チーム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuss |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### テンプレート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

アップデート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### ユーザー

|   |   | フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### ワーク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更\
<sup>2</sup>追加されたフラグ：DYNAMIC、LAZY_READ、NOT_GROUPABLE
