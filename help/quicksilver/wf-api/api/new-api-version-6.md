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
source-wordcount: '495'
ht-degree: 33%

---

# API バージョン 6 の新機能

## 新しいオブジェクト

### リソース管理者

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID | 顧客 |   |   |   |   | 追加 |
| customerID | プロジェクト |   |   |   |   | カウント |
| projectID | resourceManager |   |   |   |   | 削除 |
| resourceManagerID | テンプレート |   |   |   |   | 取得 |
| templateID |   |   |   |   |   | レポート  |
|   |   |   |   |   |   | 検索  |


### Ews

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| fileName |   |   |   |   | アップロード |   |
| 取り扱い |   |   |   |   |   |   |
| objCode |   |   |   |   |   |   |


### カスタムラベル

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| ID |   |   |   | checkDelete | customLabels | 追加 |
|   |   |   |   | inUseByOtherLayoutTemplate | userCustomLabels | カウント |
|   |   |   |   | removeCustomLabel |   | 削除 |
|   |   |   |   |   |   | 取得 |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | 検索 |


## 更新されたオブジェクト

既存のオブジェクトに対する変更：追加は単にリストに表示され、削除は取り消し線が付き、既存のオブジェクトに対する変更は表の後に付加されたメモを持ちます。

### 更新

 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| updateType<sup>1</sup> |   |   |   |   | `sinceDate` |   |
|   |   |   |   |   | objectUpdatesByCommentID<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値の変更

<sup>2</sup> hasFilters 属性が true に変更されました

 

### 承認

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| completedHours |   | resourceManagers | resourceManagerIDs |   |   |   |
| constraintDate<sup>1</sup> |   |   |   |   |   |   |
| isOriginalPlannedHoursSet |   |   |   |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 追加された日付の検証

<sup>2</sup> NOT_FILTERABLE フラグが追加されました

 

### 承認プロセス

|   | フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|---|
|   |  | `attachedApprovalPaths` |   |   |   |   |   |

{style="table-layout:auto"}

 

### 承認ステップ

 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| approvalType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値の変更

 

### 承認パス<sup>1</sup>

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| approvedStatus |   |   |   |   |   | 追加 |
| approvedStatusLabel |   |   |   |   |   | カウント |
| コメント |   |   |   |   |   | 削除 |
| enteriedByID |   |   |   |   |   | 編集 |
| entryDate |   |   |   |   |   | 取得 |
| globalPathID |   |   |   |   |   | レポート |
| isPrivate |   |   |   |   |   | 検索 |
| lastUpdateDate |   |   |   |   |   |   |
| lastUpdateByID |   |   |   |   |   |   |
| 名前<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> レポート可能に変更済み

<sup>2</sup> 最大長バリデーターの追加

 

### Work Service オブジェクト

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| constraintDate<sup>1</sup> |   |   |   | getMyWorkCountFiltered |   |   |
| workRequired<sup>2</sup> |   |   |   | workItemStatusLabels  |   |   |

{style="table-layout:auto"}

<sup>1</sup> 追加された日付の検証

<sup>2</sup> Not_Filterable フラグが追加されました

 

### 割り当て

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   | assignUserToRoleOnProjects |   |   |
|   |   |   |   | swapUsersOnProjects |   |   |
|   |   |   |   | unassignUserFromProjects |   |   |

{style="table-layout:auto"}

 

### ベースライン 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable フラグが追加されました

 

### ベースライン タスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| workRequired<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> Not_Filterable フラグが追加されました

 

### 請求記録

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| billingDate<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> NO_TIME フィールドフラグを追加しました。

### バーンダウンイベント 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| eventInitiator |   |   |   |   |   | `ADD` |
|   |   |   |   |   |   | `DELETE` |

{style="table-layout:auto"}

 

### カテゴリ 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   | getCascadingRules |   |   |
|   |   |   |   | reorderCategories |   |   |

{style="table-layout:auto"}

 

カスタム列挙 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   | getGroupDefaultProjectStatus | opTaskGroupStatuss |   |
|   |   |   |   | isPossibleToUnlockStatus | projectGroupStatuses |   |
|   |   |   |   |   | taskGroupStatuses |   |

{style="table-layout:auto"}

 

ドキュメント 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `checkedOutByID` | `checkedOutBy`  |   |  isDir |   |   |   |
| `isDir`  |   |   |   |   |   |   |

{style="table-layout:auto"}

 

為替レート 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| 評価<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> PRECISION バリデータを 8 から 9 に変更しました。

 

### 統合

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| syncBurndownDate |   |   |   |   |   |   |

{style="table-layout:auto"}

 

### ジャーナル エントリ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| changeType<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値の変更

 

### 商談（問題）<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 復元可能フラグ付き

<sup>2</sup> Not_Filterable フラグが追加されました

 

### プロジェクト<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| completedHours |   | `openOpTasks` |  openOpTasks |   |   |   |
| isOriginalPlannedHoursSet |   | resourceManagers | resourceManagerIDs  |   |   |   |
| originalWorkRequired |   |   | `work` |   |   |   |
| syncBurndownDate |   |   |   |   |   |   |
| 作業 |   |   |   |   |   |   |
| workRequired |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> RESTORABLE および RESOURCE_MANABLE としてフラグ付け

<sup>2</sup> Not_Filterable フラグが追加されました

 

### タスク<sup>1</sup>

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| constraintDate<sup>2</sup> |   |   |   |   |   |   |
| workRequired<sup>3</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 復元可能フラグ付き

<sup>2</sup> AT_DATE_YEAR_BEFORE バリデーターが追加されました。

<sup>3</sup> Not_Filterable フラグが追加されました

 

### チーム

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| `myWorkViewID` |  `myWorkView` |   |   |   |   |   |
| `requestsViewID`  | `myRequestsView`  |   |   |   |   |   |

{style="table-layout:auto"}

 

### テンプレート<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   | resourceManagers | resourceManagerIDs |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> RESTORABLE および RESOURCE_MANABLE としてフラグ付け

### テンプレートタスク<sup>1</sup> 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| workRequired<sup>2</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> 復元可能フラグ付き

<sup>2</sup> Not_Filterable フラグが追加されました

 

### ユーザー

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| myInfo<sup>1</sup> |   |   |   |   |   |   |

{style="table-layout:auto"}

<sup>1</sup> MAX_LENGTH 違反者

 

### ユーザーメモ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
| eventType<sup>1</sup> |   |   |   |   | myNotifications<sup>2</sup> |   |

{style="table-layout:auto"}

<sup>1</sup> 可能な値が変更されました

<sup>2</sup> には次のフィルターが変更されました： `[true]`

 

### お知らせ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | オペレーション |
|---|---|---|---|---|---|---|
|   |   |   |   | `fileHandle` |   |   |
|   |   |   |   | `zipAnnouncementAttachments`  |   |   |
