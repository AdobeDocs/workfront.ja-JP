---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「タスク制約の概要：これよりも遅く終了しない」
description: 「これよりも遅く終了しない」（FNLT）は、指定した日付より前にタスクが完了するようにスケジュール設定するタスク制約です。
author: Alina
feature: Work Management
exl-id: ea0e74fb-45a0-4466-b57d-294a9babb340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '388'
ht-degree: 100%

---

# タスク制約の概要：これよりも遅く終了しない

「これよりも遅く終了しない」（FNLT）は、指定した日付より前にタスクが完了するようにスケジュール設定するタスク制約です。

## 「これよりも遅く終了しない」制約の概要

タスクに「これよりも遅く終了しない」（FNLT）制約を使用する場合は、次の点を考慮してください。

* プロジェクトが「開始日から」にスケジュール設定されている場合は、この制約を使用する必要があります。この場合、タスクにソフト制約を指定してから、他の依存タスクをリスクとして強制的に表示させることができます。
* FNLT 制約を使用するプロジェクトが「完了日から」にスケジュール設定されていると、この制約により、「できるだけ遅く」のタスクと同様にタスクがスケジュール設定されます。
* FNET 制約を使用しているタスクを別のプロジェクトに移動またはコピーすると、制約の日付およびプロジェクトの開始日や完了日によって、タスクの制約またはプロジェクトの日付が変更される可能性があります。次のシナリオが存在します。

   * 宛先プロジェクトが開始からスケジュールされている場合：

      * タスクの制約の指定日がプロジェクトの予定開始日よりも前の場合、タスクの制約はできるだけ早くに変更されます。
      * タスクの制約の指定日がプロジェクトの予定完了日よりも後の場合、プロジェクトの予定完了日はタスクの完了の制約の指定日と一致するように変更されます。

      * 宛先プロジェクトが完了からスケジュールされている場合：

         * タスクの制約の指定日がプロジェクトの完了日よりも後の場合、タスクの制約はできるだけ遅くに変更されます。
         * タスクの制約の指定日がプロジェクトの予定開始日よりも前の場合、プロジェクトの予定開始日はタスクの開始の制約の指定日に一致するように変更されます。

      * プロジェクトのスケジュールに関係なく、タスクの制約の指定日がプロジェクトの開始日と完了日の範囲内にある場合、タスクの制約やプロジェクトの日付は変更されません。

  タスクの移動について詳しくは、[タスクを移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。タスクのコピーについて詳しくは、[タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)を参照してください。

タスクでタスクの制約を更新する方法については、[タスクでタスクの制約を更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Finish No Later Than constraint</h2>
<p>To update the Task Constraint to Finish No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Finish No Later Than</strong>.</p> <p> <img src="assets/fnlt-350x266.png" alt="FNLT.png" style="width: 350;height: 266;"> </p> </li>
<li value="5"> <p>Specify a <strong>Planned Completion Date</strong>.</p> <p>You must complete the task on and not later than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
