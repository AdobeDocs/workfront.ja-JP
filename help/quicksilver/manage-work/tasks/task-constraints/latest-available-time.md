---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'タスク制約の概要：最新の利用可能時間'
description: Latest Available Time(LAT) は、Adobe Workfrontのタスク制約の一種です。
author: Alina
feature: Work Management
exl-id: acf55004-9424-4e24-9ff5-90f6fd7f72a6
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# タスク制約の概要：最新の使用可能な時間

Latest Available Time(LAT) は、Adobe Workfrontのタスク制約の一種です。

## 最新の利用可能な時間タスク制約を使用

LAT 制約は、プロジェクト内の先行者と後続者の関係を考慮した後に、利用可能な最新の時間でタスクを開始するようにスケジュールする場合に使用できます。

この制約は、先行タスクや後続タスクの再スケジュールを強制しない点で、[ 可能な限り早く ] とは異なります。 代わりに、関連付けられているタスクのスケジュールにのみ影響を与え、他のタスクとの関係に基づいて、最新の使用可能な時間に設定されます。

タスクのタスク制約を更新する方法については、 [タスクのタスク制約の更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

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

## 最新の利用可能な時間と可能な限り遅い時間の違い

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "As Late As Possible"] - inserted snippet in both (Alina)) </p>
-->

Latest Available Time 制約は、次の条件が存在する場合、 As Late Ass Foxable 制約とは異なります。

* プロジェクトは開始日からスケジュールされています
* プロジェクト内のタスクには先行タスク関係があります
* 後続タスクには、柔軟なタスク制約があります

この場合：

* **最新の利用可能時間：** 先行タスクに対して [ 最新の利用可能時間 ] 制約を使用すると、後続タスクの柔軟な制約が優先されます。

  **例：** たとえば、タスク A はタスク B の先行タスクです。タスク A には最新の利用可能時間制約が、タスク B には [ 可能な限り早く ] 制約が設定されます。 この場合、タスク A は、可能な限りプロジェクトの開始に近い状態にスケジュールされます。

  ![](assets/latest-available-time-task-constraint-in-task-list-350x116.png)

* **できるだけ遅くまで、以下をおこないます。** このシナリオでは、先行タスクに対して [ 可能な限り遅延 ] 制約を使用すると、先行タスクが優先されます。

  **例：** たとえば、タスク A はタスク B の先行タスクです。タスク A には可能な限り遅い制約、タスク B には可能な限り早い制約があります。 この場合、タスク A は可能な限りプロジェクトの終わり近くにスケジュールされます。

  ![](assets/as-late-as-possible-task-constraint-in-task-list-350x104.png)

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
