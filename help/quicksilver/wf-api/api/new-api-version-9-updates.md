---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 9 の更新
description: 更新されたリソース
author: Becky
feature: Workfront API
role: Developer
exl-id: 51892846-d93f-4363-8416-4118fb2ef84d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 36%

---

# API バージョン 9 の更新

## 更新されたリソース

このリリースのAdobe Workfront API では、次の既存のリソースが更新されています。 バージョン 9 で初めて使用するリソースを表示するには、次を参照してください。 [API バージョン 9 の新機能](../../wf-api/api/new-api-version-9.md) および [API バージョン 9 の新機能（続き）](../../wf-api/api/new-api-version-9-continue.md). リソースに対して行われた変更は、次の方法で示されます。

* 追加は単にリストに表示されます
* 削除は取り消し線テキストで示されます
* 表の後の注記に変更が記載されます。

### AgileWork

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `opTaskID`<sup>2</sup> |  |   |  |   |   |  |
| `taskID`<sup>2</sup> |   |   |  |  |  |  |

{style="table-layout:auto"}

<sup>1</sup> 削除されたフラグ： REPORTABLE\
<sup>2</sup> 削除されたフラグ： NOT_GROUPABLE

### 承認

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   |   |   |   |

{style="table-layout:auto"}

割り当て

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| |   |  |  | `assignUserToRoleOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `assignUserToRoleOnTasks`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnProjects`<sup>1</sup> |   |   |
|   |   |   |   | `swapUsersOnTasks`<sup>1</sup> |   |   |

{style="table-layout:auto"}

<sup>1</sup> 追加されたフィールド： lockToRole

### CustomerPreferences

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `name`<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> possibleValues の変更

### 時間

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `days` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 反復

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   | `moveIssues` |   |   |

{style="table-layout:auto"}

### LayoutTemplates

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### メモ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `html` |   |   |   |   |   |   |
| `json` |   |   |   |   |   |   |
| `richTextNoteID` |   |   |   |   |   |   |

{style="table-layout:auto"}

### Opタスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `color` | `agileWork` |   |   | `convertToProject` |   |   |
| `isReady` |   |   |   | `convertToTask` |   |   |
| `storyBoardOrder` |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### ResourceBudget

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `ID` |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 削除されたフラグ： REPORTABLE

### スケジュール

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `homeGroupID` | `homeGroup` |   |   |   |   |   |

{style="table-layout:auto"}

### タスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   | `agileWork` |   |   | `convertToProject` |   |   |
|   |   |   |   | `linkExternalObject` |   |   |
|   |   |   |   | `unlinkExternalObject` |   |   |

{style="table-layout:auto"}

### チーム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `includeIssues` |   |   |   |   |   |   |

{style="table-layout:auto"}

### TimesheetProfile

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `groupID` | `group` |   |   |   |   |   |

{style="table-layout:auto"}

### UIFilter

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `filtersForObjCode` |   |

{style="table-layout:auto"}

### UIView

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   |   | `viewsForObjCode` |   |

{style="table-layout:auto"}

### ユーザー

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `logTimeInDays` |   |   |   |   |   |   |
| `workHoursPerDay` |   |   |   |   |   |   |

{style="table-layout:auto"}

### 作業

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `storyBoardOrder` | `agileWork` |   |   | `getWFHomeObjects` |   |   |
