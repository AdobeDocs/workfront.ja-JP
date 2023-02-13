---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''タスク制約の概要：次より前に開始'
description: タスクを指定した日付以降に開始するようにスケジュールするには、Start No Exare Than (SNET) Task Constraint を使用します。
author: Alina
feature: Work Management
exl-id: 857859fb-87ee-4397-b292-239ed9dc8281
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# タスク制約の概要：次の日までに開始

タスクを指定した日付以降に開始するようにスケジュールするには、Start No Exare Than (SNET) Task Constraint を使用します。

## タスク制約の「開始」の概要

Start No Exer Than Task 制約を使用する際は、次の点に注意してください。

* プロジェクトが「開始日から」にスケジュールされている場合は、「次の日までに開始」制約を使用する必要があります。 この場合、タスクにソフト制約を指定してから、他の依存タスクを [ リスク ] として強制的に表示させることができます。
* プロジェクトが「開始日から」で、新しいタスクのシステムまたはグループのデフォルトの開始日が「今日」に設定されている場合の、既定の制約は「開始日から」です。 タスクのデフォルトの設定については、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* プロジェクトのスケジュールを「開始日から」に設定し、新しいタスクのシステムのデフォルトの開始日を「プロジェクト予定日に基づく」に設定した場合、新しいタスクのデフォルトの制約は「可能な限り早く」になります。
* [ 完了日から ] プロジェクトをスケジュールし、新しいタスクの既定の開始日が [ 今日 ] に設定されている場合、[ 次の日までに開始 ] 制約では、[ 可能な限り遅く ] タスクと同じようにタスクがスケジュールされます。
* SNET 制約のあるタスクを別のプロジェクトに移動またはコピーすると、タスクの制約やプロジェクトの日付は、制約の日付と、プロジェクトの開始日と完了日に応じて変わる場合があります。 次のシナリオが存在します。

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
