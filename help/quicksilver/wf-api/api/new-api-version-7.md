---
content-type: api
navigation-topic: api-navigation-topic
title: API バージョン 7 の新機能
description: コレクション
author: John
feature: Workfront API
exl-id: 8c575251-677b-474d-84aa-02b637ef7760
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 50%

---

# API バージョン 7 の新機能

## 新しいオブジェクト

### 配達確認 Bean

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 検索 |
| deadLine |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

### DocMetadataLink

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>フィールド</th> 
   <th>参照</th> 
   <th> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">コレクション</p> <p data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;Type&quot;}">+++++++++++ </p> </th> 
   <th>検索</th> 
   <th>アクション</th> 
   <th>クエリ</th> 
   <th>操作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>追加</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>カウント </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>削除 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>取得  </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>レポート </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>検索 </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 追加 |
|   |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 削除 |
|   |   |   |   |   |   | 取得 |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | 検索 |

{style=&quot;table-layout:auto&quot;}

### ProofApproval

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 取得 |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | 検索 |

{style=&quot;table-layout:auto&quot;}

 

### ResourceContour

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | 追加 |
|   |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 削除 |
|   |   |   |   |   |   | 編集 |
|   |   |   |   |   |   | 取得 |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | 検索 |

{style=&quot;table-layout:auto&quot;}

 

### UserGroups

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| groupID | グループ |   |   |   |   |   |
| isOwner  | ユーザー  |   |   |   |   |   |
| userID  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### TimesheetProfile

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |  hourTypes |   |   |   | 追加 |
| name |   |   |   |   |   | コピー |
|   |   |   |   |   |   | カウント |
|   |   |   |   |   |   | 削除 |
|   |   |   |   |   |   | 編集 |
|   |   |   |   |   |   | 取得 |
|   |   |   |   |   |   | レポート |
|   |   |   |   |   |   | 検索 |
|   |   |   |   |   |   | 置き換え |

{style=&quot;table-layout:auto&quot;}

 

### RsrcPool

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID | 顧客 | ユーザー |   |   |   | 追加 |
| customerID  | enteredBy  |   |   |   |   | カウント |
| 説明  | lastUpdatedBy  |   |   |   |   | 削除 |
| enteriedByID  |   |   |   |   |   | 編集 |
| entryDate  |   |   |   |   |   | 取得 |
| extRefID  |   |   |   |   |   | レポート |
| lastUpdateDate |   |   |   |   |   | 検索 |
| lastUpdateByID |   |   |   |   |   |   |
| name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### DocMetadataLinkGroup

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| ID |   |   |   |   |   | カウント |
| articleName  |   |   |   |   |   | 取得 |
| pageID  |   |   |   |   |   | レポート |
| url  |   |   |   |   |   | 検索 |

{style=&quot;table-layout:auto&quot;}

 

 

 

## 更新されたオブジェクト

既存のオブジェクトに対する変更：追加は単にリストに表示され、削除は取り消し線が付き、既存の変更は表の後に付いたメモが付きます

### UpdateBean

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| updateType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹可能な値の変更 

 

### ApprovalServiceObject

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate¹ |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |    |

{style=&quot;table-layout:auto&quot;}

 

### AccessRule¹

¹レポート可能フラグ付き

 

### 承認プロセス

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   | `AttachedApprovalPaths`  |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

  

### 承認パス¹

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |   | `Add` |
|   |   |   |   |   |   | `Delete` |
|   |   |   |   |   |   | `Edit` |

{style=&quot;table-layout:auto&quot;}

¹レポート可能なフラグが削除されました

 

### Work Service オブジェクト

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹追加された日付の検証

² Not_Filterable フラグが追加されました

 

### 割り当て

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|  workPerDayList |   |   |   | assignUserToRoleOnProjects¹ |   |   |
|   |   |   |   | swapUsersOnProjects¹ |   |   |
|   |   |   |   | unassignUserFromProjects¹ |   |   |

{style=&quot;table-layout:auto&quot;}

¹フィールド includeIssues を追加しました

 

### 顧客 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| bizRuleExclusions¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹可能な値の変更 

 

### カスタム列挙 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| groupID  |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### ドキュメント 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| checkOutTimestamp |   |   |   |  createProof |   |   |

{style=&quot;table-layout:auto&quot;}

 

### DocumentVersion 

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |  getProofingTokens |   |   |

{style=&quot;table-layout:auto&quot;}

 

### グループ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| isPublic |  layoutTemplate | userGroups  |   |   |   |   |
| layoutTemplateID |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹ PRECISION バリデーターが 8 から 9 に変更されました。

 

### HourType

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   | defaultOpTaskHourType |   |
|   |   |   |   |   | defaultProjectHourType |   |
|   |   |   |   |   | defaultTaskHourType  |   |
|   |   |   |   |   | globalHourTypes  |   |
|   |   |   |   |   | objectHourTypes  |   |

{style=&quot;table-layout:auto&quot;}

 

### ジャーナル エントリ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| changeType¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹可能な値の変更

 

### 商談（問題）

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |  assignMultiple |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### プロジェクト

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   |   |   |   |
| approvalStartDate |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### QueueDef

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| allowedLegacyQueueTopicIDs |  |  |  | getQueueDefTree |   |   |

{style=&quot;table-layout:auto&quot;}

 

### QueueTopic

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |   |  queueTopicID |   |

{style=&quot;table-layout:auto&quot;}

 

### 最近使った

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|   |   |   |   |  updateLastViewedObject |   |   |

{style=&quot;table-layout:auto&quot;}

 

### タスク

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| approvalCompletionDate |   |   |   | assignMultiple  |   |   |
| approvalStartDate |   |   |   |   |   |   |
| workPerDayList |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

### TemplateTask

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| workRequired¹ |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹型が整数から倍精度浮動小数点に変更されました 

 

### ユーザー

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>フィールド</th> 
   <th>参照</th> 
   <th>コレクション</th> 
   <th>検索</th> 
   <th>アクション</th> 
   <th>クエリ</th> 
   <th>操作</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>
    <code>lastWhatsNew</code> </td> 
   <td> </td> 
   <td>
    <code>roles</code> </td> 
   <td> 役割</td> 
   <td>addMobileDevice</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;scheduleDeactivationDate&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">scheduleDeactivationDate</span></td> 
   <td> </td> 
   <td><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;timesheetProfileHourTypes&quot;}" data-sheets-userformat="{&quot;2&quot;:8707,&quot;3&quot;:{&quot;1&quot;:0},&quot;4&quot;:{&quot;1&quot;:2,&quot;2&quot;:14277081},&quot;12&quot;:0,&quot;16&quot;:10}">timesheetProfileHourTypes</span> </td> 
   <td> </td> 
   <td>getAvailableActions</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>hasAnyAccess</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>isUserTermonologyActive</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>removeMobileDevice</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>showShouldProofHQNavButton</td> 
   <td> </td> 
   <td>  </td> 
  </tr> 
 </tbody> 
</table>

### ユーザーメモ

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
| `acknowledgedmentIDs` |   |   |   |  unackknowledgeMany |   |   |
| ackDate |   |   |   |   |   |   |
| ackType |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

 

 

### CustomerPrefObject

| フィールド | 参照 | コレクション | 検索 | アクション | クエリ | 操作 |
|---|---|---|---|---|---|---|
|  name |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

¹可能な値の変更
