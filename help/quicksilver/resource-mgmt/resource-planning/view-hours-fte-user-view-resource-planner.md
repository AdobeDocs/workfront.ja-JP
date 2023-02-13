---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: ユーザー・ビューを使用する場合は、リソース・プランナで「使用可能」、「計画済」、「実績時間」または「工数」を表示します
description: RP で User viewPlanning を使用する場合は、リソース・プランナで使用可能、計画、実績時間または FTE を表示します。「RP でのリソースの予算作成」または「RP でのリソースの管理」が考えられます。 他の POV から転用する必要がある場合は、?!)」
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 1%

---

# ユーザー・ビューを使用する場合は、リソース・プランナで「使用可能」、「計画済」、「実績時間」または「工数」を表示します

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

「プロジェクト」ビューと「ロール」ビューでリソースを予算設定する以外に、Adobe Workfront Resource Planner の「ユーザー・ビュー」を使用して、プロジェクトとリソースの計画済、使用可能、実績時間または FTE 値に関する情報を表示できます。

## リソース・プランナのユーザー・ビューの概要

生産資源プランナで時間または工数の情報を表示する際は、次の点を考慮します。

* リソース・プランナのすべてのビューで、ユーザー、役割およびプロジェクトの使用可能時間および計画時間または工数情報を表示できます。
* 次の情報は、ユーザービューでのみ表示できます。

   * 計画時間数または工数の金額と、使用可能時間数または工数の金額の差。 その後、プロジェクトビューと役割ビューのこの違いに従って、ユーザーの配分を予算できます。
   * 実際の時間または工数。

* 「User Available」と「Amount of Planned Hours」または「FTE」の差分は、「User」ビューで数値またはパーセンテージ値で表示できます。
* ユーザービューにコスト別の情報を表示することはできません。
* Adobe Workfrontは、スケジュール内のユーザーに関連付けられた作業時間に従って、Available Hours または FTE を設定します。\
   スケジュールに関連付けられていないユーザーは、デフォルトのスケジュールに従って使用可能な状態を表示します。\
   デフォルトのスケジュールについては、 [スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfrontは、プロジェクトのタスクおよび問題に関する「計画時間」情報から計画時間または工程を入力します。
* Workfrontは、タスクに割り当てられたユーザーによるタスクと問題に記録された実際の時間を「実際の時間」に入力します。 これには、プロジェクトにログオンした時間が含まれます。
* ユーザービューでは、次の操作を実行できます。

   * 各ユーザーを展開して、そのユーザーが割り当てられているプロジェクトのリストを表示します。

      >[!NOTE]
      >
      >フィルターに含まれるプロジェクトに関連付けられているユーザーのみを展開できます。

   * すべてのプロジェクトを展開して、ユーザーがそれらのプロジェクトで実行できるジョブの役割のリストを表示します。
   * 各ロールを展開して、そのロールのユーザーが割り当てられているタスクのリストを表示します。

   ユーザーにジョブロールが関連付けられていない場合は、「使用可能」、「計画済み」、「実績時間」または「工数」が **ロールなし** 」セクションに入力します。\
   ユーザービューをリソースプランナーに適用する際に表示されるフィールドと項目の詳細は、 [リソースプランナーのナビゲーションの概要](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## リソースプランナーのユーザービューに表示されるフィールドの概要

次の表を参照して、リソース・プランナの「ユーザー」ビューに表示される情報を確認します。 この情報は、「時間」または「工数」の値で表示されます。

* [AVL (Available) 列](#the-avl-available-column)
* [「PLN （計画済み）」列](#the-pln-planned-column)
* [ACT （実際）列](#The%C2%A0ACT)
* [DIF（差異）列](#the-dif-difference-column)
* [「割合（計画時間割り当て率）」列](#the-planned-hours-allocation-percentage-column)

### AVL (Available) 列 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示者</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td>ユーザーのスケジュールに従った、ユーザーの使用可能な時間数または工数の合計。 </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>この情報は、リソースプランナーにユーザービューを適用する場合は、プロジェクトでは利用できません。 </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>ユーザーと <strong>FTE の可用性の割合</strong> 役割の</p> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー</td> 
   <td>この情報は、タスクまたはイシューでは使用できません。 </td> 
  </tr> 
 </tbody> 
</table>

ユーザーのスケジュールと役割の FTE 可用性の割合に基づくユーザーと役割の可用性の計算方法の詳細については、 [リソース・プランナのユーザーとロールの時間と工数の計算の概要](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### 「PLN （計画済み）」列 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示者</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> すべてのプロジェクトでユーザーに割り当てられたすべてのタスクまたは問題からの計画時間または工数の合計です。<br><p>これには、ユーザーに割り当てられ、どのジョブの役割にも関連付けられていないタスクやタスク、または管理するアクセス権のあるプロジェクトにないタスクやタスクが含まれます。</p><p>ワークロード・バランサを使用して時間のユーザー割り当てを変更した場合、選択した日付にタスクまたは問題の一部のみが含まれている場合は、リソース・プランナのデータに影響が及ぶ可能性があります。 ユーザーの割当ての変更の詳細は、 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a> . </p></td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> プロジェクト上の特定のユーザーに割り当てられたすべてのタスクおよびタスクからの計画時間数または工数の合計です。<br><p>注意：これには、どのユーザーにも割り当てられていないタスクや問題に関する計画時間や工数は含まれません。 </p></td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>プロジェクトのこの役割でユーザーに割り当てられたすべてのタスクおよびタスクからの計画時間数または工数の合計です。</p> <p> <p>注意：この役割に割り当てられているが、この役割のこのユーザーには割り当てられていないタスクや問題の予定時間や工数は含まれません。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー</td> 
   <td>プロジェクトのタスクまたは問題に関連付けられた計画時間または工数。</td> 
  </tr> 
 </tbody> 
</table>

計画時間を表示する際は、次の点を考慮してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* 計画時間は、タスクとタスクの期間内の各日に、割り当てられたリソースに対して均等に配分されます。 タスクまたは問題の期間は、計画開始日と完了日に基づき、その期間内の各カレンダー日が含まれます。\
   Workfrontは、ユーザーまたはプロジェクトに予定時間を配分する際に、ユーザーまたはプロジェクトのスケジュールを考慮に入れます。 この場合、計画時間は、週末、休日、スケジュール例外を除くタスクまたは問題の期間内に各日に均等に配分されます。

   たとえば、リソース・プランナを週別に表示し、プロジェクトに複数週間のタスクがある場合、1 週間の予定時間数は、その週内の日数がタスク期間の一部であるかどうかによって異なります。 これは、「月別」または「四半期別」で「生産資源プランナ」を表示する場合と、タスクが複数の月または四半期にまたがる場合に同様に機能します。\
   週末、スケジュールの例外、およびタイムオフ日は、この配分から除外されます。

* 各リソースの予定時間の計算には、次のタスクのカテゴリが含まれます。

   * リソースプール、ジョブロール、またはプロジェクトのチームでユーザーに割り当てられたタスク。

      >[!TIP]
      >
      >タスクがチームに割り当てられると、その割り当てが以下に表示されます。 **ロールなし** および **ユーザーなし** セクション。 チームに関連付けられた「計画時間」は表示できますが、役割もユーザーもタスクに関連付けられていないので、時間を予算できません。

* 生産資源計画担当の計画時間には、次に関連する計画時間は含まれません。

   * 親タスク
   * 未割り当てタスク
   * 問題、 **問題からの時間数を含める** の設定は無効です。

* タスクまたは発行期間がゼロの場合、計画時間はリソース・プランナに表示されません。
* 非アクティブなユーザーに関連付けられた計画時間は表示されません。

リソース・プランナの計画時間と工数の詳細は、次を参照してください： [リソースプランナーのプロジェクトビューとロールビューの時間、工数、コスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### ACT （実際）列

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示者</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー </td> 
   <td> <p>ユーザーが割り当てられたすべてのタスクまたはタスクに関して記録した時間。</p> <p>これには以下が含まれます。</p> 
    <ul> 
     <li>ユーザーに割り当てられ、ジョブの役割に関連付けられていないタスクとタスク。</li> 
     <li>「管理」へのアクセス権を持つプロジェクトにないタスクとタスク。 </li> 
    </ul> <p>これには、ユーザーがそのプロジェクトのタスクまたはタスクに割り当てられている場合にのみ、プロジェクトにログオンした時間が含まれます。  </p> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト </td> 
   <td> <p>ユーザーがプロジェクトに割り当てられたすべてのタスクとタスクに関して記録した時間。</p> <p>これには、ユーザーがプロジェクトに直接ログオンした時間も含まれます。</p> <p>これには次のものは含まれません。</p> 
    <ul> 
     <li> <p>どのユーザーにも割り当てられていないタスクと問題にログオンした時間。 </p> </li> 
     <li> <p>親タスクにログオンした時間。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>この役割のユーザーに割り当てられたすべてのタスクまたは問題にログオンした時間。 </p> <p>これには次のものは含まれません。</p> 
    <ul> 
     <li>この役割に割り当てられたタスクとタスクにログオンした時間（この役割のこのユーザーには割り当てられません）。</li> 
     <li>プロジェクトまたは親タスクに直接記録された時間。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー </td> 
   <td> <p>タスクとタスクに割り当てられているユーザーによるタスクとタスクにログオンした時間。 </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>記録される時間は、時間が記録されるタスク、問題、またはプロジェクトの期間に関係なく、時間の入力日に対応する時間枠で表示されます。

実際の時間について詳しくは、 [実際の時間の表示](../../manage-work/tasks/task-information/actual-hours.md).

### DIF（差異）列 {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示者</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>ユーザーの利用可能時間と計画時間または工数の違い。 </p> <p>時間または工数の差異は、次の数式で計算されます。</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>注意：値が負の赤い数字で表示される場合、ユーザーは割り当て超過になります。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>この情報は、プロジェクトでは使用できません。 </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>ジョブロールの使用可能時間と計画時間、または工数の違い。 </p> <p>時間または工数の差異は、次の数式で計算されます。</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>注意：値が負の赤い数字で表示されている場合、役割は割り当て超過になります。 </p> </p> </td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー</td> 
   <td>この情報は、タスク、タスク、またはプロジェクトでは使用できません。 </td> 
  </tr> 
 </tbody> 
</table>

### 「割合（計画時間割り当て率）」列 {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示者</strong> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>使用可能時間に対する計画時間または工数の割当て。 計画時間配分の割合は、次の式を使用して計算されます。</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>FTE 値にも同じ計算が使用されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td>この情報は、 <strong>ユーザー別に表示</strong> 「生産資源プランナ」に表示します。</td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> 使用可能時間に対する計画時間または工数の割当て。 <p>計画時間配分の割合は、次の式を使用して計算されます。</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>FTE 値にも同じ計算が使用されます。</p></td> 
  </tr> 
  <tr> 
   <td>タスクまたはイシュー</td> 
   <td>この情報は、タスク、タスク、またはプロジェクトでは使用できません。 </td> 
  </tr> 
 </tbody> 
</table>

計画時間または工数の値がゼロの場合、割合配分は 0%になります。 Available Hours または FTE の値がゼロの場合、割合配分は計算できません。

計画時間と工数、および生産資源プランナでの表示方法の詳細は、次を参照してください： [「プロジェクト」ビューと「ロール」ビューを使用する、リソースプランナーの予算リソース](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

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
