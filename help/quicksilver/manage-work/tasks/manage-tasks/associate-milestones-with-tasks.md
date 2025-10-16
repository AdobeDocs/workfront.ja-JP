---
product-area: projects
navigation-topic: manage-tasks
title: マイルストーンとタスクの関連付け
description: タスクにマイルストーンを関連付けることで、プロジェクト期間の重要なステップに達したことを示すことができます。プロジェクトのタスクにマイルストーンを関連付けるには、まずマイルストーンパスをプロジェクトに関連付ける必要があります。
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 93%

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
   <p>ワークまたはそれ以上</p> 
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
</table>-->

## 前提条件

タスクにマイルストーンを関連付けるには、まず以下が必要です。

* [マイルストーンパスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)の説明に従って、Workfront の管理者がマイルストーンパスを作成する必要があります。

* マイルストーンパスをプロジェクトに関連付ける必要があります。

  詳しくは、[プロジェクトの編集](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)を参照してください。

* マイルストーンパスをプロジェクトに関連付けるには、プロジェクトのステータスが「計画」または「進行中」になっている必要があります。

  >[!TIP]
  >
  >マイルストーンビューを使用してプロジェクトのマイルストーンの進行状況の概要を最も適切に把握するには、親タスクを作成し、それらをプロジェクトの各主要フェーズに関連付ける必要があります。次に、これらの親タスクをマイルストーンパスの各マイルストーンに関連付けます。

## タスクにマイルストーンを関連付け

マイルストーンパスをプロジェクトに関連付けたら、タスクにマイルストーンを割り当てることができます。

1. タスクに移動し、タスク名の右にある&#x200B;**その他**&#x200B;アイコン ![](assets/more-icon.png) をクリックして「**編集**」を選択します。

   タスクとマイルストーンには 1:1 の関係があります。 同じマイルストーンを複数のタスクに関連付けることはできません。各タスクを 1 つのマイルストーンにリンクすることも、各マイルストーンを 1 つのタスクにマッピングすることもできます。

1. 「**設定**」をクリックし、タスクの&#x200B;**マイルストーン**&#x200B;フィールドでマイルストーンを選択します。
1. 「**保存**」をクリックします。
1. （オプション）タスクの一覧で、**ステータスアイコン**&#x200B;の列を追加して、どのタスクにマイルストーンがあるか特定します。「ステータスアイコン」の列にマイルストーンのひし形インジケーターが表示されます。

   詳しくは、[Adobe Workfront でのビューの作成または編集](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)を参照してください。

   ![](assets/amwt3.png)

1. （オプション）プロジェクトの一覧で、**マイルストーン**&#x200B;のビューを選択して、マイルストーンタスクの進捗状況を特定します。

   ![](assets/milestone-view-project-list.png)
