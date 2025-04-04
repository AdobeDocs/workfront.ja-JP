---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの予定完了日を設定
description: プロジェクトの予定完了日とは、プロジェクトが完了するように設定された日付です。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 996398c5-de92-445e-8e86-36b2efdcf6b5
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 77%

---

# プロジェクトの予定完了日を設定

<!-- Audited: 4/2025 -->

プロジェクトの予定完了日は、プロジェクトが完了するように設定された日付です。

プロジェクトの予定開始日と予定完了日は、プロジェクトのタスクの日付に依存します。この記事では、プロジェクトの予定完了日を手動または自動で設定する方法について説明します。タスクの予定完了日について詳しくは、[タスクの予定完了日の概要](../../../manage-work/tasks/task-information/task-planned-completion-date.md)を参照してください。

プロジェクトの予定完了日は、プロジェクトを開始日からスケジュールするか、完了日からスケジュールするかに応じて、手動または自動で設定できます。

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>
   新規：標準

または

現在：プラン </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトの管理権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プロジェクトの予定完了日を手動で設定

プロジェクトを完了日からスケジュールする場合は、プロジェクトの予定完了日を手動で設定する必要があります。

>[!NOTE]
>
>プロジェクトの予定完了日を手動で設定すると、Workfront は、すべてのタスクの期間に基づいて、プロジェクトの予定開始日を自動的に計算します。


「完了日」からプロジェクトをスケジュールする手順は、次のとおりです。

{{step1-to-projects}}

1. **新規プロジェクト** をクリックし、表示されるドロップダウンから **新規プロジェクト** を選択します。

   プロジェクトの作成について詳しくは、「[プロジェクトを作成](../../../manage-work/projects/create-projects/create-project.md)」の記事を参照してください。

1. 左側のパネルで **プロジェクト詳細** を選択します。

1. 右上隅の **プロジェクトを編集** アイコン ![ 編集アイコン ](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) をクリックし、表示されるドロップダウンで **概要** を選択します。

1. 「**プロジェクト日付**」セクションで、「**スケジュールモード**」フィールドをクリックし、「**完了日**」を選択します。

1. プロジェクトの&#x200B;**予定完了日**&#x200B;を指定します。
1. 「**変更を保存**」をクリックします。

   プロジェクトにタスクを追加すると、プロジェクトの&#x200B;**予定開始日**&#x200B;は、すべてのタスクの合計期間に基づいて計算されます。

## プロジェクトの計画完了日を自動的に設定

プロジェクトの予定完了日は、プロジェクトの開始日からスケジュールする際に、Workfront によって自動的に計算されます。 

「開始日」からプロジェクトをスケジュールする手順は、次のとおりです。

{{step1-to-projects}}

1. **新規プロジェクト** をクリックし、表示されるドロップダウンから **新規プロジェクト** を選択します。

   プロジェクトの作成について詳しくは、「[プロジェクトを作成](../../../manage-work/projects/create-projects/create-project.md)」の記事を参照してください。

1. 左側のパネルで **プロジェクト詳細** を選択します。

1. 右上隅の **プロジェクトを編集** アイコン ![ 編集アイコン ](/help/quicksilver/manage-work/projects/planning-a-project/assets/qs-edit-icon.png) をクリックし、表示されるドロップダウンで **概要** を選択します。

1. 「**プロジェクト日付**」セクションで、「**スケジュールモード**」フィールドをクリックし、「**開始日**」を選択します。

1. プロジェクトの&#x200B;**予定開始日**&#x200B;を指定します。
1. 「**変更を保存**」をクリックします。

   プロジェクトにタスクを追加すると、プロジェクトの&#x200B;**予定完了日**&#x200B;は、すべてのタスクの合計期間に基づいて計算されます。

   タスクの期間について詳しくは、[タスクの期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

   この場合、プロジェクトの予定完了日は、プロジェクトの最後のタスクの予定完了日と一致します。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>The Planned Completion Date of a task</h2>
<p>(NOTE: drafted because I created a new article, here: /Content/Manage work/Tasks/Task information/task-planned-completion-date.htm)</p>
<p>You can either specify the Planned Completion Date of a task, or you can leave it up to Workfront to calculate it depending on certain criteria.&nbsp;</p>
<ul>
<li><a href="#manually-set-the-planned-completion-date-of-a-task" class="MCXref xref">Manually set the Planned Completion Date of a task</a> </li>
<li><a href="#how-the-planned-completion-date-is-calculated-for-a-task" class="MCXref xref">How the Planned Completion Date is calculated for a task</a> </li>
</ul>
<p><strong>Manually set the Planned Completion Date of a task</strong></p>
<p>Setting the Planned Completion Date of a task depends on the type of Task Constraint you assign to the task.&nbsp;</p>
<p>You can manually set the Planned Completion Date&nbsp;when creating a task, as described in&nbsp;the article <a href="../../../manage-work/tasks/create-tasks/create-tasks-in-project.md" class="MCXref xref">Create tasks in a project</a>.</p>
<p>You can manually specify the Planned Completion Date when you select any of the following Task Constraints:&nbsp;</p>
<table border="1" cellspacing="15" cellpadding="1">
<col>
<col>
<thead>
<tr>
<th> <p><strong>Task Constraint Type</strong> </p> </th>
<th> <p><strong>Effect of Manually Changing the Planned Completion Date</strong> </p> </th>
</tr>
</thead>
<tbody>
<tr>
<td> <p>Must Finish On</p> <p>Finish No Later Than</p> <p>Finish No Earlier Than</p> </td>
<td> <p><span class="s1">The Planned Start Date is adjusted in order to keep the Duration the same.</span> </p> </td>
</tr>
<tr>
<td> <p>Fixed Dates</p> </td>
<td> <p>The Duration is adjusted in order to keep the Planned Start Date the same.</p> </td>
</tr>
</tbody>
</table>
<p><strong>How the Planned Completion Date is calculated for a task</strong></p>
<p>When it is calculated automatically by the system, the following can influence the Planned Completion Date of a Task:</p>
<ul>
<li> <p>Task Constraint</p> <p>For more information about Task Constraints, see the article <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Task Constraint overview</a>.</p> </li>
<li> <p>Task predecessor relationship</p> <p>For more information about task predecessors, see the article <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p> </li>
<li>Project Completion Date, when the project is scheduled from Completion Date.</li>
<li> <p>The time off schedule of the Primary&nbsp;Assignee of the task. </p> <p>When the Primary Assignee has time off scheduled during the duration of the task, the planned dates of the task adjust accordingly when the <strong>Consider user time off in task durations</strong> setting is selected for the <strong>User Time Off</strong> field. New projects inherit this setting from the Project&nbsp;Preferences area, but you can edit the setting at the project level. </p> <p>For example, if a task with a Constraint of As Soon As Possible is scheduled to start on June 1 and complete on June 3, and the Primary Assignee has June 2 marked for Time-off, the task Planned Completion Date becomes June 4. </p> <p>For information about the <strong>User Time Off</strong> preference, see the articles <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a> or <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</p> </li>
</ul>
<p>When set automatically, the Planned Completion Date&nbsp;is determined based on the following calculation:&nbsp;</p>
<p><code>Planned Completion Date = Planned Start Date + Duration</code> </p>
<p>For example, if your task has a start date of September 16 and a duration of 10 days, the Planned Completion Date is September 26.</p> <note type="note">
&nbsp;The Update Type for the project must also be&nbsp;set to Automatic and On Change or Automatically in order for the Planned Hours and Duration to be automatically&nbsp;adjusted.
<br>For more information about the Update Type, see the article
<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">Select the project Update Type </a>.
</note>
</div>
-->
