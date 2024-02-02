---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: ユーザービューを使用する場合は、リソースプランナーで使用可能、予定、実際の時間数、または FTE を表示する
description: ユーザービューの使用時に、リソースプランナーで利用可能時間数、予定時間数、実績時間数、FTEの表示「RP での計画」 - おそらく「RP でのリソースの予算計上」または「RP でのリソースの管理」。など、または POV から転用する必要がある）」
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '1738'
ht-degree: 100%

---

# ユーザービューを使用する場合は、リソースプランナーで使用可能、予定、実際の時間数、または FTE を表示する

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

プロジェクトビューと役割ビューでリソースを予算計上する以外に、Adobe Workfront リソースプランナーのユーザービューを使用して、プロジェクトとリソースの予定時間数、利用可能時間数、実際の時間数または FTE 値に関する情報を表示できます。

## リソースプランナーのユーザービューの概要

リソースプランナーで時間または FTE 情報を表示する際は、次の点を考慮します。

* リソースプランナーのすべてのビューで、ユーザー、担当業務、プロジェクトの使用可能時間数および予定時間数または FTE を表示できます。
* 次の情報は、ユーザービューでのみ表示できます。

   * 予定時間数または FTE の量と、使用可能時間数または FTE の量の差。その後、プロジェクトビューと役割ビューのこの差に従って、ユーザーの配分を予算計上できます。
   * 実際の時間数または FTE。

* ユーザーの空き時間数と予定時間数の値または FTE の差は、ユーザービューで数値またはパーセンテージ値で表示できます。
* ユーザービューにコスト別の情報を表示することはできません。
* Adobe Workfront では、スケジュール内のユーザーに関連付けられた作業時間に従って、利用可能時間数または FTE を設定します。\
  スケジュールに関連付けられていないユーザーは、デフォルトのスケジュールに従って利用可能状況が表示されます。\
  デフォルトのスケジュールについては、[スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

* Workfront は、プロジェクトのタスクおよび問題に関する予定時間数情報から予定時間数または FTE を入力します。
* Workfront は、タスクに割り当てられたユーザーによるタスクとイシューに記録された実際の時間数を「実際の時間数」に入力します。これには、プロジェクトに対して記録された時間が含まれます。
* ユーザービューでは、次の操作を実行できます。

   * 各ユーザーを展開すると、そのユーザーが割り当てられているプロジェクトのリストが表示されます。

     >[!NOTE]
     >
     >フィルターに含まれるプロジェクトに関連付けられているユーザーのみを展開できます。

   * すべてのプロジェクトを展開すると、ユーザーがそれらのプロジェクトで実行できる担当業務のリストが表示されます。
   * 各役割を展開すると、その役割のユーザーが割り当てられているタスクのリストが表示されます。

  ユーザーに担当業務が関連付けられていない場合は、利用可能時間数、予定時間数、実際の時間数または FTE が「**役割なし**」セクションに入力されます。\
  ユーザービューをリソースプランナーに適用するときに表示されるフィールドと項目については、[リソースプランナーのナビゲーションの概要](../../resource-mgmt/resource-planning/resource-planner-navigation.md)の「プロジェクト／役割／ユーザービューの選択」の節を参照してください。

## リソースプランナーのユーザービューに表示されるフィールドの概要

次の表を参照して、リソースプランナーのユーザービューに表示される情報を確認します。この情報は、「時間」または「FTE」の値で表示されます。

* [AVL（利用可能）列](#the-avl-available-column)
* [PLN（予定）列](#the-pln-planned-column)
* [ACT（実際）列](#The%C2%A0ACT)
* [DIF（差異）列](#the-dif-difference-column)
* [割合（予定時間割り当て率）列](#the-planned-hours-allocation-percentage-column)

### AVL（利用可能）列 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示単位</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td>ユーザーのスケジュールに基づく、ユーザーの使用可能な時間数または FTE の合計。 </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>この情報は、リソースプランナーにユーザービューを適用する場合は、プロジェクトでは利用できません。 </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>ユーザーのスケジュールに基づく役割の利用可能時間または FTE の合計と、役割の <strong>FTE 利用可能時間の割合</strong>。</p> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー</td> 
   <td>この情報は、タスクまたはイシューでは使用できません。 </td> 
  </tr> 
 </tbody> 
</table>

ユーザーと役割の空き時間がユーザーのスケジュールと役割の FTE 利用可能時間の割合に基づいて計算される方法の詳細については、[リソースプランナーでのユーザーと役割の時間と FTE の計算の概要](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)を参照してください。

### PLN（予定）列 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示単位</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> すべてのプロジェクトでユーザーに割り当てられたすべてのタスクまたはイシューからの予定時間数または FTE の合計です。<br><p>これには、ユーザーに割り当てられているが担当業務に関連付けられていないタスクとイシュー、および管理へのアクセス権を持つプロジェクトにないタスクやイシューが含まれます。</p><p>ワークロードバランサーを使用してユーザーの時間割り当てを変更した場合、稼働率レポートで選択した日付にタスクの期間またはイシューの期間が一部しか含まれていないと、リソースプランナーのデータに影響することがあります。ユーザー割り当ての変更について詳しくは、<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>を参照してください。 </p></td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> プロジェクトで特定のユーザーに割り当てられたすべてのタスクまたはイシューからの予定時間数または FTE の合計です。<br><p>メモ：これには、どのユーザーにも割り当てられていないタスクやイシューの予定時間数や FTE は含まれません。 </p></td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>プロジェクトでユーザーに割り当てられたすべてのタスクまたはイシューからの予定時間数または FTE の合計です。</p> <p> <p>メモ：これには、この役割には割り当てられているがこの役割のこのユーザーに割り当てられていないタスクやイシューの予定時間数や FTE は含まれません。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー</td> 
   <td>プロジェクトのタスクまたはイシューに関連付けられた予定時間数または FTE。</td> 
  </tr> 
 </tbody> 
</table>

予定時間数を表示する際は、次の点を考慮してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* 予定時間数は、タスクとイシューの期間内で、割り当てられたリソースごとに毎日均等に配分されます。タスクまたはイシューの期間は、その予定開始日と完了日に基づき、その期間内の各カレンダー日が含まれます。\
  Workfront では、ユーザーまたはプロジェクトに予定時間数を配分する際に、ユーザーまたはプロジェクトのスケジュールが考慮されます。この場合、予定時間数は、週末、休日、スケジュール例外を除くタスクまたはイシューの期間内の各日に均等に配分されます。

  例えば、リソースプランナーを週別に表示していて、プロジェクトに複数週にわたるタスクがある場合、1 週間あたりの予定時間数は、その週の何日がタスク期間に含まれているかによって異なります。この動作は、月別または四半期別でリソースプランナーを表示する場合や、タスクが複数の月または四半期にまたがる場合と同様です。\
  週末、スケジュールの例外および休暇日は、この配分から除外されます。

* 各リソースの予定時間数の計算には、次のタスクのカテゴリが含まれます。

   * リソースプール、担当業務、またはプロジェクトのチームでユーザーに割り当てられたタスク。

     >[!TIP]
     >
     >タスクがチームに割り当てられると、その割り当ては、「**役割なし**」および「**ユーザーなし**」セクションに表示されます。チームに関連付けられた予定時間数は表示できますが、タスクに関連付けられた役割やユーザーがないので、時間数を予算計上することはできません。

* リソースプランナーの予定時間数には、次に関連する予定時間数は含まれません。

   * 親タスク
   * 未割り当てタスク
   * イシュー（**イシューの時間数を含める**&#x200B;の設定が無効の場合）。

* タスクまたはイシューの期間が 0 の場合、予定時間数はリソースプランナーに表示されません。
* 非アクティブ化されたユーザーに関連付けられた予定時間数は表示されません。

リソースプランナーの計画時間数と工数について詳しくは、[リソースプランナーのプロジェクトビューと役割ビューの時間、FTE、コスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)を参照してください。

### ACT（実際）列

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示単位</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー </td> 
   <td> <p>ユーザーが割り当てられたすべてのタスクまたはイシューに関して記録した時間。</p> <p>これには次が含まれます。</p> 
    <ul> 
     <li>ユーザーに割り当てられているが担当業務に関連付けられていないタスクとイシュー。</li> 
     <li>「管理」へのアクセス権を持つプロジェクトにないタスクおよびイシュー。 </li> 
    </ul> <p>これには、ユーザーがそのプロジェクトのタスクまたはイシューに割り当てられている場合にのみ、プロジェクトに対して記録された時間が含まれます。  </p> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト </td> 
   <td> <p>ユーザーがプロジェクトで割り当てられたすべてのタスクまたはイシューに関して記録した時間。</p> <p>これには、ユーザーがプロジェクトに対して直接記録した時間も含まれます。</p> <p>これには次のものは含まれません。</p> 
    <ul> 
     <li> <p>どのユーザーにも割り当てられていないタスクとイシューに対して記録された時間。 </p> </li> 
     <li> <p>親タスクに対して記録された時間。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>この役割のユーザーに割り当てられたすべてのタスクまたはイシューに対して記録された時間。 </p> <p>これには次のものは含まれません。</p> 
    <ul> 
     <li>この役割に割り当てられているがこの役割のこのユーザーには割り当てられていないタスクおよびイシューに対して記録された時間。</li> 
     <li>プロジェクトまたは親タスクに対して直接記録された時間。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー </td> 
   <td> <p>タスクおよびイシューに割り当てられているユーザーによってタスクおよびイシューに対して記録された時間。 </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>記録される時間は、時間が記録されるタスク、イシュー、またはプロジェクトの期間に関係なく、時間の入力日に対応する時間枠で表示されます。

実際の時間数について詳しくは、[実際の時間数の表示](../../manage-work/tasks/task-information/actual-hours.md)を参照してください。

### DIF（差異）列 {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示単位</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>ユーザーの利用可能時間と予定時間数または FTE の差。 </p> <p>時間または FTE の差は、次の数式で計算されます。</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>メモ：値が負の赤色の数字で表示される場合、ユーザーは割り当て超過になります。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>この情報は、プロジェクトでは使用できません。 </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>担当業務の利用可能時間数と予定時間数または FTE の差。 </p> <p>時間または FTE の差は、次の数式で計算されます。</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>メモ：値が負の赤色の数字で表示される場合、担当業務は割り当て超過になっています。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー</td> 
   <td>この情報は、タスク、イシューまたはプロジェクトでは使用できません。 </td> 
  </tr> 
 </tbody> 
</table>

### 割合（予定時間割り当て率）列 {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示先</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>予定時間数または FTE の配分を利用可能時間数の割合として表したもの。予定時間数配分率は、次の式で計算されます。</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>FTE 値にも同じ計算が使用されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td><strong>ユーザー別に表示</strong>ビューをリソースプランナーに適用する場合、この情報はプロジェクトでは使用できません。</td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> 予定時間数または FTE の配分を利用可能時間数の割合として表したもの。 <p>予定時間数配分率は、次の式で計算されます。</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>FTE 値にも同じ計算が使用されます。</p></td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー</td> 
   <td>この情報は、タスク、イシューまたはプロジェクトでは使用できません。 </td> 
  </tr> 
 </tbody> 
</table>

予定時間数または FTE の値がゼロの場合、配分率は 0％になります。利用可能時間数または FTE の値がゼロの場合、配分率は計算できません。

予定時間数と FTE およびリソースプランナーでのそれらの表示について詳しくは、[リソースプランナーのプロジェクトビューおよび役割ビューを使用したリソースの予算計上](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
