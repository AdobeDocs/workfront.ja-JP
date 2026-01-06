---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals での問題が発生した目標のレビュー
description: 進捗が「トラブル発生中」と表示された目標は達成されない危険性があり、Adobe Workfront Goalsでは赤い進行状況バーで表示されます。目標を頻繁に確認し、進行が遅れている理由を理解する必要があります。
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 77%

---

# Adobe Workfront Goals で発生している目標の確認

<!--Audited: 4/2025-->

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

進捗が「トラブル発生中」と表示された目標は達成されない危険性があり、Adobe Workfront Goals では赤い進捗バーで表示されます。目標を頻繁に確認し、進行が遅れている理由を理解する必要があります。目標の進行状況について詳しくは、[Adobe Workfront Goals の目標の進行状況と条件の概要](../../workfront-goals/goal-management/calculate-goal-progress.md)を参照してください。

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
 <td> <p>Edit access to Goals</p></td>
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

## 問題が発生しているの進行に達するための目標を回避するための推奨事項

目標が「問題あり」の進捗に達する前に、頻繁に目標を監視し、「危険」の進捗に達したときに進捗を調整できます。 リスクのある目標は、トラブルに巻き込まれる危険があります。 目標の進捗の詳細については、[Adobe Workfront Goals における目標の進捗と条件の概要 &#x200B;](../../workfront-goals/goal-management/calculate-goal-progress.md) を参照してください。

目標が「トラブル発生中」の進行状況に至る前に、次のことをお勧めします。

* 多くの場合、自分の目標の進行状況によって影響を受ける可能性のある、自分に割り当てられた「危険あり」の状況の目標とチーム、グループ、または組織に割り当てられた組織目標も確認します。「リスクあり」の目標は「トラブル発生中」の目標になる恐れがあります。「リスクあり」の目標は、黄色の進行状況バーで表示されます。目標リストを使用して、自分、チーム、グループまたは組織に属する目標を表示します。


## 目標リストで「トラブル発生中」の目標を確認

Workfront Goals の任意のセクションで目標をレビューできます。 Workfront Goals の節について詳しくは、[Adobe Workfront Goals の節の概要 &#x200B;](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md) を参照してください。

この記事では、目標リストで目標を確認する方法について説明します。

{{step1-to-goals}}

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

   ![GOal の進行状況のホバーの詳細 &#x200B;](assets/goal-progress-hover-over-detail-unshimmed.png)

1. （オプション）フィルターを使用して、特定の所有者に属する目標を検索します。

   選択したユーザーのトラブル中の目標が、目標リストに表示されます。

1. 目標名をクリックして目標ページを開き、左側のパネルで&#x200B;**進捗状況インジケーター**&#x200B;をクリックします。どの進行状況インジケーターが目標の遅れを引き起こしているかを表示し、進捗状況インジケーターリストの&#x200B;**実際の進行状況**&#x200B;の列で、インジケーターの進行状況をインラインでアップデートします。

   結果とアクティビティのアップデートについて詳しくは、[Adobe Workfront Goals での目標の進行状況のアップデート](../goal-review-and-workfront-goals-sections/check-in-goals.md)を参照してください。

   ![&#x200B; 実際の進捗状況 &#x200B;](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >進捗状況インジケーターリストでは、結果とアクティビティのみをアップデートすることができます。子の目標の進捗状況インジケーターをアップデートするには、目標にアクセスし、接続されたプロジェクトのタスクをアップデートして、プロジェクトの進行状況をアップデートする必要があります。


