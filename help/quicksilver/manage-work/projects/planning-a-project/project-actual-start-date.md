---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの実際の開始日の概要
description: Adobe Workfront では、プロジェクト、タスクおよびイシューに実際の開始日があります。タスクおよびイシューの場合、この日付は「進行中」とマークされた日です。プロジェクトの場合、この日付はプロジェクトの最初のタスクが「進行中」としてマークされたか完了した日です。
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 93%

---

# プロジェクトの実際の開始日の概要

Adobe Workfront では、プロジェクト、タスクおよびイシューに実際の開始日があります。タスクおよびイシューの場合、この日付は「進行中」とマークされた日です。プロジェクトの場合、この日付はプロジェクトの最初のタスクが「進行中」としてマークされたか完了した日です。

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
   <td><p>ライト以上</p> 
   <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトに対する表示以上のアクセス権</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する表示権限またはそれ以上の権限</p>  </td> 
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
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Workfront の実際の開始日に関する考慮事項

* 実際の開始日は、プロジェクト、タスクおよびイシューの「詳細」セクションにあります。 
* プロジェクト、タスクまたはイシューの実際の開始日は、これらの項目が作成される際には入力されません。
* 実際の開始日は、プロジェクト、タスクまたはイシューで実際に作業が始まったときに入力されます。
* プロジェクトの作業がまだ始まっていない場合、「プロジェクト詳細」タブには実際の開始日が表示されません。

  まだ作業がまだ始まっていない場合、「タスクの詳細」と「イシューの詳細」タブには実際の開始日は空白で表示されます。

* タスクやイシューの実際の開始日は手動で変更できますが、プロジェクトの実際の開始日は変更できません。

## プロジェクトの実際の開始日に関する考慮事項

* Workfront では、次のいずれかのアクションが行われた場合、プロジェクトの実際の日付が自動的に設定されます。

   * タスクの担当者がタスクのステータスを「*新規*」から「*新規*」と同等でない他のステータスに変更する。

   * タスクの担当者がタスクの完了率を変更する。

     >[!IMPORTANT]
     >
     >プロジェクトが「現在」とマークされている場合、プロジェクトの実際の開始日は入力されません。プロジェクトに実際の開始日が入力されるのは、プロジェクトのタスクで実際の作業が開始されたときです。

     こうした場合、プロジェクトの実際の開始日は、プロジェクトで最も早く発生するタスクに対してこれらのアクションが実行された日時に設定されます。これは、プロジェクトが実際にこの日時に開始されたことを示します。

## プロジェクトの実際の開始日を確認

プロジェクトの実際の開始日は、次の領域で確認できます。

* プロジェクトの「詳細」セクション。
* プロジェクトのレポートまたはビュー（レポートのプロジェクトオブジェクトに実際の開始日を追加した場合）。

  レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

プロジェクトの「詳細」セクションで実際の開始日を確認する手順は、次のとおりです。

1. Workfrontの右上隅にある **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、「**プロジェクト**」をクリックします。
1. 実際の開始日を表示するプロジェクトをクリックします。
1. 左側のパネルで「**プロジェクト詳細**」をクリックし、「**概要**」セクションに移動します。

   実際の開始日は、プロジェクトの他の日付と共に表示されます。

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)


