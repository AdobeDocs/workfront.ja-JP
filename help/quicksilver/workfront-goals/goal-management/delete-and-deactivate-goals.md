---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Adobe Workfront Goals での目標の削除と非アクティブ化
description: 目標に取り組み始めた後で、組織との関連性がなくなった場合は、目標を削除するのではなく、非アクティブ化することをお勧めします。目標を非アクティブ化すると、履歴情報が保持され、後で再度アクティブ化することができます。ただし、目標リストを正確に保つために、目標を削除することがよいことももあります。
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 80%

---

# Adobe Workfront Goals での目標の削除と非アクティブ化

<!--Audited for P&P only: 4/2025-->

目標に取り組み始めた後で、組織との関連性がなくなった場合は、目標を削除するのではなく、非アクティブ化することをお勧めします。目標を非アクティブ化すると、履歴情報が保持され、後で再度アクティブ化することができます。ただし、目標リストを正確に保つために、目標を削除することがよいことももあります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
  <ul><li>Ultimateプラン </li></ul>
   </p>
<p>現在のプランおよびライセンス構造の場合： 
<ul><li> プロまたはそれ以上 </li>
  <li>Workfront ライセンスに加えて、Adobe Workfront Goals ライセンス。</li></ul></p>
   </td>  
  </tr>
 <tr>
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
  <p> 新しい製品要件：Workfront</p>
 <p>または</p>
  <p>現在の製品要件：Workfront ライセンスに加えて、Adobe Workfront Goals のライセンスを購入する必要があります。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">アクセスレベル</td>
 <td> <p>Goals への編集アクセス権</p> </td>
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

+++

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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. 右上隅の **メインメニュー** アイコン ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) をクリックし、**目標** をクリックします。

   目標リストが表示されます。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. （オプション）フィルターを変更して、アクティブな目標のみを表示します。

   Workfront Goals での情報のフィルタリングについて詳しくは、[Adobe Workfront Goals での情報のフィルタリング](../goal-management/filter-information-wf-goals.md)を参照してください。

1. アクティブな目標をクリックします。

   目標ページが開きます。

   ![&#x200B; 目標ページ &#x200B;](assets/goal-page-unshimmed.png)

1. 目標名の右側にある **その他** メニュー ![&#x200B; その他アイコン &#x200B;](assets/more-icon.png) をクリックしてから、「**アクティベートを解除** をクリックします。

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

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. 右上隅の「メインメニュー」アイコン ![&#x200B; 「メインメニュー」アイコン &#x200B;](assets/main-menu-icon.png) をクリックし、「**目標**」をクリックします。

   目標リストが表示されます。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 目標の名前をクリックします。目標ページが開きます。
1. 目標名の右側にある **その他** メニュー ![&#x200B; その他アイコン &#x200B;](assets/more-icon.png) をクリックし、**目標を削除** をクリックしてから、**削除** をクリックします。

   目標とそのアクティビティおよび結果も削除され、復元することはできません。目標または子目標に関連付けられたプロジェクトは削除されません。


