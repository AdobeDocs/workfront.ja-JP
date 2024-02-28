---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: リソース管理 の概要
description: リソース管理を使用すると、リソースの空き時間に基づいてリソースの使用状況を正確に予測し、完了すべき作業を時間どおり、かつ予算どおりに完了するようにシステムを設定できます。
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 94%

---

# リソース管理 の概要

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

リソース管理を使用すると、リソースの空き時間に基づいてリソースの使用状況を正確に予測し、完了すべき作業を時間どおり、かつ予算どおりに完了するようにシステムを設定できます。

## Adobe Workfront でのリソース管理の概要

リソース管理とは、Adobe Workfront 管理者、リソースマネージャーおよびプロジェクト所有者が、組織のリソースを計画（リソースプランニングまたはシナリオプランニング）およびスケジュール（ワークロードバランサー）し、リソースの空き時間を考慮して、完了する必要がある作業にリソースを割り当てるために実行するすべてのアクティビティを指します。さらに、リソース管理とは、レポートビュー（稼働率レポート）で、計画されたリソース割り当てと実際のリソース割り当てに関する情報を表示することも指します。

Workfront には、リソースの管理に使用されるツールが数セット用意されています。各ツールには個々のスコープがあります。現在、リソース管理のどの段階にあるかに応じて、Workfront で以下のリソース管理ツールを使用できます。

* プロジェクトでの実際の作業を開始する前に、より高いレベルでリソースを割り当てる方法を計画するには、以下のツールを使用します。

   * **リソースプランナー**：リソース管理の最初のステージでリソースプランナーを使用して、予定の空き時間に応じて、リソースのプロジェクト時間を計上できます。リソースの計画段階では、リソースプール内でユーザーを編成し、複数のリソースプールをプロジェクトに割り当てることができます。

     リソース計画の詳細は、「 [リソース計画：記事インデックス](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **シナリオプランナー**：これはリソースのより高度なレベルの計画で、1 年、3 年、5 年にまたがる計画の複数のイニシアチブにわたってリソースを管理でき、複数のプロジェクトを含めることができます。最適なシナリオを使用して、空き時間と予算を最大限に活用できます。

     シナリオプランナーには、Workfront ライセンスに加えて、別のライセンスが必要です。Workfront Scenario Planner について詳しくは、[Scenario Planner の概要](../../scenario-planner/scenario-planner-overview.md)を参照してください。

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* リソースを実際の作業（タスクとイシュー）にスケジュールする、または割り当てるには、以下のツールを使用します。

   * **ワークロードバランサー**：リソース管理の下位レベルの段階に属しており、完了するために必要な時間数とリソースの空き時間に基づいて、完了する必要がある実際の作業（タスクとイシュー）にリソースを割り当てることができます。ワークロードバランサーを使用して、現在割り当てられていない、または担当業務に割り当てられている実際の作業に、ユーザーを割り当てることができます。

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
* 複数のプロジェクトに対する予算計上された割当、予定割当および実際の割当を分析するには、以下のツールを使用します。

   * **稼動率レポート**：このレポートを使用して、プロジェクトのリソースの稼動率を表示します。プロジェクトに対する予算計上された割当、予定割当および実際の割当と、プロジェクトのコストおよび収益に対する影響を比較できます。

     稼動率レポートについて詳しくは、[リソース稼動率情報を表示](../../resource-mgmt/resource-utilization/view-utilization-information.md)を参照してください。

## リソース管理プロセスのコンポーネント

>[!NOTE]
>
>Workfront では、リソース管理が停滞するプロセスになることは、決してありません。プロジェクトのスケジュール、ユーザーの空き時間やユーザーの役割が変化するにつれて、リソースとその割り当て、およびリソースのプロジェクト、タスク、イシューへの割り当てに関する情報を継続的に調整する必要があります。

Workfront でのリソース管理プロセスには、以下の段階があります。

* **設定**：システム管理者、リソースマネージャーまたはプロジェクト所有者は、リソースを管理する前に、Workfront インスタンスで特定のフィールドとオブジェクトを設定する必要があります。Workfront でのリソース管理の開始に必要な前提条件について詳しくは、この記事にある[正確なリソース管理の前提条件](#prerequisites-for-accurate-resource-management)の節を参照してください。\
  Workfront では、作業アイテムを含むプロジェクトに加え、以下の項目を設定する必要があります。

   * ユーザー\
     ユーザーの作成について詳しくは、[ユーザーの追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)の記事を参照してください。

   * 担当業務\
     担当業務の作成について詳しくは、[担当業務の作成と管理](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)の記事を参照してください。

   * スケジュール\
     スケジュールの作成について詳しくは、[スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)の記事を参照してください。

   * プロジェクト環境設定

     >[!TIP]
     >
     >システム管理者またはグループ管理者のみが、システムまたはグループのプロジェクトの環境設定を変更できます。

     プロジェクトの環境設定の定義について詳しくは、[システム全体のプロジェクトの環境設定を指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)の記事を参照してください。

   * リソースプール

     リソースプールの作成について詳しくは、[リソースプールを作成](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)を参照してください。

   * リソース管理の環境設定

     システムとして、ユーザーのスケジュールとシステムのデフォルトスケジュールのどちらを使用しているかに関わらず、Workfront がシステムレベルでユーザーの空き時間を計算する方法を決定する必要があります。

     詳しくは、[リソース管理の環境設定を設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

* **リソースの割り当て**：リソースマネージャーやプロジェクト所有者は、プロジェクトに対するリソースの割り当てを定義し、作業を割り当てることができます。この手順では、リソースプランナーまたはシナリオプランナーを使用して、リソースの割り当て見積もりを管理し、ワークロードバランサーのユーザーに実際の作業を割り当てることができます。

  リソース計画と作業の割り当てについて詳しくは、以下の節を参照してください。

   * [リソース計画：記事インデックス](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Adobe Workfront シナリオプランナー](../../scenario-planner/scenario-planning.md)
   * [ワークロードバランサー：記事インデックス](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **分析**：リソースマネージャ、プロジェクト所有者または管理職として、稼動率レポートをレビューして、リソースの予算計上配分および予定配分が実際の配分と比較してどうかを理解します。時間数、コスト、収益別に情報をレビューします。稼動率レポートについて詳しくは、[リソース稼動率情報の表示](../../resource-mgmt/resource-utilization/view-utilization-information.md)を参照してください。

## Workfront のリソース管理ツールを使用してリソースを表示および管理するために必要なアクセス

次のユーザーは、Workfront のリソース管理ツールにアクセスできます。

リソース管理ツールにアクセスするには、次のいずれかのユーザーであり、次のアクセス権と権限を持っている必要があります。

* システム管理者。
* プランライセンスを持つユーザー。

  ワークライセンスを持つユーザーは、プロジェクトのワークロードバランサーを使用して、割り当てと配分を管理できます。

  特定のリソース管理ツールを使用するには、ワーク以上のライセンスに加え、次のアクセス権が必要です。

   * リソース管理に対する編集アクセス権（ワークロードバランサーで割り当てを行う場合は不要）
   * リソースプランナーでコスト情報を表示するための、財務データに対する編集アクセス権
   * 稼動率レポートでコストおよび収益の情報を表示するための、財務データに対する表示アクセス権（プランライセンスを持つユーザーのみ）

* リソース管理の対象となるプロジェクトでの割り当ての作成を含む、参加以上の権限。

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

リソース予算計上に必要なアクセス権について詳しくは、[リソース予算計上に必要なアクセス権](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)の記事を参照してください。

ワークロードバランサーでのリソースの管理に必要なアクセス権については、[ワークロードバランサーでのリソース管理に必要なアクセス権](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md)を参照してください。

## 正確なリソース管理の前提条件  {#prerequisites-for-accurate-resource-management}

Workfront のリソース管理ツールを効率的に使用するには、一連の要件を満たす必要があります。

Workfront の各リソース管理ツールの要件について詳しくは、以下を参照してください。

* セクション [リソース・プランナでの作業の前提条件](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) 記事内 [リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* セクション [ワークロードバランサーの使用に関するベストプラクティス](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) 記事内 [ワークロードバランサーの概要](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Adobe Workfront でのリソース予算計上に必要なアクセス](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)。
* [ワークロードバランサーでリソースを管理するために必要なアクセス](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md)。

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
