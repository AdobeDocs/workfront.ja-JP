---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 「タスク制約の概要：できるだけ遅く」
description: できるだけ遅く（ALAP）は、タスクの完了時間をプロジェクトの終了時間にできるだけ近づける Adobe Workfront のタスク制約です。
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '368'
ht-degree: 100%

---

# タスク制約の概要：できるだけ遅く

できるだけ遅く（ALAP）は、タスクの完了時間をプロジェクトの終了時間にできるだけ近づける Adobe Workfront のタスク制約です。

この制約を使用すると、先行タスクまたは依存タスクが再スケジュールされる場合があります。

先行タスクの関係について詳しくは、[タスクの先行タスクの使用](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md)を参照してください。

プロジェクトが使用するスケジュールモードが「完了日からスケジュール」で、タスクの開始日のシステムまたはグループのデフォルトが、「プロジェクト予定日に基づく」場合、「できるだけ遅く」がデフォルトの制約になります。

新しいタスクのデフォルトの制約を設定する場所については、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

タスクでタスクの制約を更新する方法については、[タスクでタスクの制約を更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible:&nbsp;</p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click&nbsp;<strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the&nbsp;<strong>Overview</strong>&nbsp;section, expand the&nbsp;<strong>Task Constraint</strong>&nbsp;drop-down menu.</p> </li>
<li value="4"> <p>Select&nbsp;<strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.&nbsp;</li>
</ol>
</div>
-->

## 「最も遅い空き時間」と「できるだけ遅く」の違い

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

次の条件に該当する場合、「最も遅い空き時間」の制約は「できるだけ遅く」の制約とは異なります。

* プロジェクトが開始日からスケジュールされています
* プロジェクト内のタスクには、先行タスク関係があります
* 後続タスクに柔軟なタスクの制約があります

この状況では、次のようになります。

* **最も遅い空き時間：**&#x200B;先行タスクで「最も遅い空き時間」の制約を使用すると、後続タスクの柔軟な制約が優先されます。

  **例：**&#x200B;例えば、タスク A がタスク B の先行タスクであるとします。タスク A には「最も遅い空き時間」の制約が適用され、タスク B には「できるだけ早く」の制約が適用されます。この場合、タスク A はプロジェクトの開始にできるだけ近いタイミングでスケジュールされます。

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **できるだけ遅く：**&#x200B;このシナリオでは、先行タスクに「できるだけ遅く」の制約を適用すると、先行タスクが優先されます。

  **例：**&#x200B;例えば、タスク A がタスク B の先行タスクであるとします。タスク A には「できるだけ遅く」の制約が適用され、タスク B には「できるだけ早く」の制約が適用されます。この場合、タスク A はプロジェクトの終了にできるだけ近いタイミングでスケジュールされます。

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

 

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest&nbsp;Available Time constraint differs from the As Late&nbsp;As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest&nbsp;Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest&nbsp;Available Time constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close&nbsp;to the start&nbsp;of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late&nbsp;As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late&nbsp;As Possible&nbsp;constraint and Task A has the As Soon&nbsp;As Possible constraint. In this situation, the task is scheduled as close to the end&nbsp;of the project as possible.</p> </li>
</ul>
</div>
-->
