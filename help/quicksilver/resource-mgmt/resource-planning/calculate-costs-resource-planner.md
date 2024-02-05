---
product-area: resource-management
navigation-topic: resource-planning
title: リソースプランナーでコストを計算
description: Adobe Workfront リソースプランナーでリソースを予算計上するには、時間や FTE 値の代わりにコストの値を使用します。 リソースプランナーの「**ユーザー別に表示**」ビューでは、コストの値は使用できません。
author: Lisa
feature: Resource Management
exl-id: 2f3ca8c2-51b3-4282-af8b-7f433365d386
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1458'
ht-degree: 100%

---

# リソースプランナーでコストを計算

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)</p>
-->

<!--'(Alina: ***Linked to the Planning in the Resource Planner article, Understanding areas of the Resource Planner. - do not move/ change/ delete.)'-->

Adobe Workfront リソースプランナーでリソースを予算計上するには、時間や FTE 値の代わりにコストの値を使用します。 リソースプランナーの「**ユーザー別に表示**」ビューでは、コストの値は使用できません。

>[!IMPORTANT]
>
>リソースプランナーでコスト情報を表示するには、ユーザーと担当業務を 1 時間あたりのコスト率に関連付ける必要があります。\
>1 時間あたりのコスト率の担当業務との関連付けについて詳しくは、[担当業務を作成と管理](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。\
>1 時間あたりのコスト率のユーザーとの関連付けについて詳しくは、[ユーザーのプロファイルを編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

リソースを予算計上する前に、実行する必要のある作業（予定時間数、FTE、コスト）と、ユーザーが作業できる時間（利用可能な時間数、FTE、コスト）を十分に把握しておく必要があります。\
時間数または FTE で予算計上する場合のリソースプランナーの情報について詳しくは、[リソースプランナーのプロジェクトビューと役割ビューの時間、FTE、コスト情報の概要](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソースプランナーの優先度と予算計上時間数の編集へのアクセスを含むリソース管理へのアクセスを編集</p> <p>財務データ、プロジェクトおよびユーザーへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、「<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>」を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務の管理機能を持つ、予算情報が必要なプロジェクトに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;自分のプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## リソースプランナーでコスト別の情報を表示

デフォルトでは、可用性と割り当ての情報は、リソースプランナーの時間に表示されます。

リソースプランナーで利用可能、予定、予算計上の情報をコスト別に表示するには、次の手順を実行します。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**リソース**」をクリックします。
1. リソースプランナーに移動します。
1. （条件付き）「**プロジェクト別に表示**」ビューまたは「**役割別に表示**」ビューを選択します。\
   デフォルトでは、「**プロジェクト別に表示**」が選択されています。\
   割り当てと可用性の情報は、時間に表示されます。

1. **時間**&#x200B;ドロップダウンメニューで「**コスト**」を選択します。

   アクセスレベルで財務データにアクセスできない場合、このオプションは使用できません。\
   プロジェクトの通貨がシステム通貨と異なる場合、これらのプロジェクトのコストがシステムの通貨に変換されて、リソースプランナーに表示されます。システム管理者がシステム通貨を定義します。\
   Workfront でのシステム通貨の設定と換算レートについて詳しくは、[為替レートを設定](../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)を参照してください。\
   ![costs_in_the_planner_with_no_budgeting.png](assets/costs-in-the-planner-with-no-budgeting-350x240.png)

## リソースプランナーで利用可能なコストを計算

利用可能なコストの値をリソースプランナーで表示するには、次の条件を満たす必要があります。

* ユーザーおよび役割の 1 時間あたりのコスト
* ユーザーの可用性に関する情報。

  ユーザーの可用性に関する情報の取得方法は、Workfront 管理者がリソース管理環境設定を設定する方法によって異なります。\
  ユーザーの可用性の計算とリソース管理環境設定の指定について詳しくは、[リソース管理環境設定を指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

次の表に、リソースプランナーでの利用可能なコストの計算方法を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>利用可能なコスト</strong> </th> 
   <th><strong>計算</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ユーザー利用可能コスト</td> 
   <td> <p>ユーザーあたりの利用可能コストは、次の式を使用して計算されます。</p> <p><code>Available User Cost = User Available Hours * User Cost per Hour Rate</code> </p> <p><b>メモ</b>

ユーザーのプロファイルに 1 時間あたりのコスト率がない場合は、ユーザーがリストされている担当業務の 1 時間あたりのコスト率が計算で使用されます。ユーザーに役割が関連付けられていない場合、利用可能なユーザーコストは $0 です。 </p> </td>
</tr> 
  <tr> 
   <td>役割利用可能コスト</td> 
   <td> <p>役割あたりの利用可能コストは、次の式を使用して計算されます。</p> <p><code>Available Role Cost = Role Available Hours * Role Cost per Hour Rate</code> </p> <p><b>メモ</b>

役割に 1 時間あたりのコスト率がない場合、利用可能な役割コストは $0 です。</p> </td>
</tr> 
  <tr> 
   <td>プロジェクト利用可能コスト</td> 
   <td> <p>プロジェクトあたりの利用可能コストは、次の式を使用して計算されます。</p> <p><code>Available Project Cost = SUM(User Available Hours * User Cost per Hour Rate)</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

## リソースプランナーでの予定コストの計算

リソースプランナーではタスク情報を表示できませんが、ユーザー、役割およびプロジェクトの予定コストは、次のタスク情報を考慮して計算されます。

* タスクに対する割り当ての種類。\
  タスクを未割り当てのままにするか、タスクに次のエンティティを割り当てることができます。

   * ユーザー（担当業務の有無に関わらず）
   * 役割
   * チーム\
     チームに割り当てられたタスクは、リソースプランナーの観点からは、未割り当てと見なされます。

* プロジェクト上のタスクの&#x200B;**コストの種類**。\
  タスクのコストの種類について詳しくは、[コストの追跡](../../manage-work/projects/project-finances/track-costs.md)を参照してください。

* 担当業務およびユーザーのコスト率の有効日。

  例えば、役割またはユーザーの 2月の予定時間数が 10 時間、3月の予定時間数が 10 時間で、3月にコスト率が $12 から $20 に変更された場合、2月の予定コストの値は $120、3月の予定コストは $200 になります。

>[!NOTE]
>
>ユーザーの予定コストは、プロジェクト予定コストに影響しません。リソースプランナーでは、役割予定コストのみが、プロジェクト予定コストに影響します。

ユーザー、役割およびプロジェクトの予定コストを計算する場合、次のシナリオが存在します。

* **コストの種類**&#x200B;が「ユーザー（毎時）」で、タスクに&#x200B;**割り当てがない**&#x200B;場合：

   * **役割とユーザーの予定コスト**：

     役割およびユーザーの予定コストは $0.00 です。

   * **プロジェクト予定コスト**：

     プロジェクト予定コストは $0.00 です。

* **コストの種類**&#x200B;が&#x200B;**「ユーザー（毎時）」**&#x200B;で、タスクに&#x200B;**ユーザー割り当て**&#x200B;がある場合：

   * **役割とユーザーの予定コスト**：

     ユーザーの予定コストは、次の式を使用して計算されます。

     `User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate`

     ユーザーのプロファイルにコスト率が含まれている場合は、その比率を使用して予定コストが計算されます。それ以外の場合は、プライマリ役割のシステムレベルの 1 時間あたりのコスト率が使用されます。

     >[!NOTE]
     >
     >ユーザーを、セカンダリ担当業務の 1 つを含むタスクに割り当てることができますが、ここでは、代わりにプライマリ担当業務の比率が使用されます。

     役割の予定コストは、次の式を使用して計算されます。

     `Role Planned Cost = SUM(User Planned Cost)`

   * **プロジェクト予定コスト**：

     プロジェクト予定コストは $0.00 です。

* **コストの種類**&#x200B;が&#x200B;**「ユーザー（毎時）」**&#x200B;で、タスクに&#x200B;**担当業務割り当て**&#x200B;がある場合：

   * **役割とユーザーの予定コスト**：

     ユーザーの予定コストは $0.00 です。

     役割の予定コストは、次の式を使用して計算されます。

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     タスクに割り当てられた担当業務のシステムレベルの 1 時間あたりのコスト率を使用して、予定コストが計算されます。

   * **プロジェクト予定コスト**：

     プロジェクト予定コストは $0.00 です。

* **コストの種類**&#x200B;が&#x200B;**「役割（毎時）」**&#x200B;で、タスクに&#x200B;**割り当てがない**&#x200B;場合：

   * **役割とユーザーの予定コスト**：

     役割およびユーザーの予定コストは $0.00 です。

   * **プロジェクト予定コスト**：

     プロジェクト予定コストは $0.00 です。

* **コストタイプ**&#x200B;が&#x200B;**役割（毎時）**&#x200B;で、タスクに&#x200B;**ユーザー割り当て**&#x200B;がある場合：

   * **役割とユーザーの予定コスト**：

     ユーザーの予定コストは $0.00 です。

     「役割の予定コスト」は、次の式で計算されます。

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront は、ユーザーがタスクで実行する担当業務を調べて、役割の予定コストを計算します。

     ユーザーがタスク上の役割に関連付けられていない場合、予定コストは $0.00 になります。

   * **プロジェクト予定コスト**：

     プロジェクト予定コストは、次の式で計算されます。

     `Project Planned Cost = SUM(Role Planned Costs)`

* **コストタイプ**&#x200B;が&#x200B;**役割（毎時）**&#x200B;で、タスクに&#x200B;**担当業務割り当て**&#x200B;がある場合：

   * **役割とユーザーの予定コスト**：

     ユーザーの予定コストは $0.00 です。

     「役割の予定コスト」は、次の式で計算されます。

     `Role Planned Cost = Role Planned Hours * Role Cost per Hours`

     Workfront は、ユーザーがタスクで実行する担当業務を調べて、役割の予定コストを計算します。

   * **プロジェクト予定コスト**：

     プロジェクト予定コストは、次の式で計算されます。

     `Project Planned Cost = SUM(Role Planned Costs)`

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(table below ideal but drafted because it does not display correctly in Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td rowspan="2">&nbsp;</td>
<td colspan="3"> <p><strong>Cost Type = User Hourly</strong> </p><strong>User Planned Cost</strong> </td>
<td colspan="3"> <p><strong>Cost Type = Role Hourly</strong> </p><strong>Role Planned Cost</strong> </td>
</tr>
<tr>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>User and Role Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is calculated using the following formula: </p> <p><code> User Planned Cost Rate = User Planned Hours * User Cost per Hour Rate </code> </p> <p> If a user has a cost rate in their profile, then that rate is used to calculate Planned Cost. Otherwise, the system-level Cost per Hour rate of their Primary Role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code>Role Planned Cost = SUM(User Planned Cost)</code> </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated using the following formula: </p> <p><code> Role Planned Cost = Role Planned Hours * Role Cost per Hours </code> </p> <p> The system-level Cost per Hour rate of the job role assigned to the task is used to calculate Planned Cost. </p> </td>
<td> <p>The Role and User Planned Costs are $0.00.</p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> If the user is not associated with any role on the task, the Planned Cost is $0.00. </p> </td>
<td> <p> The User Planned Cost is $0.00. </p> <p> The Role Planned Cost is calculated by the following formula: </p> <p><code>Role Planned Cost = Role Planned Hours * Role Cost per Hours</code> </p> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Cost for the role. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td rowspan="2"> <p><strong>Project Planned Cost</strong> </p> <p> </p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td> <p>The Project Planned Cost is $0.00.</p> </td>
<td colspan="2"> <p> The Project Planned Cost is calculated using the following formula: </p> <p><code> Project Planned Cost = SUM(Role Planned Costs) </code> </p> <p> </p> </td>
</tr>
<tr>
<td colspan="6"> <note type="note">
User Planned Costs do not influence the Project Planned Cost. Only the Role Planned costs affect the Project Planned Costs, in the Resource Planner.
</note> </td>
</tr>
</tbody>
</table>
-->

## リソースプランナーでの予算計上コストの計算

予算計上コストの値を生産リソースプランナーに表示するには、次の条件を満たす必要があります。

* 役割、ユーザーおよびプロジェクトの予算時間。
* ユーザーおよび役割の 1 時間あたりのコスト。

>[!NOTE]
>
>プロジェクトの予算時間は、ユーザーの予算時間ではなく、役割の予算時間に基づいて計算されます。

次の表に、リソースプランナーでの予算計上コストの計算方法を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>予算計上コスト</strong> </th> 
   <th><strong>計算</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ユーザーの予算計上コスト</td> 
   <td> <p>ユーザーあたりの予算計上コストは、次の式を使用して計算されます。</p> <p><code>Budgeted User Cost = User Budgeted Hours * User Cost per Hour Rate</code> </p> <p> <p><b>メモ</b>

ユーザーのプロファイルに「時間当たりのコスト」レートがない場合、予算計上ユーザーコストは $0.00 になります。</p> </p> </td>
</tr> 
  <tr> 
   <td>役割の予算計上コスト</td> 
   <td> <p>役割の予算計上コストは、次の式を使用して計算されます。</p> <p><code>Role Budgeted Cost = Role Budgeted Hours * Role Cost per Hour Rate</code> </p> <p> <p><b>メモ</b>

役割に時間あたりのコストがない場合、予算計上役割コストは $0.00 です。</p> </p> </td>
</tr> 
  <tr> 
   <td>プロジェクト予算計上コスト</td> 
   <td> <p>プロジェクトあたりの予算計上コストは、次の式を使用して計算されます。</p> <p><code>Project Budgeted Cost = SUM(Role Budgeted Cost). </code> </p> </td> 
  </tr> 
 </tbody> 
</table>
