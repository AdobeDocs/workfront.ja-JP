---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: 'タスク制約の概要：最古の利用可能時間'
description: 最も早い使用可能時間は、先行タスク関係を考慮した後に、使用可能な最も早い時間にタスクを開始するようにスケジュールするタスク制約です。
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# タスク制約の概要：最古の利用可能時間

最も早い使用可能時間は、先行タスク関係を考慮した後に、使用可能な最も早い時間にタスクを開始するようにスケジュールするタスク制約です。

タスクのタスク制約を更新する方法については、 [タスクのタスク制約の更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above) </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To update the Task Constraint to Earliest Available Time:</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to a task whose constraint you want to modify. </li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Edit Task</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Overview</strong> section, expand the <strong>Task Constraint</strong> drop-down menu.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Earliest Available Time</strong>.</p>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save Changes</strong>.</li>
   -->

## 可能な限り早い時間と可能な限り早い時間の違い

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

最も早い利用可能な時間制約は、次の条件がすべて存在する場合、「可能な限り早く」制約とは異なります。

* プロジェクトは完了からスケジュールされています
* プロジェクト内のタスクには先行タスク関係があります
* 先行タスクには柔軟なタスク制約があります

この場合：

* **最も早い利用可能時間：** 後続タスクに対して [ 最も早い時間 ] 制約を使用すると、先行タスクの柔軟な制約が優先されます。

   **例**

   タスク A はタスク B の先行タスクです。タスク B は最も早い有効時間制約を持ち、タスク A はできるだけ遅く制約を持ちます。 この場合、タスク B は、可能な限りプロジェクトの完了に近い状態でスケジュールされます。

   ![タスクの日付がプロジェクトの完了日に近い場合の最も古い使用可能な時間制限](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **できるだけ早く：** このシナリオでは、後続タスクに対して As As As Possible 制約を使用すると、後続タスクが優先されます。

   **例**

   タスク A はタスク B の先行タスクです。タスク B は可能な限り早い制約を持ち、タスク A は可能な限り遅い制約を持ちます。 この場合、タスク B は、可能な限りプロジェクトの開始に近い状態でスケジュールされます。

   ![タスクの日付がプロジェクトの開始日に近い場合の [ 可能な限り早く ] 制約](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
