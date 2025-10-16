---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Adobe Workfront Goals の目標リストでの目標の管理
description: 自分または他のユーザーが目標を作成した後、その進行状況と情報を目標リストでレビューできます。目標の作成について詳しくは、「Adobe Workfront Goals での目標の作成」を参照してください。
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 76%

---

# Adobe Workfront Goals の目標リストでの目標の管理

<!--Audited for P&P only: 10/2025-->

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

自分または他のユーザーが目標を作成した後、その進行状況と情報を目標リストでレビューできます。目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。

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
    <p> New product requirement: Workfront</p>
    Or
    <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p>  </td>
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

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

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

   ![Goal list with goal expanded](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![Right-pointing arrow](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

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

1. Click the **Alignment icon** ![Alignment icon](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

目標リストで目標を管理するには、次の手順に従います。

1. 右上隅の **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**目標** をクリックします。

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

1. 目標リストの右上隅にあるフィルターアイコン ![ フィルターアイコン ](assets/filter-icon.png) をクリックし、フィルターを適用して、重要な目標のみを表示します。

   Workfront Goals でのフィルターの使用について詳しくは、[Adobe Workfront Goals での情報のフィルター](../goal-management/filter-information-wf-goals.md)を参照してください。

1. 列ヘッダーのフィールドのいずれかをクリックして、そのフィールドでリストを並べ替えます。
リストの並べ替えに使用するフィールドの右側に矢印が表示されます。

1. （オプション）同じ列を降順で並べ替えるには、列のフィールドを再度クリックします。
1. 目標の名前をクリックして、目標のページを開きます。
1. リストから 1 つの目標を選択し、リストの上部にある次のオプションの 1 つをクリックします。
   * **編集** アイコン ![ 編集アイコン ](assets/edit-icon.png) 目標に関する情報を編集できます。 詳しくは、[Adobe Workfront Goals の目標を編集](../goal-management/edit-goals.md)を参照してください。
   * **共有** アイコン ![ 共有アイコン ](assets/share-icon.png) を使用して、他のユーザーと目標を共有します。 詳しくは、[Adobe Workfront Goals の目標を共有](../workfront-goals-settings/share-a-goal.md)を参照してください。
   * **関連付けを開く** アイコン ![ 関連付けを開くアイコン ](assets/align-icon-unshimmed.png) 目標の関連付け領域を開く このオプションは、選択した目標が別の目標に一致している場合にのみ表示されます。
   * 目標を削除するには **削除** アイコン ![ 削除アイコン ](assets/delete-icon.png) をクリックし、確認するには **削除** をクリックします。  詳しくは、[Adobe Workfront Goals の目標を削除および非アクティブ化](../goal-management/delete-and-deactivate-goals.md)を参照してください。





