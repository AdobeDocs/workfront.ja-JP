---
navigation-topic: use-the-gantt-chart
title: ガントチャートをPDFにエクスポート
description: ガントチャートをPDFにエクスポートできます。
author: Alina
feature: Work Management
exl-id: 91aad9e0-25c9-4eae-aa66-8aab763d3b76
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 0%

---

# を書き出します。 [!UICONTROL ガントチャート] PDF

次の項目を書き出すことができます。 [!UICONTROL ガントチャート] PDFに

を書き出した後 [!UICONTROL ガントチャート] PDFを印刷したり、電子メールに添付したりして、他のユーザーと共有できます。

## アクセス要件

この記事の手順に従うには、次の手順を実行する必要があります。

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
   <td> <p>[!UICONTROL 表示 ] 以降のプロジェクトおよびタスクへのアクセス権</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>プロジェクトへの [!UICONTROL 表示 ] 以降のアクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## を書き出します。 [!UICONTROL ガントチャート]

1. 次にアクセス： [!UICONTROL ガントチャート] PDFに書き出す [の基本を学ぶ [!UICONTROL ガントチャート]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).
1. 次の項目が設定されていることを確認します。 [!UICONTROL ガントチャート] をクリックして、適切な情報を表示してから書き出します。

   >[!NOTE]
   >
   >次を書き出す場合： [!UICONTROL ガントチャート] プロジェクトのリストでは、PDFファイルには、各プロジェクトのタスクではなく、リスト内のプロジェクトのみが含まれます。 タスクのリストをエクスポートする場合は、タスクが関連付けられているプロジェクトから、またはタスクレポートを作成してレポートの結果を [!UICONTROL ガントチャート表示].

   次の情報を設定できます。

   * タスクのリストで必要に応じて、フィルター、表示およびグループ化を設定します。 リスト表示で選択されたフィルターおよびグループは、 [!UICONTROL ガントチャート]. ビューは、書き出された [!UICONTROL ガントチャート] の横に表示されるリスト内のみ [!UICONTROL ガントチャート] を最初のページに追加します。 ビューは、 [!UICONTROL ガントチャート] それ自体。

     >[!TIP]
     >
     >より広いスペースを [!UICONTROL ガントチャート] を使用する場合は、できるだけ少ない列を含むビューを適用します。

   * 「 [!UICONTROL ガントチャート]. 例えば、マイルストーン、日付、 [!UICONTROL 基準]または [!UICONTROL 完了率] ～に現れる [!UICONTROL ガントチャート].

     詳しくは、   [情報を [!UICONTROL ガントチャート]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

     >[!NOTE]
     >
     > 割り当ては、 [!UICONTROL ガントチャート] 時に [!UICONTROL ガントチャート] がPDFに書き出されます。 次の場合に [!UICONTROL ガントチャート] がPDFに書き出され、割り当てはリストビューにのみ表示されます。

   * 表示される期間 [!UICONTROL ガントチャート].\

     詳しくは、 [での情報の表示 [!UICONTROL ガントチャート]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

     エクスポートファイルで期間を表示する方法は、 **[!UICONTROL 表示内容]** または **[!UICONTROL 複数のページ]** 後の手順で実行します。

1. （オプション）エクスポートするPDFに特定のタスクのみを含める場合は、含めるタスクを選択します。

   タスクを選択しない場合は、書き出されたタスクにすべてのタスクが含まれますPDF。

   例えば、 [!UICONTROL ガントチャート] 50 個のタスクを含むが、エクスポートされたタスクに対して 10 個のタスクのみを表示するプロジェクトの場合 [!UICONTROL ガントチャート]「 」で、表示する 10 個のタスクを選択します。

1. プリンタのアイコンをクリックします。\
   The **[!UICONTROL 書き出しPDF]** ダイアログボックスが表示されます。\
   ![exported_gantt_UI.png](assets/exported-gantt-ui-350x225.png)

1. 表示されているもののみを書き出すか、全体を書き出すかを選択します [!UICONTROL ガントチャート]:

   * **[!UICONTROL 表示内容]:** 最大 500 個の項目を書き出す前に画面に表示されるすべてのタスク（サブタスクを含む）を書き出します。 ( これは、 **[!UICONTROL プレビュー]** セクション； [!UICONTROL プレビュー] 「 」セクションには、サンプルデータのみが含まれています )。

     親タスクが折りたたまれ、サブPDFが表示されない場合でも、書き出されたタスクにサブタスクが含まれます。 親タスクのみを含めるには、含める親タスクを選択し、サブタスクを選択しないままにします。

     以下を使用すると、 **[!UICONTROL ズーム先]** ドロップダウンメニューまたはスライダーツールを使用して、 [!UICONTROL ガントチャート]を参照してください。 [での情報の表示 [!UICONTROL ガントチャート]](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md) .

   * **[!UICONTROL 複数のページ]:** 全体を書き出す [!UICONTROL ガントチャート]（現在の画面に表示されない項目が 500 個まで）。\

     以下を使用すると、 **[!UICONTROL ズーム先]** 各ページに表示する情報の量を指定するドロップダウンメニューまたはスライダーツール ( [情報を [!UICONTROL ガントチャート]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md). より詳細なオプションを選択して、書き出すページを増やすか、より詳細なオプションを選択して、書き出すページを少なく表示するかを選択します。

     >[!NOTE]
     >
     >を書き出す必要がある場合は、 [!UICONTROL ガントチャート] 500 個を超える項目を含むを表示するには、リストにフィルターを適用してから、 [!UICONTROL ガントチャート] 表示される項目数が 500 個未満または 250 ページ未満になるようにします。 フィルターの適用方法について詳しくは、  [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).
     >
     >
     >次の状況では、ガントチャート全体をエクスポートできません。
     >
     >   
     >   
     >   * 250 ページを超える場合
     >   * 項目が 500 を超える場合




1. PDFをPDFに書き出した後に印刷する場合は、 **[!UICONTROL ページサイズ]** ドロップダウンメニューから、印刷する用紙のサイズを選択します。\
   次の項目を選択できます。 **[!UICONTROL レター]**, **[!UICONTROL 法的事項]**, **[!UICONTROL 元帳]**, **[!UICONTROL A1]**, **[!UICONTROL A2]**, **[!UICONTROL A3]** （一部の言語でのみ使用可能）、または **[!UICONTROL A4]**.
1. Adobe Analytics の **[!UICONTROL ページの向き]** 「 」セクションで、PDFを横置きと縦置きのどちらで書き出すかを選択します。
1. 選択 **[!UICONTROL 凡例を表示]** 書き出したPDFに凡例を含める場合。
1. クリック **[!UICONTROL 書き出し]**.

   の pdf [!UICONTROL ガントチャート] が作成され、お使いのコンピューターにダウンロードされます。

   書き出されたファイルの下部に凡例が表示されます。 これにより、 [!UICONTROL ガントチャート] タスクリストに含まれる

   例えば、マイルストーンに関連付けられたタスクが 1 つ以上ある場合にのみ、マイルストーンが凡例に表示されます。

   ![gantt_chart_with_updated__limed__legend.png](assets/gantt-chart-with-updated--limited--legend-350x271.png)
