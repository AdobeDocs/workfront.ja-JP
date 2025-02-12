---
product-area: resource-management
navigation-topic: resource-pools
title: リソース プールとプロジェクトおよびテンプレートの関連付け
description: リソースプールは、Adobe Workfront でのリソースの管理に役立つ、ユーザーのコレクションです。
author: Lisa
feature: Resource Management
exl-id: bbfe8257-ff02-4f06-9763-3f2ae4871c9d
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 86%

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

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：任意</p>
       <p>または</p>
       <p>現在：Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>リソース プール管理へのアクセスを含むリソース管理へのアクセスを編集します</p> <p>プロジェクト、テンプレート、ユーザーへのアクセスの編集</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>リソース プールを関連付けるプロジェクト、テンプレート、およびユーザーの権限の管理</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 1 つのプロジェクトまたはテンプレートへのリソースプールの関連付け

リソースプールにプロジェクトを関連付けるのと同じ方法で、テンプレートにリソースプールを関連付けることができます。この記事では、リソースプールをプロジェクトに関連付ける方法について説明します。

1. プロジェクトに移動して、プロジェクト名の横にある **詳細** アイコン ![ 詳細アイコン ](assets/more-icon.png) をクリックし、**編集** をクリックします。

1. 「**プロジェクト設定**」をクリックします。

1. 「**リソースプール**」フィールドでリソースプールの名前の入力を開始し、リストにその名前が表示されたら選択します。\
   1 つのプロジェクトまたはテンプレートに複数のリソースプールを関連付けることができます。

   ![ プロジェクト設定 ](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. 「**保存**」をクリックします。

プロジェクトを編集してリソースプールに関連付ける方法について詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

テンプレートを編集してリソースプールに関連付ける方法について詳しくは、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

## 複数のプロジェクトまたはテンプレートへのリソースプールの一括での関連付け

複数のプロジェクトまたはテンプレートを一括で編集し、同じリソースプールをすべて同時に関連付けることができます。

リソースプールをプロジェクトに関連付けるのと同じ方法で、リソースプールをテンプレートに関連付けることができます。

リソースプールを複数のプロジェクトに一括で関連付けるには：

1. プロジェクトのリストに移動します。
1. 複数のプロジェクトを選択し、リスト上部の **編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

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
