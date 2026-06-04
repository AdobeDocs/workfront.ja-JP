---
product-area: projects
navigation-topic: manage-tasks
title: マイルストーンとタスクの関連付け
description: タスクにマイルストーンを関連付けることで、プロジェクト期間の重要なステップに達したことを示すことができます。 プロジェクトのタスクにマイルストーンを関連付けるには、まずマイルストーンパスをプロジェクトに関連付ける必要があります。
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/rKFISDf42SK5rzZ4Wj09sdSHme-s8D8xSsZzQuumDQw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 372
ht-degree: 90%

---

# タスクへのマイルストーンの関連付け

<!--Audited: 01/2024-->

タスクにマイルストーンを関連付けて、プロジェクトの全期間中に重要なステップに達したときに、それを示すことができます。

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
   <p>Work またはそれ以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクへのアクセスを編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する管理権限</p></td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   <p>Current license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## 前提条件

タスクにマイルストーンを関連付けるには、まず以下が必要です。

* [マイルストーンパスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)の説明に従って、Workfront の管理者がマイルストーンパスを作成する必要があります。

* マイルストーンパスをプロジェクトに関連付ける必要があります。

  詳しくは、[プロジェクトの編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)を参照してください。

* マイルストーンパスをプロジェクトに関連付けるには、プロジェクトのステータスが「計画」または「進行中」になっている必要があります。

  >[!TIP]
  >
  >マイルストーンビューを使用してプロジェクトのマイルストーンの進行状況の概要を最も適切に把握するには、親タスクを作成し、それらをプロジェクトの各主要フェーズに関連付ける必要があります。 次に、これらの親タスクをマイルストーンパスの各マイルストーンに関連付けます。

## タスクにマイルストーンを関連付け

マイルストーンパスをプロジェクトに関連付けたら、タスクにマイルストーンを割り当てることができます。

1. タスクに移動し、タスク名の右側にある&#x200B;**詳細** アイコン ![詳細アイコン &#x200B;](assets/more-icon.png)をクリックしてから、**編集**&#x200B;をクリックします。

   タスクとマイルストーンの関係は1:1です。 同じマイルストーンを複数のタスクに関連付けることはできません。 各タスクを 1 つのマイルストーンにリンクすることも、各マイルストーンを 1 つのタスクにマッピングすることもできます。

1. 「**設定**」をクリックし、タスクの&#x200B;**マイルストーン**&#x200B;フィールドでマイルストーンを選択します。
1. 「**保存**」をクリックします。
1. （オプション）タスクの一覧で、**ステータスアイコン**&#x200B;の列を追加して、どのタスクにマイルストーンがあるか特定します。 「ステータスアイコン」の列にマイルストーンのひし形インジケーターが表示されます。

   詳しくは、[Adobe Workfront でのビューの作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)を参照してください。

   ![&#x200B; ステータスアイコン &#x200B;](assets/amwt3.png)

1. （オプション）プロジェクトの一覧で、**マイルストーン**&#x200B;のビューを選択して、マイルストーンタスクの進捗状況を特定します。

   ![&#x200B; マイルストーンビュープロジェクトリスト &#x200B;](assets/milestone-view-project-list.png)
