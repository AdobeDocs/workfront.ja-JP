---
product-area: resource-management
navigation-topic: resource-pools
title: リソースプールとプロジェクトおよびテンプレートを関連付ける
description: リソースプールは、Adobe Workfront でのリソースの管理に役立つ、ユーザーのコレクションです。
author: Alina
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: 171ccfe5d2bc9825c9cdb195df1a97a32e515646
workflow-type: ht
source-wordcount: '649'
ht-degree: 100%

---

# リソースプールとプロジェクトおよびテンプレートを関連付ける


<!-- drafted for bulk editing projects: keep this in yellow till this releases to ALL customers - May 1, 2023

Also - take out all the references to Preview and Prod at prod final
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->


<!--
<p>The sections about how to add resource pools to templates, projects are duplicated from the articles listed in those sections (Editing Projects, Creating a Template, etc).</p>
<p>***I decided to keep these steps here, though, because it's hard to parse through those much lunger articles for just updating this one field.)</p>
-->

リソースプールは、Adobe Workfront でのリソースの管理に役立つ、ユーザーのコレクションです。

リソースプールを作成したら、プロジェクトまたはテンプレートに関連付けて、プロジェクトのリソースに対して後で予算を設定できます。

プロジェクトを開始する前にリソースプールを作成してプロジェクトに関連付け、リソースに対して予算を設定することをお勧めします。

リソースプールについて詳しくは、[リソースプールの概要](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)を参照してください。

リソースプールの作成について詳しくは、[リソースプールの作成](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)を参照してください。

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
   <td> <p>リソースプールの管理へのアクセスを含む、リソース管理への編集アクセス権</p> <p>プロジェクト、テンプレート、ユーザーへのアクセスの編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リソースプールを関連付けるプロジェクト、テンプレート、およびユーザーの権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 1 つのプロジェクトまたはテンプレートへのリソースプールの関連付け

リソースプールにプロジェクトを関連付けるのと同じ方法で、テンプレートにリソースプールを関連付けることができます。この記事では、リソースプールをプロジェクトに関連付ける方法について説明します。

1. プロジェクトに移動し、プロジェクト名の横にある&#x200B;**その他**&#x200B;アイコン ![](assets/more-icon.png) をクリックし、「**編集**」をクリックします。

1. 「**プロジェクト設定**」をクリックします。

1. 「**リソースプール**」フィールドでリソースプールの名前の入力を開始し、リストにその名前が表示されたら選択します。\
   1 つのプロジェクトまたはテンプレートに複数のリソースプールを関連付けることができます。

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. 「**保存**」をクリックします。

プロジェクトを編集してリソースプールに関連付ける方法について詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

テンプレートを編集してリソースプールに関連付ける方法について詳しくは、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

## 複数のプロジェクトまたはテンプレートへのリソースプールの一括での関連付け

複数のプロジェクトまたはテンプレートを一括で編集し、同じリソースプールをすべて同時に関連付けることができます。

リソースプールをプロジェクトに関連付けるのと同じ方法で、リソースプールをテンプレートに関連付けることができます。

リソースプールを複数のプロジェクトに一括で関連付けるには：

1. プロジェクトのリストに移動します。
1. 複数のプロジェクトを選択し、**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。

1. 「**設定**」をクリックします。
1. 「**リソースプール**」フィールドでリソースプールの名前の入力を開始し、リストでその名前が表示されたら選択します。\
   プロジェクトまたはテンプレートには、複数のリソースプールを関連付けることができます。

   >[!NOTE]
   >
   >* テンプレートを一括で編集する場合は、選択したすべてのテンプレートに共通のリソースプールのみがこのフィールドに表示されます。選択したテンプレートに共有リソースプールがない場合、このフィールドは空です。ここで指定したリソースプールは、プロジェクトまたはテンプレートの個々のリソースプールを上書きします。
   >
   >* プロジェクトを一括で編集する際に、選択したプロジェクトに異なるリソースプールがある場合は、「複数の値」のインジケーターが表示されます。プロジェクトのリソースプールを一括で追加する場合、選択したプロジェクトにすべてのプールが追加され、元のリソースプールが上書きされます。

   ![add_resource_pools_to_multiple_projects.png](assets/add-resource-pools-to-multiple-projects-350x358.png)

1. 「**変更を保存**」をクリックします。\
   リソースプールがプロジェクトまたはテンプレートに関連付けられていると、リソースプランナー内のプロジェクトに対するユーザー割り当ての予算を設定できます。\
   リソースプランナーについて詳しくは、[リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

プロジェクトを一括編集する方法について詳しくは、[プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md)内の「プロジェクトを一括編集」の節を参照してください。

テンプレートを一括編集する方法について詳しくは、[プロジェクトテンプレートを編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)内の「テンプレートを一括編集」の節を参照してください。
