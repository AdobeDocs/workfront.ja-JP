---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals での目標へのアクセスとオープン
description: この記事では、Adobe Workfront で目標を検索し、管理する方法について説明します。
author: Alina
feature: Workfront Goals
exl-id: a729f334-6ca4-4cf5-a3ef-01a7effb7153
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 77%

---

# Adobe Workfront Goals で目標にアクセスして開く

<!--Audited P&P only: 4/2025-->

この記事では、Adobe Workfront で戦略目標を検索し、管理する方法について説明します。


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

## Workfront Goals へのアクセス

1. 右上隅の **メインメニュー** アイコン ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) をクリックし、**目標** をクリックします。

   <!-- drafted for Shell release: Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   目標リストが表示されます。


   >[!IMPORTANT]
   >
   >   Workfront Goals に正しくアクセスできたら、デフォルトでは、目標リストに自分または他のユーザーが作成した目標を表示できます。

   <!--   
   (NOTE: This might change when sharing is in place; right now, with sharing in place, they can VIEW all goals in the system but they cannot EDIT the ones others created!)
   -->

1. （オプション）目標の名前をクリックして、目標を開いたり編集したりします。

   または

   「**新規目標**」をクリックして、新しい目標を追加します。

   目標の作成について詳しくは、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。

## 個々の目標を開いて管理

目標を管理するには、個々の目標にアクセスして次の操作を実行する必要があります。

* 編集
* 結果またはアクティビティを追加
* 結果および関連付けられたアクティビティを編集
* アクティブ化
* 非アクティブ化
* 削除
* 別の目標と整合性をとる
* 結果またはアクティビティを他の目標に変換
* 更新
<!--
Accessing goals differs depending on what environment you use.

To access an individual goal in the Production environment:

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Goals** .

     (!--drafted for Shell release: Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List displays by default. 

1. Click the name of a goal in the list 

   Or

   Click one of the options below in the left panel, then click the name of a goal to access it:

   * Goal Alignment
   * Check-in 
   * Pulse 

   >[!NOTE]
   >
   >Depending on what action you want to perform on the individual goal, you might choose to select different sections every time. For information about the differences between the Workfront Goals sections, see [Overview of the Adobe Workfront Goals sections](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

   The Goal Details panel displays on the right. You can update the goal, its results, and activities in the Goal Details panel when you have access to manage it. For information about updating goals using the Goal Details panel, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
-->

個々の目標にアクセスするには次の手順に従います。

1. Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコンをクリックし、「**目標**」をクリックします。
デフォルトでは、目標リストが表示されます。
   ![&#x200B; 目標リスト &#x200B;](assets/goal-list-unshimmed.png)
1. リストで目標の名前をクリックします。
目標のページが表示されます。
   ![&#x200B; 目標ページ &#x200B;](assets/goal-page-unshimmed.png)
1. 目標名の右側にある **その他** メニュー ![&#x200B; その他アイコン &#x200B;](assets/more-icon.png) をクリックすると、目標をさらに編集または共有できます。
1. 左側のパネルにある「**目標の詳細**」をクリックして、目標に関する情報を編集します。詳しくは、[Adobe Workfront Goals の目標の詳細セクションで目標を更新](../goal-management/update-goals-in-goal-details-panel.md)を参照してください。


