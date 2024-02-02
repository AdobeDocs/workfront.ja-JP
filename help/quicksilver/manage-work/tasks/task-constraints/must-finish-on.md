---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「タスクの制約の概要：指定日に終了」
description: タスクの「指定日に終了（MFO）」制約を使用して、タスクを特定の日付に終了するようにスケジュールできます。
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '395'
ht-degree: 100%

---

# タスク制約の概要：指定日に終了

タスクの「指定日に終了（MFO）」制約を使用して、タスクを特定の日付に終了するようにスケジュールできます。

「指定日に終了」制約では、「**予定完了日**」フィールドで指定した日時に正確にタスクが終了するようにスケジュールします。

>[!TIP]
>
>タスクの「計画完了日」を手動で更新すると、タスクの制約が「指定日に終了」に変更されます。

## タスクの「指定日に終了」制約の概要

「指定日に終了」制約を持つタスクをスケジュールする場合は、次の点を考慮してください。

* 先行タスクの関係は、タスクの再スケジュールを強制しません。Adobe Workfront は基本的に、先行関係を無視します。
* 先行タスクが遅れ始めたり遅れたりした場合、タスクは「**危険あり**」と表示されます。

* MFO 制約を使用しているタスクを別のプロジェクトに移動またはコピーすると、制約の日付およびプロジェクトの開始日や完了日によって、タスクの制約またはプロジェクトの日付が変更される可能性があります。次のシナリオが存在します。

   * 宛先プロジェクトが開始からスケジュールされている場合：

      * タスクの制約の指定日がプロジェクトの予定開始日よりも前の場合、タスクの制約はできるだけ早くに変更されます。
      * タスクの制約の指定日がプロジェクトの予定完了日よりも後の場合、プロジェクトの予定完了日はタスクの完了の制約の指定日と一致するように変更されます。

      * 宛先プロジェクトが完了からスケジュールされている場合：

         * タスクの制約の指定日がプロジェクトの完了日よりも後の場合、タスクの制約はできるだけ遅くに変更されます。
         * タスクの制約の指定日がプロジェクトの予定開始日よりも前の場合、プロジェクトの予定開始日はタスクの開始の制約の指定日に一致するように変更されます。

      * プロジェクトのスケジュールに関係なく、タスクの制約の指定日がプロジェクトの開始日と完了日の範囲内にある場合、タスクの制約やプロジェクトの日付は変更されません。

  タスクの移動について詳しくは、[タスクの移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。タスクのコピーについて詳しくは、[タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)を参照してください。

タスクでタスクの制約を更新する方法については、[タスクの制約の更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Must Finish On Task Constraint</h2>
<p>To update the Task Constraint to Must Finish On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Finish On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>The task must complete by this date, and no later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
