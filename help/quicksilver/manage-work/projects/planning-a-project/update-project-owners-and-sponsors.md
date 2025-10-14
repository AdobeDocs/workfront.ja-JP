---
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの所有者とスポンサーの更新
description: Adobe Workfront でプロジェクトを作成すると、そのプロジェクトのプロジェクト所有者として自動的に設定されます。このフィールドは別のユーザーに更新できます。また、プロジェクトの「プロジェクトスポンサー」フィールドを更新することもできます。
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 85%

---


# プロジェクトの所有者とスポンサーの更新

<!--Audited: 07/2024-->

Adobe Workfront でプロジェクトを作成すると、自動的にそのプロジェクトのプロジェクト所有者として設定されます。このフィールドは別のユーザーに更新できます。また、プロジェクトの「プロジェクトスポンサー」フィールドを更新することもできます。

プロジェクトの所有者とスポンサーについて詳しくは、[プロジェクト所有者とスポンサーの概要](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md)を参照してください。

>[!TIP]
>
>テンプレートの所有者とスポンサーを特定できます。そのテンプレートからプロジェクトを作成すると、テンプレート所有者がプロジェクト所有者に、テンプレートスポンサーがプロジェクトスポンサーになります。
>
>テンプレートに所有者が設定されていない場合、チームプレートからプロジェクトを作成したユーザーがプロジェクト所有者になります。
>
>テンプレートの編集について詳しくは、[プロジェクトテンプレートを編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> <p>  </p> </td> 
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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td><p>新規：標準</p> 
   <p>現在：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限の編集</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## プロジェクトのプロジェクト所有者の更新

ユーザーをプロジェクトのプロジェクト所有者として追加すると、Workfront は自動的にそのユーザーにプロジェクトの表示権限を付与します。

1. 更新するプロジェクトに移動します。
1. 左側のパネルで「**プロジェクト詳細**」をクリックします。
1. 「プロジェクトの詳細」領域の右上隅にある **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/qs-edit-icon.png) をクリックしてから、「**概要** をクリックします。

1. 「**プロジェクト所有者**」フィールドのユーザーの名前を指定します。

   アクティブなユーザーのみをプロジェクト所有者として指定できます。

1. 「**変更を保存**」をクリックします。

   プロジェクトヘッダーおよび「プロジェクト詳細」エリアの「プロジェクト所有者」が更新されます。

   ![&#x200B; プロジェクトの利害関係者の所有者がハイライト表示されている &#x200B;](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## プロジェクトのプロジェクトスポンサーの更新

ユーザーをプロジェクトのプロジェクトスポンサーとして追加すると、Workfront は自動的にそのユーザーにプロジェクトの表示権限を付与します。

>[!TIP]
>
>プロジェクトスポンサーとして追加したユーザーがシステム管理者である場合、そのユーザーはプロジェクトの共有リストに追加されません。

1. 更新するプロジェクトに移動します。
1. 左パネルの「**プロジェクト詳細**」をクリックします。
1. 「プロジェクトの詳細」領域の右上隅にある **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/qs-edit-icon.png) をクリックしてから、「**概要** をクリックします。

1. 「**プロジェクトスポンサー**」フィールドのユーザーの名前を指定します。

   アクティブなユーザーのみをプロジェクトスポンサーとして指定できます。

1. 「**変更を保存**」をクリックします。

   「プロジェクト詳細」エリアの「プロジェクトスポンサー」が更新されます。

   ![&#x200B; プロジェクト関係者のスポンサーがハイライト表示 &#x200B;](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
