---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートの作成
description: テンプレートエリアからテンプレートを作成および削除できます。新しいテンプレートを作成するときは、すべてのタスクと、将来のプロジェクト設定についての情報を入力できます。この情報は、テンプレートから作成するプロジェクトに転送されます。
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 94%

---

# プロジェクトテンプレートの作成

<!-- Audited: 1/2024 -->

テンプレートエリアからテンプレートを作成および削除できます。新しいテンプレートを作成するときは、すべてのタスクと、将来のプロジェクト設定についての情報を入力できます。この情報は、テンプレートから作成するプロジェクトに転送されます。

>[!NOTE]
>
>テンプレートとそのタスクには実際の日付はありませんが、タスクが開始される可能性がある日（将来のプロジェクトが開始される可能性がある日）と、タスクを完了する必要がある可能性の日を示します。テンプレートを使用して将来のプロジェクトを作成する場合、プロジェクトは実際の日付を受け取ります。詳しくは、[プロジェクトの作成](../create-projects/create-project.md)を参照してください。


次の方法で新しいテンプレートを作成できます。

* 最初から（この記事で説明）。
* 既存のプロジェクトから、プロジェクトをテンプレートとして保存。

  既存のプロジェクトからテンプレートを作成する方法について詳しくは、[プロジェクトをテンプレートとして保存](../../../manage-work/projects/manage-projects/save-project-as-template.md)を参照してください。

* 別のテンプレートからコピー。

  既存のテンプレートのコピーについて詳しくは、[プロジェクトテンプレートをコピー](../../../manage-work/projects/create-and-manage-templates/copy-template.md)を参照してください。

* ブループリントを読み込む。ブループリントを読み込むには、Workfront の管理者である必要があります。詳しくは、[ブループリントの設定](../../../administration-and-setup/blueprints/configure-template-package.md)を参照してください。

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
   <td> <p>標準 </p><p>プラン</p> <p>ブループリントからテンプレートを読み込むには、システム管理者である必要があります</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>テンプレートへの編集アクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>デフォルトでは、作成したテンプレートに対する管理権限があります。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
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
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## テンプレートの作成

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) をクリックするか、（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックし、**テンプレート**&#x200B;をクリックします。

1. 「**新規テンプレート**」をクリックします。

   テンプレートは名称未設定です。

   ![新規テンプレート](assets/create-template-nwe-2022-350x102.png)

1. テンプレートヘッダーで新しいテンプレートの名前を指定し、**Enter** キーを押します。
1. 左側のパネルで「**テンプレートタスク**」セクションをクリックします。
1. 「**テンプレートタスクの追加を開始**」をクリックします。

   または

   「**新規テンプレートタスク**」をクリックして、テンプレートへのタスク追加を開始します。

   テンプレートタスクをテンプレートに追加することは、タスクをプロジェクトに追加することと同じです。

   プロジェクトへのタスクの追加の詳細については、[プロジェクトへのタスクの作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)を参照してください。

   >[!NOTE]
   >
   >繰り返しタスクをテンプレートに追加することはできません。

1. （オプション）タスクリストの右上隅にある&#x200B;**ガントチャート**&#x200B;アイコンをクリックすると、テンプレートのタスクリストが視覚的に表示されます。

   >[!TIP]
   >
   >このガントチャートから直接タスクを編集することはできません。

1. 新しいテンプレートに情報を追加するには、**詳細** メニュー ![ 詳細アイコン ](assets/more-icon.png) をクリックしてから、**編集** をクリックします。

   テンプレートの編集について詳しくは、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

1. 「**変更を保存**」をクリックします。
1. （オプション）テンプレートに項目を追加する場合は、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)の記事の[テンプレートに項目を追加](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template)のセクションを参照してください。

## グループの関連性によって決定されるテンプレート設定

プロジェクトテンプレートとグループの関連付け（またはグループの欠如）は、プロジェクト、タスク、イシューの環境設定がテンプレート内の特定の設定をどのように決定するかに影響します。詳しくは、[グループのプロジェクトテンプレートの作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)の記事の[グループのプロジェクトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates)のセクションを参照してください。
