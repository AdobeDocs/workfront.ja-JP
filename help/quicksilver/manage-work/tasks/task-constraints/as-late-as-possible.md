---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: タスク制約の概要：できるだけ遅く
description: できるだけ遅く（ALAP）は、タスクの完了時間をプロジェクトの終了時間にできるだけ近づける Adobe Workfront のタスク制約です。
author: Alina
feature: Work Management
exl-id: 475427d0-020b-4851-a614-c9931659e07d
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 77%

---

# タスク制約の概要：できるだけ遅く

できるだけ遅く（ALAP）は、タスクの完了時間をプロジェクトの終了時間にできるだけ近づける Adobe Workfront のタスク制約です。

この制約を使用すると、先行タスクまたは依存タスクのスケジュールが変更される可能性があります。

先行タスク関係の詳細については、「[ タスク先行タスクの使用：記事のインデックス ](../../../manage-work/tasks/use-prdcssrs/use-task-predecessors.md)」を参照してください。

プロジェクトで「完了日から」のスケジュール・モードを使用し、タスクの開始日のデフォルトがプロジェクトの予定日に基づいている場合、デフォルト制約は「可能な限り遅く」です。

新しいタスクのデフォルトの制約を設定する場所については、[システム全体のタスクとイシューの環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

タスクでタスクの制約を更新する方法については、[タスクでタスクの制約を更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the As Late As Possible Task Constraint</h2>
<p>(NOTE: replaced with new article linked above) </p>
<p>To update the Task Constraint to As Late As Possible: </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3"> <p>In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p> </li>
<li value="4"> <p>Select <strong>As Late As Possible</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## 「最も遅い空き時間」と「できるだけ遅く」の違い

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Latest Available Time"] - inserted a snippet for both articles (Alina)) </p>
-->

次の条件に該当する場合、「最も遅い空き時間」の制約は「できるだけ遅く」の制約とは異なります。

* プロジェクトが開始日からスケジュールされています
* プロジェクト内のタスクには、先行タスク関係があります
* 後続タスクに柔軟なタスクの制約があります

この状況では、次のようになります。

* **最も遅い空き時間：**&#x200B;先行タスクで「最も遅い空き時間」の制約を使用すると、後続タスクの柔軟な制約が優先されます。

  **例：**&#x200B;例えば、タスク A がタスク B の先行タスクであるとします。タスク A には「最も遅い空き時間」の制約が適用され、タスク B には「できるだけ早く」の制約が適用されます。この場合、タスク A はプロジェクトの開始にできるだけ近いタイミングでスケジュールされます。

  ![ 利用可能な最新の時間タスク制約 ](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **できるだけ遅く：**&#x200B;このシナリオでは、先行タスクに「できるだけ遅く」の制約を適用すると、先行タスクが優先されます。

  **例：**&#x200B;例えば、タスク A がタスク B の先行タスクであるとします。タスク A には「できるだけ遅く」の制約が適用され、タスク B には「できるだけ早く」の制約が適用されます。この場合、タスク A はプロジェクトの終了にできるだけ近いタイミングでスケジュールされます。

  ![ タスクリスト内の「可能な限り遅く」タスク制約 ](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)



<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: this content was here before but it was wrong - according to this issue in Hub, per Dev, the correct functionality is in the snippet above: https://hub.workfront.com/task/6193c6910004bce9de07cda7757f3ce8/updates?email-source=subscribedCommunication) </p>
<p>The Latest Available Time constraint differs from the As Late As Possible constraint when the following criteria exist:</p>
<ul>
<li> The project is scheduled From Completion </li>
<li> Tasks in the project have a predecessor relationship </li>
<li> The predecessor task has a flexible task constraint </li>
</ul>
<p> In this situation: </p>
<ul>
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, the task is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
