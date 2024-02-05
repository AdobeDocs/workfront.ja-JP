---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: リソース計画の概要
description: リソース計画ツールを使用して、担当業務、空き時間、およびこの空き時間に基づくプロジェクトへの一般的な割り当てを管理できます。
author: Alina
feature: Resource Management
exl-id: 0db9fbb3-4e94-47bd-b272-00b3ca4decaf
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 97%

---

# リソース計画の概要

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(**** THIS WILL BE LINKED TO THE PRODUCT UI IN THE PLANNER AREA***DO NOT DELETE OR CHANGE URL FOR THIS ARTICLE****) </p>
<p>(Alina ***Keep the pink blurb for all articles in this NEW section.***More prerequisites for Users (with later releases): - users have an accurate number for their FTE field; The Prerequisites section: (this is linked to other articles, do not change name and link/ anchor))</p>
</div>
-->

Adobe Workfront のリソース管理ツールを使用してリソースの配分を予測し、プロジェクトが予定と予算どおりに納品されたかを正確に把握できます。Workfront のリソース管理の概要については、[リソース管理の概要](../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)を参照してください。

リソース計画ツールを使用して、担当業務、空き時間、およびこの空き時間に基づくプロジェクトへの一般的な割り当てを管理できます。

プロジェクトへのユーザーの一般的な割り当てを予算計上しても、実際の作業（タスクとイシュー）には割り当てられません。ワークロードバランサーを使用して、作業するリソースを割り当てる必要があります。

ワークロードバランサーを使用したWorkfrontでのリソースのスケジュール設定の詳細については、 [ワークロードバランサーの概要](../workload-balancer/overview-workload-balancer.md).

## Workfront のリソース計画ツール

割り当て予定のプロジェクトにリソースの時間を割り当てるには、次のツールを使用します。

* 複数のプロジェクトに対する予算割り当てを行い、システムレベルで優先順位を付ける場合：システムレベルのリソースプランナーを使用します。

  リソースプランナーにアクセスするには、「リソース」エリアの「プランナー」セクションに移動します。

  リソースプランナーについて詳しくは、[リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

* 単一プロジェクトに対する予算割り当ての場合：プロジェクトのビジネスケースの「リソース予算計上」エリアで、プロジェクトレベルのリソースプランナーを使用します。1 つのプロジェクトのリソースの予算計上について詳しくは、[ビジネスケースのリソース予算計上](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。

  共通のスキルや部門構造に基づいてユーザーを管理し、それらをプールに整理し、割り当て先のプロジェクトに対する配分を管理するには、リソースプールを作成する必要があります。リソースプールの作成について詳しくは、[リソースプールの作成](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)を参照してください。

  >[!TIP]
  >
  >プロジェクトの「リソース予算計上」領域は、プロジェクトレベルのリソースプランナーです。プロジェクトのビジネスケースでリソースの予算計上をする場合、その情報はシステムレベルのリソースプランナーにも反映されます。

* 複数のイニシアチブにわたる高レベルでリソースを管理し、作業を組織の戦略に合わせるには、Adobe Workfront シナリオプランナーを使用します。シナリオプランナには、追加のライセンスが必要です。Workfront シナリオプランナーについて詳しくは [シナリオプランナーの概要](../../scenario-planner/scenario-planner-overview.md)を参照してください。

  リソースプランナーは、システムレベルで、複数のプロジェクトにわたって、また、ビジネスケースの「リソース予算計上」領域で、1 つのプロジェクトに対してのリソース予算計上の両方で使用できます。ビジネスケースでのプロジェクトのリソース予算計上について詳しくは、[ビジネスケースのリソース予算計上](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。

## リソース計画ツールの目的

* リソースプランナーを使用して、次の操作を実行できます。

   * プロジェクトに優先順位を付け、最初にリソースを受け取るプロジェクトを決定します。（リソースプランナー内のみ）
   * ユーザーのスケジュールに基づいて、リソースの空き時間を把握します。
   * 割り当て先のプロジェクトのリソース（ユーザーおよび担当業務）に対する時間、FTEまたはコストの配分を予算計上します。

  リソースプランナーでの作業について詳しくは、[リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)の記事を参照してください。

* シナリオプランナーを使用すると、複数のイニシアチブにわたる企業レベルの計画を構築し、企業全体の戦略的成果を概説することができます。詳しくは、[シナリオプランナーの概要](../../scenario-planner/get-started-with-scenario-planning.md)を参照してください。

  シナリオプランナには、追加のライセンスが必要です。Workfront シナリオプランナーについて詳しくは、[シナリオプランナーの概要](../../scenario-planner/scenario-planner-overview.md)を参照してください。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Prerequisites for resource planning</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This section drafted because it was moved to the "Resource Planner overview" article instead. But this used to be true: THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To successfully use the Resource Planner for budgeting your resources, you must first ensure that you, your projects, and your tasks meet a set of prerequisites. These prerequisites are mandatory to display the correct information in the Resource Planner and to accurately manage your resources. </p>
-->

<!--
<note type="important">  If any of the following prerequisites are missing, you might find that some of the information about the allocation or the availability of the resources is missing or has a zero value.
<br>For more information understanding why fields are missing data or have zero values, hover over the fields.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/no-users-with-this-role-in-the-res-pool-350x57.png" style="width: 350;height: 57;"> </p>
-->

<!--
<note type="note">
The following prerequisites are required only when viewing the Resource Planner by project or by job role or when budgeting resources in the Business Case of a project.
<br>For more information about the views in the Resource Planner, see the "Project/ Role/ User view" selection section in the article
<a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.
<br>
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following types of prerequisites are required for the correct functionality of the Resource Planner: </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user-prerequisites" class="MCXref xref">User prerequisites</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#project-prerequisites" class="MCXref xref">Project prerequisites</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#tasks-and-issues-prerequisites" class="MCXref xref">Tasks and issues prerequisites</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user-prerequisites">User prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following user setup exists before starting using the Resource Planner:</p>
<li>  <ul>   <li> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have the correct access to budget resources.</p><p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p>   </li>  </ul> </li>
-->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Users who are assigned to tasks are added to the Resource Pools associated with the project.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about adding users to Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a> and <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</p>
  -->

<!--
  >[!NOTE]
  >
  >
  >
  ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">When users are not added to Resource Pools, the following scenarios may exist: </p>  >
  >
  >
  >   
  >   
  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">The users do not appear in the Resource Planner although they might be assigned to tasks on the projects. </li>  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">If the tasks they are associated with have Planned Hours, those hours do not appear for the project in the Resource Planner, unless the user is also associated with a job role on those tasks. </li>  >   
  >     <li style="font-style: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">If the users are associated with a job role on a task on the project, the Planned Hours display in the Resource Planner for the job role, but the job role cannot be budgeted. </li>  >
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Users who are assigned to work and Resource Pools must have Schedules and Job Roles associated with their profile.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about associating Schedules and Job Roles with users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Add users</a></p>
  -->

<!--
  <note type="note">  Users who are not associated with a Schedule but are in the Resource Pool of the project cannot be budgeted in the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For accurate Available Hours information, ensure that the schedules associated with your users have the schedule exceptions and time off updated.</p>
  -->

<!--
  <note type="note">  If a user is not associated with a Schedule, the Default Schedule of your Workfront system is associated with the user by default, for the purposes of the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about creating schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.<br></p>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If you want to budget your resources by Cost, you must associate Job Roles with Cost/Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.<br>For information about associating job roles with rates, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.<br>For information about calculating Budgeted Labor Cost, see the article <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>.<br>For information about calculating Budgeted Cost, see the article <a href="../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calculate Budgeted Cost</a>.</li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="project-prerequisites">Project prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following project setup exists before starting using the Resource Planner:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> Your projects are associated with Resource Pools.<br>For more information about adding Resource Pools to projects, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref">Associate resource pools with projects and templates</a>.<br>
  <note type="important">  Projects without Resource Pools do not display Planned Hour or assignments information in the Resource Planner.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You have the correct access to budget resources.</p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="tasks-and-issues-prerequisites">Tasks and issues prerequisites</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Ensure the following tasks and issues setup exists before starting budgeting resources in the Resource Planner:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> The tasks or issues on the projects for which you are budgeting resources are assigned to one of these entities:<br>
  <ul>
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Users in the Resource Pools of the project who are also associated with Job Roles</li>
  <li>
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Job Roles</p>
  </li>  
  </ul>
  <note type="note">
  Teams assigned to tasks or issues do not display in the Resource Planner. The Planned Hours of tasks and issues assigned to job roles display in the Resource Planner, but these hours cannot be budgeted unless a user who is associated with the job role is listed in a Resource Pool associated with the project.
  </note>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Parent tasks should not be assigned to users or roles. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">This will impact the value of Planned Hours for the project. </p>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Tasks and issues have a value for Planned Hours which is greater than zero. </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Tasks and issues have a value for their Duration which is greater than zero. </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Planned Dates of the issues are within the timeline of the project. </li>
  -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Access resource planning tools in&nbsp;Workfront</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can access the Planner from the  People Planner section  of the Resourcing area. </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about accessing the Planner, see <a href="../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Create Resource Pools</h2>
<p>(drafted because it's redundant with the user prerequisites above) </p>
<p>You can manage your user resources by adding users to Resource Pools. Having users organized in Resource Pools and associating the pools with your projects are prerequisites to Resource Planning.</p>
<p>For information about adding users to Resource Pools and associating them with projects, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a> and <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associate resource pools with users </a>.</p>
</div>
-->
