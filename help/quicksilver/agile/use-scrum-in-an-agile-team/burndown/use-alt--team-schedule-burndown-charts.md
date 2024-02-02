---
product-area: agile-and-teams
navigation-topic: burndown
title: バーンダウンチャートに代替のチームスケジュールを使用
description: ' [!DNL Adobe Workfront]  で定義されたスケジュールは、バーンダウンから休日（週末と祝日）を除外することにより、バーンダウンチャートに影響を与えます。'
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: ht
source-wordcount: '314'
ht-degree: 100%

---

# バーンダウンチャートに代替のチームスケジュールを使用

[!DNL Adobe Workfront] で定義されたスケジュールは、バーンダウンから休日（週末と祝日）を除外することにより、バーンダウンチャートに影響を与えます。

デフォルトでは、バーンダウンチャートはデフォルトのスケジュールを使用します。アジャイルチームは、デフォルトのスケジュールに加えて、チーム固有の非稼働日を組み込むために代替スケジュールを使用することも選択できます。この代替スケジュールは、チームに割り当てられたイテレーションのバーンダウンチャートに反映されます。代替スケジュールは、バーンダウンチャートにのみ影響します。（デフォルトのスケジュールと、[!DNL Workfront] 管理者がチーム固有のスケジュールを作成する方法について詳しくは、[スケジュールを作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。）

バーンダウンチャートでは、半日は考慮されません。例えば、チームが毎週金曜日に 4 時間働く場合、バーンダウンチャートでは丸 1 日として表されます。

バーンダウンチャートの使用方法について詳しくは、[アジャイルバーンダウンチャートの概要](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランやライセンスの種類を確認するには、管理者に連絡[!DNL Workfront]してください。

## バーンダウンチャートに代替のチームスケジュールを使用

1. [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)の説明に従って、[!DNL Workfront] 管理者が代替スケジュールをすでに作成していることを確認してください。
1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**[!UICONTROL ボード]**」の順にクリックします。

1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームの切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 管理するアジャイルチームを選択します。
1. **[!UICONTROL 詳細]**&#x200B;メニューをクリックして、「**[!UICONTROL 編集]**」を選択します。

1. 「**[!UICONTROL アジャイル]**」セクションの&#x200B;**[!UICONTROL スケジュール]**&#x200B;領域で、ドロップダウンメニューから新しいスケジュールを選択します。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
