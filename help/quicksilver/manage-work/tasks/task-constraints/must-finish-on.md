---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'タスク制約の概要：終了日'
description: Must Finish On (MFO) Task Constraint を使用して、タスクを特定の日付に終了するようにスケジュールできます。
author: Alina
feature: Work Management
exl-id: 9e546a0f-7f7a-4f1c-9d9d-aa3cea377fdf
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# タスク制約の概要：終了日

Must Finish On (MFO) Task Constraint を使用して、タスクを特定の日付に終了するようにスケジュールできます。

[ 終了日が必要 ] 制約では、指定した日時にタスクが完了するようにスケジュールを設定します。 **計画完了日** フィールドに入力します。

>[!TIP]
>
>タスクの「計画完了日」を手動で更新すると、タスクの制約が「完了日」に変更されます。

## タスク上の完了が必要制約の概要

Must Finish On 制約を持つタスクをスケジュールする場合は、次の点を考慮してください。

* 先行タスクの関係は、タスクの再スケジュールを強制しません。 Adobe Workfrontは基本的に、先行関係を無視します。
* このタスクは次のように表示されます **リスク** 先行タスクが遅れ始めた場合、または遅れた場合。

* MFO 制約を持つタスクを別のプロジェクトに移動またはコピーする場合、タスクの制約やプロジェクトの日付は、制約の日付と、プロジェクトの開始日と完了日に応じて変わる場合があります。 次のシナリオが存在します。

   * 宛先プロジェクトが開始からスケジュールされたとき：

      * タスクの制約日がプロジェクトの「計画開始日」よりも前の場合、タスク制約は「可能な限り早く」に変わります。
      * タスクの制約日がプロジェクトの「計画完了日」より後の場合、プロジェクトの「計画完了日」は、タスクの完了制約日に合わせて変更されます。

      * 宛先プロジェクトが「完了から」でスケジュールされる場合：

         * タスクの制約日が [ プロジェクト完了日 ] より後の場合、タスクの制約は [ 可能な限り遅く ] に変わります。
         * タスクの制約日がプロジェクトの計画開始日より前の場合、プロジェクトの計画開始日はタスクの開始日に合わせて変更されます。
      * プロジェクトのスケジュールに関係なく、タスクの制約日がプロジェクトの開始日と終了日の範囲内にある場合、タスク制約やプロジェクトの日付は変更されません。

   タスクの移動について詳しくは、 [タスクを移動](../../../manage-work/tasks/manage-tasks/move-tasks.md). タスクのコピーについて詳しくは、 [タスクのコピーと複製](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

タスクのタスク制約を更新する方法については、 [タスクのタスク制約の更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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
