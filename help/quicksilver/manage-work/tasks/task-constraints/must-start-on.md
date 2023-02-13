---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'タスク制約の概要：開始日'
description: タスクを特定の日付に正確に開始するようにスケジュールするには、[ 開始日 (MSO)] タスク制約を使用します。
author: Alina
feature: Work Management
exl-id: 09062d46-2b80-4758-946e-d6dec0f7a7c0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# タスク制約の概要：開始日

タスクを特定の日付に正確に開始するようにスケジュールするには、[ 開始日 (MSO)] タスク制約を使用します。

「開始日が必要」制約では、 **計画開始日** フィールドに入力します。

>[!TIP]
>
>タスクの「計画開始日」を手動で更新すると、タスクの制約が「開始日」に変更されます。

## タスク制約での Must Start On Task の概要

「Must Start On」制約を持つタスクをスケジュールする際は、次の点を考慮してください。

* 先行タスクの関係は、このタスクの再スケジュールを強制しません。 Workfrontは、基本的に、この制約を持つタスクの先行タスク関係を無視します。
* この仕事は見えない **リスク** 先行タスクが遅れたり遅れたりし始めた場合

* MSO 制約のあるタスクを別のプロジェクトに移動またはコピーすると、タスクの制約は、制約の日付と、プロジェクトの開始日と終了日に応じて変わる場合があります。 次のシナリオが存在します。

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
