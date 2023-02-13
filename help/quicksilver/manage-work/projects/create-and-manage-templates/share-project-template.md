---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートの共有
description: テンプレートをユーザーと共有することも、テンプレートレベルで次の共有オプションを使用して、テンプレートから作成されたプロジェクトをユーザーと共有する方法を定義することもできます。
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# プロジェクトテンプレートの共有

テンプレートをユーザーと共有することも、テンプレートレベルで次の共有オプションを使用して、テンプレートから作成されたプロジェクトをユーザーと共有する方法を定義することもできます。

Adobe Workfrontでオブジェクトを共有する場合、他のユーザーがそのオブジェクトの表示、投稿、編集をおこなうことを許可します。

Workfront権限について詳しくは、 [オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

テンプレートを共有する際にユーザーに与える権限について詳しくは、 [テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>テンプレートへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>テンプレートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## テンプレートの共有 {#share-a-template}

テンプレート共有を使用して、他のユーザーとテンプレートを共有できます。 このアクションは、テンプレートに対する権限を持つユーザーを定義します。

>[!NOTE]
>
>アクティブなユーザーをテンプレート所有者に指定すると、そのユーザーは自動的にテンプレートに対する管理権限を受け取ります。 テンプレート所有者に指定する方法については、 [プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

テンプレートを共有するには：

1. 次の **メインメニュー** アイコン ![](assets/main-menu-icon.png)をクリックし、 **テンプレート**.

1. 次のいずれかの操作を行います。\
   テンプレート名をクリックして開き、 **詳細** メニュー ![](assets/qs-more-icon-on-an-object.png)を、 **テンプレート共有**.

   または

   リストからテンプレートを選択し、共有アイコンをクリックします。 ![](assets/share-icon.png)を選択し、「**テンプレート。**

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、会社のみです。

1. 内 **テンプレートアクセス** ボックスで、テンプレートを共有するユーザー、チーム、役割、グループまたは会社を選択します。

   また、 **オプション** アイコンを使用して、テンプレートをシステム全体で使用できるようにします。

1. 共有する各エンティティのドロップダウンメニューから、次のいずれかを選択します。

   * **表示**:これらの権限を持つユーザーは、テンプレートを表示し、それを使用してプロジェクトを作成したり、既存のプロジェクトに添付したりできます。

      >[!TIP]
      >
      >プロジェクトを作成するには、Workfront管理者からプロジェクトへの編集アクセス権が与えられる必要があります。

   * **管理**:これらの権限を持つユーザーは、テンプレートを編集または削除できます。

      詳細設定について詳しくは、 ![](assets/gear-icon-in-access-levels.png) こちらから、 [テンプレート共有の詳細設定](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) 記事内 [テンプレートの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. 「**保存**」をクリックします。

## テンプレートからプロジェクトを共有する {#share-a-project-from-a-template}

テンプレートのプロジェクト共有を使用すると、テンプレートから作成されたプロジェクトに対する権限を持つユーザーをテンプレートレベルで定義できます。

テンプレートから作成された今後のプロジェクトをユーザーと共有するには：

1. 次のいずれかの操作を行います。\
   テンプレート名をクリックして開き、 **詳細** メニュー ![](assets/qs-more-icon-on-an-object.png)を、 **テンプレート共有**.

   ![テンプレートからプロジェクトを共有](assets/project-sharing-on-template-nwe-2022-350x172.png)

   または

   リストからテンプレートを選択し、 **共有**&#x200B;を選択し、「**プロジェクト。**

1. 内 **プロジェクトアクセス** ボックスで、テンプレートの共有先となるユーザー、チーム、ロール、グループまたは会社を選択します。

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、会社のみです。

1. 各エンティティのドロップダウンメニューから、次のいずれかを選択します。

   * **アクセスなし**:テンプレートにアクセスできないユーザーを指定できます。\
      このオプションは、テンプレートからプロジェクトを一括共有する場合にのみ使用できます。 
   * **表示**:これらの権限を持つユーザーは、テンプレートから作成されたプロジェクトを表示できます。
   * **投稿**:これらの権限を持つユーザーは、テンプレートから作成されたプロジェクトに投稿できます 
   * **管理**:これらの権限を持つユーザーは、このテンプレートから作成されたプロジェクトを管理または削除できます。

1. （オプション） **オプション** アイコンを使用して、プロジェクトをシステム全体で使用できるようにします。
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

## テンプレートとプロジェクトを一括で共有する

複数のテンプレートと、複数のテンプレートのプロジェクトを同時に共有できます。

>[!NOTE]
>
>複数のテンプレートを選択すると、個々のテンプレートに対する権限を既に持つユーザーは表示できません。

1. テンプレートのリストに移動します。
1. 複数のテンプレートを選択して、 ![共有](assets/share-icon.png).

   ![テンプレートまたはプロジェクトを一括で共有する](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、会社のみです。

1. クリック **テンプレート** 選択したテンプレートを共有するには、をクリックします。

   または

   クリック **プロジェクト** 選択したテンプレートから作成されるプロジェクトを共有する場合。

1. この記事の次の節で説明するように、引き続きテンプレートまたはプロジェクトを共有します。

   * [テンプレートの共有](#share-a-template)
   * [テンプレートからプロジェクトを共有する](#share-a-project-from-a-template)
