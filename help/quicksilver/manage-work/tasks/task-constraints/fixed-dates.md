---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「タスク制約の概要：固定日付」
description: タスクの正確な開始日と終了日を指定する場合は、固定日付のタスク制約を使用できます。タスク制約について詳しくは、「タスク制約の概要」を参照してください。
author: Alina
feature: Work Management
exl-id: 084f54a6-e757-405c-b388-5d5f61608e71
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '437'
ht-degree: 100%

---

# タスク制約の概要：固定日付

タスクの正確な開始日と終了日を指定する場合は、固定日付のタスク制約を使用できます。タスク制約について詳しくは、[タスク制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)を参照してください。

## 固定日付の制約の概要

固定日付の制約を使用する際は、次の点に注意してください。

* 固定日付（FIXT）タスク制約を選択する場合は、タスクの「予定開始日」と「予定完了日」を指定する必要があります。この場合、タスクの先行タスク関係は無視されます。
* FIXT 制約を使用する場合、タスクの「期間」フィールドは編集できません。期間は、タスクの予定開始日と予定完了日の差として計算されます。
* タスクの「期間タイプ」が「残存作業時間の優先」の場合は、タスクの担当者の数もタスクの期間に影響を与えます。
* FIXT 制約のあるタスクを別のプロジェクトに移動またはコピーすると、タスクの制約やプロジェクトの日付は、制約の日付と、プロジェクトの開始日と完了日に応じて変わる場合があります。次のシナリオが存在します。

   * 宛先プロジェクトが開始からスケジュールされている場合：

      * タスクの制約日のいずれかがプロジェクトの開始日よりも前の場合、タスクの制約は「できるだけ早く」に変わります。
      * タスクの制約日のいずれかまたは両方が、プロジェクトの予定完了日より後の場合、プロジェクトの予定完了日は、タスクの完了の制約日に合わせて変更されます。

   * 宛先プロジェクトが完了からスケジュールされている場合：

      * タスクの制約日がいずれかがプロジェクト完了日より後の場合、タスク制約は「できるだけ遅く」に変わります。
      * タスクの制約日のいずれかまたは両方が、プロジェクトの予定開始日よりも前の場合、プロジェクトの予定開始日は、タスクの開始の制約日に合わせて変更されます。

   * プロジェクトのスケジュールに関係なく、タスクの制約日がプロジェクトの開始日と完了日の範囲内にある場合、タスク制約やプロジェクトの日付は変更されません。

  タスクの移動について詳しくは、[タスクの移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。タスクのコピーについて詳しくは、[タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)を参照してください。

タスクでタスクの制約を更新する方法については、[タスクでタスクの制約を更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Fixed Dates Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above) </p>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Fixed Dates</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start on this date. </p> </li>
<li value="6"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete on this date. </p> </li>
<li value="7">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
