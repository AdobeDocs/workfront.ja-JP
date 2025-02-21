---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: グラフを確認して Adobe Workfront Goals の目標進捗の傾向を理解する
description: 目標の全体的な正常性とその進捗の経時的な傾向は、Adobe Workfront Goals の「グラフ」セクションで確認できます。このセクションのグラフでは、各目標の進捗を分類することはできませんが、代わりに、すべての目標の進捗ステータスと指定した期間の進捗の全体的なスナップショットが表示されます。
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 91%

---

# グラフを確認して Adobe Workfront Goals の目標進捗の傾向を理解する

<!-- drafted mostly for P&P release-->

目標の全体的な正常性とその進捗の経時的な傾向は、Adobe Workfront Goals の「グラフ」セクションで確認できます。このセクションのグラフでは、各目標の進捗を分類することはできませんが、代わりに、すべての目標の進捗ステータスと指定した期間の進捗の全体的なスナップショットが表示されます。

>[!IMPORTANT]
>
>選択した期間の目標の合計数を「グラフ」セクションで確認できます。ただし、Workfront Goals では、全体的な目標の進捗ステータスと完了率を計算する際に、ステータスがアクティブおよびクローズの目標のみを考慮します。

## アクセス要件

この記事で説明する操作を実行するには、次のアクセス権が必要です。

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
 <p> 新製品の要件は、次のいずれかです。 </p>
<ul>
<li>Select またはPrime Adobe Workfront プランと、追加のAdobe Workfront Goals ライセンス。</li>
<li>Ultimate Workfrontプラン。デフォルトでWorkfront Goals が含まれています。 </li></ul>
 <p>または</p>
 <p>現在の必要な製品：Workfront プランとAdobe Workfront Goals の追加ライセンス。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>アクセスレベル</p></td>
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

## Workfront Goals のグラフのタイプ

グラフのセクションまたは Workfront Goals では、次のグラフを使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">目標ヘルスチャート</td> 
   <td> <p>次を表示するゲージチャート。</p> 
    <ul> 
     <li>選択した期間の目標の合計数。ステータスの異なる目標が考慮されます。 </li> 
     <li>ステータスがアクティブおよびクローズの目標の進捗ステータス。</li> 
    </ul> <p>Workfront Goals での進捗ステータスの決定方法について詳しくは、<a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront Goals の目標進捗と状況の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目標進捗グラフ</td> 
   <td> <p>目標期間中の目標に対する更新を週単位で表示する折れ線グラフです。目標の進捗チャートには、次の情報が表示されます。</p> 
    <ul> 
     <li>選択した期間内のすべてのアクティブな目標およびクローズした目標の平均予想および実際の完了率。完了率の進捗は、ノードで示される週単位の増分に分割されます。 </li> 
     <li>前週以降のアクティブな目標とクローズした目標の全体的な進捗の平均割合。 </li> 
    </ul> <p>ヒント：目標の進捗チャートは、選択した期間外で目標に対して更新が行われた場合、情報が表示されない場合があります。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## グラフでの目標の進捗の確認

1. 右上隅の **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png)/**目標** をクリックします。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Workfront Goals エリアが開きます。

1. 左側のパネルで「**グラフ**」をクリックします。

   ![ 左パネルのグラフ ](assets/graphs-in-left-panel.png)

   「グラフ」セクションが表示されます。

   デフォルトでは、「グラフ」セクションに表示される目標は、次の条件によって制限されます。

   * 「グラフ」エリアに適用されるフィルター。
   * ステータスがアクティブおよびドラフトの目標。

1. （オプション）グラフのセクションの右上隅にあるフィルターを更新して、表示する情報のタイプを選択します。

   目標のフィルタリングについて詳しくは、[Adobe Workfront Goals での情報のフィルター](../../workfront-goals/goal-management/filter-information-wf-goals.md)を参照してください。

   >[!TIP]
   >
   >複数の期間を表示するように選択した場合は、各期間のヘルスチャート（ゲージ）と進捗チャート（線）が表示されます。

1. 以下の表の情報を確認し、目標のヘルスチャートを確認してください。

   ![ ゲージグラフ ](assets/gauge-graph-wf-align-350x230.png)

   | 目標の合計数 | チャートの下部にある数は、選択した期間内のすべての目標の数を、選択したすべてのステータスで示します。 |
   |---|---|
   | 平均完了率 | チャートの上部にあるこの数は、選択した期間のアクティブな目標とクローズした目標の平均完了率を示します。 |
   | 目標とその進捗 | チャートのセグメントにポインタを合わせた際の各進捗ステータスセグメントの目標数。アクティブまたはクローズのステータスの目標のみがセグメントでカウントされます。 |


1. 目標進捗チャートを確認する際に、以下の表の情報を確認してください。

   ![ 折れ線グラフ ](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>ベースラインの進捗</td> 
      <td>緑色の傾き線は、選択した期間のアクティブな目標とクローズした目標の、予想される全体的な完了率の平均を示します。ある期間内のすべての目標は完了すると予想されるので、ベースラインの進捗は常にその期間の終わりに 100%になります。 </td> 
     </tr> 
     <tr> 
      <td>実際の進捗状況</td> 
      <td> <p>青色の線は、選択した期間のアクティブな目標とクローズした目標の、週単位の増分での実際の完了率平均を示します。目標期間中の各週は、行内のノードでマークされます。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 目標の進捗チャートで 1 週間のノードにポインタを合わせて、次の内容を確認します。

   * **週の日付**：選択した週の月、日および年。
   * **進捗**：選択した週のすべての目標の実際の完了率の平均。
   * **ベースライン**：選択した週のすべての目標の予想完了率の平均。

1. （オプション）進捗チャートの下部にある「**進捗**」をクリックして、実際の進捗の行全体を削除します。

   または

   チャートの下部にある「**ベースライン**」をクリックすると、チャートから予想される進捗が削除されます。

 
