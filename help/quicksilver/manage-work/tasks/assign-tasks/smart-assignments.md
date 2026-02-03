---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: スマート割り当ての概要
description: タスクとイシューの割り当てを管理する場合、スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。スマート割り当てとは、仕事に最も適したリソースを決定するアルゴリズムに基づいて作業アイテムをリソースに割り当てる際に Adobe Workfront が提示する候補です。
author: Lisa
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 77%

---

# スマート割り当ての概要

<!--Audited: 07/2024-->

タスクとイシューの割り当てを管理する際に、スマート割り当てを使用して、作業を完了するのに最適なリソースを特定できます。

スマート割り当ては、作業アイテムをリソースに割り当てる際に、その作業に最も適したリソースを決定するアルゴリズムに基づいて Adobe Workfront が示す提案です。スマート割り当てでは、ユーザー、担当業務、チームを指定できます。

>[!NOTE]
>
>ユーザーを提案する場合、スマート割り当てはユーザーの空き時間を考慮しません。ただし、スケジュールに従った稼動状況は、タスクの予定日と見込日に影響し、タスクが割り当てられた際に問題が発生します。スケジュールについて詳しくは、[スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)の記事を参照してください。

この記事には、スマート割り当てに関する一般的な情報が含まれています。スマート割り当てを使用してタスクとイシューをユーザーに割り当てる方法について詳しくは、[スマート割り当てを行う](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)を参照してください。

## スマート割り当ての概要

スマート割り当てを使用する際は、次の点を考慮してください。

<!--* <span class="preview">The algorithm works independently for tasks and issues. This means that the list of suggested users for issues might differ from the list of suggested users for a task because Workfront builds the lists according to criteria pertaining to issues and tasks separately. </span>-->
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* 推奨される割り当ては、常にアクティブユーザー、担当業務またはチームです。
* 最初にリストされるリソースは、そのタスクに最も一致するリソースである必要があります。

## スマート割り当て候補の検索

スマート割り当ては、タスクまたはイシューを割り当てることができる次のエリアで表示できます。

* 割り当て列のイシューのリストまたはレポート

  ![ 問題リストの割り当て列 ](assets/smart-assignments-issue-list.png)

* 割り当て列のタスク リストまたはレポート

  ![ 「タスク・リストの割当て」列 ](assets/smart-assignments-task-list.png)

* 「割り当て」フィールドのタスクヘッダー

  ![ タスク ヘッダーの [ 割り当て ] フィールド ](assets/smart-assignments-task-header-nwe-350x302.png)

* 「割り当て」フィールドのイシューヘッダー

  ![ 問題ヘッダー割り当てフィールド ](assets/smart-assignments-issue-header.png)

* 割り当てエリアのタスクまたはイシューの概要パネル

  ![ 概要パネルの割り当て領域 ](assets/issue-assignments-summary-panel.png)

<!--* The Assignments field in the New Task box, when adding a task to a project

  (![Smart assignments new task]assets/smart-assignments-new-task-modal.png)-->

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![Smart assignments in Home](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* タスクまたはイシューを割り当てる際のこの割り当て先エリアのワークロードバランサー

  ![ ワークロードバランサーの「割り当て」領域 ](assets/smart-assignments-workload-balancer-bulk-assignments.png)

## スマート割り当て条件

<!--Smart assignments work differently for tasks than for issues.  -->

<!--### Smart assignments criteria for tasks

The task smart assignments calculation works in <span class="preview">two phases which use two different algorithms.</span>

<span class="preview">Depending on which algorithm finds the smart assignment, the assignments are listed under two separate sections in the Assignments field.</span> For information, see [Make smart assignments](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md). 

![Smart assignments in tasks list](assets/smart-assignments-task-list.png)

<div class="preview">

#### First phase of smart assignment calculation for tasks 

In the first phase of calculating smart assignments, Workfront calculates a similarity score for every assignment. 

>[!NOTE]
>
>The first phase of the smart assignments calculation does not apply to the following task areas:
>
>* Bulk Assignments in the Workload Balancer.
>* Connected cards on boards.


The calculation for the similarity score and the order in which the assignments are listed take into account the following:  

* A score of 100% is given to an existing assignment where the task, project, and portfolio names are identical to the task you're trying to assign. The project and portfolio names of the task of an existing assignment must also match the project and portfolio of the task you are trying to assign.   

* If only some of this information from other assignments matches on the existing tasks, the score might be lower than 100%.  

  For example, if you are assigning a task called "My second task" on a project called "My project" in a portfolio called "My portfolio" and you have an existing task called "My task" in another project called "My project" in a portfolio called "My portfolio", the user assigned to "My task" might get a score of 95% because the name of the existing task and the task you're trying to assign now are similar, but not identical.  
 
    >[!TIP]
    >
    >  Workfront looks for matches only in the Name fields of tasks, projects, and portfolios and not in any other fields. 

* An assignment could get a higher score when they are assigned to a lot of tasks in the system that have similar names. For example, if a team called "Development" is assigned to 50% of the tasks in the system containing "AI" in the name and you are now assigning another task with "AI" in the name, the score of the "Development" team is higher. In this case, the names of  projects and portfolios are not as important.  

* Taking into account this scoring system, the first 7 suggestions are listed as smart assignments, in the descending order of their scores. Assignments with scores lower than 40% do not display.  

* If several assignments have identical scores, they display in order of the date on which the assignments were made, starting from the most recent date.  

  For example, if Rick was assigned to a similar task earlier today and Jennifer was assigned to a similar task two days ago, Rick displays first.  

* Assignments identified in this phase are listed in the    **Suggested assignments**  section of the Assignments field for tasks. 

* If there are no matches using this calculation, the second phase of smart assignments starts which is calculated using a different algorithm.  

</div>

#### Second phase of smart assignment calculation for tasks-->

<!--If the first step of task smart assignments has found no matches,-->

Workfrontは、イシューに対して計算するのと同じ方法で、タスクのスマート割り当てを計算します。

<!--For more information, see the section [Smart assignments criteria for tasks and issues](#smart-assignments-criteria-for-tasks-and-issues) in this article. -->

識別された割り当ては、「割り当て」フィールドの **ユーザーとチーム** および **担当業務**<!--, and <span class="preview">**Rate card roles**</span>--> セクションにリストされます。<!--<span class="preview">For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>. keep the rate cards roles in yellow after the release of assignments to Prod-->

<!--
### Smart assignments criteria for tasks and issues 

>[!NOTE]
>
>The following criteria applies for tasks only when the first phase of the task smart assignment calculation did not find any matches. For information, see the section [First phase of smart assignment calculation for tasks](#first-phase-of-smart-assignment-calculation-for-tasks) in this article. The following criteria always applies for issues, by default. -->

![ スマート割り当ての例 ](assets/smart-assignments-issue-header.png)

次の条件の組み合わせに基づいて、スマート割り当てドロップダウンリストでユーザー候補が提示されます（最も重要候補から最も重要でない候補の順に表示されます）。

1. 過去 30 日間に、割り当てを行ったユーザーによって他の作業アイテムに割り当てられたユーザー。この条件に一致する最初の 50 名のユーザーが表示されます。最も頻繁に割り当てられたユーザーが最初に表示されます。

2. 作業アイテムがチームまたは役割に割り当てられている場合は、以下の既存の割り当てを考慮して、候補に挙げられたユーザーのリストがさらにフィルタリングされます。この場合、候補のリストには次のユーザーのみが表示されます。

   * ホームチームが作業アイテムに割り当てられているユーザー。
   * プライマリ役割が、作業アイテムに割り当てられているユーザーです。

>[!TIP]
>
>* タスクまたはイシューに割り当てられた役割やチームがない場合、Workfront は過去 30 日間に割り当てられたすべてのユーザー（最大 50 名）を表示します。
>
>* 過去 30 日間に割り当てを行っていない場合は、割り当てられたチームに属しているユーザー、または自身の役割が作業アイテムに割り当てられているユーザーのみが、スマート割り当てリストに表示されます。



<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE: this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
