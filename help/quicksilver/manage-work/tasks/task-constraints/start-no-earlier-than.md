---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「タスク制約の概要：指定日以後に開始」
description: 指定した日付以降にタスクを開始するようにスケジュールするには、「指定日以後に開始」（SNET）タスク制約を使用します。
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '491'
ht-degree: 100%

---

# タスク制約の概要：指定日以後に開始

指定した日付以降にタスクを開始するようにスケジュールするには、「指定日以後に開始」（SNET）タスク制約を使用します。

## 「指定日以後に開始」タスク制約の概要

「指定日以後に開始」タスク制約を使用する際は、以下の点を考慮してください。

* プロジェクトが「開始日」からスケジュール設定されている場合は、「指定日以後に開始」制約を使用する必要があります。この場合、タスクにソフト制約を指定してから、他の依存タスクをリスクとして強制的に表示させることができます。
* 「指定日以後に開始」は、プロジェクトのスケジュールが「開始日」からで、新規タスクのシステムまたはグループのデフォルトの開始日が「今日」に設定されている場合の、デフォルトの制約です。タスクのデフォルトの設定について詳しくは、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

* プロジェクトのスケジュールを「開始日」から設定し、新規タスクのシステムのデフォルトの開始日を「プロジェクト予定日に基づく」に設定した場合、新規タスクのデフォルトの制約は「できるだけ早く」になります。
* プロジェクトのスケジュールを「完了日から」に設定し、新規タスクのシステムのデフォルトの開始日を「今日」に設定した場合、「指定日以後に開始」制約によってそのタスクのスケジュールは「できるだけ早く」と同様の設定になります。
* SNET 制約のあるタスクを別のプロジェクトに移動またはコピーすると、タスクの制約やプロジェクトの日付は、制約の日付、およびプロジェクトの開始日と完了日の設定に応じて変更する場合があります。次のシナリオが存在します。

   * 宛先プロジェクトが開始からスケジュールされている場合：

      * タスクの制約の指定日がプロジェクトの予定開始日よりも前の場合、タスクの制約はできるだけ早くに変更されます。
      * タスクの制約の指定日がプロジェクトの予定完了日よりも後の場合、プロジェクトの予定完了日はタスクの完了の制約の指定日と一致するように変更されます。

      * 宛先プロジェクトが完了からスケジュールされている場合：

         * タスクの制約の指定日がプロジェクトの完了日よりも後の場合、タスクの制約はできるだけ遅くに変更されます。
         * タスクの制約の指定日がプロジェクトの予定開始日よりも前の場合、プロジェクトの予定開始日はタスクの開始の制約の指定日に一致するように変更されます。

      * プロジェクトのスケジュールに関係なく、タスクの制約の指定日がプロジェクトの開始日と完了日の範囲内にある場合、タスクの制約やプロジェクトの日付は変更されません。

  タスクの移動について詳しくは、[タスクの移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。タスクのコピーについて詳しくは、[タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)を参照してください。

タスクでタスクの制約を更新する方法については、[タスクでタスクの制約を更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the Start No Earlier Than Task Constraint</h2>
<p>(NOTE:&nbsp;replaced with new article linked above)&nbsp;</p>
<p>To update the Task Constraint to Start No Later Than:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Start No Earlier Than</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>This is the date by which the task must start, and not earlier than this date. </p> </li>
<li value="6">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->
