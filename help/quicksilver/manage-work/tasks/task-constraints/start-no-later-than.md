---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: タスクの制約の概要：指定日までに開始
description: 指定日までに開始（SNLT）は、指定した日付より前にタスクを開始するようにスケジュールを設定するタスクの制約です。
author: Alina
feature: Work Management
exl-id: 86139ce6-c6b1-4ac4-a5cb-fd4aa899a025
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '435'
ht-degree: 100%

---

# タスクの制約の概要：指定日までに開始

指定日までに開始（SNLT）は、指定した日付より前にタスクを開始するようにスケジュールを設定するタスクの制約です。

SNLT 制約を使用する際は、次の点に注意してください。

* プロジェクトが完了日以降にスケジュール設定されている場合は、指定日までに開始制約を使用する必要があります。この場合、タスクにソフト制約を指定してから、他の依存タスクをリスクとして強制的に表示させることができます。
* プロジェクトでスケジュールモードに完了日以降にスケジュール設定が指定されており、タスクの開始日のシステムまたはグループのデフォルトが今日である場合、指定日までに開始がデフォルトの制約になります。新しいタスクのデフォルトの制約を設定する場所については、[システム全体のタスクとイシューの環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。
* 開始日からスケジュールプロジェクトで SNLT 制約を使用すると、Adobe Workfront はできるだけ早くタスクと同様にタスクをスケジュール設定します。
* SNLT 制約のあるタスクを別のプロジェクトに移動またはコピーすると、制約の日付およびプロジェクトの開始日と完了日によって、タスクの制約またはプロジェクトの日付が変更される可能性があります。次のシナリオが存在します。

   * 宛先プロジェクトが開始からスケジュールされている場合：

      * タスクの制約の指定日がプロジェクトの予定開始日よりも前の場合、タスクの制約はできるだけ早くに変更されます。
      * タスクの制約の指定日がプロジェクトの予定完了日よりも後の場合、プロジェクトの予定完了日はタスクの完了の制約の指定日と一致するように変更されます。

      * 宛先プロジェクトが完了からスケジュールされている場合：

         * タスクの制約の指定日がプロジェクトの完了日よりも後の場合、タスクの制約はできるだけ遅くに変更されます。
         * タスクの制約の指定日がプロジェクトの予定開始日よりも前の場合、プロジェクトの予定開始日はタスクの開始の制約の指定日に一致するように変更されます。

      * プロジェクトのスケジュールに関係なく、タスクの制約の指定日がプロジェクトの開始日と完了日の範囲内にある場合、タスクの制約やプロジェクトの日付は変更されません。

  タスクの移動について詳しくは、[タスクの移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。

  タスクのコピーについて詳しくは、[タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)を参照してください。

タスクでタスクの制約を更新する方法については、[タスクでタスクの制約を更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Later Than Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Later Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>.<br></li>
</ol>
</div>
-->
