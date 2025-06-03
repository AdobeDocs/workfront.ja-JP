---
navigation-topic: use-the-gantt-chart
title: ガントチャートを PDF に書き出す
description: ガントチャートはPDFに書き出すことができます。 その後、印刷したりメールに添付したりして、他のユーザーと共有できます。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 40%

---

# [!UICONTROL ガントチャート]の PDF への書き出し

<!--Audited: 5/2025-->

[!UICONTROL  ガントチャート ] をPDFに書き出すことができます。 その後、印刷したりメールに添付したりして、他のユーザーと共有できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL ライト ] 以上</p>
   <p>現在：[!UICONTROL Review] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトとタスクに対する[!UICONTROL View]以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する[!UICONTROL View]以上のアクセス権</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!UICONTROL ガントチャート]を書き出します。

1. PDF に書き出す[!UICONTROL ガントチャート]をアクセスします（[[!UICONTROL ガントチャートの基本を学ぶ]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)を参照）。
1. [!UICONTROL  ガントチャート ] を設定して、書き出す適切な情報を表示します。

   >[!NOTE]
   >
   >プロジェクトのリストから[!UICONTROL ガントチャート]を書き出す場合、PDF ファイルには、各プロジェクトのタスクではなく、リスト内のプロジェクトのみが含まれます。タスクのリストを書き出す場合は、タスクが関連付けられているプロジェクトから実行するか、タスクレポートを作成してレポートの結果を[!UICONTROL ガントチャート表示]に表示することで実行することができます。

   次のいずれかの情報を設定します。

   * **ガントチャート** の上にある **フィルター [!UICONTROL 、] 表示**、**グループ化** の各アイコンをクリックして、[!UICONTROL  ガントチャート ] のアイテムのリストに適用する既存のフィルター、表示、グループ化を追加または編集します。

     リスト表示で選択したフィルターとグループは、[!UICONTROL  ガントチャート ] を表示する際に維持されます。 ビューは、書き出された [!UICONTROL  ガントチャート ] に、最初のページで [!UICONTROL  ガントチャート ] の横に表示されるリスト内にのみ反映されます。 ビューは、[!UICONTROL ガントチャート]自体に表示されません。

     >[!TIP]
     >
     >[!UICONTROL  ガントチャート ] の領域を広げるには、できるだけ少ない列を含むビューを適用します。

   * 「**予定日に切り替え**」オプションを選択して、予定日ではなく見込み日を表示します。 デフォルトでは、予定日が表示されます。

   * ガントチャートの右上隅にある **設定** アイコン ![ 設定アイコン ](assets/settings-icon.png) をクリックして、表示する情報を選択します。 選択すると、この情報は書き出されたガント PDF ファイルに含まれます。

     次のオプションから選択します。

      * 実際の日付
      * 割り当て
      * ベースライン
      * コミット日
      * 完了率（％）
      * クリティカルパス
      * マイルストーンひし形
      * マイルストーン線
      * 先行タスク
      * 進捗ステータス
      * （条件付き）予定日
      * （条件付き）予定日

     詳しくは、[[!UICONTROL ガントチャートでの情報の表示設定]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)を参照してください。

     >[!NOTE]
     >
     > [!UICONTROL ガントチャート] が PDF に書き出される場合、割り当ては[!UICONTROL ガントチャート]に表示されません。エクスポートすると、割り当てはリスト表示にのみ表示されます。

   * [!UICONTROL  ガント チャート ] に表示される期間です。 これがエクスポートファイルに表示される方法は、後の手順で **[!UICONTROL 表示されるもの]** または **[!UICONTROL 複数のページ]** のどちらを選択したかによって異なります。

     詳しくは、[[!UICONTROL ガントチャートでの情報の表示]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)を参照してください。



1. （オプション）書き出されたPDFに特定のタスクのみを含めるには、含めるタスクを選択します。 タスクを選択しない場合は、書き出された PDF にすべてのタスクが含まれます。

   例えば、50 件のタスクを含むプロジェクトの[!UICONTROL ガントチャート]を表示する際、書き出した[!UICONTROL ガントチャート]に 10 件のタスクのみを表示する場合、表示する 10 件のタスクを選択します。

1. ガントチャートの右上隅にあるプリンタアイコン ![ プリンタアイコン ](assets/printer-icon.png) をクリックします。
**[!UICONTROL PDFに書き出し]** ダイアログボックスが表示されます。

   ![PDFに書き出しダイアログボックス ](assets/exported-gantt-ui-350x225.png)

1. [**エクスポート**] セクションで、次のいずれかのオプションを選択して、表示されている内容のみをエクスポートするか、[!UICONTROL  ガント チャート ] 全体をエクスポートするかを指定します。

   * **[!UICONTROL 表示ビュー]：**&#x200B;最大 500 件の項目を書き出す前に、画面に表示されるすべてのタスク（サブタスクを含む）を書き出します。（「プレビュー **[!UICONTROL セクションに表示されるものではなく、]** プレビュー **セクションにはサンプルデータのみが含まれ** います）。

     親タスクが折りたたまれ、サブタスクが表示されない場合でも、書き出された PDF にサブタスクが含まれます。親タスクのみを含めるには、含める親タスクを選択し、サブタスクを選択解除の状態にします。

     >[!TIP]
     >
     >ズームツールまたはスライダーツールを使用して、「[!UICONTROL  ガントチャート ] での情報の表示 [ で説明しているように、[!UICONTROL  ガントチャート ]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) の一部のみを表示できます。 「よりきめ細かい」オプションを選択して書き出すページを多く表示するか、「よりきめ細かい」オプションを選択して書き出すページの表示を少なくします。


   * **[!UICONTROL 複数ページ ]:** 現在の画面に表示されない項目を含め、[!UICONTROL  ガントチャート ] 全体（最大 500 項目）を書き出します。

     >[!NOTE]
     >
     >* 500 項目を超える [!UICONTROL  ガントチャート ] を書き出す必要がある場合は、フィルターをリストに適用してから [!UICONTROL  ガントチャート ] を表示すると、表示される項目が 500 項目、つまりページの数が 250 個未満になります。 フィルターの適用方法について詳しくは、[フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)を参照してください。
     >
     >
     >* 次の状況では、ガント チャート全体をエクスポートできません：
     >   
     >   * 250 ページを超える場合。
     >   * 500 個を超える項目が含まれている場合。


1. PDFに書き出した後にPDFを印刷する場合は、印刷する用紙のサイズを **[!UICONTROL ページサイズ]** ドロップダウンメニューで選択します。
以下のオプションから選択できます。

   * **[!UICONTROL レター]**
   * **[!UICONTROL 法的事項]**
   * **[!UICONTROL 台帳]**
   * **[!UICONTROL A1]**
   * **[!UICONTROL A2]**
   * **[!UICONTROL A3]** （一部の言語のみ使用可能）
   * **[!UICONTROL A4]**
1. 「**[!UICONTROL ページオリエンテーション]**」セクションで、PDF を横向き方向と縦向き方向のどちらで書き出すかを選択します。
1. 書き出した PDF に凡例を含める場合、「**[!UICONTROL 凡例の表示]**」を選択します。
1. **[!UICONTROL 書き出し]** をクリックします。 PDF が作成され、コンピューターにダウンロードされます。

   書き出されたファイルの下部にある凡例は、[!UICONTROL  ガント チャート ] で有効にしたオプションと、タスクリストで使用可能なオプションのみを説明します。 例えば、マイルストーンに関連付けられたタスクが 1 つ以上ある場合にのみ、マイルストーンが凡例に表示されます。

   ![gantt_chart_with_updated__limed__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
