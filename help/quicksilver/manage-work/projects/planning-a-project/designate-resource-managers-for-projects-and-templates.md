---
product-area: projects;templates
navigation-topic: plan-a-project
title: プロジェクトまたはテンプレートに対するリソースマネージャの指定
description: プロジェクトのリソースマネージャを指定して、プロジェクト上のリソースの管理担当者を指定できます。
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# プロジェクトまたはテンプレートに対するリソースマネージャの指定

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

プロジェクトのリソースマネージャを指定して、プロジェクト上のリソースの管理担当者を指定できます。 これは情報フィールドであり、どのリソース管理ツールにも接続されていません。

<!-- drafted for res scheduling deprecation blurb for preview release
Designating Resource Managers for a project is a prerequisite for using the Scheduling tools in Adobe Workfront, in the Production environment.
  
>[!CAUTION]  
>  
>  
> <span class="preview">Some of the information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span>  
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span>  
>  
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../../resource-mgmt/workload-balancer/workload-balancer.md).</span>  
>  
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

## アクセス要件

<!--drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Templates</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project or template</p> 
   
   <p><b>NOTE</b>
   
   Users who are added as Resource Managers to a project or a template immediately gain Manage permissions on the project or the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトとテンプレートへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトまたはテンプレートに対する権限の管理</p>

<p><b>メモ</b>

リソースマネージャーとしてプロジェクトまたはテンプレートに追加されたユーザーは、すぐに、プロジェクトまたはテンプレートに対する管理権限を取得します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td>
</tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## リソースマネージャに関する考慮事項

>[!NOTE]
>
>リソースマネージャはジョブの役割ではありません。手動で更新できる、プロジェクトまたはテンプレートで使用可能なフィールドです。

* 個々のプロジェクトまたはテンプレートに対して、最大 30 人のユーザーをリソースマネージャーとして指定できます。

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Overview of the Workload Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* チームまたはグループをリソースマネージャとして指定することはできません。 ユーザーをリソースマネージャとして指定できるのは、ユーザーだけです。

* プロジェクトまたはテンプレートでリソースマネージャとして指定したユーザーは、自動的にはプロジェクトチームに含まれません。

   プロジェクトチームについて詳しくは、 [プロジェクトチームを管理](../../../manage-work/projects/planning-a-project/manage-project-team.md).

* プロジェクトまたはプロジェクトテンプレートに対して、リソースマネージャを指定できます。 プロジェクトテンプレートでリソースマネージャを指定すると、そのテンプレートでリソースマネージャとして指定したユーザは、そのテンプレートを使用して作成された任意のプロジェクトのリソースマネージャに自動的になります。
* 次の領域で、「リソースマネージャー」フィールドを表示できます。

   * プロジェクトの編集時に、この記事で説明する。
   * テンプレートの編集時に、この記事で説明します。
   * プロジェクトまたはテンプレートレポートを作成する際。 レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
   * リストのプロジェクトまたはテンプレートビューを作成またはカスタマイズする場合。 詳しくは、 [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* リストまたはプロジェクトのビューに [ リソースマネージャ ] フィールドを追加し、インライン編集を使用してこのフィールドを編集することで、複数のプロジェクトまたはテンプレートでリソースマネージャを簡単に追加または削除できます。

## プロジェクトのリソースマネージャを指定する

1. 次のいずれかの操作を行います。

   * 1 つのプロジェクトにリソースマネージャを追加するには、1 つ以上のリソースマネージャを指定するプロジェクトに移動し、 **その他のメニュー** プロジェクト名の横に表示され、 **を編集します。**

   * 複数のプロジェクトに同時にリソースマネージャを追加するには、プロジェクトの一覧に移動し、1 つ以上のリソースマネージャを指定するプロジェクトを選択して、 **編集**.

      既存のリソースマネージャは、編集中のプロジェクトから削除されません。この方法で追加したユーザーは、既存のリソースマネージャに加えて、プロジェクトのリソースマネージャとして追加されます。

   * 新しいプロジェクトにリソースマネージャを追加するには、新しいプロジェクトの作成を開始します。

      プロジェクトの作成について詳しくは、 [プロジェクトの作成](../../../manage-work/projects/create-projects/create-project.md).

1. 内 **概要** をクリックします。 **リソースマネージャ** フィールドに入力します。
1. プロジェクトのリソースマネージャーとして追加するユーザーの名前を入力し、一覧に表示されたら名前をクリックします。

   この手順を繰り返して、プロジェクトに複数のリソースマネージャを追加します。

1. クリック **変更を保存**.

## テンプレートに対するリソースマネージャの指定

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **テンプレート**.

1. 次のいずれかの操作を行います。

   * 1 つのテンプレートにリソースマネージャを追加するには、1 つ以上のリソースマネージャを指定するテンプレートに移動し、 **その他のメニュー** テンプレート名の横に表示され、 **を編集します。**

   * 複数のテンプレートにリソースマネージャを同時に追加するには、テンプレートの一覧に移動し、1 つ以上のリソースマネージャを指定するテンプレートを選択し、 **編集**.

      既存のリソースマネージャは、編集中のテンプレートから削除されません。この方法で追加したユーザーは、既存のリソースマネージャに加えて、テンプレートのリソースマネージャとして追加されます。

   * 新しいテンプレートにリソースマネージャを追加するには、 **新規テンプレート**&#x200B;次に、 **その他のメニュー** テンプレート名の横に表示され、 **を編集します。**

1. 内 **概要** セクションで、 **リソースマネージャ** フィールドに入力します。
1. テンプレートのリソースマネージャーとして追加するユーザーの名前を入力し、リストに表示されたら、名前をクリックします。

   この手順を繰り返して、複数のリソースマネージャをテンプレートに追加します。

1. クリック **変更を保存**.
