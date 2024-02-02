---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 「期間タイプの概要：予定作業」
description: 予定作業は、Adobe Workfront のタスクに設定できる期間タイプです。Workfront の期間タイプに関する一般情報については、タスク期間の概要と期間タイプを参照してください。
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '541'
ht-degree: 100%

---

# 期間タイプの概要：予定作業

予定作業は、Adobe Workfront のタスクに設定できる期間タイプです。Workfront の期間タイプに関する一般情報については、[タスク期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

## 予定作業の期間タイプの概要

予定作業は、タスクを完了するのに必要な作業量（予定時間数）を決定します。タスクに割り当てられたリソースがタスクの期間全体に割り当てられる場合は、予定作業の期間タイプを使用することをお勧めします。

Workfront またはグループ管理者は、システムまたはグループのデフォルトの期間タイプを予定作業に設定できます。この場合、すべての新しいタスクは、この期間タイプで作成されます。システムレベルまたはグループレベルのプロジェクト環境設定の一部として、タスクやイシューの環境設定を変更する方法については、[システム全体のタスクとイシュー環境を設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

リソースがタスクに追加されると、プロジェクトマネージャーは予定作業量の増加を確認することができます。例えば、1 時間の定例会議に 3 人のリソースが参加する場合は合計 3 時間、10 人のリソースが参加する場合には合計 10 時間の作業が必要です。この場合、各リソースに 100％の割り当てでタスクが割り当てられていると想定します。

## 予定作業の期間タイプを使用する場合に必要な作業時間を計算する数式をレビュー

タスクで予定作業の期間タイプを使用すると、Workfront は次の 2 つの数式を使用して各タスクの作業時間を計算します。数式は、各リソースがタスクに割り当てられる時間の割合と、各タスクに割り当てられたリソース数に応じて異なります。

* 簡易式：タスクに 1 つのリソースが割り当てられ、使用可能な時間の 100％のタスクに割り当てられている場合、各タスクの所要作業時間の値は次の数式で計算されます。

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* 複雑な数式：各リソースに様々な割り当てを割り当てる場合、その数式では、これらの割り当てが考慮され、次のバリエーションを構成します。

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## タスクにリソースを追加または削除した場合の影響をレビュー

予定作業の期間タイプでタスクを割り当てられた担当者を追加または削除する場合は、期間を手動で編集できます。担当者がタスクに追加または削除されると、予定時間数が変更されます。

次の例では、設定のプロジェクト環境設定で勤務 1 日あたりの標準的な時間数が 8 に設定されています。各タスクの期間は 1 日です。担当者数が変わると、予定時間数は特定のタスクの担当者数に応じて変わります。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>担当者数（100％ずつ割り当て）</strong> </p> </th> 
   <th> <p><strong>期間</strong> </p> </th> 
   <th> <p><strong>予定時間数</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 日</p> </td> 
   <td> <p>8 時間</p> <p>（1 日 x 8 時間（就業日当たり）x 1 担当者 = 8 予定時間数）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 日</p> </td> 
   <td> <p>16 時間</p> <p>（1 日 x 8 時間（就業日当たり） x 2 担当者 = 16 予定時間数）</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 日</p> </td> 
   <td> <p>24 時間</p> <p>（1 日 x 8 時間（就業日当たり）x 3 担当者 = 24 予定時間数）</p> </td> 
  </tr> 
 </tbody> 
</table>

この場合、各担当者は予定作業タスクを 100％割り当てられます。

![](assets/calcwork-350x71.png)

## タスクの期間タイプを予定作業に変更

タスクの期間タイプの変更について詳しくは、[タスクの期間タイプを更新](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)を参照してください。

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
