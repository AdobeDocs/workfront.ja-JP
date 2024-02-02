---
product-area: projects;templates
navigation-topic: plan-a-project
title: プロジェクトまたはテンプレートのリソース管理者の指定
description: プロジェクトのリソース管理者を指定して、プロジェクトのリソース管理の責任者を指名できます。
author: Alina
feature: Work Management
exl-id: ae2a89e7-8049-4ee6-9b28-ce247d3f2a6f
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: ht
source-wordcount: '826'
ht-degree: 100%

---

# プロジェクトまたはテンプレートのリソース管理者の指定

<!--
<p This article might have to be deleted when the Resource Manager field/ requirement will be forever removed from the system; right now it's still a requirement for Scheduler - January 2023/p>
-->

<!-- remove Prod and Prev references with Prod release - Jan 2023-->

プロジェクトのリソース管理者を指定して、プロジェクトのリソース管理の責任者を指名できます。これは情報フィールドであり、どのリソース管理ツールにも結び付けられていません。

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトとテンプレートへの編集アクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトまたはテンプレートに対する管理権限</p>

<p><b>メモ</b>

リソース管理者としてプロジェクトまたはテンプレートに追加されたユーザーは、プロジェクトまたはテンプレートに対する管理権限を直ちに取得します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td>
</tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## リソース管理者に関する考慮事項

>[!NOTE]
>
>リソース管理者は担当業務ではありません。手動で更新可能な、プロジェクトまたはテンプレートで利用可能なフィールドです。

* 個々のプロジェクトまたはテンプレートに対して、最大 30 名のユーザーをリソース管理者として指定できます。

<!--
* In the Production environment,designating Resource Managers on projects is a prerequisite to allowing users to schedule resources for work on the project when using the Scheduling tools.

  For information about resource scheduling, see [Resource Scheduling](../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md). 

  <span class="preview">Scheduling tools have been removed from the Preview environment.</span>

* Designating Resource Managers on projects is not a prerequisite to allowing users to schedule resources for work using the Workload Balancer.

  For information about the Workload Balancer, see [Workload Balancer overview](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md). 

 -->

* チームまたはグループをリソース管理者として指定することはできません。ユーザーのみをリソース管理者として指定できます。

* プロジェクトまたはテンプレートでリソース管理者として指定したユーザーは、自動的にプロジェクトチームの一員になるわけではありません。

  プロジェクトチームについて詳しくは、[プロジェクトチームの管理](../../../manage-work/projects/planning-a-project/manage-project-team.md)を参照してください。

* プロジェクトまたはプロジェクトテンプレートに対して、リソース管理者を指定できます。プロジェクトテンプレートにリソース管理者を指定すると、そのプロジェクトテンプレートのリソース管理者として指定された任意のユーザーは、自動的にそのテンプレートを使用して作成された任意のプロジェクトのリソース管理者になります。
* 次の場合に「リソース管理者」フィールドを表示できます。

   * プロジェクトを編集する場合（この記事で説明）。
   * テンプレートを編集する場合（この記事で説明）。
   * プロジェクトまたはテンプレートレポートを作成する場合。レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。
   * リストに対してプロジェクトまたはテンプレートビューを作成またはカスタマイズする場合。詳しくは、[Adobe Workfront のビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)を参照してください。

* リストまたはプロジェクトのビューに「リソース管理者」フィールドを追加し、インライン編集を使用してこのフィールドを編集することで、複数のプロジェクトまたはテンプレートでリソース管理者を簡単に追加または削除できます。

## プロジェクトのリソース管理者の指定

1. 次のいずれかの操作を行います。

   * 単一のプロジェクトにリソース管理者を追加するには、リソース管理者を 1 名以上の指定するプロジェクトに移動し、プロジェクト名の横にある&#x200B;**その他**&#x200B;メニューをクリックし、「**編集**」をクリックします。

   * 複数のプロジェクトに同時にリソース管理者を追加するには、プロジェクトのリストに移動し、リソース管理者を 1 名以上指定するプロジェクトを選択して、「**編集**」をクリックします。

     既存のリソース管理者は、編集中のプロジェクトから削除されません。この方法で追加したユーザーは、既存のリソース管理者に加えて、プロジェクトのリソース管理者として追加されます。

   * 新しいプロジェクトにリソース管理者を追加するには、新しいプロジェクトの作成を開始します。

     プロジェクトの作成について詳しくは、[プロジェクトの作成](../../../manage-work/projects/create-projects/create-project.md)を参照してください。

1. 「プロジェクトを編集」ダイアログボックスの「**概要**」セクションで、「**リソース管理者**」フィールドをクリックします。
1. プロジェクトのリソース管理者として追加するユーザーの名前を入力し、その名前がリストに表示されたらクリックします。

   この手順を繰り返して、プロジェクトに複数のリソース管理者を追加します。

1. 「**変更を保存**」をクリックします。

## テンプレートのリソース管理者の指定

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**テンプレート**」をクリックします。

1. 次のいずれかの操作を行います。

   * 単一のテンプレートにリソース管理者を追加するには、リソース管理者を 1 名以上の指定するテンプレートに移動し、テンプレート名の横にある&#x200B;**その他**&#x200B;メニューをクリックし、「**編集**」をクリックします。

   * 複数のテンプレートに同時にリソース管理者を追加するには、テンプレートのリストに移動し、リソース管理者を 1 名以上の指定するテンプレートを選択して、「**編集**」をクリックします。

     既存のリソース管理者は、編集中のテンプレートから削除されません。この方法で追加したユーザーは、既存のリソース管理者に加えて、テンプレートのリソース管理者として追加されます。

   * 新しいテンプレートにリソース管理者を追加するには、「**新規テンプレート**」をクリックし、テンプレート名の横にある&#x200B;**その他**&#x200B;メニューをクリックし、「**編集**」をクリックします。

1. 「**概要**」セクションで、「**リソース管理者**」フィールドをクリックします。
1. テンプレートのリソース管理者として追加するユーザーの名前を入力し、その名前がリストに表示されたらクリックします。

   この手順を繰り返して、テンプレートに複数のリソース管理者を追加します。

1. 「**変更を保存**」をクリックします。
