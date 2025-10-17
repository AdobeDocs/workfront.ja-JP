---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: カレンダーレポートとイベントの詳細の表示
description: Adobe Workfront で作成または共有したカレンダーレポートおよびイベントの詳細を表示できます。
author: Jenny
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 71%

---

# カレンダーレポートとイベントの詳細を表示

Adobe Workfront で作成または共有したカレンダーレポートおよびイベントの詳細を表示できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>コントリビューター</p>
       <p>リクエスト</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>報告書、ダッシュボード、およびカレンダーへの表示以上のアクセス</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>カレンダーレポートに対する表示以上の権限</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カレンダーレポートの表示

<!--{{step1-to-calendars}}-->

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) をクリックするか、（利用可能であれば）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)、「**[!UICONTROL カレンダー]**」の順にクリックします。

   アクセスレベルに応じて、次のカレンダーが表示される場合があります。

   * 既定の [!DNL Adobe Workfront] カレンダー

     Workfront は、自分に割り当てられているプロジェクト、タスクおよびイシューに基づいて、または自分が割り当てられているチーム、グループまたは役割に基づいて、ユーザー用のカレンダーを作成します。

   * 作成したカレンダー

     カレンダーの作成について詳しくは、[カレンダーレポートの概要](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)を参照してください。

   * 他のユーザーが共有しているカレンダー

     カレンダーの共有については、[[!UICONTROL カレンダーの共有]レポート](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)を参照してください。

1. （条件付き）**[!UICONTROL 表示]**&#x200B;ドロップダウンリストをクリックして、表示するカレンダー期間を選択します。
   ![&#x200B; カレンダー期間 &#x200B;](assets/view-menu-calendar-report-350x189.png)
次のカレンダーレポートビューから選択できます。

   * **[!UICONTROL 月]**：4 週間のカレンダーを表示します
   * **[!UICONTROL 週]**：1 週間のカレンダーを表示します
   * **[!UICONTROL ガント]**：カレンダーの連続したビューを表示します

     下または横にスクロールすると、**ガント** ビューでより多くのイベントを表示できます。 ビューのデータが入力されると、読み込み記号が表示されます。

   >[!NOTE]
   >
   >**月**&#x200B;のビューおよび&#x200B;**週**&#x200B;のビューでは、現在または将来のイベント（今日の日付または将来の日付を含められた複数日にわたるイベントを含む）には、プロジェクトまたはカレンダーグループの色に対応する網掛けが適用されます。過去のイベントの淡色の網掛けで表示され、現在のイベントではないことを示しますが、これらのイベントを選択して表示することはできます。

1. （オプション）カレンダーを&#x200B;**月**&#x200B;のビューまたは&#x200B;**週**&#x200B;のビューで表示する場合、次のオプションを使用してカレンダー表示を変更できます。

   <!--   * To include or exclude weekends:
      1. On the **[!UICONTROL Calendar]** toolbar, click **[!UICONTROL Calendar Actions]**, then from the drop-down list select either **[!UICONTROL Show Weekend]** or **[!UICONTROL Hide Weekend]**.-->

   * 表示される日付をすばやく変更するには、次の手順に従います。

      1. **[!UICONTROL カレンダー]** ツールバーで、日付インジケーターの左矢印をクリックしてカレンダー内に戻るか、右矢印をクリックして前方に移動します。

         ![矢印をクリックして日付を変更](assets/click-arrows-to-change-dates-calendar-report.png)

         表示される日付は、現在のカレンダービューに基づく間隔で調整されます。例えば、**週**&#x200B;のビューでカレンダーを表示している場合、選択した矢印に応じて、1 週間後に進むかまたは 1 週間前に戻った表示になります。

      1. （任意）現在の日付に戻るには、[[!UICONTROL **今日**]] をクリックします。

1. （オプション）カレンダーにリンクされたプロジェクトまたはカレンダーのグループ化のイベントを非表示にするには、プロジェクトリストのプロジェクトまたはカレンダーのグループ化をオフにします。
   ![&#x200B; イベントを非表示 &#x200B;](assets/hide-events-for-project-or-cal-grouping.png)
プロジェクトリストで [!UICONTROL &#x200B; プロジェクト &#x200B;] またはカレンダーのグループ化を選択すると、イベントを再び表示できます。

## カレンダーレポートイベントの詳細を表示

現在のイベントおよび過去のイベントの詳細は、カレンダーに表示されます。

1. 詳細を把握したいイベントに移動し、イベントをクリックします。 詳細は、右側のパネルに開きます。
1. （オプション）関連するプロジェクト、タスクまたはイシューを開くには、オブジェクトのタイトルをクリックします。
