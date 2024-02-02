---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Adobe Workfront Goals の目標リストでの目標の管理
description: 自分または他のユーザーが目標を作成した後、その進行状況と情報を目標リストでレビューできます。目標の作成について詳しくは、「Adobe Workfront Goals での目標の作成」を参照してください。
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: ht
source-wordcount: '779'
ht-degree: 100%

---

# Adobe Workfront Goals の目標リストでの目標の管理

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

自分または他のユーザーが目標を作成した後、その進行状況と情報を目標リストでレビューできます。目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。

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

この記事で説明する操作を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p> <p>詳しくは、<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront ライセンスの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、Adobe Workfront Goals の追加ライセンスを購入する必要があります。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>目標に対する表示以上のアクセス権</p> <p><b>メモ</b><p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がユーザーのアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront Goals へのアクセス権の付与</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <div> 
     <p>目標の表示以上の権限</p> 
     <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 前提条件

開始するには、まず以下が必要です。

* メインメニューの目標エリアを含むレイアウトテンプレート。

## 目標リストでの目標の管理

目標の表示と管理は、Workfront Goals の以下のセクションで行えます。

* 目標リスト
* 目標の整合性

各セクションには、目標が少し異なる形式で表示されます。どのセクションを使用するかは、目標を扱う際に達成する目的によって異なります。

詳しくは、[Adobe Workfront Goals のセクションの概要](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)を参照してください。

この記事では、目標リストで目標を確認する方法について説明します。

目標リストをレビューする際は、次の点を考慮します。

* 自分または組織内の他のユーザーが作成した目標を目標リストに表示できます。目標を編集できるようにするには、目標の管理権限が必要です。

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

目標リストで目標を管理するには、次の手順に従います。

1. **メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**目標**」をクリックします。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   デフォルトでは「目標リスト」セクションが表示されます。デフォルトでは、目標のステータス、期間または所有者に関係なく、目標を表示できます。

   目標のリストには、各目標についての情報を含んだ次のフィールドが含まれています。

   * **名前**：目標の名前。
   * **所有者**：目標の所有者の名前。
   * **期間**：目標がスケジュールされている期間。
   * **ステータス**：目標のステータスは、次のいずれかになります。
      * アクティブ
      * ドラフト
      * 非アクティブ
      * クローズ

     目標ステータスについて詳しくは、[Adobe Workfront Goals の目標ステータスの概要](../goal-management/goal-status-overview.md)を参照してください。

     他の目標に整合された目標には、「整合性」アイコンが表示されます。目標の整合について詳しくは、[Adobe Workfront Goals で目標をに結び付けて整合させる](../goal-alignment/align-goals-by-connecting-them.md)を参照してください。

   * **条件**：目標が完了するまでに割り当てられた期間内の目標の進行状況を視覚的に表します。

     目標の条件は、次のいずれかになります。

      * 新規
      * 目標どおり
      * リスクあり
      * トラブル発生中

     目標の条件について詳しくは、[Adobe Workfront Goals の目標の進行状況と条件の概要](../goal-management/calculate-goal-progress.md)を参照してください。

   * **進行状況**：割合（％）の値による目標の進捗状況インジケーター。進行状況インジケーターの色は、目標の条件の色と一致します。

     詳しくは、[目標の進捗状況を Adobe Workfront Goals で計算](../goal-management/calculate-goal-progress.md)を参照してください。

1. 目標リストの右上隅にあるフィルターアイコン ![](assets/filter-icon.png) をクリックし、フィルターを適用して、重要な目標のみを表示します。

   Workfront Goals でのフィルターの使用について詳しくは、[Adobe Workfront Goals での情報のフィルター](../goal-management/filter-information-wf-goals.md)を参照してください。

1. 列ヘッダーのフィールドのいずれかをクリックして、そのフィールドでリストを並べ替えます。
リストの並べ替えに使用するフィールドの右側に矢印が表示されます。

1. （オプション）同じ列を降順で並べ替えるには、列のフィールドを再度クリックします。
1. 目標の名前をクリックして、目標のページを開きます。
1. リストから 1 つの目標を選択し、リストの上部にある次のオプションの 1 つをクリックします。
   * **編集**&#x200B;アイコン ![](assets/edit-icon.png) で、目標に関する情報を編集します。詳しくは、[Adobe Workfront Goals の目標を編集](../goal-management/edit-goals.md)を参照してください。
   * 他の人と目標を共有する「**共有**」アイコン ![](assets/share-icon.png) 詳しくは、[Adobe Workfront Goals の目標を共有](../workfront-goals-settings/share-a-goal.md)を参照してください。
   * 「**整合性を開く**」アイコン ![](assets/align-icon-unshimmed.png) で、目標の整合性エリアを開きます。このオプションは、選択した目標が別の目標に一致している場合にのみ表示されます。
   * 目標を削除する&#x200B;**削除**&#x200B;アイコン ![](assets/delete-icon.png) で、「**削除**」をクリックして確定します。詳しくは、[Adobe Workfront Goals の目標を削除および非アクティブ化](../goal-management/delete-and-deactivate-goals.md)を参照してください。





