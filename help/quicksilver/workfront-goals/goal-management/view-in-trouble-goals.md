---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals での問題の発生している目標の確認
description: 障害が発生しているオールは、達成されない危険があり、Adobe Workfront目標の赤いプログレスバーで表されます。 目標を頻繁に確認し、進行が遅れている理由を理解する必要があります。
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Adobe Workfront Goals での問題の発生している目標の確認

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

問題の進行を伴う目標は達成されない危険があり、Adobe Workfront目標では赤いプログレスバーで表されます。 目標を頻繁に確認し、進行が遅れている理由を理解する必要があります。 目標の進捗について詳しくは、 [Adobe Workfront目標の目標の達成状況と条件の概要](../../workfront-goals/goal-management/calculate-goal-progress.md).

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

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

を起動する前に、次の条件を満たす必要があります。

* メインメニューの目標領域を含むレイアウトテンプレート。

## Recommendations：トラブルの進行に達する目標を防ぐため

目標が問題の進行に達する前に、頻繁に監視し、リスクが高い状態の進行に達した場合にその進捗を調整することができます。 危険な目標は困難に陥る恐れがある。 目標の進捗について詳しくは、 [Adobe Workfront目標の目標の達成状況と条件の概要](../../workfront-goals/goal-management/calculate-goal-progress.md)

目標が「問題あり」の進行に達する前に、以下をお勧めします。

* 多くの場合、自分に割り当てられる「リスクが高い」条件を持つ目標と、自分のチーム、グループまたは自分の組織に割り当てられ、目標の進捗に影響を受ける可能性のある組織の目標をレビューします。 危険な目標は問題の中の目標になる危険性にある。 危険度の高い目標は、黄色のプログレスバーで示されます。 目標リストを使用して、自分、チーム、グループまたは組織に属する目標を表示します。


## 目標リストで問題のある目標を確認

目標は、Workfront目標の任意のセクションで確認できます。 Workfront目標の節について詳しくは、 [「Adobe Workfront目標」セクションの概要](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

この記事では、目標リストで目標を確認する方法について説明します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) > **目標** をクリックします。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   「 Workfront目標」領域が開き、デフォルトで「目標リスト」セクションが表示されます。

1. （推奨）「目標リスト」領域で以下のフィルターを調整して、リスクの高い目標を確認します。

   * クリック **会社**&#x200B;を、 **マイチーム**&#x200B;を、 **マイグループ**&#x200B;を、 **個人** 目標を設定して、組織、チーム、グループおよび自分の目標に属する目標を表示します。

      >[!TIP]
      >
      >「Adobe Workfront目標」では、「会社」フィルターに、組織が所有者として選択された目標が表示されます。
      >
      >
      >このフィールドを使用して会社を検索することはできません。 デフォルトでは、Workfrontインスタンスの所有者である組織のみが選択されています。

   * 上で選択した各組織単位で、 **新しいフィルター** > **進行状況** > **トラブル状態** >**適用**
   * （オプション）目標を表示する期間を選択します。

      目標リスト内の各目標について、進行状況バーのインジケーターが赤で表示されます。

      右パネルにある他のすべての条件を使用した目標のフィルタリングについて詳しくは、 [Adobe Workfront目標での情報のフィルター](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 進行状況バーのインジケーターの上にマウスポインターを置くと、実際の進行状況の割合と、現在の日の期待値が表示されます。

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. （オプション）フィルターを使用して、特定の所有者に属する目標を検索します。

   選択したユーザーのトラブル内目標が目標リストに表示されます。

1. 目標名をクリックして目標ページを開き、「 **進行状況インジケーター** をクリックします。 目標を達成する前に目標を表示し、指標の進行状況を **実際の進捗状況** 「進行状況指標」リストの列

   結果とアクティビティの更新について詳しくは、 [Adobe Workfront目標での目標の進捗状況の更新](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >進行状況インジケーターリストでは、結果とアクティビティのみを更新できます。 子の目標の進捗状況インジケーターを更新するには、目標にアクセスし、接続されたプロジェクトのタスクを更新して、プロジェクトの進捗状況を更新する必要があります。


