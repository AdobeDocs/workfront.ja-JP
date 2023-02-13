---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: リソース・プランナのユーザーとロールの時間と工数の計算の概要
description: リソース・プランナのユーザーとロールの時間と工数の計算の概要
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 1%

---

# リソース・プランナのユーザーとロールの時間と工数の計算の概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

リソース・プランナで、リソースの配分と可用性を時間、工数、原価のいずれかで表示できます。\
リソース・プランナでのコストの計算の詳細は、 [リソースプランナーでコストを計算する](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

「FTE」は、Full Time Equivalent（フルタイム相当）を表します。 ユーザーまたはジョブの役割の 1 日または 1 週間の実際の作業に費やされる時間を表す時間の単位です。

次のリソース情報のセットは、リソース・プランナでは異なる方法で計算されます。

* Available Hours または FTE の値は、システム管理者がシステムで Resource Management プリファレンスを設定する方法に基づいて計算されます。\
   使用可能な時間と FTE の値の計算方法について詳しくは、 [リソース・プランナのユーザーおよび役職ロールの使用可能時間または工数の計算](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
   Adobe Workfrontシステムのリソース管理環境設定の定義について詳しくは、 [リソース管理環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* その他のすべての FTE 値は、システムのデフォルトスケジュールに基づいて計算されます。\
   FTE を使用する場合に、他のすべての値がリソース・プランナにどのように表示されるかの詳細は、「 [リソース・プランナのユーザーおよびジョブ・ロールのその他すべての時間および FTE 値を計算します。](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) 」を参照してください。

各ユーザーとそのジョブの役割に対する FTE の内容を理解し、リソースを作業に割り当てる際にリソースを正確に管理することが重要です。

## リソース・プランナのユーザーおよび役職ロールの使用可能時間または工数の計算 {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [リソース・プランナでユーザーの使用可能時間と工数を計算する](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [リソース・プランナの役割の使用可能時間と工数を計算します。](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [リソース・プランナのユーザーの使用可能時間と工数を計算する（例）](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### リソース・プランナでユーザーの使用可能時間と工数を計算する {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfrontの管理者は、「セットアップ」の「リソース管理」領域で次のいずれかを使用するように選択することで、ユーザーの使用可能時間を計算する方法を決定します。

* システムのデフォルトのスケジュールとユーザーの FTE。
* ユーザーのスケジュール。

詳しくは、 [リソース管理環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><br></p>
<p> <img src="assets/nwe-resource-management-system-setting-user's-schedule-350x157.png" style="width: 350;height: 157;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p>
<p>(NOTE: The determines how to calculate resource availability at the system level.For more information about defining the Resource Management preferences for the system, see Configure Resource Management preferences.)</p>
<p>Based on how this setting is configured, the availability of the users in the Resource Planner (hours as well as FTE availability) is calculated by using the following methods: </p>
<ul>
<li><strong>The Default Schedule</strong>: The Default Schedule of the system and the user FTE are used to determine the Available Hours and FTE value for the user in the Resource Planner. The Schedule of the user is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are calculated using the following formula:<br><code>User Available Hours = Default Schedule Hours * User FTE value</code> <span style="color: #dc143c;">( NOTE: this is the correct value. If this shows as a division in other articles, that is wrong. It's a multiplication between these 2 values).</span><br>For example, if the Default Schedule has 40 hours a week available for work, and the user FTE is 0.5, the user is available to work for 20 hours a week in the Resource Planner.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a></li>
<li style="font-weight: normal;"> The <strong>Available FTE</strong> for the user in the<strong>Resource Planner</strong> is the same as the user FTE specified in the user settings. <br>For example, if the user FTE is 0.5 in the user settings, the available FTE of the user is 0.5 in the Resource Planner. For more information about the value of the user FTE as it displays in the user settings, see <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.<br></li>
</ul></li>
<li><strong>The User's Schedule</strong>: The Schedule of the user is used to determine the availability of the user in the Resource Planner. The value of the user FTE is ignored. In this case:
<ul>
<li> The <strong>Available Hours</strong> in the<strong>Resource Planner</strong> are the same as the Hours from the Schedule of the user.<br>For example, if the Schedule of the user has 40 hours a week available for work, the user is available to work for 40 hours a week in the Resource Planner. </li>
<li> The <strong>Available FTE</strong> in the<strong>Resource Planner</strong> is calculated by the following formula:<br><em><code>User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours</code><br></em>For example, if the Schedule of the user has 20 hours available to work, and the Default Schedule in Workfront has 40 hours available to work, the user's FTE is 0.5.<br>For more information about schedules, including the Default Schedule, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</li>
</ul></li>
</ul> <note type="note">
If the user is not associated with a schedule, the Available Hours for the user are calculated using the Default Schedule.
</note>
</div>
-->

### リソース・プランナの役割の使用可能時間と工数を計算します。 {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

最初にユーザーの可用性を計算し、次に各ジョブの役割の可用性を計算する必要があります。

リソース・プランナでのジョブ・ロールの使用可能性は、ユーザーの使用可能性の合計と **FTE の可用性の割合** ユーザーの各役割に関連付けられています。\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

関連付けの詳細については、 **FTE の可用性の割合** ユーザーのジョブロールを持つ値 ( [ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

たとえば、あるプライマリの「使用可能時間」の値が 40 で、その時間の 75%に対して 1 つのユーザー・ロールを、その時間の 25%に対して 1 つの「その他のロール」を満たす場合、リソース・プランナは、 **利用可能な時間** 1 週間のプライマリロールの値は 30 時間で、 **利用可能な時間** の値は 10 時間です。 この場合、プライマリロールの FTE は 0.75、他のロールの FTE は 0.25 です。

>[!NOTE]
>
>ユーザーの合計使用可能時間は、 [リソース・プランナでユーザーの使用可能時間と工数を計算する](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) 」の節を参照してください。

「ロール・ビュー」でリソース・プランナを表示する場合、1 つのジョブ・ロールの可用性は、そのジョブ・ロールを満たすことができるすべてのユーザーの可用性の合計です。\
リソース・プランナでのリソースの可用性の詳細は、 [リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### リソース・プランナのユーザーの使用可能時間と工数を計算する（例） {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

次の表は、「生産資源管理プリファレンス」の FTE 計算にシステム管理者が使用する方法に応じて、生産資源プランナのユーザーに対して使用可能時間と使用可能時間が計算される方法を示しています。

この例では、次の数値を使用します。

* 40 時間のシステムデフォルトスケジュール
* 20 時間のユーザースケジュール
* 0.75 のユーザ FTE。

| 工数計算方法（システム設定） | **ユーザーのスケジュールからの時間** | **デフォルトのスケジュールからの時間** | **ユーザー FTE フィールド** | **生産資源プランナで使用可能な時間** | **リソース・プランナで使用可能な FTE** |
|---|---|---|---|---|---|
| **既定のスケジュール** | 無視 | 40 | 0.75 | **30** （計算済み） | **0.75** |
| **ユーザーのスケジュール** | 20 | 40 | 無視 | **20** | **0.5** （計算済み） |

スケジュールの例外とタイムオフは、計画時間または工数の量に影響を与える場合があります。 詳しくは、 [リソース管理環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## リソース・プランナのユーザーおよびジョブ・ロールのその他すべての時間および FTE 値を計算します。 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

「使用可能時間」または「工数」に加えて、次の時間情報も「生産資源プランナ」に表示されます。

* 予定時間数
* 予算計上時間数
* 時間差異
* 正味時間\
   これらの値について詳しくは、 [リソースプランナーのプロジェクトビューとロールビューの時間、工数、コスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* 時間差\
   この値が何を表すかについて詳しくは、 [リソースプランナーのプロジェクトビューとロールビューの時間、工数、コスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

生産資源プランナーには、FTE と同じ情報を表示することも、時間として表示することもできます。

Workfrontは、次の式を使用して、その他すべての値をリソース・プランナに FTE として表示します。

```
FTE = Resource Planner Hours/ Default Schedule Hours
```

>[!NOTE]
>
>リソース・プランナで、「使用可能 (AVL)」FTE 値以外のすべての値に対して FTE を計算する場合、ユーザーのスケジュールは無視されます。 計算にはデフォルトのスケジュールのみが考慮されます。

この計算は、次の値に適用されます。

* 計画工数 (PLN)
* 予算工数 (BDG)
* 工数差異 (VAR)
* 正味工数
* FTE 差 (DIF)
