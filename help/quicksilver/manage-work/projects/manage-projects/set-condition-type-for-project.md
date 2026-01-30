---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトの状態タイプの設定
description: プロジェクトマネージャーは、プロジェクトの状況タイプを更新して、プロジェクトの状況の計算方法を決定できます。プロジェクト状況は、プロジェクトの進行状況を視覚的に表したものです。
author: Alina
feature: Work Management
exl-id: e6b99c48-5ccc-4956-8465-6f22f14468ef
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 72%

---

# プロジェクトの状況タイプを設定

プロジェクトマネージャーは、プロジェクトの状況タイプを更新して、プロジェクトの状況の計算方法を決定できます。プロジェクト状況は、プロジェクトの進行状況を視覚的に表したものです。

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
   <td><p>標準</p> 
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <ul> 
     <li> <p>プロジェクトに権限を付与して「プロジェクトの詳細」領域で条件タイプを編集する </p> </li> 
     <li> <p>プロジェクトに対する権限を管理し、「プロジェクトを編集」ボックスで条件タイプを編集します</p> </li> 
    </ul> </td> 
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
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a project to edit the Condition Type in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit the Condition Type in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## プロジェクトの状況タイプの設定

1. 状況タイプを更新するプロジェクトに移動します。
1. 次のいずれかの操作を行います。

   * プロジェクト名の右側にある **その他** メニュー ![&#x200B; その他メニュー &#x200B;](assets/qs-more-menu.png) をクリックし、**編集** をクリックします。
   * 左側のパネルにある「**プロジェクト詳細**」をクリックします。

   ![&#x200B; 条件タイプを更新 &#x200B;](assets/update-condition-type-nwe-350x108.png)

1. 「**状況タイプ**」フィールドで、次のいずれかを選択します。

   * **手動：** プロジェクト所有者が、プロジェクトに対して手動で状況を設定します。

     この場合、プロジェクト所有者は、プロジェクトヘッダーまたは「プロジェクト詳細」セクションで、プロジェクトの状況を更新できます。

   * **進捗ステータス：** Workfront は、プロジェクトの進捗ステータスに基づいて状況を設定します。進捗ステータスの計算方法について詳しくは、[プロジェクトの進捗ステータスの概要](../../../manage-work/projects/planning-a-project/project-progress-status.md)を参照してください。

1. 「プロジェクトを編集」ボックスで条件タイプを修正したら、「**保存**」をクリックします。

   「プロジェクト詳細」セクションで条件タイプを変更したら、「**変更を保存**」をクリックします。


