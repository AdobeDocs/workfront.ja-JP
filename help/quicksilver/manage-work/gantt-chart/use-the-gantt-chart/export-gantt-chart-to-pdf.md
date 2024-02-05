---
navigation-topic: use-the-gantt-chart
title: ガントチャートを PDF に書き出す
description: ガントチャートを PDF に書き出しできます。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 98%

---

# [!UICONTROL ガントチャート]を PDF に書き出します。

[!UICONTROL ガントチャート]を PDF に書き出すことができます。

[!UICONTROL ガントチャート]を PDF に書き出した後、印刷したり、メールに添付したりして、他のユーザーと共有できます。

## アクセス要件

この記事の手順に従うには、以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトとタスクに対する[!UICONTROL View]以上のアクセス権</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する[!UICONTROL View]以上のアクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!UICONTROL ガントチャート]を書き出します。

1. PDF に書き出す[!UICONTROL ガントチャート]をアクセスします（[[!UICONTROL ガントチャートの基本を学ぶ]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)を参照）。
1. [!UICONTROL ガントチャート]が設定されていることを確認して、書き出す前に適切な情報を表示します。

   >[!NOTE]
   >
   >プロジェクトのリストから[!UICONTROL ガントチャート]を書き出す場合、PDF ファイルには、各プロジェクトのタスクではなく、リスト内のプロジェクトのみが含まれます。タスクのリストを書き出す場合は、タスクが関連付けられているプロジェクトから実行するか、タスクレポートを作成してレポートの結果を[!UICONTROL ガントチャート表示]に表示することで実行することができます。

   次の情報を設定できます。

   * タスクのリストで必要に応じて、フィルター、表示、およびグループ化を設定します。[!UICONTROL ガントチャート]を表示する際、リストビューで選択されたフィルターおよびグループは維持されます。書き出された[!UICONTROL ガントチャート]にビューが反映されるのは、最初のページの[!UICONTROL ガントチャート]の横に表示されるリスト内のみです。ビューは、[!UICONTROL ガントチャート]自体に表示されません。

     >[!TIP]
     >
     >[!UICONTROL ガントチャート]に対してよりスペースを確保する場合は、できるだけ少ない列を含むビューを適用します。

   * [!UICONTROL ガントチャート]の設定オプション。例えば、マイルストーン、日付、[!UICONTROL ベースライン]、または[!UICONTROL 完了率]を有効にして、[!UICONTROL ガントチャート]に表示できます。

     詳しくは、[[!UICONTROL ガントチャートでの情報の表示設定]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)を参照してください。

     >[!NOTE]
     >
     > [!UICONTROL ガントチャート] が PDF に書き出される場合、割り当ては[!UICONTROL ガントチャート]に表示されません。[!UICONTROL ガントチャート]が PDF に書き出された場合、割り当てはリストビューにのみ表示されます。

   * [!UICONTROL ガントチャート]に表示される期間。\

     詳しくは、[[!UICONTROL ガントチャートでの情報の表示]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)を参照してください。

     書き出したファイルでの期間の表示は、後の手順で「**[!UICONTROL 表示ビュー]**」または「**[!UICONTROL 複数ページ]**」のどちら選択するかによって異なります。

1. （オプション）書き出す PDF に特定のタスクのみを含める場合は、含めるタスクを選択します。

   タスクを選択しない場合は、書き出された PDF にすべてのタスクが含まれます。

   例えば、50 件のタスクを含むプロジェクトの[!UICONTROL ガントチャート]を表示する際、書き出した[!UICONTROL ガントチャート]に 10 件のタスクのみを表示する場合、表示する 10 件のタスクを選択します。

1. プリンターアイコンをクリックします。\
   **[!UICONTROL PDF に書き出し]**&#x200B;ダイアログボックスが表示されます。\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 表示されているもののみを書き出すか、[!UICONTROL ガントチャート]全体を書き出すかを選択します。

   * **[!UICONTROL 表示ビュー]：**&#x200B;最大 500 件の項目を書き出す前に、画面に表示されるすべてのタスク（サブタスクを含む）を書き出します。（これは「**[!UICONTROL プレビュー]**」セクションに表示されるものではありません。「[!UICONTROL プレビュー]」セクションには、サンプルデータのみが含まれています）。

     親タスクが折りたたまれ、サブタスクが表示されない場合でも、書き出された PDF にサブタスクが含まれます。親タスクのみを含めるには、含める親タスクを選択し、サブタスクを選択解除の状態にします。

     **[!UICONTROL ズーム]**&#x200B;ドロップダウンメニューまたはスライダーツールを使用して、[!UICONTROL ガントチャート]の一部のみを表示します（[[!UICONTROL ガントチャートでの情報の表示]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)を参照）。

   * **[!UICONTROL 複数のページ]：**[!UICONTROL ガントチャート]全体を書き出します。現在の画面に表示されていない項目も含めて最大 500 個あります。\

     [[!UICONTROL ガントチャートでの情報の表示方法]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)で説明したように、各ページに表示する情報の量を指定する&#x200B;**[!UICONTROL ズーム先]**&#x200B;ドロップダウンメニューまたはスライダーツールを使用できます。より詳細なオプションを選択して、書き出すページを増やして表示するか、より概略なオプションを選択して、書き出すページを少なく表示するかを選択します。

     >[!NOTE]
     >
     >500 個を超える項目を含む[!UICONTROL ガントチャート]を書き出す必要がある場合は、表示される項目数が 500 個未満またはページ数が 250 ページ未満になるように、リストにフィルターを適用してから、[!UICONTROL ガントチャート]を表示します。フィルターの適用方法について詳しくは、  [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >次の状況では、ガントチャート全体を書き出すことはできません。
     >
     >   
     >   
     >   * 250 ページを超える場合
     >   * 項目が 500 を超える場合




1. PDF を PDF に書き出した後に印刷する場合は、**[!UICONTROL ページサイズ]**&#x200B;ドロップダウンメニューから、印刷する用紙のサイズを選択します。\
   **[!UICONTROL レター]**、**[!UICONTROL リーガル]**、**[!UICONTROL 帳簿]**、**[!UICONTROL A1]**、**[!UICONTROL A2]**、**[!UICONTROL A3]**（一部の言語でのみ使用可能）、または **[!UICONTROL A4]** を選択できます。
1. 「**[!UICONTROL ページオリエンテーション]**」セクションで、PDF を横向き方向と縦向き方向のどちらで書き出すかを選択します。
1. 書き出した PDF に凡例を含める場合、「**[!UICONTROL 凡例の表示]**」を選択します。
1. 「**[!UICONTROL 書き出し]**」をクリックします。

   [!UICONTROL ガントチャート]の PDF が作成され、お使いのコンピューターにダウンロードされます。

   書き出されたファイルの下部には、凡例があります。これは、[!UICONTROL ガントチャート]で有効にしたオプションのみを説明し、それはタスクリストで使用できます。

   例えば、マイルストーンに関連付けられたタスクが 1 つ以上ある場合にのみ、マイルストーンが凡例に表示されます。

   ![gantt_chart_with_updated__limed__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
