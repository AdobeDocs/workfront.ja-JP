---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Adobe Workfront Goals での目標の進捗の更新
description: 目標を定期的に確認し、進捗を更新して、目標が遅れていないか、達成されない危険が生じていないかを確認する必要があります。
author: Alina
feature: Workfront Goals
exl-id: 5092f508-e52c-4934-a8c1-d0be04ecce13
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 89%

---

# Adobe Workfront Goals での目標の進捗の更新

目標を定期的に確認し、進捗を更新して、目標が遅れていないか、達成されない危険が生じていないかを確認する必要があります。

<!--And: take this last sentence ^^ out when you update this for goal redesign production.-->

## アクセス要件

以下が必要です。

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
   <p>新しいプランとライセンス構造の場合：
  <ul><li>究極の計画 </li></ul>
   </p>
<p>現在のプランおよびライセンス構造の場合： 
<ul><li> プロまたはそれ以上 </li>
  <li>Workfront ライセンスに加えて、Adobe Workfront Goals ライセンス。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront プラン*</td>
 <td>
 <p>新規ライセンス：コントリビューター以上</p>
 または
 <p>現在のライセンス：リクエスト以上</p> <p>詳しくは、<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront ライセンスの概要</a>を参照してください。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">製品*</td>
 <td>
 <p> 新製品の要件は、次のいずれかです。 </p>
<ul>
<li>Select または Prime Adobe Workfront プランと、追加のAdobe Workfront Goals ライセンス。</li>
<li>Workfront Goals をデフォルトで含む究極のWorkfront プラン。 </li></ul>
 <p>または</p>
 <p>現在の必要な製品：Workfront プランとAdobe Workfront Goals の追加ライセンス。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">アクセスレベル</td>
 <td> <p>Goals への編集アクセス権</p></td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">オブジェクト権限</td>
 <td>
  <div>
  <p>目標の表示には表示権限以上が必要</p>
  <p>目標に対する編集権限を管理</p>
  <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者を含むすべてのユーザーには、メインメニューに「目標」エリアが含まれるレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 前提条件

開始するには、アクティブな目標が必要です。

ドラフト、非アクティブ、またはクローズ済みの目標に関する進捗を更新することはできません。

## 目標を更新する際の考慮事項

目標の進捗状況を更新する際は、以下の点を考慮してください。

* Workfront Goals の進行状況インジケーターの進行状況を更新すると、目標の進行状況が自動的に計算されます。

  >[!TIP]
  >
  >目標に関する進捗を直接更新することはできません。目標の進捗状況インジケーター（アクティビティ、結果、接続されたプロジェクト）の進捗状況を更新し、目標の進捗状況を更新する必要があります。プロジェクトの進捗状況を更新するには、プロジェクトのタスクを更新する必要があります。

  次の記事も参照してください。

   * 目標へのアクティビティの追加について詳しくは、[Adobe Workfront Goals の目標にアクティビティを追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)を参照してください。
   * 目標への結果の追加について詳しくは、[Adobe Workfront Goals の目標に結果を追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)を参照してください。
   * Workfront Goals での進捗ステータスの決定方法について詳しくは、[Adobe Workfront Goals の目標進捗と状況の概要](../../workfront-goals/goal-management/calculate-goal-progress.md)を参照してください。

* 進行状況を更新する前に、目標を作成してアクティベートする必要があります。

  次の記事も参照してください。

   * 目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。
   * 目標のアクティブ化については、[Adobe Workfront Goals での目標のアクティブ化](../../workfront-goals/goal-management/activate-goals.md)を参照してください。

  >[!IMPORTANT]
  >
  >ドラフト、クローズ、非アクティブになっている目標の進捗状況を更新することはできません。

* 目標に関する結果やアクティビティの進行状況を初めて更新する場合、目標の「進歩状況」が「新規」から変わり、Workfront Goals が進行状況と目標の進行状況の更新を記録し始めます。

<!--

## Update goal progress by using Check-in in the Production environment

>[!IMPORTANT]
>
> <span class="preview"> The Check-in functionality has been removed from the Preview environment and will be removed from Workfront Goals with the 23.1 release. See the [Update goal progress in the Preview environment](#update-goal-progress-in-the-preview-environment) section in this article to update goal progress in Preview. </span>


You can check in on goals at the individual goal level, or you can check in on multiple goals from the Check-in section of Workfront Goals.

* [Update individual goals](#update-individual-goals) 
* [Update goals in the Check-in section](#update-goals-in-the-check-in-section)

### Update individual goals {#update-individual-goals}

When you check in on a goal at the goal level, you can update the progress of the results and activities that are assigned to you or other users.

For information about how to update additional information about results and activities, see [Edit results and activities in Adobe Workfront Goals](../../workfront-goals/results-and-activities/edit-results-and-activities.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area.

   All goals display by default. 

1. (Optional) Click any of the following sections in the left panel to access a list of goals:

   * Goal Alignment 
   * Pulse 
   * Check-in

   Or

   From the Goal List, click the name of a goal to open the **Goal Details** panel on the right.

   >[!TIP]
   >
   >You must have Edit access to Goals in your Access Level to view the Check-in section or the Check in button.

1. Click **Check in**.

   ![](assets/check-in-link-inside-goal-details-highlighted-350x156.png)

   The progress of results and activities becomes editable.

1. Update the current progress on each of the results. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

1. Update the percent complete on the Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

1. Click **Back to Summary** to return to the Goal Details panel.

   Your goal progress updates as you update the results and activities of your goal. 

1. Click the **X icon** in the upper-right corner of the Goal Details panel to close it.

### Update goals in the Check-in section {#update-goals-in-the-check-in-section}

You can use the Check-in section to check in on goals when you want to quickly provide updates for several goals at the same time.

>[!TIP]
>
>You can access the Check-in section from any of the following sections:
>
>* Goal List 
>* Goal Alignment 
>* Pulse 
>

When you check in on a goal in the Check-in section, you can update the progress of the results and activities that are assigned only to you. You cannot update the progress of results and activities that are assigned to other users in this section.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List section displays by default. 

1. Click Check-in in the left panel.

   Or

   (Conditional) If you are in the Goal List, Goal Alignment, or Pulse sections, click the **Check in** button in the upper-right of the screen. This opens the Check-in section.

   ![](assets/check-in-button-highlighted-350x102.png)

   Goals display in a list and results and activities are listed under each goal.

   ![](assets/check-in-page-with-show-all-aligned-goals-link-350x178.png)

1. (Optional) Click **Show all results**, **Show all activities**, or **Show all aligned goals** to the far right of the goal name to display all results, activities, and aligned goals of a goal whose progress you want to update.

   >[!CAUTION]
   >
   >You cannot directly update aligned goals, but you can update their results and activities.

1. Update the current progress on each of the results assigned to you. Depending on what type of result you selected, you can do one of the following:

   * Update the quantity 
   * Update the currency amount
   * Update the percent complete

   The result and the goal progress updated automatically and you receive a confirmation of your changes.

1. Update the percent complete on your Manual progress bar activity.

   >[!TIP]
   >
   >When you add projects as activities to your goals, you cannot manually update projects at the goal level. Workfront automatically updates project progress based on the project of their tasks. When the project percent complete updates in Workfront, the goal progress associated with the project also updates automatically.

   The activity and the goal progress updated automatically and you receive a confirmation of your changes.

1. (Optional) Add a comment for your goal, then click **Post** to save your comment.

-->

目標の進行状況を更新する手順は、次のとおりです。

1. 右上隅の&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)／**目標**&#x200B;をクリックします。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   これにより、目標リストが開きます。デフォルトでは、表示するアクセス権を持つすべての目標が表示されます。

   または、左パネルの「目標の整合性」をクリックすることもできます。

1. 目標リストで目標の名前をクリックし、目標ページを開きます。
1. 左パネルの「**進行状況インジケーター**」をクリックします。

   「進行状況インジケーター」リストには、選択した目標に関するすべての進行状況インジケーターが表示されます。

   >[!NOTE]
   >
   >  * 更新できるのは、結果とアクティビティのみです。
   >  * 子の目標の進行状況を表示するには、子の目標の進行状況インジケーターを更新する必要があります。
   >  * プロジェクトの進行状況を表示するには、接続されたプロジェクトのタスクを更新する必要があります。
   >   
   >    次に、子の目標の進行状況とプロジェクトの進行状況が、選択した目標の進行状況を左右します。


1. 結果またはアクティビティの進行状況を更新するには、結果またはアクティビティの&#x200B;**実際の進行状況**&#x200B;列の数値をクリックして、値を入力して更新し、Enter キーを押します。

   ![](assets/actual-progress-result-updating-highlighted-unshimmed.png)

   「進行状況」列の進行状況インジケーターの進行状況バーと、目標ヘッダーの目標の進行状況は直ちに更新されます。

