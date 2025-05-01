---
product-area: projects
navigation-topic: create-projects
title: Microsoft Project からプロジェクトを読み込む
description: Microsoft Project から Adobe Workfront にプロジェクトを読み込み、すべてのプロジェクトを 1 つのアプリケーションで管理できます。Microsoft Project からプロジェクトを読み込むたびに、Workfront に新しいプロジェクトが作成されます。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: b38c98ec79617a78c76510bcb109da2ff83247af
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 65%

---

# Microsoft Project からプロジェクトを読み込む

<!-- Audited: 4/2025 -->

Microsoft Project から Adobe Workfront にプロジェクトを読み込み、すべてのプロジェクトを 1 つのアプリケーションで管理できます。Microsoft Project からプロジェクトを読み込むたびに、Workfront に新しいプロジェクトが作成されます。

>[!IMPORTANT]
>
>すべての Microsoft Project フィールドが Workfront に転送されるわけではありません。
>
>Workfront と Microsoft Project の間のフィールドの互換性について詳しくは、[Microsoft Project フィールドを Adobe Workfront プロジェクトにマッピング](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：標準 </p> 
   または
   <p>現在：プラン </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトを作成すると、プロジェクトに対する管理権限が自動的に付与されます。 </p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--old permissions model: 

You must have the following access to perform the steps in this article:

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
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## MS プロジェクトからのプロジェクトの作成

プロジェクトは、**メインメニュー** の **プロジェクト** エリアから、またはポートフォリオやプログラムの **プロジェクト** エリアから作成できます。

1. Microsoft プロジェクトにログインし、から読み込むプロジェクトをWorkfrontで開きます。
1. **ファイル**、次に&#x200B;**名前を付けて保存**&#x200B;の順にクリックして、プロジェクトを .xml ファイルとして保存します。

1. Workfront にログインします。
1. 次のいずれかの操作を行います。

   * Workfrontの右上隅にある **メインメニュー**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックするか、左上隅にある **メインメニュー**![ メインメニューライン ](assets/lines-main-menu.png) をクリックします（使用可能な場合）。**プロジェクト** をクリックしてから、**新規プロジェクト** を展開します。
   * ポートフォリオに移動し、**新規プロジェクト**&#x200B;を展開します。
   * プログラムに移動し、「**新規プロジェクト**」を展開します。
   * グループ管理者の場合は、管理するグループの **プロジェクト** セクションでプロジェクトを作成できます。 詳しくは、[グループのプロジェクトの作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)を参照してください。

1. 「**MS Project をインポート**」をクリックします。 **MS ファイルのインポート** ダイアログボックスが表示されます。

   ![ 新規プロジェクトドロップダウン ](assets/import-ms-project-option.png)

1. **ファイルを選択** をクリックして、Microsoft Project から書き出した.xml ファイルを参照します。
1. 選択したファイルを読み込みます。 Workfront によって読み込み処理が開始され、Microsoft Project から書き出されたファイルに基づいて新しいプロジェクトが作成されます。

   読み込み処理が完了すると、新しいプロジェクトページが表示され、読み込みが正常に完了したことを示す確認が表示されます。

   >[!NOTE]
   >
   >Workfront では、ファイルのアップロードに 15 分の時間制限があります。ファイルのアップロードにそれ以上の時間がかかる場合は、プロジェクトを小さなプロジェクトに分割し、個別に読み込むことをお勧めします。タスクを Workfront に読み込みしたら、タスクを 1 つのプロジェクトから別のプロジェクトに移動して、1 つのプロジェクトに結合します。タスクの移動の詳細については、[タスクの移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。

1. （オプション）Workfront でプロジェクトの編集を続けます。プロジェクトの編集の詳細については、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。


   >[!NOTE]
   >
   >テンプレートから作成された新しいプロジェクトのステータスは、「**プロジェクト環境設定**」領域でWorkfront管理者が定義したステータス、または「**グループプロジェクト環境設定**」領域でグループ管理者が定義したステータスに対応します。 プロジェクト環境設定について詳しくは、[システム全体のプロジェクト環境設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。
