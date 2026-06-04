---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトのステータスの変更
description: 必要に応じて、プロジェクトのステータスを他の任意のステータスに、手動で更新できます。 プロジェクトの「完了モード」が「手動」に設定されている場合にのみ、プロジェクトのステータスを「完了」と同等のステータスに手動で更新できます。
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/PRLph0Euqn69SUFkRMT1N7BmJinnao-xfzMWWEE407Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 358
ht-degree: 85%

---

# プロジェクトのステータスの変更

<!--Audited: 02/2024-->

必要に応じて、プロジェクトのステータスを他の任意のステータスに、手動で更新できます。

プロジェクトの「完了モード」が「手動」に設定されている場合にのみ、プロジェクトのステータスを「完了」と同等のステータスに手動で更新できます。

それ以外の場合、プロジェクトのすべてのタスクとイシューが完了して承認されると、Adobe Workfront は自動的にプロジェクトを「完了」としてマークします。

プロジェクトの完了モードについて詳しくは、[プロジェクトの編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)を参照してください。

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
   <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限を管理</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## 特定のステータスに更新する際の考慮事項

* **プロジェクトを完了に更新する場合：**&#x200B;プロジェクトですべてのタスクとイシューが完了していることを確認します。 プロジェクトに完了していないタスクやイシューがある場合は、プロジェクトの「完了」のステータス、または「完了」と同等のステータスは選択できません。 これには、「完了 - 保留中の承認」ステータスのタスクまたはイシューを承認する場合も含まれます。
* **プロジェクトを「完了」から「現在」に更新する場合：**&#x200B;プロジェクトのすべてのタスクとイシューが完了した場合は、プロジェクトの完了モードが「手動」に設定されていることを確認します。 プロジェクトの完了モードが「自動」の場合、プロジェクトのステータスは「完了」のままになります。

## プロジェクトステータスを変更する

1. ステータスを更新するプロジェクトに移動します。
1. プロジェクトヘッダーの「**ステータス**」フィールドでステータスの名前をクリックし、新しいステータスを選択します。

   ![&#x200B; プロジェクトの状態を変更](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   または

   プロジェクト名の横にある&#x200B;**詳細** メニュー![詳細メニュー](assets/qs-more-menu.png)をクリックし、**編集**&#x200B;をクリックして、**ステータス** フィールドで新しいステータスを選択し、**保存**&#x200B;をクリックします。

   プロジェクトのステータスは、選択したステータスに更新されます。
