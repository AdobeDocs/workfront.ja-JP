---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals で発生している目標の確認
description: 進捗が「トラブル発生中」と表示された目標は達成されない危険性があり、Adobe Workfront Goalsでは赤い進行状況バーで表示されます。目標を頻繁に確認し、進行が遅れている理由を理解する必要があります。
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: ht
source-wordcount: '794'
ht-degree: 100%

---

# Adobe Workfront Goals でイシューがある目標を確認

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

進捗が「トラブル発生中」と表示された目標は達成されない危険性があり、Adobe Workfront Goals では赤い進捗バーで表示されます。目標を頻繁に確認し、進行が遅れている理由を理解する必要があります。目標の進行状況について詳しくは、[Adobe Workfront Goals の目標の進行状況と条件の概要](../../workfront-goals/goal-management/calculate-goal-progress.md)を参照してください。

## アクセス要件

<!--drafted for P&P release: replace the existing requirements with this:

You must have the following: 

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
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>Goals 以上への編集アクセス権</p> <p><b>メモ</b><p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がユーザーのアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront Goals へのアクセス権の付与</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <div> 
     <p>目標に対する権限の管理</p> 
     <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;自分のプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

開始するには、まず以下が必要です。

* メインメニューの目標エリアを含むレイアウトテンプレート。

## 目標が「トラブル発生中」の進行状況に至ることを防ぐための推奨事項

目標が、「トラブル発生中」の進行状況に至る前に、頻繁にモニタリングして、「危険あり」の進行状況になったときに、その進行状況を調整することができます。「危険あり」の目標は「トラブル発生中」の進行状況に至る恐れがあります。目標の進行状況について詳しくは、[Adobe Workfront Goals の目標の進行状況と条件の概要](../../workfront-goals/goal-management/calculate-goal-progress.md)を参照してください。

目標が「トラブル発生中」の進行状況に至る前に、次のことをお勧めします。

* 多くの場合、自分の目標の進行状況によって影響を受ける可能性のある、自分に割り当てられた「危険あり」の状況の目標とチーム、グループ、または組織に割り当てられた組織目標も確認します。「リスクあり」の目標は「トラブル発生中」の目標になる恐れがあります。「リスクあり」の目標は、黄色の進行状況バーで表示されます。目標リストを使用して、自分、チーム、グループまたは組織に属する目標を表示します。


## 目標リストで「トラブル発生中」の目標を確認

目標は、Workfront Goals のどのセクションでも確認できます。Workfront Goals のセクションについて詳しくは、[Adobe Workfront Goals セクションの概要](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)を参照してください。

この記事では、目標リストで目標を確認する方法について説明します。

1. 右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)／**目標**&#x200B;をクリックします。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Workfront Goal エリアが開き、デフォルトで「目標リスト」セクションが表示されます。

1. （推奨）目標リストのエリアで、以下のフィルターを調整して、「リスクあり」の目標を確認します。

   * **会社情報**／**マイチーム**／**マイグループ**／**個人**&#x200B;の順にクリックすると、組織、チーム、グループおよび自分の目標の順に表示されます。

     >[!TIP]
     >
     >Adobe Workfront Goals では、会社情報フィルターに、組織が所有者として選択されている目標が表示されます。
     >
     >
     >このフィールドを使用して会社を検索することはできません。デフォルトでは、Workfront インスタンスの所有者である組織のみが選択されます。

   * 上記で選択した各組織の単位で、**新しいフィルター**／**進捗**／**トラブル発生中**／**適用**&#x200B;の順でクリックします。
   * （オプション）目標を表示する期間を選択します。

     目標リスト内の各目標について、進行状況バーのインジケーターが赤で表示されます。

     右側のパネルにある他のすべての条件を使用した目標のフィルタリングに関して詳しくは、[Adobe Workfront Goalsでの情報のフィルター](../../workfront-goals/goal-management/filter-information-wf-goals.md)を参照してください。

1. 進行状況バーのインジケーターの上にポインタを合わせると、実際の進行状況の割合と、今日の期待値が表示されます。

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. （オプション）フィルターを使用して、特定の所有者に属する目標を検索します。

   選択したユーザーのトラブル中の目標が、目標リストに表示されます。

1. 目標名をクリックして目標ページを開き、左側のパネルで&#x200B;**進捗状況インジケーター**&#x200B;をクリックします。どの進行状況インジケーターが目標の遅れを引き起こしているかを表示し、進捗状況インジケーターリストの&#x200B;**実際の進行状況**&#x200B;の列で、インジケーターの進行状況をインラインでアップデートします。

   結果とアクティビティのアップデートについて詳しくは、[Adobe Workfront Goals での目標の進行状況のアップデート](../goal-review-and-workfront-goals-sections/check-in-goals.md)を参照してください。

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >進捗状況インジケーターリストでは、結果とアクティビティのみをアップデートすることができます。子の目標の進捗状況インジケーターをアップデートするには、目標にアクセスし、接続されたプロジェクトのタスクをアップデートして、プロジェクトの進行状況をアップデートする必要があります。


