---
content-type: overview
product-area: projects
navigation-topic: task-information
title: プロジェクトの完了率の概要
description: プロジェクトの [ 完了率 ] の値は、プロジェクト内のタスクの [ 予定期間 ] または [ 予定時間 ] に基づいて計算されます。 Adobe Workfront管理者またはグループ管理者は、「プロジェクトの環境設定」領域で情報を設定する際に、システムでの完了率を計算する際に考慮に入れる値を定義します。 プロジェクトの基本設定の構成については、「システム全体のプロジェクト基本設定を構成する」を参照してください。
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: 31533bd7ee1890a8343d32770d623d5d9a6007d2
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# プロジェクトの完了率の概要

プロジェクトの [ 完了率 ] の値は、プロジェクト内のタスクの [ 期間 ] または [ 予定時間 ] に基づいて計算されます。 Adobe Workfront管理者またはグループ管理者は、「プロジェクトの環境設定」領域で情報を設定する際に、システムでの完了率を計算する際に考慮に入れる値を定義します。

プロジェクトの環境設定の詳細については、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

親タスクの完了率は、各サブタスクの期間または計画時間に基づきます。

同様に、プロジェクトの [ 完了率 ] は、プロジェクトの各メインタスクの期間または予定時間に基づきます。

主なタスクは、親タスクと、子を持たないスタンドアロンタスクです。

>[!TIP]
>
>主なタスクは、プロジェクトプラン内でインデントされません。

## Workfrontが達成率を計算する方法

* [タスクの完了率の更新](#update-the-percent-complete-on-a-task)
* [Workfrontが親タスクの完了率を計算する方法](#how-workfront-calculates-percent-complete-on-a-parent-task)
* [Workfrontがプロジェクトの完了率を計算する方法](#how-workfront-calculates-percent-complete-on-a-project)

### タスクの完了率の更新 {#update-the-percent-complete-on-a-task}

タスクの完了率は手動で変更できます。 これは計算ではありません。

Workfrontは、個々のタスクの完了率を使用して、親タスクの完了率またはプロジェクトの完了率を計算します。

タスクの完了率を更新する方法については、 [タスクの完了率の表示と更新](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Workfrontが親タスクの完了率を計算する方法 {#how-workfront-calculates-percent-complete-on-a-parent-task}

親タスクの完了率は、システムレベルまたはグループレベルのプロジェクトプリファレンスでWorkfrontまたはグループ管理者が選択した内容に応じて、「期間」または「予定時間」のどちらかに基づいて計算されます。

次のシナリオを考慮します。

* 計画時間に基づいて完了率が計算される場合、親タスクの完了率は次の式を使用して計算されます。

   `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

   親の合計計画時間は、各子の全計画時間の合計を表します。

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* 期間に基づいて完了率が計算される場合、親タスクの完了率は次の式を使用して計算されます。

   `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!IMPORTANT]
   >
   >親タスクの合計期間は、子タスクの全期間の合計です。 例えば、2 つの子を持つ親タスクで、それぞれの期間が 1 日、2 日の場合、2 つの子を同じ日に開始できる場合でも、合計期間は 3 日になります。


### Workfrontがプロジェクトの完了率を計算する方法 {#how-workfront-calculates-percent-complete-on-a-project}

プロジェクトの完了率は、システムレベルまたはグループレベルのプロジェクト環境設定でWorkfrontまたはグループ管理者が選択した内容に応じて、プロジェクトの主要タスクの「期間」または「予定時間」に基づいて計算されます。

* 計画時間に基づいて完了率が計算される場合、プロジェクト完了率は次の式を使用して計算されます。

   `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

   プロジェクトの合計計画時間は、プロジェクトのすべての主要タスクの計画時間の合計です。

   ![](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

   >[!NOTE]
   >
   >タスク 1 またはタスク 2 は、親タスクまたはスタンドアロンタスクのみにすることができます。 この計算では、子タスクの計画時間と完了率は使用されません。

* 期間に基づいて完了率が計算される場合、プロジェクトの完了率は次の式を使用して計算されます。

   `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

   >[!IMPORTANT]
   >
   >Project の期間は、完了率を示すメインタスクの全期間の合計です。 例えば、2 つのタスクが同じ日に開始できる場合でも、2 日間のタスクがスタンドアロンタスクで、期間が 5 日間の親タスクで作業が完了しているプロジェクトの期間は、合計 7 日間になります。

   ![](assets/project-with-tasks-percent-complete-duration-calculation.png)

   >[!NOTE]
   >
   >タスク 1 またはタスク 2 は、親タスクまたはスタンドアロンタスクのみにすることができます。 この計算では、子タスクの期間と完了率は使用されません。

## 期間を使用したプロジェクトの完了率の例

タスクの「期間」を使用してプロジェクトの完了率を計算する場合、次の例を考えてみます。

![](assets/project-with-tasks-percent-complete-duration-calculation.png)

次の情報は、プロジェクトの完了率を計算するために使用されます

* スタンドアロンタスクの完了率（タスク 1 ～ 20%）
* 親タスクの完了率（タスク 2 - 25%）
* タスク 1 の期間（5 日）
* タスク 2 の期間（2 日）
* プロジェクトの期間（7 日）


「期間」を使用してプロジェクトの完了率を計算する手順は、次のとおりです。

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

または

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->