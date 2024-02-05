---
product-area: projects
navigation-topic: create-projects
title: Microsoft Project からプロジェクトを読み込む
description: Microsoft Project から Adobe Workfront にプロジェクトを読み込み、すべてのプロジェクトを 1 つのアプリケーションで管理できます。Microsoft Project からプロジェクトを読み込むたびに、Workfront に新しいプロジェクトが作成されます。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 98%

---

# Microsoft Project からプロジェクトを読み込む

Microsoft Project から Adobe Workfront にプロジェクトを読み込み、すべてのプロジェクトを 1 つのアプリケーションで管理できます。Microsoft Project からプロジェクトを読み込むたびに、Workfront に新しいプロジェクトが作成されます。

>[!IMPORTANT]
>
>すべての Microsoft Project フィールドが Workfront に転送されるわけではありません。
>
>Workfront と Microsoft Project の間のフィールドの互換性について詳しくは、[Microsoft Project フィールドを Adobe Workfront プロジェクトにマッピング](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md)を参照してください。

## アクセス要件

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>新しいライセンス：標準 </p> 
   または
   <p>現在のライセンス：プラン </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。プロジェクトへのアクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">プロジェクトへのアクセス権の付与</a>を参照してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。 </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトを作成すると、プロジェクトに対する管理権限が自動的に付与されます。 </p> <p> プロジェクト権限について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront でのプロジェクトの共有</a>を参照してください。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

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

## MS プロジェクトからプロジェクトを作成する

プロジェクトは、メインメニューのプロジェクト領域、またはポートフォリオまたはプログラムのプロジェクト領域から作成できます。

1. Microsoft Project に移動し、Workfront で読み込み元のプロジェクトを開きます。
1. **ファイル**、次に&#x200B;**名前を付けて保存**&#x200B;の順にクリックして、プロジェクトを .xml ファイルとして保存します。

1. Workfront にログインします。
1. 次のいずれかの操作を行います。

   * 「**メインメニュー** ![](assets/main-menu-icon.png)」、「**プロジェクト**」の順にクリックして、**新規プロジェクト**&#x200B;を展開します。
   * ポートフォリオに移動し、**新規プロジェクト**&#x200B;を展開します。
   * プログラムに移動し、「**新規プロジェクト**」を展開します。
   * グループ管理者の場合は、管理するグループの「プロジェクト」セクションでプロジェクトを作成することもできます。詳しくは、[グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)を参照してください。

1. 「**MS プロジェクトを読み込む**」オプションを選択します。

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 「**ファイルの選択**」をクリックし、Microsoft Project から書き出した .xml ファイルをコンピューター上で参照します。
1. 選択したファイルを読み込みます。

   Workfront によって読み込み処理が開始され、Microsoft Project から書き出されたファイルに基づいて新しいプロジェクトが作成されます。

   読み込み処理が完了すると、新しいプロジェクトページが表示され、読み込みが正常に完了したことを示す確認が表示されます。

   >[!NOTE]
   >
   >Workfront では、ファイルのアップロードに 15 分の時間制限があります。ファイルのアップロードにそれ以上の時間がかかる場合は、プロジェクトを小さなプロジェクトに分割し、個別に読み込むことをお勧めします。タスクを Workfront に読み込みしたら、タスクを 1 つのプロジェクトから別のプロジェクトに移動して、1 つのプロジェクトに結合します。タスクの移動の詳細については、[タスクの移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。

1. （オプション）Workfront でプロジェクトの編集を続けます。プロジェクトの編集の詳細については、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

   テンプレートから作成された新しいプロジェクトのステータスは、Workfront 管理者がプロジェクト環境設定領域で定義したステータス、またはグループ管理者がグループプロジェクト環境設定領域で定義したステータスに対応します。プロジェクト環境設定の詳細については、[システム全体のプロジェクト環境設定の設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。
