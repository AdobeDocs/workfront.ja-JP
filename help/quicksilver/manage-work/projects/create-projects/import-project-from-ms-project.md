---
product-area: projects
navigation-topic: create-projects
title: Microsoft Project からプロジェクトを読み込む
description: Microsoft Project から Adobe Workfront にプロジェクトを読み込み、すべてのプロジェクトを 1 つのアプリケーションで管理できます。 Microsoft Project からプロジェクトを読み込むたびに、Workfront に新しいプロジェクトが作成されます。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/drxvgi-xQLjEt5JOL6-MxLdkmVcXxkcXMN14nwmNZvs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 604
ht-degree: 58%

---

# Microsoft Project からプロジェクトを読み込む

<!-- Audited: 10/2025 -->

Microsoft Project から Adobe Workfront にプロジェクトを読み込み、すべてのプロジェクトを 1 つのアプリケーションで管理できます。 Microsoft Project からプロジェクトを読み込むたびに、Workfront に新しいプロジェクトが作成されます。

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
   <td> <p>プロジェクトへのアクセスを編集</p> 
   <p>プロジェクトをポートフォリオまたはプログラムに追加する場合は、「ポートフォリオとプログラムの編集」アクセス権が必要です。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトを作成すると、プロジェクトに対する管理権限が自動的に付与されます。</p>
   <p>プロジェクトをポートフォリオまたはプログラムに追加する場合は、ポートフォリオとプログラムに対する管理権限が必要です。</p>
   </td> 
    </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
old permissions model: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## MS プロジェクトからのプロジェクトの作成

プロジェクトは、**メインメニュー**&#x200B;の&#x200B;**プロジェクト**&#x200B;領域、またはポートフォリオまたはプログラムの&#x200B;**プロジェクト**&#x200B;領域から作成できます。

1. Microsoft プロジェクトにログインし、読み込むプロジェクトをWorkfrontで開きます。
1. **ファイル**、次に&#x200B;**名前を付けて保存**&#x200B;の順にクリックして、プロジェクトを .xml ファイルとして保存します。

1. Workfront にログインします。
1. 次のいずれかの操作を行います。

   * 左上隅の&#x200B;**[!UICONTROL メインメニュー]** アイコン ![ メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックし、**プロジェクト**&#x200B;をクリックして&#x200B;**新規プロジェクト**&#x200B;を展開します。
   * ポートフォリオに移動し、**新規プロジェクト**&#x200B;を展開します。
   * プログラムに移動し、「**新規プロジェクト**」を展開します。
   * グループ管理者の場合は、管理するグループの&#x200B;**プロジェクト** セクションでプロジェクトを作成できます。 詳しくは、[グループのプロジェクトの作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)を参照してください。

1. 「**MS プロジェクトの読み込み**」をクリックします。

   ![新規プロジェクトのドロップダウン ](assets/import-ms-project-option.png)

   「**MS ファイルを読み込み**」ボックスが開きます。

1. 「**ファイルを選択**」をクリックし、Microsoft プロジェクトから書き出したコンピューター上の.xml ファイルを参照します。
1. 選択したファイルを読み込みます。 Workfront によって読み込み処理が開始され、Microsoft Project から書き出されたファイルに基づいて新しいプロジェクトが作成されます。

   >[!NOTE]
   >
   >Workfront では、ファイルのアップロードに 15 分の時間制限があります。 ファイルのアップロードにそれ以上の時間がかかる場合は、プロジェクトを小さなプロジェクトに分割し、個別に読み込むことをお勧めします。 タスクを Workfront に読み込みしたら、タスクを 1 つのプロジェクトから別のプロジェクトに移動して、1 つのプロジェクトに結合します。 タスクの移動の詳細については、[タスクの移動](../../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。

   読み込み処理が完了すると、新しいプロジェクトページが表示され、読み込みが正常に完了したことを示す確認が表示されます。

   >[!CAUTION]
   >
   >Workfront インスタンスがWorkfrontとAdobe クラウドストレージの両方にアクセスできる場合、Workfront管理者がWorkfront クラウドストレージをシステムのデフォルトにした場合でも、MS プロジェクトからプロジェクトを読み込むと、従来のAdobe ストレージプロジェクトが作成されます。
   >
   >詳しくは、[ プロジェクトおよび関連オブジェクトのドキュメント管理の概要](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)を参照してください。


1. （オプション）Workfront でプロジェクトの編集を続けます。 プロジェクトの編集の詳細については、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。


   >[!NOTE]
   >
   >テンプレートから作成された新しいプロジェクトのステータスは、**プロジェクト環境設定**&#x200B;領域のWorkfront管理者または&#x200B;**グループプロジェクト環境設定**&#x200B;領域のグループ管理者によって定義されたステータスと一致します。 プロジェクト環境設定について詳しくは、[システム全体のプロジェクト環境設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。
