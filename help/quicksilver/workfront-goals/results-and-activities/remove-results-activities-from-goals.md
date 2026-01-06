---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront Goals の目標からの進行状況インジケーターの削除
description: 関連性がなくなった場合は、Adobe Workfront Goals の目標から結果、アクティビティおよびプロジェクトを削除できます。
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 83%

---

# Adobe Workfront Goals の目標からの進行状況インジケーターの削除

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

関連性がなくなった場合は、目標から結果、アクティビティおよびプロジェクトを削除できます。

目標の作成と目標への結果とアクティビティの追加について詳しくは、次の記事を参照してください。

* [Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)
* [Adobe Workfront Goals で目標にアクティビティを追加する方法](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Adobe Workfront Goals の目標への結果の追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Adobe Workfront Goals での結果とアクティビティの編集](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

目標は、親目標に合わせて、子目標にすることもできます。子の目標は、親の目標の進捗状況インジケーターでもあります。

目標間の接続を削除することにより、目標間の整合性を削除することができます。詳しくは、[Adobe Workfront Goals での目標の整合性を削除](../goal-alignment/remove-goal-alignment.md)を参照してください。

## アクセス要件

>[!NOTE]
>
>過去にこのパッケージを購入したことがある会社は、Adobe Workfront Goals を引き続き使用する場合があります。 詳細については、アカウント担当者にお問い合わせください。
>
>Adobe Workfront Goals は購入できなくなりました。

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront パッケージ</p> </td> 
   <td> 
   <p>Adobe WorkfrontUltimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront プラン</td>
 <td>
 <p>投稿者以上</p>
<p>リクエスト以上</p></td>
 </tr>
  <tr>
 <td role="rowheader">アクセスレベル設定</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">オブジェクト権限</td>
 <td>
  <div>
  <p>目標の表示には表示権限以上が必要</p>
  <p>目標に対する編集権限を管理</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>システム管理者を含むすべてのユーザーには、メインメニューの目標エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## 前提条件

結果、アクティビティまたはプロジェクトに目標を関連付ける必要があります。

## 結果、アクティビティ、および目標からのプロジェクトの接続を削除する際の考慮事項

* 結果とアクティビティは、アクティブな目標からのみ削除できます。
* 目標から結果とアクティビティを削除すると、それらを削除できます。削除した結果とアクティビティは復元できません。
* 目標から結果またはアクティビティを削除すると、削除された結果またはアクティビティの進捗状況が目標の全体的な進捗状況に影響します。
* プロジェクトを目標から削除することはできませんが、目標からプロジェクトを接続解除することはできます。プロジェクトを目標から接続解除すると、プロジェクトの完了率が目標の進捗状況に影響を与えなくなります。

  プロジェクトが目標の進捗状況に与える影響について詳しくは、[Adobe Workfront Goals でプロジェクトを目標に追加する方法](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)を参照してください。

* それらが目標に対する最後の進捗状況インジケーターである場合は、目標から結果やアクティビティを削除したり、子目標やプロジェクトを接続解除することはできません。
* プロジェクトがプロジェクトエリアから削除され、目標の最後の進捗状況インジケーターである場合、目標は非アクティブになります。

## 目標からの結果とアクティビティの削除

目標から結果とアクティビティを削除すると、それらを削除できます。目標からの結果とアクティビティの削除は同じです。

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![Delete result](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

{{step1-to-goals}}

これにより、Workfront 目標エリアが開き、デフォルトで目標リストが表示されます。

1. 結果とアクティビティを削除する目標の名前をクリックします。

   目標ページが開きます。

1. 左パネルの「**進行状況インジケーター**」をクリックします。

1. 結果またはアクティビティを選択し、リスト上部の **削除** アイコン ![&#x200B; 削除アイコン &#x200B;](assets/delete-icon.png) をクリックします。

1. 「**削除**」をクリックして削除を確定します。結果またはアクティビティは削除され、復元できません。目標の完了率が更新され、削除されたアクティビティまたは結果が除外されます。


## 目標からプロジェクトを削除

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![Disconnect](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


{{step1-to-goals}}

これにより、Workfront 目標エリアが開き、デフォルトで目標リストが表示されます。

1. 結果とアクティビティを削除する目標の名前をクリックします。

   目標ページが開きます。
1. 左パネルの「**進行状況インジケーター**」をクリックします。
1. プロジェクトを選択し、リストの上部にある **切断** アイコン ![&#x200B; 切断アイコン &#x200B;](assets/disconnect-icon.png) をクリックします。
1. 「**連携解除**」をクリックして確定します。

   プロジェクトは目標に接続されていません。目標の完了率が更新され、連携解除されたプロジェクトが除外されます。

