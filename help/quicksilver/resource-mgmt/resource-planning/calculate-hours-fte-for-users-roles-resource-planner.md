---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: リソースプランナーのユーザーと役割の時間とFTEの計算の概要
description: リソースプランナーのユーザーと役割の時間とFTEの計算の概要。
author: Lisa
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
TQID: https://experienceleague.adobe.com/plzNKZEP3YSHuUZt2MrWb9Q--QemkwCEJD3JxWlB6x4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1325
ht-degree: 67%

---

# リソースプランナーでのユーザーと役割に対する時間と FTE の計算の概要

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

リソースプランナーで、リソースの割り当てとリソースの空き時間を時間、FTE、コストのいずれかで表示できます。\
リソースプランナーでのコストの計算について詳しくは、[リソースプランナーでのコストの計算](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)を参照してください。

FTE （Full Time Equivalent）は、ユーザーまたはジョブロールの1日または1週間の実際の作業に費やす時間を表す時間の指標です。

次のリソース情報のセットは、リソースプランナーでは異なる方法で計算されます。

* 空き時間または FTE の値は、システム管理者がシステムでリソース管理環境設定を設定する方法に基づいて計算されます。\
  空き時間と FTE の値の計算方法について詳しくは、[リソースプランナーでユーザーおよび担当業務の空き時間または FTE を計算](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner)を参照してください。\
  Adobe Workfront システムのリソース管理環境設定の定義について詳しくは、[リソース管理環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

* その他のすべての FTE 値は、システムのデフォルトのスケジュールに基づいて計算されます。\
  FTE を使用する場合に、他のすべての値がリソースプランナーにどのように表示されるかについて詳しくは、この記事の[リソースプランナーでユーザーおよび担当業務のその他すべての時間および FTE 値を計算](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner)の節を参照してください。

各ユーザーとその担当業務に対する FTE の内容を理解し、リソースを作業に割り当てる際にリソースを正確に管理することが重要です。

## リソースプランナーでユーザーおよび担当業務の空き時間または FTE を計算 {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

### リソースプランナーでユーザーの空き時間と FTE を計算 {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

Workfront管理者は、設定のリソース管理領域で次のいずれかを選択して、ユーザーの利用可能な時間を計算する方法を決定します。

* システムのデフォルトのスケジュールとユーザーの FTE。
* ユーザーのスケジュール。

![ユーザースケジュールのシステム設定](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>これにより、システムレベルでのリソースの空き時間を計算する方法が決まります。 システムのリソース管理環境設定の定義について詳しくは、[リソース管理環境設定の指定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

この設定の構成に基づいて、リソースプランナーでのユーザーの空き時間（時間数および FTE の空き時間）は、次の方法で計算されます。

* **デフォルトのスケジュール**：システムのデフォルトのスケジュールとユーザーの FTE を使用して、リソースプランナーのユーザーの空き時間数と FTE 値を決定します。 ユーザーのスケジュールは無視されます。 この場合、次のようになります。

   * リソースプランナーで利用可能な時間は、次の式を使用して計算されます。

     `User Available Hours = Default Schedule Hours * User FTE value`

     例えば、デフォルトのスケジュールで空き時間が週に 40 時間、ユーザー FTE が 0.5 の場合、ユーザーはリソースプランナーで週 20 時間作業することができます。

     デフォルトのスケジュールを含むスケジュールについて詳しくは、[スケジュールの作成](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

   * リソースプランナーのユーザーの使用可能なFTEは、ユーザー設定で指定されたユーザーFTEと同じです。

     例えば、ユーザー設定でユーザー FTE が 0.5 の場合、ユーザーの利用可能な FTE は、リソースプランナーで 0.5 となります。 ユーザー設定に表示されるユーザー FTE の値について詳しくは、[ユーザーのプロファイルの編集](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

* **ユーザーのスケジュール**: ユーザーのスケジュールは、リソースプランナーでのユーザーの可用性を判断するために使用されます。 ユーザーの FTE の値は無視されます。 この場合、次のようになります。

   * リソースプランナーで使用可能な時間は、ユーザーのスケジュールの時間と同じです。

     例えば、ユーザーのスケジュールで週に40時間の作業が可能な場合、リソースプランナーで週に40時間の作業が可能になります。

   * リソースプランナーで使用可能なFTEは、次の式で計算されます。

     `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

     例えば、ユーザーのスケジュールに20時間、Workfrontのデフォルトスケジュールに40時間の時間がある場合、ユーザーのFTEは0.5になります。

     デフォルトのスケジュールを含むスケジュールについて詳しくは、[スケジュールの作成](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

>[!NOTE]
>
>ユーザーがスケジュールに関連付けられていない場合、ユーザーの空き時間数はデフォルトのスケジュールを使用して計算されます。

### リソースプランナーで担当業務の空き時間と FTE を計算 {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

最初にユーザーの空き時間を計算し、次に各担当業務の空き時間を計算する必要があります。

リソースプランナーの担当業務の可用性は、ユーザーの合計可用性と、ユーザーの各役割に関連付けられたFTE可用性の割合を考慮します。\
![percent_of_fte_availability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

FTE可用性の割合の値をユーザーの担当業務に関連付ける方法について詳しくは、[&#x200B; ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

例えば、ユーザーの「利用可能な時間」の値が40で、その時間の75%に1つのプライマリロールを果たし、その時間の25%に1つの他のロールを果たすことができる場合、リソースプランナーは、プライマリロールの1週間の利用可能な時間の値が30時間であり、他のロールの利用可能な時間の値が10時間であることを示します。 この場合、プライマリ役割の FTE は 0.75、その他の役割の FTE は 0.25 となります。

>[!NOTE]
>
>ユーザーの空き時間の合計は、この記事の[リソースプランナーでユーザーの空き時間と FTE を計算](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)の節で説明されている、2 つの方法のいずれかによって計算されます。

役割ビューでリソースプランナーを表示する場合、1 つの担当業務の空き時間は、その担当業務を果たすことができるすべてのユーザーの空き時間の合計です。

リソースプランナーでのリソースの空き時間について詳しくは、[リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

### リソースプランナーでユーザーの空き時間と FTE を計算（例） {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

次の表に、「リソース管理」環境設定のFTE計算にシステム管理者が使用する方法に応じて、リソースプランナーのユーザーに対して利用可能な時間と利用可能なFTEがどのように計算されるかを示します。

この例では、以下の数値を使用します。

* システムのデフォルトのスケジュール：40 時間
* ユーザーのスケジュール：20 時間
* ユーザーの FTE：0.8

| FTE の計算方法（システム設定） | **ユーザーのスケジュールからの時間数** | **デフォルトのスケジュールからの時間数** | **「ユーザーの FTE」フィールド** | **リソースプランナーでの利用可能時間数** | **リソースプランナーでの利用可能な FTE** |
|---|---|---|---|---|---|
| **デフォルトのスケジュール** | 無視 | 40 | 0.8 | **32**（計算値） | **0.8** |
| **ユーザーのスケジュール** | 20 | 40 | 無視 | **20** | **0.5**（計算値） |

スケジュール例外と休暇が、予定時間数または FTE の値に影響を与える可能性があります。 詳しくは、[リソース管理の環境設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

ユーザーおよび時間数別のリソースプランナービューの例：

![ユーザーおよび時間別のリソースプランナービュー](assets/resource-planner-by-user-by-hours.png)

ユーザーおよび FTE 別のリソースプランナービューの例：

![ユーザーおよび FTE 別のリソースプランナービュー](assets/resource-planner-by-user-by-fte.png)

## リソースプランナーでユーザーおよび担当業務の他のすべての時間数および FTE の値を計算 {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

利用可能時間数や FTE に加えて、以下の時間情報もリソースプランナーに表示されます。

* 予定時間数
* 予算計上時間数
* 時間差異
* 正味時間数\
  詳しくは、[リソースプランナーのプロジェクトビューと役割ビューでの時間数、FTE、コスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)を参照してください。

* 時間差\
  詳しくは、[リソースプランナーのプロジェクトビューと役割ビューでの時間数、FTE、コスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)を参照してください。

リソースプランナーには、FTEまたは時間と同じ情報を表示できます。

Workfront では、リソースプランナーで他のすべての値を FTE として表示する場合、次の式を使用します。

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>リソースプランナーで利用可能（AVL） FTE値を除くすべての値のFTEを計算する場合、ユーザーのスケジュールは無視されます。 計算にはデフォルトのスケジュールのみが考慮されます。

この計算は次の値に適用されます。

* 予定 FTE（PLN）
* 予算計上 FTE（BDG）
* FTE の差（VAR）
* 正味 FTE
* FTE の差（DIF）
