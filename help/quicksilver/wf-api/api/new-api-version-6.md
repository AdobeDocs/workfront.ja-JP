---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 6 の新機能
description: API バージョン 6 の新機能
author: Becky
feature: Workfront API
role: Developer
exl-id: e671a881-b8c2-4234-a3a0-76b1fbfafd32
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 100%

---

# API バージョン 6 の新機能

## 新規オブジェクト

### リソース管理者

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID | customer |   |   |   |   | 追加 |
| customerID | プロジェクト |   |   |   |   | カウント |
| projectID | resourceManager |   |   |   |   | 削除 |
| resourceManagerID | テンプレート |   |   |   |   | 取得 |
| templateID |   |   |   |   |   | レポート |
|   |   |   |   |   |   | 検索  |


### Ews

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | upload |   |
| handle |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### カスタムラベル

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | 追加 |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | カウント |
|   |   |   |   | removeCustomLabel |   | 削除 |
|   |   |   |   |   |   | 取得 |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | 検索 |


## 更新されたオブジェクト

既存のオブジェクトに対する変更：追加は単に記載され、削除には取り消し線が付いています。既存のオブジェクトに対する変更に対してはテーブルの後にメモが付加されています。

### アップデート

 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値に変更

<sup>2</sup> hasFilters 属性を true に変更

 

### 承認

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 日付の検証を追加

<sup>2</sup> NOT_FILTERABLE フラグを追加

 

### 承認プロセス

|   | フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### 承認ステップ

 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値に変更

 

### 承認パス<sup>1</sup>

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | 追加 |
| approvedStatusLabel |   |   |   |   |   | カウント |
| コメント |   |   |   |   |   | 削除 |
| enteredByID |   |   |   |   |   | 編集 |
| entryDate |   |   |   |   |   | 取得 |
| globalPathID |   |   |   |   |   | レポート |
| isPrivate |   |   |   |   |   | 検索 |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| name<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> レポート可能に変更

<sup>2</sup> 最大長バリデーターを追加

 

### Work Service オブジェクト

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> 日付の検証を追加

<sup>2</sup> Not_Filterable フラグを追加

 

### 割り当て

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### ベースライン

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable フラグを追加

 

### ベースライン タスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable フラグを追加

 

### 請求記録

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> NO_TIME フィールドフラグを追加

### バーンダウンイベント

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### カテゴリ 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

カスタム列挙 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuss |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

ドキュメント 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   | isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

為替レート 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| rate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> PRECISION バリデーターを 8 から 9 に変更

 

### 統合

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### ジャーナルエントリ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値に変更

 

### Optask (イシュー)<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> RESTORABLE としてフラグ付け

<sup>2</sup> Not_Filterable フラグを追加

 

### Project<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` | openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| ワーク |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> RESTORABLE および RESOURCE_MANABLE としてフラグ付け

<sup>2</sup> Not_Filterable フラグを追加

 

### Task<sup>1</sup>

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> RESTORABLE としてフラグ付け

<sup>2</sup> AT_DATE_YEAR_BEFORE バリデーターを追加

<sup>3</sup> Not_Filterable フラグを追加

 

### チーム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `myWorkViewID` | `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### Template<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> RESTORABLE および RESOURCE_MANAGEABLE としてフラグ付け

### Template Task<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> RESTORABLE としてフラグ付け

<sup>2</sup> Not_Filterable フラグを追加

 

### ユーザー

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH バイオレーター

 

### ユーザーメモ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値を変更

<sup>2</sup> フィルターを `[true]` に変更

 

### お知らせ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
