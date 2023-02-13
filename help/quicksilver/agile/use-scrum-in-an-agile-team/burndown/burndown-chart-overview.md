---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: アジャイルバーンダウンチャートの概要
description: バーンダウングラフには、ストーリーが反復またはプロジェクトでどのように進行しているかが視覚的に表示されます。 実際のバーンダウン率は、反復またはプロジェクトタイムラインの理想的なバーンダウン率に対して測定されます。
author: Lisa
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# アジャイルバーンダウンチャートの概要

バーンダウングラフは、ストーリーが反復を通じてどのように進んでいるかを視覚的に示します。 実際のバーンダウン率は、反復タイムラインの理想的なバーンダウン率に対して測定されます。

選択した日に基づいてバーンダウンチャートが調整されます。 現在の日付がデフォルトです。 前日を選択した場合、バーンダウングラフのすべてのデータと [!UICONTROL 完了ステータス] 「 」セクションを選択すると、選択した日の終わりのデータを表すために、バーンダウングラフの上のセクションが再計算されます。 ( 過去の日付または現在の日付を選択できます。将来の日数は選択できません。)

![](assets/agile-iteration-burndown-350x88.png)

## 視覚指標

バーンダウンチャートには、次の視覚的指標が含まれます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt=""> </td> 
   <td> <p>反復が開始された時点に基づく理想的なバーンダウン率。</p> <p>繰り返しの範囲が変更されない（時間やポイントが追加または削除されない）場合、この行は表示されません。</p> <p>この線は、休日に作業が行われる場合は平坦に表示されます。 詳しくは、 <a title="アジャイルバーンダウンチャートの使用" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休日がバーンダウンチャートに与える影響</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt=""> </td> 
   <td> <p>現在のストーリーまたはタスクに基づく理想的なバーンダウン率。</p> <p>現在の理想的なバーンダウン率（実線の青い線）は、反復が開始した後の反復に時間やポイントが追加または削除された場合の、元の理想的なバーンダウン率（実線の青い線）と異なります。</p> <p>この線は、休日に作業が行われる場合は平坦に表示されます。</p> <p>詳しくは、 <a title="アジャイルバーンダウンチャートの使用" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">休日がバーンダウンチャートに与える影響</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt=""> </td> 
   <td> <p>バーンダウン率が理想的な値（理想的なバーンダウン計算より 1 日あたりの残りポイント数または時間数が多い）未満の場合、実際のバーンダウン率は赤で表示されます。</p> <p>次の式は、実際のバーンダウン率を計算するために使用されます。</p> <p>[SUM(Point or Hour Value of In-Progress Work * Percent Complete) + Point or Hour Value of Completed Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt=""> </td> 
   <td> <p>バーンダウン率が理想的な値以上（理想的なバーンダウン計算より 1 日当たりの残りポイント数が同じか、または少ない場合）には、実際のバーンダウン率が緑色で表示されます。</p> <p>次の式は、実際のバーンダウン率を計算するために使用されます。</p> <p>[SUM(Point or Hour Value of In-Progress Work * Percent Complete) + Point or Hour Value of Completed Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>範囲の変更（時間またはポイントがイテレーションから追加または削除される）。</p> <p>スコープの変更は、常に 1 日の中央に縦線で表示されます。 また、スコープの変更が発生した日の中央に青い点が表示されます。</p> <p>バーンダウンチャートの縦軸は、ストーリーのポイントまたは時間を示します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>日付範囲の変更（反復期間が増加または減少）。</p> <p>繰り返し期間が変更された日の中央に、青い点が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt=""> </td> 
   <td> <p>作業が燃え尽きるたびに、実際の燃え尽き率に緑または赤の点が表示されます。 ( その日の実際の燃え下がり率が赤い場合、点は赤です。その日の実際の燃え下がり率が緑の場合、点は緑です。</p> <p>次のいずれかが発生すると、作業は焼け落ちます。</p> 
    <ul> 
     <li> ストーリーの [!UICONTROL パーセント完了 ] が増加します。<br>[!UICONTROL 完了率 ] は、次の場合に増加します。 
      <ul> 
       <li> <p>手動で変更済み</p> </li> 
       <li> <p>ストーリーのポイントまたは時間数が更新されます</p> </li> 
      </ul></li>  
     <li>ストーリーのステータスが [!UICONTROL 完了 ] に変わります</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 休日がバーンダウンチャートに与える影響 {#how-days-off-affect-the-burndown-chart}

で定義されたデフォルトのスケジュール [!DNL Workfront] は、バーンダウンから休日（週末と休日）を除外することで、バーンダウンチャートに影響します。 バーンダウングラフでは、デフォルトのスケジュールを使用して稼働日を定義します (  [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)) をクリックします。

「アジャイル」チームは、代替スケジュールを定義することで、チーム固有の非就業日を組み込むことができます（記事を参照） [バーンダウングラフに代替のチームスケジュールを使用](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md)) をクリックします。 その後、この代替スケジュールは、チームに割り当てられたイテレーションのバーンダウンチャートに反映されます。 代替スケジュールは、バーンダウンチャートにのみ影響します。

次の場合にのみ、休日がバーンダウンチャートに反映されます。

* 仕事は以前休みの日にログに記録されていた。 （作業が記録された日が表示されます）。

   仕事が休日にログオンしたとき：

   * チームが何らかの作業を行う予定がないため、ログに記録された作業は、理想的なバーンダウンの計算時に含まれません。
   * 理想的なバーンダウン線（実線の青線と破線の青線）は、作業が行われた日、またはバーンダウン図を表示している日（休日に表示している場合）に関しては、バーンダウン図にフラットとして表示されます。
   * ログに記録された作業は、推定完了数、1 日あたりの平均ポイント数や時間数など、他のバーンダウン統計を計算する際に含まれます。

* 休日にバーンダウンチャートを表示しています。 （表示している日がバーンダウンチャートに表示されます。）
* 休日にその反復の残り作業の合計を完了します。

   ユーザーが 1 日のオフにその反復の残り作業の合計を完了すると、 [!UICONTROL 推定完了] 「 」フィールドには、反復が完了した日付が表示されます。

   反復を計画する際に、非稼働日の反復終了日を設定し、その反復が時間通りに完了するように追跡している場合、 [!UICONTROL 推定完了] 設定した反復終了日の前の最終稼動日に日付が設定されます（非稼働日に作業が焼き切られるようにスケジュールされていないため）。

   繰り返しの終了日は、記事で説明されているように、繰り返しが計画される際に指定されます [反復を作成](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
