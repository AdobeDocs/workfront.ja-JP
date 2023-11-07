---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 8 の更新
description: このリリースのAdobe Workfront API では、次の既存のリソースが更新されています。 バージョン 8 で初めて使用されるリソースを確認するには、 API バージョン 8 の新機能を参照してください。 リソースに対して行われた変更は、次の方法で示されます — EDIT ME.
author: Becky
feature: Workfront API
role: Developer
exl-id: c6d7d2d2-cd21-4ca8-a5a0-afe3669dc959
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 26%

---

# API バージョン 8 の更新

## 更新されたリソース

このリリースのAdobe Workfront API では、次の既存のリソースが更新されています。 バージョン 8 で初めて使用されるリソースを表示するには、 [API バージョン 8 の新機能](../../wf-api/api/new-api-version-8.md). リソースに対して行われた変更は、次の方法で示されます。

* 追加は単にリストに表示されます
* 削除は取り消し線テキストで示されます
* 表の後の注記に変更が記載されます。

### AccessRequest

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| アクション<sup>1</sup>  |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値の変更

### AccessRule<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| coreAction<sup>2</sup>  |   |   |   |   |   |   |
| forbiddenActions<sup>2</sup> |   |   |   |   |   |   |
| secondaryActions<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 削除されたフラグ： REPORTABLE\
<sup>2</sup> 可能な値の変更

### 承認

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  | resourcePools |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更\
<sup>2</sup>追加されたフラグ：DYNAMIC、LAZY_READ、NOT_GROUPABLE

### 割り当て

|   |   |   |   | フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnTasks | getAssignAssignmentsForTasks  |   |   |   |   |   |
|   |   |   |   | swapUsersOnTasks | getUnassignAssignmentsForTasks |   |   |   |   |   |
|   |   |   |   | unassignUserFromTasks |   |   |   |   |   |   |

{style="table-layout:auto"}

### 顧客

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| bizRuleExclusions<sup>1</sup> |   |   |   | getPackagingOptionValue |   |   |
| proofPlan<sup>1</sup> |   |   |   | isPackagingOptionEnabled |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### CustomerPreferences

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| 名前<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### DocumentApproval

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>追加されたフラグ： NOT_FILTERABLE

### DocumentVersion

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| activeProofStages |   |   |   |   |   |   |

{style="table-layout:auto"}

### グループ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   | 所有者 |   |   |   |   |

{style="table-layout:auto"}

### HourType

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| appGlobalID<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>追加されたフラグ： NOT_FILTERABLE

### 反復

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   | moveStories |   |   |

{style="table-layout:auto"}

### いいね!

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |

{style="table-layout:auto"}

### メモ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### Opタスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | defaultShownTimesheetIssues  |   |
| backlogOrder | 反復 |   |   |   |   |   |
| backlogParent |   |   |   |   |   |   |
| 見積 |   |   |   |   |   |   |
| iterationID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### ポートフォリオ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### プログラム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### プロジェクト

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   | resourcePools |   |   | defaultShownTimesheetProjects |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### ProofApproval

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| approverID | 承認者 |   |   |   |   |   |
| documentVersionID | documentVersion |   |   |   |   |   |
| ID<sup>1</sup> |   |   |   |   |   |   |
| proofCreationDate |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>追加されたフラグ： NOT_FILTERABLE

### QueueDef

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| requestorCoreAction<sup>1</sup> |   |   |   |   |   |   |
| requestorForbiddenActions<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### レート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| endDate |   |   |   | setRatesForRole  |   |   |
| name |   |   |   |   |   |   |
| startDate |   |   |   |   |   |   |

{style="table-layout:auto"}

### ReservedTime

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| extRefID |   |   |   |   |   |   |

{style="table-layout:auto"}

### ResourceManager

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| projectPriority |   |   |   |   |   |   |

{style="table-layout:auto"}

### タスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   | allTasksOnIterations  |   |
| backlogParent | kanbanBoard |   |   |   | defaultShownTimesheetTasks |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### チーム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| agileMethodology |   |   |   |   |   |   |
| autoAddNextStory |   |   |   |   |   |   |
| includeIssues |   |   |   |   |   |   |
| teamStoryBoardIssueStatuss |   |   |   |   |   |   |
| wipLimit |   |   |   |   |   |   |

{style="table-layout:auto"}

### テンプレート

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |

{style="table-layout:auto"}

### TemplateTask

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

更新

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> | `updateEndorsement` |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### ユーザー

|   |   | フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|---|---|
|   |   | resourcePools |   |   |   |   |   |   |
|   |   | userGroups |   |   |   |   |   |   |
|   |   | userRoles |   |   |   |   |   |   |

{style="table-layout:auto"}

### UserNote

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `endorsementID` | `endorsement` |   |   |   |   |   |
| `endorsementShareID` | `endorsementShare` |   |   |   |   |   |
| eventType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更

### 作業

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| auditTypes<sup>1</sup> | agileWork  |   |   |   |   |   |
| backlogOrder<sup>2</sup> | kanbanBoard  |   |   |   |   |   |
| backlogParent  |   |   |   |   |   |   |
| kanbanBoardID |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup>可能な値の変更\
<sup>2</sup>追加されたフラグ：DYNAMIC、LAZY_READ、NOT_GROUPABLE
