---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: task-constraints
title: タスク制約の概要：使用可能な最短時間
description: 最も早い空き時間は、先行タスク関係を考慮した後で、最も早い空き時間にタスクを開始するようにスケジュール設定するタスクの制約です。
author: Alina
feature: Work Management
exl-id: 9c01e4bd-c6ca-4540-a0f1-ecdd44df84e0
TQID: https://experienceleague.adobe.com/htQAqPWSYcdft3g3RDQuRu3VdmxmvVQt2EFrvFJsRU4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 299
ht-degree: 97%

---

# タスクの制約の概要：最も早い空き時間

最も早い空き時間は、先行タスク関係を考慮した後で、最も早い空き時間にタスクを開始するようにスケジュール設定するタスクの制約です。

タスクでタスクの制約を更新する方法については、[タスクでタスクの制約を更新](../../../manage-work/tasks/task-constraints/update-task-constraint-of-task.md)を参照してください。

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

## 最も早い空き時間とできるだけ早くの違い

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This section is duplicated in "Earliest Available Time"])</p>
-->

「最も早い空き時間」の制約は、次の条件がすべて存在する場合、「できるだけ早く」の制約とは異なります。

* プロジェクトは完了からスケジュールされます
* プロジェクト内のタスクには、先行タスク関係があります
* 先行タスクには、柔軟なタスクの制約があります

この状況では、次のようになります。

* **最も早い空き時間：**&#x200B;後続タスクに「最も早い空き時間」の制約を使用すると、先行タスクの柔軟な制約が優先されます。

  **例**

  タスク A がタスク B の先行タスクであるとします。タスク B には「最も早い空き時間」の制約が適用され、タスク A には「できるだけ遅く」の制約が適用されます。 この場合、タスク B はプロジェクトの完了にできるだけ近いタイミングでスケジュールされます。

  ![タスクの日付がプロジェクトの完了日に近い場合の「最も早い空き時間」の制約](assets/earliest-available-constraint-dates-closer-to-project-completion-350x137.png)

* **できるだけ早く：**&#x200B;このシナリオでは、後続タスクに「できるだけ早く」の制約を使用すると、後続タスクが優先されます。

  **例**

  タスク A がタスク B の先行タスクであるとします。タスク B には「できるだけ早く」の制約が適用され、タスク A には「できるだけ遅く」の制約が適用されます。 この場合、タスク B はプロジェクトの開始にできるだけ近いタイミングでスケジュールされます。

  ![タスクの日付がプロジェクトの開始日に近い場合の「できるだけ早く」の制約](assets/as-soon-as-possible-dates-closer-to-project-start-350x126.png)
