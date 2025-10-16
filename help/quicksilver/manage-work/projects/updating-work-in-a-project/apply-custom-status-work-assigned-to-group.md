---
product-area: projects
navigation-topic: update-work-in-a-project
title: グループに関連付けられた作業に状態を適用します。
description: プロジェクトがグループに関連付けられている場合は、システムレベルのステータスと、そのグループに関連付けられたカスタムステータスの両方を、そのプロジェクトのプロジェクト、タスク、またはイシューに適用できます。
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 86%

---

# グループに関連付けられた作業へのステータスの適用

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

プロジェクトがグループに関連付けられている場合、システムレベルのステータスと、そのグループに関連付けられたカスタムステータスの両方を、そのプロジェクト、またはタスクとイシューに適用できます。Adobe Workfront のグループステータスについて詳しくは、[ステータスを作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

>[!TIP]
>
>プロジェクトのみをグループに関連付けることができます。イシューとタスクは、それらが属するプロジェクトからグループを継承します。

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
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトの管理権限</p> </td> 
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
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## プロジェクトのグループとステータスを更新する

プロジェクトのグループを更新すると、タスクのステータス、イシュー、またはプロジェクトのステータスに使用できるオプションが、グループに合わせて変更されます。

1. [プロジェクトを作成](../../../manage-work/projects/create-projects/create-project.md)で説明されているように、プロジェクトに移動するか、新しいプロジェクトを作成します。
1. **その他** アイコン ![&#x200B; その他アイコン &#x200B;](assets/more-icon.png) をクリックしてから、**編集** をクリックします。

1. 「**概要**」セクションの下部近くに表示される「**プロジェクトを編集**」ボックスで、「**グループ**」ドロップダウンメニューからグループを選択します。

1. 「**ステータス**」ドロップダウンメニューから、「カスタムステータス」を選択します。

   >[!NOTE]
   >
   >「**グループ**」ドロップダウンメニューで別のグループを選択すると、「**ステータス**」メニューのカスタムステータスが新規グループに関連付けられるように自動的に変更されます。
   >
   >
   >![&#x200B; プロジェクトのカスタムステータスを含んで展開された「ステータス」ドロップダウン &#x200B;](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)
   >

1. プロジェクトのステータスを選択します。作成し、そのグループに適用したカスタムステータスがリストに表示されます。
