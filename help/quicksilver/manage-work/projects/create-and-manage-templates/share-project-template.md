---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートを共有
description: テンプレートをユーザーと共有したり、テンプレートレベルで以下の共有オプションを使用して、テンプレートから作成されたプロジェクトをユーザーと共有する方法を定義したりできます。
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 91%

---

# プロジェクトテンプレートを共有

テンプレートをユーザーと共有したり、テンプレートレベルで以下の共有オプションを使用して、テンプレートから作成されたプロジェクトをユーザーと共有する方法を定義したりできます。

Adobe Workfront でオブジェクトを共有する場合、他のユーザーがそのオブジェクトの表示、オブジェクトへの参加、あるいは編集を行うことを許可します。

Workfront の権限について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

テンプレートを共有する際にユーザーに付与できる権限について詳しくは、[テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>テンプレートへの編集アクセス</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>テンプレートに対する管理権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## テンプレートの共有 {#share-a-template}

テンプレート共有を使用して、他のユーザーとテンプレートを共有できます。このアクションは、テンプレートに対する権限を持つユーザーを定義します。

>[!NOTE]
>
>アクティブなユーザーをテンプレート所有者に指定すると、そのユーザーは自動的にテンプレートに対する管理権限を受け取ります。テンプレート所有者に指定する方法については、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

テンプレートを共有するには、以下のように行います。

1. **メインメニュー** アイコン ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) から、「**テンプレート**」をクリックします。

1. 次のいずれかの操作を行います。\
   テンプレートの名前をクリックして開き、**詳細** メニュー ![&#x200B; 詳細アイコン &#x200B;](assets/qs-more-icon-on-an-object.png)/**テンプレート共有** をクリックします。

   または

   リストからテンプレートを選択し、共有アイコン ![](assets/share-icon.png) をクリックし、さらに「**テンプレート**」をクリックします。

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、または会社のみです。

1. 「**テンプレートアクセス**」ボックスで、テンプレートを共有するユーザー、チーム、役割、グループ、会社を選択します。

   **オプション**&#x200B;アイコンをクリックして、テンプレートをシステム全体で使用できるようにします。

1. 共有するそれぞれのエンティティのドロップダウンメニューから、次のいずれかを選択します。

   * **表示**：この権限を持つユーザーは、テンプレートを表示し、テンプレートを使用してプロジェクトを作成したり、既存のプロジェクトに添付したりすることができます。

     >[!TIP]
     >
     >プロジェクトを作成できるようにするには、Workfront 管理者がプロジェクトへの編集アクセス権を付与する必要があります。

   * **管理**：この権限を持つユーザーは、テンプレートを編集または削除できます。

     ここで利用できる詳細設定 ![](assets/gear-icon-in-access-levels.png) について詳しくは、[テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)の記事にある[テンプレート共有の詳細設定](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions)の節を参照してください。

1. 「**保存**」をクリックします。

## テンプレートからプロジェクトを共有 {#share-a-project-from-a-template}

テンプレート「プロジェクトの共有」を使用すると、テンプレートから作成されたプロジェクトに対する権限を持つユーザーを、テンプレートレベルで定義できます。

テンプレートから作成された今後のプロジェクトをユーザーと共有するには、以下のように行います。

1. 次のいずれかの操作を行います。\
   テンプレートの名前をクリックして開き、**詳細** メニュー ![&#x200B; 詳細アイコン &#x200B;](assets/qs-more-icon-on-an-object.png)/**テンプレート共有** をクリックします。

   ![テンプレートからプロジェクトを共有](assets/project-sharing-on-template-nwe-2022-350x172.png)

   または

   リストからテンプレートを選択し、「**共有**」をクリックし、さらに「**プロジェクト**」をクリックします。

1. 「**プロジェクトアクセス**」ボックスで、テンプレートを共有するユーザー、チーム、役割、グループ、会社を選択します。

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、または会社のみです。

1. 各エンティティのドロップダウンメニューから、次のいずれかを選択します。

   * **アクセスなし**：テンプレートにアクセスできないユーザーを指定できます。\
     このオプションは、テンプレートからプロジェクトを一括共有する場合にのみ使用できます。 
   * **表示**：この権限を持つユーザーは、テンプレートから作成されたプロジェクトを表示できます。
   * **参加**：この権限を持つユーザーは、テンプレートから作成されたプロジェクトに参加できます。
   * **管理**：この権限を持つユーザーは、このテンプレートから作成されたプロジェクトを管理または削除できます。

1. （オプション）**オプション**&#x200B;アイコンをクリックして、プロジェクトをシステム全体で使用できるようにします。
1. 「**保存**」をクリックします。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## テンプレートとテンプレートからのプロジェクトを一括で共有

複数のテンプレートと、複数のテンプレートからのプロジェクトを同時に共有できます。

>[!NOTE]
>
>複数のテンプレートを選択した場合、個々のテンプレートに対して権限を既に持っているユーザーを表示することができません。

1. テンプレートのリストに移動します。
1. 複数のテンプレートを選択し、「![共有](assets/share-icon.png)」をクリックします。

   ![テンプレートまたはプロジェクトを一括で共有](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、または会社のみです。

1. 「**テンプレート**」をクリックして、選択したテンプレートを共有します。

   または

   「**プロジェクト**」をクリックして、選択したテンプレートから作成されるプロジェクトを共有します。

1. この記事の以下の節で説明するように、テンプレートまたはプロジェクトを共有していきます。

   * [テンプレートを共有](#share-a-template)
   * [テンプレートからプロジェクトを共有](#share-a-project-from-a-template)
