---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: グラフを確認してAdobe Workfront目標の目標の進行状況の傾向を理解する
description: 目標の全体的な正常性とその進行状況の経時的なトレンドを、Adobe Workfront目標の「グラフ」セクションで確認できます。 このセクションのグラフでは、各目標の進行状況を分類することはできませんが、代わりに、すべての目標の進行状況ステータスと、指定した期間内の進行状況の全体的なスナップショットが表示されます。
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# グラフを確認してAdobe Workfront目標の目標の進行状況の傾向を理解する

<!-- drafted mostly for P&P release-->

目標の全体的な正常性とその進行状況の経時的なトレンドを、Adobe Workfront目標の「グラフ」セクションで確認できます。 このセクションのグラフでは、各目標の進行状況を分類することはできませんが、代わりに、すべての目標の進行状況ステータスと、指定した期間内の進行状況の全体的なスナップショットが表示されます。

>[!IMPORTANT]
>
>選択した期間の目標の合計数を「グラフ」セクションで確認できます。 ただし、Workfront目標の全体的な目標の進捗状況ステータスと完了率を計算する際には、ステータスが「アクティブ」と「クローズ」の目標のみが考慮されます。

## アクセス要件

<!--drafted for P&P release: 

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

この記事で説明する操作を実行するには、次のアクセス権が必要です。

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
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>目標へのアクセス権を表示またはそれ以上に設定</p> <p><b>メモ</b><p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront目標へのアクセス権の付与</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <div> 
     <p>目標に対する権限の表示以上</p> 
     <p>目標の共有について詳しくは、 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront目標での目標の共有</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 前提条件

を起動する前に、次の条件を満たす必要があります。

* メインメニューの目標領域を含むレイアウトテンプレート。

## Workfront目標のグラフのタイプ

グラフセクションまたはWorkfront目標では、次のグラフを使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">目標ヘルスチャート</td> 
   <td> <p>以下を表示するゲージチャート。</p> 
    <ul> 
     <li>選択した期間の目標の合計数。 ステータスの異なる目標が考慮されます。 </li> 
     <li>ステータスが「アクティブ」および「クローズ」の目標の進捗状況ステータス。</li> 
    </ul> <p>Workfront目標での進捗状況ステータスの計算方法について詳しくは、 <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront目標の目標の達成状況と条件の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目標進捗状況グラフ</td> 
   <td> <p>目標期間中の目標に対する更新を週単位で表示する折れ線グラフです。 目標の進捗状況グラフには、次の情報が表示されます。</p> 
    <ul> 
     <li>選択した期間内のすべてのアクティブな目標およびクローズした目標の平均予想および実際の完了率。 完了の割合の進行状況は、ノードで示される週単位の増分に分類されます。 </li> 
     <li>前週以降のアクティブな目標とクローズした目標の全体的な進行状況の平均割合。 </li> 
    </ul> <p>ヒント：目標達成度グラフは、選択した期間外に目標に対して更新がおこなわれた場合、情報を表示しない場合があります。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## グラフでの目標の進捗状況の確認

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) > **目標** をクリックします。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   「Workfront目標」領域が開きます。

1. クリック **グラフ** をクリックします。

   ![](assets/graphs-in-left-panel.png)

   「グラフ」セクションが表示されます。

   デフォルトでは、「グラフ」セクションに表示される目標は、次の条件によって制限されます。

   * 「グラフ」領域に適用されるフィルター。
   * ステータスが「アクティブ」および「ドラフト」の目標。

1. （オプション）「グラフ」セクションの右上隅にあるフィルターを更新して、表示する情報のタイプを選択します。

   目標のフィルタリングについて詳しくは、 [Adobe Workfront目標での情報のフィルター](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   複数の期間を表示するように選択した場合は、各期間のヘルスチャート（ゲージ）と進捗チャート（線）が表示されます。

1. 以下の表の情報を確認し、目標稼働状況チャートを確認してください。

   ![](assets/gauge-graph-wf-align-350x230.png)

   | 目標の合計数 | グラフの下部にある数は、選択した期間内のすべての目標の数を、選択したすべてのステータスで示します。 |
   |---|---|
   | 平均完了率 | グラフの上部にあるこの数は、選択した期間のアクティブな目標とクローズした目標の平均達成率を示します。 |
   | 目標とその進捗 | グラフのセグメントにカーソルを合わせたときの、各進捗状況ステータスセグメントの目標数。 「アクティブ」または「閉じた」ステータスの目標のみがセグメントでカウントされます。 |


1. 以下の表で、「目標進捗状況」グラフを確認する際に、情報を確認してください。

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>ベースラインの進行状況</td> 
      <td>緑の傾き線は、選択した期間のアクティブな目標とクローズした目標の、予想される全体的な完了率の平均を示します。 ある期間内のすべての目標は完了すると予想されるので、ベースラインの進捗状況は常にその期間の終わりに 100%になります。 </td> 
     </tr> 
     <tr> 
      <td>実際の進捗状況</td> 
      <td> <p>青い線は、選択した期間のアクティブな目標とクローズした目標の、週単位の増分での実際の完了率の平均を示します。 目標期間中の各週には、行内のノードがマークされます。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 目標の進捗状況グラフで 1 週間のノードにマウスポインターを置き、以下の内容を確認します。

   * **週の日付**:選択した週の月、日、年。
   * **進行状況**:選択した週のすべての目標の実際の達成率の平均。
   * **ベースライン**:選択した週のすべての目標の予想完了率の平均。

1. （オプション）「 **進行状況** 進行状況グラフの下部に、実際の進行状況行全体を削除します。

   または

   クリック **ベースライン** をクリックすると、グラフから期待される進捗状況が削除されます。

 
