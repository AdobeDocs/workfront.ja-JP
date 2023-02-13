---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '期間タイプの概要：計算済み作業'
description: 計算作業時間は、Adobe Workfrontのタスクに設定できる期間タイプです。 Workfrontの期間のタイプに関する一般情報については、タスク期間の概要および期間のタイプを参照してください。
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# 期間タイプの概要：計算作業時間

計算作業時間は、Adobe Workfrontのタスクに設定できる期間タイプです。 Workfrontの期間のタイプに関する一般情報については、 [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 計算された作業時間タイプの概要

計算作業時間は、タスクを完了するのに必要な作業量（計画時間）を決定します。 タスクに割り当てられたリソースがタスクの期間全体に割り当てられる場合は、「計算された作業時間の期間タイプ」を使用することをお勧めします。

Workfrontまたはグループ管理者は、システムまたはグループのデフォルトの「期間タイプ」を「計算作業」に設定できます。 この場合、すべての新しいタスクは、この期間タイプで作成されます。 システムレベルまたはグループレベルのプロジェクト環境設定の一部として、タスクや問題の環境設定を変更する方法については、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

リソースがタスクに追加されると、プロジェクトマネージャは計画作業量の増加を見ることができます。 例えば、3 つのリソースを含む 1 時間計画会議は合計 3 時間の作業が必要で、10 リソースを含む 1 時間計画会議は 10 時間の作業が必要です。 この場合、各リソースが 100%の割り当てを持つタスクに割り当てられていると想定します。

## 計算された作業時間タイプを使用する場合に必要な作業時間を計算する数式を確認します

タスクで [ 計算された作業時間の期間の種類 ] を使用すると、Workfrontは次の 2 つの数式を使用して各タスクの作業時間を計算します。 式は、各リソースがタスクに割り当てられる割合と、各タスクに割り当てられたリソース数に応じて異なります。

* 簡易式：タスクに 1 つのリソースが割り当てられ、使用可能な時間の 100%にタスクに割り当てられている場合、各タスクの [ 作業時間 ] の値は次の式で計算されます。

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* 複雑な数式：各リソースに様々な割当てを割り当てる場合、式では、これらの割当てが考慮され、次のバリエーションが考慮されます。

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## タスクに対するリソースの追加または削除の効果のレビュー

「計算された作業時間」の期間タイプでタスクに割り当て先を追加または削除する場合は、「期間」を手動で編集できます。 担当者がタスクに追加または削除されると、予定時間が変更されます。

次の例では、セットアップのプロジェクト環境設定で「Typical Hours per Work Day」が 8 に設定されています。 各タスクの期間は 1 日です。 担当者の数が変わると、「予定時間」は、特定のタスクの担当者数に応じて変わります。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>担当者数（100%ずつ割り当て）</strong> </p> </th> 
   <th> <p><strong>期間</strong> </p> </th> 
   <th> <p><strong>予定時間数</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 日</p> </td> 
   <td> <p>8 時間</p> <p>（1 日 x 8 時間/就業日 x 1 担当者= 8 時間予定）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 日</p> </td> 
   <td> <p>16 時間</p> <p>（1 日 x 8 時間/稼働日 x 2 担当者= 16 時間予定時間）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 日</p> </td> 
   <td> <p>24 時間</p> <p>（1 日 x 8 時間/稼働日 x 3 担当者= 24 時間計画）</p> </td> 
  </tr> 
 </tbody> 
</table>

この場合、各担当者は計算作業時間タスクに 100%割り当てられます。

![](assets/calcwork-350x71.png)

## タスクの期間の種類を計算作業時間に変更する

タスクの期間の種類の変更について詳しくは、 [タスクの期間タイプの更新](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
