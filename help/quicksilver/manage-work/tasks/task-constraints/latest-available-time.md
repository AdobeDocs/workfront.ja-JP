---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: タスク制約の概要：最新の使用可能な時間
description: 最も遅い空き時間（LAT）は、Adobe Workfront のタスクの制約の一種です。
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
TQID: https://experienceleague.adobe.com/o896UT7C1VcKJzu-8tzqjZfnq838zQfpWxxTndSz3YQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 352
ht-degree: 93%

---

# タスク制約の概要：最も遅い空き時間

最も遅い空き時間（LAT）は、Adobe Workfront のタスクの制約の一種です。

## タスクの制約「最も遅い空き時間」を使用

LAT 制約を使用すると、プロジェクト内の先行タスクと後続タスクの関係を考慮した後で、最も遅い空き時間にタスクを開始するようにスケジュール設定できます。

この制約は、先行タスクや後続タスクの再スケジュールを強制しない点で、「できるだけ早く」の制約とは異なります。 関連付けられているタスクのスケジュールにのみ影響し、他のタスクとの関係に基づいて、最も遅い空き時間に設定されます。

タスクでタスクの制約を更新する方法については、[タスクでタスクの制約を更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To update the Task Constraint to Latest Available Time:</p>
<p>(NOTE: replaced with new article linked above) </p>
<ol>
<li value="1">Go to a task whose Task Constraint you want to update.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> </li>
<li value="3">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</li>
<li value="4"> <p>Select <strong>Latest Available Time</strong>.</p> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## 「最も遅い空き時間」と「できるだけ遅く」の違い

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

次の条件に該当する場合、「最も遅い空き時間」の制約は「できるだけ遅く」の制約とは異なります。

* プロジェクトが開始日からスケジュールされています
* プロジェクト内のタスクには、先行タスク関係があります
* 後続タスクに柔軟なタスクの制約があります

この状況では、次のようになります。

* **最も遅い空き時間：**&#x200B;先行タスクで「最も遅い空き時間」の制約を使用すると、後続タスクの柔軟な制約が優先されます。

  **例：**&#x200B;例えば、タスク A がタスク B の先行タスクであるとします。タスク A には「最も遅い空き時間」の制約が適用され、タスク B には「できるだけ早く」の制約が適用されます。 この場合、タスク A はプロジェクトの開始にできるだけ近いタイミングでスケジュールされます。

  ![ タスクリストの最新の利用可能な時間タスクの制約](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **できるだけ遅く：**&#x200B;このシナリオでは、先行タスクに「できるだけ遅く」の制約を適用すると、先行タスクが優先されます。

  **例：**&#x200B;例えば、タスク A がタスク B の先行タスクであるとします。タスク A には「できるだけ遅く」の制約が適用され、タスク B には「できるだけ早く」の制約が適用されます。 この場合、タスク A はプロジェクトの終了にできるだけ近いタイミングでスケジュールされます。

  ![ タスクリスト内のタスク制約をできるだけ遅く](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

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
<li> <p><strong>Latest Available Time:</strong> Using the Latest Available Time constraint on the successor task gives priority to flexible constraint of the predecessor.</p> <p>For example, Task A is a predecessor to Task B. Task B has the Latest Available Time constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the start of the project as possible.</p> </li>
<li> <p><strong>As Late As Possible:</strong> In this scenario, using the As Late As Possible constraint on the successor task gives the priority to the successor task.</p> <p>For example, Task A is a predecessor to Task B. Task B has the As Late As Possible constraint and Task A has the As Soon As Possible constraint. In this situation, Task B is scheduled as close to the end of the project as possible.</p> </li>
</ul>
</div>
-->
