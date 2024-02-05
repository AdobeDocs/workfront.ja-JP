---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: リソースプランナーの概要
description: リソースプランナーを使用すると、リソースが割り当てられているプロジェクトへのリソースの割り当てを見積もって予算を計上し、将来の作業に使用できるリソースを予測できます。
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: 1c8d9a62f5582b0dbc3c72b5881bb5d8f0b790ba
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 97%

---

# リソースプランナーの概要

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

リソースプランナーを使用すると、リソースが割り当てられているプロジェクトへのリソースの割り当てを見積もって予算を計上し、将来の作業に使用できるリソースを予測できます。

Adobe Workfront でのリソースプランの概要について詳しくは、[リソースプランの概要](../../resource-mgmt/resource-planning/get-started-resource-planning.md)の記事を参照してください。

## リソースプランナーの概要

リソースプランナーを使用すると、ユーザーや担当業務の空き状況、プロジェクトの作業を完了するために必要な予定時間を簡単に把握できます。その後、ユーザーの利用可能な時間に基づいて、ユーザーとそのユーザーが割り当てられているプロジェクトでの担当業務をどのように割り当てるのかを決定できます。

>[!IMPORTANT]
>
>リソースプランナーを使用して、実際の作業（タスクとイシュー）をユーザーに割り当てることはできません。割り当てられているタスクやイシューにかかわらず、ユーザーまたは担当業務がプロジェクトを完了するのに必要な時間のみを見積もることができます。\
>実際の作業をユーザーに割り当てるには、ワークロードバランサーを使用する必要があります。ワークロード・バランサの詳細は、 [ワークロードバランサーの概要](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

リソースプランナーでは、3 つの異なるビューを使用して情報を表示できます。各ビューを使用して、次の目的のいずれかを実行できます。

* プロジェクトビューと役割ビューを使用して、実行する必要がある作業に割り当てるリソースの時間またはコストの予算を計上します。これが、リソースプランナーの主な目的です。\
  リソースプランナーでの予算計上について詳しくは、[プロジェクトビューと役割ビューを使用したリソースプランナーでのリソースの予算計上](../resource-planning/budget-resources-project-role-views-resource-planner.md)の記事を参照してください。

* ユーザービューを使用して、次の情報を表示できます。

   * スケジュールに従ったユーザーの可用性
   * プロジェクト計画に従って作業を完了するのに必要な予定時間
   * ユーザーが実際の作業項目に既にログオンしている時間

  リソースプランナーでのユーザーの利用可能時間数、予定時間数、実際の時間数または FTE の表示について詳しくは、[ユーザービューを使用したリソースプランナーでの利用可能時間数、予定時間数、実際の時間数または FTE の表示](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using)の記事を参照してください。

## リソースプランナーの考慮事項

* 取り組んでいるプロジェクトに優先順位を付け、その優先順位に従ってリソース割り当ての予算を立てることで、最も重要なプロジェクトにリソースを最初に割り当てることができます。

  リソースプランナーでのプロジェクトの優先順位付けについて詳しくは、[リソースプランナーでのプロジェクトの優先順位付け](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)を参照してください。

* プロジェクトのタスクやイシューの時間、FTE、コストの情報を表示できます。

  >[!NOTE]
  >
  >タスクとイシューはリソースプランナーには表示されません。ただし、タスクへのリソースの割り当ての時間、FTE、コストの情報は、プロジェクトの合計数としてリソースプランナーに表示されます。

* 親タスクの時間、FTE、コストの情報は、リソースプランナーに表示されるプロジェクトから除外されます。リソースプランナーでリソースの時間やコストを管理する場合、子タスクにのみリソースを割り当てることをお勧めします。

  親タスクについて詳しくは、次の記事を参照してください。

   * [タスクの概要](../../manage-work/tasks/task-information/tasks-overview.md)
   * [サブタスクを作成](../../manage-work/tasks/create-tasks/create-subtasks.md)

  >[!TIP]
  >
  >親タスクには、子タスクの時間とコストの合計が表示されます。このため、子タスクと親タスクから時間、FTE、コストをカウントすると、これらの金額が 2 回カウントされます。これが、親タスクの情報がリソースプランナーから除外される理由です。

* リソースプランナーでは、タスクやイシューがあるプロジェクトに対するチームの割り当てを管理できません。
* リソースプランナーを使用して一度に複数のプロジェクトのリソースの予算を計上することも、ビジネスケースのリソース予算計上領域を使用して単一のプロジェクトのリソースの予算を計上することもできます。1 つのプロジェクトの予算情報もリソースプランナーに表示されます。

  単一のプロジェクトのリソースの予算計上について詳しくは、[ビジネスケースのリソースの予算計上](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)の記事を参照してください。

  リソースプランナーで一度に複数のプロジェクトのリソースの予算を計上することについて詳しくは、[プロジェクトビューと役割ビューを使用したリソースプランナーのリソースの予算計上](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)の記事における「リソースプランナーでのリソースの予算計上」セクションを参照してください。

## リソースプランナーでの作業の前提条件 {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

リソースプランナーを使用してリソースの予算を計上するには、まず自分、プロジェクト、タスクが一連の前提条件を満たしていることを確認する必要があります。これらの前提条件は、リソースプランナーで正しい情報を表示し、リソースを正確に管理するために必須です。

>[!IMPORTANT]
>
>次の前提条件のいずれかが満たされていない場合、リソースの配分または空き時間に関する情報の一部が欠落しているか、値がゼロになることがあります。\
>フィールドにデータが欠落している、または値がゼロである理由を詳しく理解するには、フィールドにポインタを合わせます。

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>次の前提条件は、リソースプランナーをプロジェクト別または担当業務別に表示する場合、またはプロジェクトのビジネスケースでリソースの予算を計上する場合にのみ必要です。

リソースプランナーをプロジェクトごとまたは役割ごとに表示するときに、リソースプランナーが正しく機能するには、次の種類の前提条件を満たす必要があります。

* [ユーザーの前提条件](#user-prerequisites)
* [プロジェクトの前提条件](#project-prerequisites)
* [タスクとイシューの前提条件](#tasks-and-issues-prerequisites)
* [システムレベルの前提条件](#system-level-prerequisites)

### ユーザーの前提条件 {#user-prerequisites}

リソースプランナーの使用を開始する前に、以下のユーザー設定が存在することを確認します。

* リソース予算計上の正しいアクセス権がある。

  リソース予算計上に必要なアクセス権について詳しくは、[Adobe Workfront でのリソース予算計上に必要なアクセス権](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)の記事を参照してください。

* タスクに割り当てられたユーザーは、プロジェクトに関連付けられたリソースプールに追加される。

  リソースプールにユーザーを追加する方法について詳しくは、[リソースプールとユーザーの関連付け](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md)を参照してください。

  >[!NOTE]
  >
  >ユーザーがリソースプールに追加されない場合、以下のシナリオが存在する可能性があります。
  >
  >   
  >   
  >   * ユーザーはプロジェクトのタスクに割り当てられているが、リソースプランナーには表示されない。
  >   * 関連付けられているタスクに予定時間数が設定されている場合、ユーザーがそれらのタスクの担当業務にも関連付けられていない限り、その時間数はリソースプランナーのプロジェクトに表示されない。
  >   * ユーザーがプロジェクトのタスクの担当業務に関連付けられている場合、その担当業務のリソースプランナーに予定時間数が表示されるが、担当業務は予算計上できない。
  >   
  >

* 作業およびリソースプールに割り当てられているユーザーは、自分のプロファイルに関連付けられたスケジュールと担当業務を持っている必要がある。

  スケジュールおよび担当業務とユーザーの関連付けについて詳しくは、[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

  >[!NOTE]
  >
  >スケジュールに関連付けられていないが、プロジェクトのリソースプールに存在するユーザーに関しては、リソースプランナーで予算を計上できません。

* 正確な利用可能時間数の情報を得るために、ユーザーに関連付けられたスケジュールで例外スケジュールと休暇がアップデートされている。

  >[!NOTE]
  >
  >ユーザーがスケジュールに関連付けられていない場合、Workfront システムのデフォルトのスケジュールは、リソースプランナーのために、デフォルトでユーザーに関連付けらます。

  スケジュールの作成について詳しくは、[スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)の記事を参照してください。

* コスト別にリソースの予算を計上したい場合は、担当業務をコスト/時間レートにに関連付ける必要がある。リソースプール内のユーザーに割り当てられた担当業務に関連付けられたコストは、プロジェクトの予算計上労力コストと予算計上コストの計算に使用されます。\
  担当業務とレートの関連付けについて詳しくは、[担当業務の作成および管理](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。\
  予算計上労力コストの計算について詳しくは、[プロジェクトの予算計上労力コストと予算計上時間数について](../../manage-work/projects/project-finances/budgeted-labor-cost.md)を参照してください。\
  予算計上コストの計算について詳しくは、[予算計上コストの計算](../../manage-work/projects/project-finances/budgeted-cost.md)を参照してください。

### プロジェクトの前提条件 {#project-prerequisites}

リソースプランナーを使い始める前に、以下のプロジェクト設定が存在することを確認してください。

* プロジェクトがリソースプールに関連付けられている。\
  プロジェクトへのリソースプールの追加について詳しくは、[リソースプールとプロジェクトおよびテンプレートの関連付け](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md)を参照してください。

  >[!IMPORTANT]
  >
  >リソースプールのないプロジェクトでは、リソースプランナーに予定時間数や割り当ての情報が表示されません。

### タスクとイシューの前提条件 {#tasks-and-issues-prerequisites}

リソースプランナーにタスクとイシューを表示することはできませんが、その情報はリソースプランナーに表示されるプロジェクトに転送されます。

リソースプランナーでリソースの予算計上を開始する前に、以下のようなタスクとイシューの設定が存在することを確認します。

* リソースを予算計上しているプロジェクトのタスクまたはイシューは、以下のエンティティのいずれかに割り当てられる。

   * プロジェクトのリソースプール内のユーザーで、担当業務にも関連付けられているユーザー
   * 担当業務

  >[!NOTE]
  >
  >担当業務に割り当てられたタスクの予定時間数とタスクおよびイシューはリソースプランナーに表示されますが、担当業務に関連付けられたユーザーがプロジェクトに関連付けられたリソースプールにリストされていない場合、この時間数は予算計上できません。

* 親タスクを、ユーザーや役割に割り当てない。

  親タスクに関連付けられたユーザーや役割の時間情報をリソースプランナーに表示するには、子タスクにも割り当てる必要があります。リソースプランナーには、親タスクからの情報は表示されません。

* タスクとイシューには、予定時間数の値が 0 より大きい値が設定されます。
* タスクとイシューの期間には 0 より大きい値が設定されます。
* イシューの予定日は、プロジェクトのタイムライン内に表示されます。

### システムレベルの前提条件 {#system-level-prerequisites}

Workfront のインスタンスが、システムのリソース管理の環境設定に従ってユーザーの空き時間を計算する方法を理解する必要があります。Workfront は、ユーザープロファイルページで定義されたユーザーのスケジュール、またはシステムのデフォルトスケジュールを使用して、ユーザーの空き時間を計算できます。

![](assets/resource-management-preferences-section-in-setup-350x89.png)

Workfront 管理者がリソース管理の環境設定を指定します。

詳しくは、[リソース管理の環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

## リソースプランナーを配置

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

複数のプロジェクトに対してリソースを予算計上するか、1 つのプロジェクトに対してのみ予算を計上するかに応じて、リソースプランナーを Workfront の 2 つのエリアに配置することができます。

リソースプランナーの配置について詳しくは、[リソースプランナーの配置](../../resource-mgmt/resource-planning/locate-resource-planner.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## リソースプランナーのエリア

リソースプランナーで次の情報を表示したり、次のアクションを実行したりできます。

* 一般的なタイムラインのリソースプランナーでプロジェクトに割り当てられたリソースに関する情報。
* リソースプランナーでのリソースの割り当て超過または割り当て不足。
* 手動または自動で作業するためのリソースの予算計上。

リソースプランナーに表示される領域の詳細と、それらの領域に表示される情報の設定方法については、[リソースプランナーのナビゲーションの概要](../../resource-mgmt/resource-planning/resource-planner-navigation.md)を参照してください。

## リソースプランナーに情報を表示する際の制限

パフォーマンスを向上させるため、Workfront では、リソースプランナーに表示できる項目の数を制限しています。

これらの制限について詳しくは、[リソースプランナーの表示制限](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)の記事を参照してください。

## リソースプランナーでの FTE の計算

リソースプランナーに、使用可否、割り当ておよび予定値を、時間、FTEまたはコストで表示できます。

リソースプランナーに表示する情報の変更について詳しくは、[Adobe Workfront リソースプランナーを使用したリソースの可用性と割り当てのレビュー](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md)の「[時間別、FTE 別またはコスト別の情報の表示](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu)」セクションを参照してください。

Workfront でのユーザーおよび役割の時間と FTE の計算方法について詳しくは、[リソースプランナーでのユーザーおよび役割の時間と FTE の計算の概要](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)の記事を参照してください。

## リソースプランナーでコストを計算

リソースプランナーでコスト別に情報を表示するには、財務データの表示アクセス権とプロジェクトの財務データの表示権限が必要です。

リソースプランナーで可用性、割り当ておよび予定値を時間および FTE で表示するほかに、コスト別に表示することもできます。

>[!TIP]
>
>リソースプランナーでコスト別に情報を表示するには、ユーザーと担当業務を 1 時間あたりのコストに関連付ける必要があります。

1 時間あたりのコストと担当業務との関連付けについて詳しくは、[担当業務の作成と管理](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)の記事を参照してください。\
1 時間あたりのコストとユーザーとの関連付けについて詳しくは、[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)の記事を参照してください。

リソースプランナーでコスト別に情報を表示する際は、次の点を考慮します。

* 各時間タイプのコスト（ユーザー、役割、プロジェクトの計画、利用可能、予算、実績）は、異なるコストレートを使用して計算されます。
* 予定コストは、プロジェクトのタスクのコストタイプの影響を受けます。
* ユーザービューをリソースプランナーに適用する場合、割り当てと使用可否の情報をコスト別に表示することはできません。

ユーザーおよび役割のリソースプランナーでのコストの計算方法の詳細は、[リソースプランナーでのコストの計算](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)の記事を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## リソースプランナーで情報をフィルタリング

フィルターを作成することで、リソースプランナーに表示されるプロジェクト、役割またはユーザーの数を減らすことができます。\
詳しくは、[リソースプランナーでの情報のフィルタリング](../../resource-mgmt/resource-planning/filter-resource-planner.md)の記事を参照してください。
