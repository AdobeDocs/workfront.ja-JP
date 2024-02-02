---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Adobe Workfront Goals での目標の削除と非アクティブ化
description: 目標に取り組み始めた後で、組織との関連性がなくなった場合は、目標を削除するのではなく、非アクティブ化することをお勧めします。目標を非アクティブ化すると、履歴情報が保持され、後で再度アクティブ化することができます。ただし、目標リストを正確に保つために、目標を削除することがよいことももあります。
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: ht
source-wordcount: '652'
ht-degree: 100%

---

# Adobe Workfront Goals での目標の削除と非アクティブ化

目標に取り組み始めた後で、組織との関連性がなくなった場合は、目標を削除するのではなく、非アクティブ化することをお勧めします。目標を非アクティブ化すると、履歴情報が保持され、後で再度アクティブ化することができます。ただし、目標リストを正確に保つために、目標を削除することがよいことももあります。

## アクセス要件

<!--drafted for P&P release: 

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
   <td> <p>Goals 以上への編集アクセス権</p> <p><b>メモ</b>

<p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がユーザーのアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
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

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 前提条件

開始するには、まず以下が必要です。

* メインメニューの Workfront Goals 領域を含んだレイアウトテンプレート。

## 目標の非アクティブ化

関連性がなくなり、将来的に再度アクティブ化する可能性がある目標を非アクティブ化できます。

* [目標を非アクティブ化する場合の考慮事項](#considerations-when-deactivating-goals)
* [目標の非アクティブ化](#deactivate-goals)

### 目標を非アクティブ化する場合の考慮事項

目標を非アクティブ化するときは、次の点に注意してください。

* アクティブステータスの目標のみを非アクティブ化できます。目標のアクティブ化については、[Adobe Workfront Goals での目標のアクティブ化](../../workfront-goals/goal-management/activate-goals.md)を参照してください。

  >[!TIP]
  >
  >ドラフトステータスの目標を非アクティブ化することはできません。

* Workfront は、非アクティブ化された目標の進捗状況の計算を停止します。
* 非アクティブな目標は、ワークフロント目標のグラフセクションに表示されなくなり、考慮されなくなります。Workfront Goals グラフについて詳しくは、[グラフを確認して Adobe Workfront Goals の目標進捗の傾向を理解する](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md)を参照してください。

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* 非アクティブ化された目標を更新することはできなくなります。
* 目標とその連携に関する情報を編集できます。
* 以前に非アクティブ化した目標を再度アクティブ化できます。

### 目標の非アクティブ化

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![](assets/more-icon.png), then click **Deactivate**.

   ![](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. 右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**目標**」をクリックします。

   目標リストが表示されます。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. （オプション）フィルターを変更して、アクティブな目標のみを表示します。

   Workfront Goals での情報のフィルタリングについて詳しくは、[Adobe Workfront Goals での情報のフィルタリング](../goal-management/filter-information-wf-goals.md)を参照してください。

1. アクティブな目標をクリックします。

   目標ページが開きます。

   ![](assets/goal-page-unshimmed.png)

1. 目標名の右側にある&#x200B;**その他**&#x200B;メニュー![](assets/more-icon.png)をクリックし、**非アクティブ化**&#x200B;を選択します。

1. 目標が非アクティブ化され、そのステータスは非アクティブになります。

## 目標の削除

関連性がなくなった目標や、今後も関連性がないであろう目標は削除できます。

* [目標を削除する場合の考慮事項](#considerations-when-deleting-goals)
* [目標の削除](#delete-goals)

### 目標を削除する場合の考慮事項 {#considerations-when-deleting-goals}

* クローズした目標も含め、どのステータスの目標も削除できます。
* 削除した目標は復元できません。
* 目標に関連付けられた結果と手動の進行状況バーのアクティビティも削除されます。
* 目標に関連付けられたプロジェクトは削除されませんが、目標との関連付けは削除されます。

### 目標の削除

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![](assets/more-icon.png), then click **Delete**.

   ![](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. 右上隅にあるメインメニューアイコン ![](assets/main-menu-icon.png) をクリックし、**目標**&#x200B;をクリックします。

   目標リストが表示されます。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 目標の名前をクリックします。目標ページが開きます。
1. 目標名の右側にある&#x200B;**その他**&#x200B;メニュー![](assets/more-icon.png)をクリックし、**目標を削除**&#x200B;し、次に&#x200B;**削除**&#x200B;をクリックします。

   目標とそのアクティビティおよび結果も削除され、復元することはできません。目標または子目標に関連付けられたプロジェクトは削除されません。


