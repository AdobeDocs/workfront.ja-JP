---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: '''タスク制約の概要：できるだけ早く`'
description: '[ 可能な限り早く ] は、タスクの開始時刻をプロジェクトの開始時刻にできるだけ近い位置に配置するタスクの制約です。'
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# タスク制約の概要：できるだけ早く

[ 可能な限り早く ] は、タスクの開始時刻をプロジェクトの開始時刻にできるだけ近い位置に配置するタスクの制約です。

## As As As A Possible 制約の使用に関する考慮事項

* プロジェクトで「開始日からスケジュール」の「スケジュール・モード」を使用し、新規タスクのシステムのデフォルト開始日が「プロジェクト計画日に基づく」に設定されている場合は、「可能な限り早く」がデフォルトの制約です。

* プロジェクトで [ 開始日からのスケジュール ] のスケジュールモードを使用し、新しいタスクの既定の開始日が [ 今日 ] に設定されている場合、既定の [ タスクの制約 ] は [ 次よりも前に開始 ] に設定されます。

   新しいタスクの既定の制約を設定する場所については、を参照してください。 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

タスクのタスク制約を更新する方法については、 [タスクのタスク制約の更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Soon As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Soon As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 可能な限り早い時間と可能な限り早い時間の違い

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

最も早い利用可能な時間制約は、次の条件がすべて存在する場合、「可能な限り早く」制約とは異なります。

* プロジェクトは「完了からスケジュール」に設定されます。
* プロジェクト内のタスクには、先行タスク関係があります。
* 先行タスクには、柔軟なタスク制約があります。

この場合：

* **最も早い利用可能時間：** 後続タスクに対して [ 最も早い時間 ] 制約を使用すると、先行タスクの柔軟な制約が優先されます。

   たとえば、タスク A がタスク B の先行タスクであるとします。タスク B には最も早い使用可能時間制約が適用され、タスク A には [ 可能な限り遅く ] 制約が適用されます。 この場合、タスクは、可能な限りプロジェクトの完了に近い状態でスケジュールされます。

* **できるだけ早く：** このシナリオでは、後続タスクに対して As As As Possible 制約を使用すると、後続タスクが優先されます。

   たとえば、タスク A がタスク B の先行タスクであるとします。タスク B には [ 可能な限り早く ] 制約が、タスク A には [ 可能な限り遅く ] 制約が設定されています。 この場合、タスクは可能な限りプロジェクトの開始に近い状態にスケジュールされます。
