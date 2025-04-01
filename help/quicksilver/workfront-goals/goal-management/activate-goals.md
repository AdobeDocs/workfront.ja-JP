---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals で目標をアクティブ化
description: 目標を作成すると、Adobe Workfront Goals はそれをドラフトのステータスで保存します。下書きの目標は目標管理には含まれません。
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 83%

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

1. 目標名の右側にある **その他** メニュー ![ その他のアイコン ](../goal-management/assets/more-icon.png) をクリックしてから、「**アクティベート**」をクリックします。

   ![ 詳細メニューが展開されました ](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   目標のステータスがアクティブに変わります。目標の進捗状況をトラックできるようになり、目標はチェックインセクションに表示されるほか、Workfront 目標のグラフセクションでも考慮されるようになりました。
