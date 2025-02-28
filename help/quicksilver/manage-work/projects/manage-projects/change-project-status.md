---
product-area: projects
navigation-topic: manage-projects
title: プロジェクトのステータスの変更
description: 必要に応じて、プロジェクトのステータスを他の任意のステータスに、手動で更新できます。プロジェクトの「完了モード」が「手動」に設定されている場合にのみ、プロジェクトのステータスを「完了」と同等のステータスに手動で更新できます。
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 91%

---

# プロジェクトのステータスの変更

<!--Audited: 02/2024-->

必要に応じて、プロジェクトのステータスを他の任意のステータスに、手動で更新できます。

プロジェクトの「完了モード」が「手動」に設定されている場合にのみ、プロジェクトのステータスを「完了」と同等のステータスに手動で更新できます。

それ以外の場合、プロジェクトのすべてのタスクとイシューが完了して承認されると、Adobe Workfront は自動的にプロジェクトを「完了」としてマークします。

プロジェクトの完了モードについて詳しくは、[プロジェクトの編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規：標準 </p> 
   または
   <p>現在：プラン </p>
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

&#42;保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 特定のステータスに更新する際の考慮事項

* **プロジェクトを完了に更新する場合：**&#x200B;プロジェクトですべてのタスクとイシューが完了していることを確認します。プロジェクトに完了していないタスクやイシューがある場合は、プロジェクトの「完了」のステータス、または「完了」と同等のステータスは選択できません。これには、「完了 - 保留中の承認」ステータスのタスクまたはイシューを承認する場合も含まれます。
* **プロジェクトを「完了」から「現在」に更新する場合：**&#x200B;プロジェクトのすべてのタスクとイシューが完了した場合は、プロジェクトの完了モードが「手動」に設定されていることを確認します。プロジェクトの完了モードが「自動」の場合、プロジェクトのステータスは「完了」のままです。

## プロジェクトステータスを変更する

1. ステータスを更新するプロジェクトに移動します。
1. プロジェクトヘッダーの「**ステータス**」フィールドでステータスの名前をクリックし、新しいステータスを選択します。

   ![ プロジェクトステータスの変更 ](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   または

   プロジェクト名の横にある **詳細** メニュー ![ 詳細メニュー ](assets/qs-more-menu.png) をクリックして、**編集** をクリックし、**ステータス** フィールドで新しいステータスを選択して、**保存** をクリックします。

   プロジェクトのステータスは、選択したステータスに更新されます。
