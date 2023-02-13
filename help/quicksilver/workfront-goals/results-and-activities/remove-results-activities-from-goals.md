---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront目標の目標から結果、アクティビティ、プロジェクトを削除
description: 関連がなくなった場合は、Adobe Workfront目標の目標から結果、アクティビティおよびプロジェクトを削除できます。
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Adobe Workfront目標の目標から結果、アクティビティ、プロジェクトを削除

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

関連性がなくなった場合は、目標から結果、アクティビティ、プロジェクトを削除できます。

目標の作成と、目標の作成、および目標の結果とアクティビティの追加について詳しくは、次の記事を参照してください。

* [Adobe Workfront目標での目標の作成](../../workfront-goals/goal-management/create-goals.md)
* [Adobe Workfront目標での目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [Adobe Workfront目標の目標に結果を追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Adobe Workfront目標で結果とアクティビティを編集](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

目標は、親目標に合わせて、子目標にすることもできます。 子の目標は、親の目標の進捗状況インジケーターでもあります。

目標間の関係を削除することで、目標間の位置合わせを削除できます。 詳しくは、 [Adobe Workfront目標の目標の整合を削除](../goal-alignment/remove-goal-alignment.md).

## アクセス要件

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>
-->

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> <p>詳しくは、 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfrontライセンスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、 Adobe Workfront Goals の追加ライセンスを購入する必要があります。 </p> <p>詳しくは、 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront目標の使用要件</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>目標以降へのアクセスを編集</p> <p><b>メモ</b><p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront目標へのアクセス権の付与</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <div> 
     <p>目標に対する権限の管理</p> 
     <p>目標の共有について詳しくは、 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront目標での目標の共有</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 前提条件

を起動する前に、次の条件を満たす必要があります。

* メインメニューの目標領域を含むレイアウトテンプレート。
* 結果、アクティビティまたはプロジェクトを含む目標。

## 結果、アクティビティ、および目標からのプロジェクトの切断を削除する際の考慮事項

* 結果とアクティビティは、アクティブな目標からのみ削除できます。
* 結果とアクティビティを削除して、目標から削除できます。 削除した結果とアクティビティは復元できません。
* 目標から結果またはアクティビティを削除すると、削除された結果またはアクティビティの進行状況が、目標の全体的な進行状況に影響します。
* プロジェクトを目標から削除することはできませんが、目標からプロジェクトを切断することはできます。 プロジェクトを目標から切り離すと、プロジェクトの完了率が目標の進行状況に影響を与えなくなります。

   プロジェクトが目標の進行状況に与える影響について詳しくは、 [Adobe Workfront目標の目標へのプロジェクトの追加](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* 目標に対する最後の進捗状況インジケーターである場合は、目標から結果やアクティビティを削除したり、子目標やプロジェクトを切断することはできません。
* プロジェクトが「プロジェクト」領域から削除され、目標の最後の進捗状況インジケーターである場合、目標は「非アクティブ」になります。

## 目標からの結果とアクティビティの削除

結果とアクティビティを削除して、目標から削除します。 目標からの結果とアクティビティの削除は同じです。

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) 右上隅で、「 **目標**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   「Workfront目標」領域が開き、デフォルトで「目標リスト」が表示されます。

1. 結果およびアクティビティを削除する目標の名前をクリックします。

   これにより、目標ページが開きます。

1. クリック **進行状況指標** をクリックします。

1. 結果またはアクティビティを選択し、 **削除** アイコン ![](assets/delete-icon.png) をクリックします。

1. クリック **削除** 削除を確定します。 結果またはアクティビティは削除され、復元できません。 目標の完了率が更新され、削除されたアクティビティまたは結果が除外されます。


## 目標からプロジェクトを削除

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. 次をクリック： **メインメニュー** アイコンをクリックし、 **目標**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   「Workfront目標」領域が開き、デフォルトで「目標リスト」が表示されます。

1. 結果およびアクティビティを削除する目標の名前をクリックします。

   これにより、目標ページが開きます。
1. クリック **進行状況指標** をクリックします。
1. プロジェクトを選択し、 **切断** アイコン ![](assets/disconnect-icon.png) をクリックします。
1. クリック **切断** をクリックして確定します。

   プロジェクトは目標に接続されていません。 目標の完了率が更新され、切断されたプロジェクトが除外されます。

