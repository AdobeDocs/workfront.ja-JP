---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals で目標をアクティブ化
description: 目標を作成すると、Adobe Workfront Goals はそれをドラフトのステータスで保存します。下書きの目標は目標管理には含まれません。
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 76%

---

# Adobe Workfront Goals で目標をアクティブ化

<!--Audited for P&P only: 4/2025-->

目標を作成すると、Adobe Workfront Goals はそれをドラフトのステータスで保存します。下書きの目標は目標管理には含まれません。

進捗状況を更新して目標達成にどれだけ近づいているかを追跡するには、それをアクティブ化する必要があります。これにより、ステータスがアクティブに変わります。

目標の作成については、[Adobe Workfront Goals での目標の作成](../../workfront-goals/goal-management/create-goals.md)を参照してください。

>[!IMPORTANT]
>
>結果とアクティビティの進行状況を更新するには、その前に目標をアクティブ化する必要があります。


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
 <td role="rowheader">アクセスレベル設定</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr>
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
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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

## 前提条件

目標をアクティブ化するには、その目標がアクティビティ、結果、プロジェクトなどの進行状況インジケーターに関連付けられているか、別のアクティブな目標と連携している必要があります。

目標をアクティブ化するには、次のうち 1 つ以上を実行します。

* 目標への結果の追加

  詳しくは、[Adobe Workfront Goals の目標に結果を追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)を参照してください。

* 目標へのアクティビティの追加

  詳しくは、[Adobe Workfront Goals の目標へのアクティビティの追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)を参照してください。

* プロジェクトを目標に結びつける

  詳しくは、[Adobe Workfront Goals の目標にプロジェクトを追加](../results-and-activities/connect-projects-to-goals-overview.md)を参照してください。

* アクティブ化する目標に別の目標を整合させる

  詳しくは、[Adobe Workfront Goals で目標を結び付けて整合させる](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)を参照してください。

## 目標のアクティブ化

作成した目標、または管理権限を持つ目標をアクティブ化できます。

1. アクティブ化する目標に移動します。目標ページが開きます。

1. 目標名の右側にある **その他** メニュー ![&#x200B; その他のアイコン &#x200B;](../goal-management/assets/more-icon.png) をクリックしてから、「**アクティベート**」をクリックします。

   ![&#x200B; 詳細メニューが展開されました &#x200B;](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   目標のステータスがアクティブに変わります。目標の進捗状況をトラックできるようになり、目標はチェックインセクションに表示されるほか、Workfront 目標のグラフセクションでも考慮されるようになりました。
