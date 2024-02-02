---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「タスクの制約の概要：できるだけ早く」
description: 「できるだけ早く」は、タスクの開始時間をプロジェクトの開始時間にできるだけ近づけるタスクの制約です。
author: Alina
feature: Work Management
exl-id: 9cb232fe-bc74-4433-afac-88be69514c88
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '391'
ht-degree: 100%

---

# タスクの制約の概要：できるだけ早く

「できるだけ早く」は、タスクの開始時間をプロジェクトの開始時間にできるだけ近づけるタスクの制約です。

## 「できるだけ早く」の制約を使用する場合の考慮事項

* プロジェクトで「開始日からスケジュール」のスケジュールモードを使用し、新規タスクのシステムのデフォルト開始日が「プロジェクトの予定日に基づく」に設定されている場合、「できるだけ早く」がデフォルトの制約になります。

* プロジェクトで「開始日からスケジュール」のスケジュールモードを使用し、新規タスクのシステムまたはグループのデフォルトの開始日が「今日」に設定されている場合、デフォルトのタスクの制約は「開始日以降」になります。

  新しいタスクのデフォルトの制約を設定する場所については、[システム全体のタスクとイシューの環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

タスクの制約を更新する方法について詳しくは、[タスクの制約の更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

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

## 最も早い空き時間とできるだけ早くの違い

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])&nbsp;</p>
-->

「最も早い空き時間」の制約は、次の条件がすべて存在する場合、「できるだけ早く」の制約とは異なります。

* プロジェクトは完了からスケジュールされます。
* プロジェクト内のタスクには、先行タスク関係があります。
* 先行タスクには、柔軟なタスクの制約があります。

この状況では、次のようになります。

* **最も早い空き時間：**&#x200B;後続タスクに「最も早い空き時間」の制約を使用すると、先行タスクの柔軟な制約が優先されます。

  例えば、タスク A がタスク B の先行タスクであるとします。タスク B には「最も早い空き時間」の制約が適用され、タスク A には「できるだけ遅く」の制約が適用されます。この場合、タスクはプロジェクトの完了にできるだけ近い状態でスケジュールされます。

* **できるだけ早く：**&#x200B;このシナリオでは、後続タスクに「できるだけ早く」の制約を使用すると、後続タスクが優先されます。

  例えば、タスク A がタスク B の先行タスクであるとします。タスク B には「できるだけ早く」の制約が適用され、タスク A には「できるだけ遅く」の制約が適用されます。この場合、タスクはプロジェクトの開始にできるだけ近い状態でスケジュールされます。
