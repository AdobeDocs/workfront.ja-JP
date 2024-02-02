---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「タスク制約の概要：指定日に開始」
description: タスクを特定の日付に正確に開始するようにスケジュールするには、タスクの「指定日に開始（MSO）」制約を使用します。
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '395'
ht-degree: 100%

---

# タスク制約の概要：指定日に開始日

タスクを特定の日付に正確に開始するようにスケジュールするには、タスクの「指定日に開始（MSO）」制約を使用します。

「指定日に開始」制約では、**予定開始日**&#x200B;フィールドで指定した日時ちょうどにタスクが開始するようにスケジュールします。

>[!TIP]
>
>タスクの「予定開始日」を手動で更新すると、タスクの制約が「指定日に開始」に変更されます。

## タスクの「指定日に開始」制約の概要

「指定日に開始」制約を持つタスクをスケジュールする際は、次の点を考慮してください。

* 先行タスクの関係は、このタスクの再スケジュールを強制しません。Workfront は基本的に、この制約を持つタスクの先行タスク関係を無視します。
* 先行タスクが遅れ始めたり遅れたりした場合、タスクでは&#x200B;**リスクあり**&#x200B;と表示されます 。

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
<h2>Use the Must Start On Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to Must Start On:</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Must Start On</strong>.</p> </li>
<li value="5"> <p>Specify a <strong>Planned Start Date</strong>.</p> <p>The task must start by this date, and no later than this date.</p> </li>
<li value="6">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
