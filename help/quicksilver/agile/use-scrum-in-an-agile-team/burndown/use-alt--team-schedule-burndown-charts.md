---
product-area: agile-and-teams
navigation-topic: burndown
title: バーンダウングラフに代替のチームスケジュールを使用
description: で定義されたスケジュール [!DNL Adobe Workfront] は、バーンダウンから休日（週末と休日）を除外することで、バーンダウンチャートに影響を与えます。
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# バーンダウングラフに代替のチームスケジュールを使用

で定義されたスケジュール [!DNL Adobe Workfront] は、バーンダウンから休日（週末と休日）を除外することで、バーンダウンチャートに影響を与えます。

デフォルトでは、バーンダウングラフはデフォルトのスケジュールを使用します。 デフォルトのスケジュールに加えて、アジャイルチームは、チーム固有の非就業日を組み込むために、別のスケジュールを使用することも選択できます。 その後、この代替スケジュールは、チームに割り当てられているイテレーションのバーンダウンチャートに反映されます。 代替スケジュールは、バーンダウンチャートにのみ影響します。 ( デフォルトのスケジュールの詳細と [!DNL Workfront] 管理者は、チーム固有のスケジュールを作成できます。詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

バーンダウンチャートでは、一部の日数は考慮されません。 例えば、チームが金曜日に 4 時間働く場合、バーンダウングラフには 1 日と表示されます。

バーンダウングラフの使用方法の詳細については、 [アジャイルバーンダウンチャートの概要](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランやライセンスの種類を確認するには、 [!DNL Workfront] 管理者。

## バーンダウングラフに代替のチームスケジュールを使用

1. 次を確認します。 [!DNL Workfront] 管理者は、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL チーム]**.

1. （オプション） **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 管理するアジャイルチームを選択します。
1. 次をクリック： **[!UICONTROL 詳細]** メニューから、 **[!UICONTROL 編集]**.

1. 内 **[!UICONTROL アジャイル]** セクション内の **[!UICONTROL スケジュール]** 「 」領域で、ドロップダウンメニューから新しいスケジュールを選択します。

1. クリック **[!UICONTROL 変更を保存]**.
