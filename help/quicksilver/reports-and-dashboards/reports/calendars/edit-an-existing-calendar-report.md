---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 既存のカレンダーレポートの編集
description: プロジェクトへのリンクを追加または削除することで、既存のカレンダーを変更できます。また、カレンダーレポートに関連付けられているカレンダーのグループ化を変更することもできます。
author: Lisa
feature: Reports and Dashboards
exl-id: 494d040c-bd1d-4356-824f-a75890803617
source-git-commit: c8f4d8e460ed9247ca5d89c9a711ecb1ec5ed1e9
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 61%

---

# 既存のカレンダーレポートの編集

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

プロジェクトへのリンクを追加または削除することで、既存のカレンダーを変更できます。また、カレンダーレポートに関連付けられているカレンダーのグループ化を変更することもできます。

>[!NOTE]
>
>1 つのカレンダーレポートで使用できるグループは 15 個までです。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!UICONTROL Reports]、[!UICONTROL Dashboards]、および[!UICONTROL Calendars]に対する[!UICONTROL Edit]アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>カレンダーレポートに対する [!UICONTROL Manage] 権限</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 実稼動環境での既存のカレンダーレポートの編集

{{step1-to-calendars}}

1. （オプション）カレンダーレポートの名前を変更するには、「[!UICONTROL  カレンダー名 ]」フィールドをクリックして必要な変更を行います。 互換性の問題を回避するには、UTF-8 文字のみを使用することをお勧めします。

   ![レポート名の変更](assets/titlechange-250x230.png)

   カレンダーレポートを他のユーザーやチームと共有している場合は、変更したカレンダー名が自動的に共有相手のカレンダービューに反映されます。

1. （オプション）カレンダーレポートにプロジェクトを追加するには、次の手順に従います。

   1. 「**[!UICONTROL カレンダーに追加]」をクリックします。**
   1. 「**[!UICONTROL プロジェクト名]**」フィールドに、カレンダーイベントを追加するプロジェクトの名前の入力を開始し、ドロップダウンリストに表示される名前をクリックします。

      ![プロジェクト名を選択](assets/calendar-project-name.png)
プロジェクトのアイテムとそれに関連するタスクおよびイシューがカレンダーレポートに追加されます。

1. （オプション）カレンダーのグループ化を追加するか、カレンダーの既存のグループ化を変更するには、次の手順に従います。

   1. プロジェクト名にポインタを合わせ、プロジェクト名の横のドロップダウン矢印をクリックして、「**[!UICONTROL 編集]**」をクリックします。

      ![カレンダーのグループ化の編集](assets/editcalendergroup-350x126.png)

   1. アイテムをグループ化する方法を次の中から選択します。

      * [カレンダーレポートでの[!UICONTROL 予定日]の使用](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
      * [カレンダーレポートで[!UICONTROL 見込み日]を使用](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
      * [カレンダーレポートでのカスタム日付フィールドの使用](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)


<div class="preview">

## プレビューで既存のカレンダーレポートを編集する

{{step1-to-calendars}}

1. （オプション）カレンダーレポートの名前を変更するには、**詳細** メニューをクリックして **編集** を選択します。
   ![ その他メニュー ](assets/new-more-menu-calendar.png)
他のユーザーやチームとカレンダーレポートを共有した場合、変更されたカレンダー名はカレンダー表示で自動的に更新されます。

1. （オプション）カレンダーレポートにプロジェクトを追加するには、次の手順に従います。
   1. 「**[!UICONTROL カレンダーに追加]」をクリックします。**
   1. カレンダーイベントを追加するプロジェクトの名前の入力を開始し、ドロップダウンリストに表示されたら名前をクリックします。
   1. 「**追加**」をクリックします。
      ![ カレンダーへのプロジェクトの追加 ](assets/add-a-calendar-project.png)


1. （オプション）カレンダーのグループ化を追加するか、カレンダーの既存のグループ化を変更するには、次の手順に従います。
   1. プロジェクト名の横にある **詳細** メニューをクリックし、「**編集**」をクリックします。
      ![ カレンダーでプロジェクトを編集 ](assets/edit-project-in-calendar.png)e

   1. アイテムをグループ化する方法を次の中から選択します。

      * [カレンダーレポートでの[!UICONTROL 予定日]の使用](../../../reports-and-dashboards/reports/calendars/use-planned-dates.md)
      * [カレンダーレポートで[!UICONTROL 見込み日]を使用](../../../reports-and-dashboards/reports/calendars/use-projected-dates.md)
      * [カレンダーレポートでのカスタム日付フィールドの使用](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md)


      </div>