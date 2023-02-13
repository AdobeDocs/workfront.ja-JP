---
product-area: resource-management
navigation-topic: resource-scheduling
title: Workfrontがスケジューリング領域のリソース時間と FTE の可用性を計算する方法を設定します
description: Adobe Workfrontの管理者は、Workfrontがリソース管理環境設定を行う際に、リソースの可用性とユーザー割り当てをシステムレベル（時間と FTE の可用性を考慮）で計算する方法を決定します。
author: Alina
feature: Resource Management
exl-id: 75bf6d3a-95e9-4cef-a1cc-f19a0f56a42e
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Workfrontがスケジューリング領域のリソース時間と FTE の可用性を計算する方法を設定します

<!-- should this article be removed at production? Or is it still pertinent for the WB functionality??? -->

>[!IMPORTANT]
>  
><span class="preview">この記事で説明するスケジュール機能は、2023 年 1 月の 23.1 リリースから廃止され、Adobe Workfrontから削除されました。   </span>
>  
> <span class="preview"> この記事は、2023 年初頭の 23.1 リリースの直後にも削除されます。 現時点では、ブックマークを適宜更新することをお勧めします。 </span>
> 
><span class="preview"> これで、ワークロードバランサーを使用して、リソースの作業をスケジュールできます。 </span>
>  
> <span class="preview">ワークロード・バランサを使用したリソースのスケジュール設定の詳細は、「 [ワークロードバランサー](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--   


>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->
<!--
<p>***Notice that the FTE for scheduling is not yet working the same way as the FTE for planning - confirmed with Vazgen and this parity is planned for the future, but not right now. This article has to remain live in addition to the Planning article that talks about the calculation of FTEs in the Planner.</p>
<p>[The information in this article was taken from "Calculating Hours and FTE for Users and Roles in the Resource Planner". Specifically, from section "Calculating the Available Hours and FTE for a User in the Resource Planner". It was re-worded slightly.]</p>
<p>Article linked to Managing User Allocations and Managing User Assignments (in the Scheduling section), so do not remove unless you resolve links.) </p>
</div>
-->

Adobe Workfrontの管理者は、Workfrontがリソース管理環境設定を行う際に、リソースの可用性とユーザー割り当てをシステムレベル（時間と FTE の可用性を考慮）で計算する方法を決定します。

次のいずれかを選択して使用できます。

* システムのデフォルトのスケジュールとユーザーの FTE。
* ユーザーのスケジュール。

詳しくは、 [リソース管理環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

この設定は、リソースをスケジュールする際に次の状況でのユーザーの可用性に影響します。

* Workfrontでリソースを自動的に割り当てることを許可する場合は、次の記事を参照してください。

   * [スケジュール領域で未割り当てタスクとタスクを手動で割り当てる](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p><a href="../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md" class="MCXref xref">Assign work in bulk using the Workload Balancer</a></p><p>(NOTE: this is not needed unless we make this article more broad and not refer just to Scheduling??) </p></li>   
     -->

* 配分指標を表示する際に使用する指標を次の記事で説明します。

   * 記事の「配分指標」の節  [スケジューリング領域でユーザー割り当てを管理します](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The section "User availability in the Workload Balancer" in the article <a href="../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md" class="MCXref xref">Overview of assigning work in the Workload Balancer</a>. </li>   
     -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2>Access requirements</h2>
<p>(NOTE: the rest of this article is drafted because these steps are admin steps and live in the admin area) </p>
<p>You must have the following:</p>
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
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>System administrator</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see
<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr data-mc-conditions="QuicksilverOrClassic.Draft mode">
<td role="rowheader">Object permissions</td>
<td> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
<h2>Configure how Workfront calculates resource availability when scheduling resources</h2>
<ol>
<li value="1">Log in to Workfront as an administrator. </li>
<li value="2">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront. <br></li>
<li value="3">  Click&nbsp; <strong>Setup</strong>.  </li>
<li value="4"> <p> Click&nbsp;<strong>Resource Management</strong>.<br></p> <p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <br> </p> </li>
<li value="5"> Select to calculate the availability of users in Workfront using&nbsp;one of the following methods:
<ul>
<li><strong>The Default Schedule</strong>:&nbsp;The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user when scheduling resources. The Schedule of the user is ignored. In this case:&nbsp;
<ul>
<li> The&nbsp;<strong>Available Hours</strong> for a user when scheduling resources<strong></strong>are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE </code><em><code>value</code>&nbsp;</em><br>For example, if the&nbsp;Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Scheduling area.<br>For more information about schedules, including the Default Schedule, see&nbsp;<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
<li> The&nbsp;<strong>Available FTE</strong>for the user when scheduling resources<strong></strong>is the same as the user FTE specified in the user settings.&nbsp;&nbsp;<br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner.&nbsp;For more information about the value of the user FTE as it displays in the user settings, see&nbsp;<a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user&nbsp;is used to determine the availability of the user when scheduling resources.&nbsp;The value of the user FTE is ignored. In this case:&nbsp;
<ul>
<li> The&nbsp;<strong>Available Hours</strong>in the<strong>Resource Planner</strong>are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available&nbsp;for work, the user is available to work for 40 hours a week in the Resource Planner.&nbsp; </li>
<li> The&nbsp;<strong>Available FTE</strong>in the<strong>Resource Planner</strong>&nbsp;is calculated by the following formula:<br><em>User Available FTE =&nbsp;Hours from the Schedule of the User/ Default Schedule Hours<br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see&nbsp;<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul> <note type="note"> &nbsp;If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note></li>
</ul></li>
</ol>
</div>
-->
