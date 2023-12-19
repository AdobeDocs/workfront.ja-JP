---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: リソース管理の概要
description: リソース管理を使用すると、システムの可用性に基づいてリソースの使用状況を正確に予測し、必要な作業を時間通りに予算通りに完了するようにシステムを設定できます。
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 0%

---

# リソース管理の概要

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

リソース管理を使用すると、システムの可用性に基づいてリソースの使用状況を正確に予測し、必要な作業を時間通りに予算通りに完了するようにシステムを設定できます。

## Adobe Workfrontのリソース管理の概要

リソース管理とは、Adobe Workfront管理者、リソースマネージャーおよびプロジェクト所有者が組織のリソースを計画およびスケジュール（ワークロードバランサー）し、使用可否を考慮して実行する作業に割り当てるために実行するすべてのアクティビティを指します。 また、生産資源管理では、計画生産資源割当および実績生産資源割当に関する情報をレポート・ビュー（稼働状況レポート）で表示することも指します。

Workfrontには、リソースの管理に使用されるツールのセットがいくつか用意されています。 各ツールには個々のスコープがあります。 現在、現在使用しているリソース管理のステージに応じて、Workfrontで次のリソース管理ツールを使用できます。

* プロジェクトでの実際の作業を開始する前に、より高いレベルでリソースを割り当てる方法を計画するには、次のツールを使用します。

   * **リソースプランナー**：リソース管理の最初のステージでリソースプランナーを使用して、予定されている可用性に応じて、リソースのプロジェクト時間を予算できます。 リソースの計画段階では、リソースプール内のユーザーを整理し、複数のリソースプールをプロジェクトに割り当てることができます。

     リソース計画の詳細は、「 [Adobe Workfrontでのリソース計画](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **シナリオプランナー**：これは、リソースの高レベルな計画で、1 年、3 年、5 年のプランにまたがる複数のイニシアチブ全体でリソースを管理でき、複数のプロジェクトを含めることができます。 最適なシナリオを使用して、可用性と予算を最大限に活用できます。

     シナリオプランナーには、Workfrontライセンスに加えて、別のライセンスが必要です。 Workfront Scenario Planner の詳細は、 [シナリオプランナーの概要](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* リソースを実際の作業（タスクとタスク）にスケジュールまたは割り当てるには、次のツールを使用します。

   * **ワークロードバランサー**：リソース管理の下位レベルの段階に属しており、リソースの完了に必要な時間数と使用可否に基づいて、リソースを完了する必要がある実際の作業（タスクと問題）に割り当てることができます。 ワークロード・バランサを使用して、現在割り当てられていない、またはジョブ・ロールに割り当てられている実際の作業にユーザーを割り当てることができます。

     Workfront Balancer について詳しくは、 [ワークロードバランサー：記事インデックス](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* 複数のプロジェクトに対する予算割当、計画割当および実績割当を分析するには、次のツールを使用します。

   * **使用率レポート**：このレポートを使用して、プロジェクトのリソースの使用率を表示します。 プロジェクトに対する予算、計画および実際の配賦と、プロジェクトのコストおよび収益に対する影響を比較できます。

     使用率レポートの詳細は、 [リソース使用率情報の表示](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## リソース管理プロセスのコンポーネント

>[!NOTE]
>
>リソース管理は、Workfrontでのプロセスの停滞ではありません。 プロジェクトのスケジュール、ユーザーの可用性、またはユーザーの役割が変化すると、リソース、割り当て、およびプロジェクト、タスク、タスクへの割り当てに関する情報を継続的に調整する必要があります。

Workfrontでのリソース管理プロセスには、次の段階があります。

* **設定**：システム管理者、リソースマネージャーまたはプロジェクト所有者は、リソースを管理する前に、Workfrontインスタンスで特定のフィールドとオブジェクトを設定する必要があります。 Workfrontでのリソース管理の開始に必要な前提条件について詳しくは、 [正確なリソース管理の前提条件](#prerequisites-for-accurate-resource-management) 」の節を参照してください。\
  作業項目を含むプロジェクトを作成するに加えて、Workfrontで次の項目を設定する必要があります。

   * ユーザー\
     ユーザーの作成について詳しくは、 [ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * 担当業務\
     ジョブの役割の作成について詳しくは、この記事を参照してください。 [ジョブの役割の作成と管理](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * スケジュール\
     スケジュールの作成について詳しくは、「 [スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * プロジェクト環境設定

     >[!TIP]
     >
     >システムまたはグループのプロジェクト環境設定を変更できるのは、システムまたはグループ管理者だけです。

     プロジェクトの環境設定の定義の詳細については、「 [システム全体のプロジェクト環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * リソース プール

     リソースプールの作成の詳細については、「 [資源プールの作成](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * リソース管理環境設定

     システムとして、Workfrontがユーザーのスケジュールとシステムのデフォルトスケジュールのどちらを使用しているかに関わらず、システムレベルでユーザーの可用性を計算する方法を決定する必要があります。

     詳しくは、 [リソース管理環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **リソースの割り当て**：リソースマネージャーまたはプロジェクト所有者として、プロジェクトに対するリソースの割り当てを定義し、作業を割り当てることができます。 この手順では、リソース・プランナまたはシナリオ・プランナを使用して、リソースの割り当て見積を管理し、ワークロード・バランサのユーザーに実績作業を割り当てることができます。

  リソース計画と作業の割り当ての詳細は、次の項を参照してください。

   * [Adobe Workfrontでのリソース計画](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront Scenario Planner](../../scenario-planner/scenario-planning.md)
   * [ワークロードバランサー：記事インデックス](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **分析**：リソースマネージャ、プロジェクト所有者または担当者マネージャとして、使用率レポートをレビューして、リソースの予算割当ておよび計画割当てを実際の割当てと比較する方法を理解します。 時間、コスト、売上高別に情報を確認します。 使用率レポートについて詳しくは、 [リソース使用率情報の表示](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Workfrontのリソース管理ツールを使用して、リソースを表示および管理するために必要なアクセス

次のユーザーは、Workfrontのリソース管理ツールにアクセスできます。

リソース管理ツールにアクセスするには、次のユーザーの 1 人で、次のアクセス権と権限を持っている必要があります。

* システム管理者。
* プランライセンスを持つユーザー。

  作業ライセンスを持つユーザーは、プロジェクトのワークロードバランサーを使用し、割り当てと割り当てを管理できます。

  Work 以上のライセンスを持つに加え、特定のリソース管理ツールを使用するには、次の手順を実行する必要があります。

   * リソース管理へのアクセスを編集（ワークロードバランサーでの割り当てには不要）
   * 財務データへのアクセスを編集して、リソース・プランナにコスト情報を表示します。
   * 財務データへのアクセスを表示して、使用率レポートに原価と収益の情報を表示します（プラン・ライセンスを持つユーザーのみ）

* リソースを管理するプロジェクトで割り当てを行う権限を含む、Contribute 以上の権限。

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

予算リソースに必要なアクセスの詳細については、「 [予算リソースに必要なアクセス](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

ワークロード・バランサでリソースを管理するために必要なアクセスの詳細は、 [ワークロードバランサーでリソースを管理するために必要なアクセス](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## 正確なリソース管理の前提条件  {#prerequisites-for-accurate-resource-management}

Workfrontのリソース管理ツールを効率的に使用するには、一連の要件を満たす必要があります。

Workfrontの各リソース管理ツールの要件について詳しくは、次を参照してください。

* セクション [リソース・プランナでの作業の前提条件](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) 記事内 [リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* セクション [ワークロードバランサーの使用に関するベストプラクティス](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) 記事内 [ワークロードバランサーの概要](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Adobe Workfrontの予算リソースに必要なアクセス](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [ワークロードバランサーでリソースを管理するために必要なアクセス](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
