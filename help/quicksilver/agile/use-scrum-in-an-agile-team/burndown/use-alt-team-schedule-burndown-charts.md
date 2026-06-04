---
product-area: agile-and-teams
navigation-topic: burndown
title: バーンダウンチャートに別のチームスケジュールを使用する
description: ' [!DNL Adobe Workfront]  で定義されたスケジュールは、バーンダウンから休日（週末と祝日）を除外することにより、バーンダウンチャートに影響を与えます。'
author: Courtney
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/BWnnytUMaoygpGpDdjQ5dmdBZrR1IWAu7onkwVizvUc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 304
ht-degree: 86%

---

# バーンダウンチャートに代替のチームスケジュールを使用

[!DNL Adobe Workfront] で定義されたスケジュールは、バーンダウンから休日（週末と祝日）を除外することにより、バーンダウンチャートに影響を与えます。

デフォルトでは、バーンダウンチャートはデフォルトのスケジュールを使用します。 アジャイルチームは、デフォルトのスケジュールに加えて、チーム固有の非稼働日を組み込むために、代替スケジュールを使用することもできます。 この代替スケジュールは、チームに割り当てられたイテレーションのバーンダウンチャートに反映されます。 代替スケジュールは、バーンダウンチャートにのみ影響します。 （デフォルトのスケジュールと、[!DNL Workfront] 管理者がチーム固有のスケジュールを作成する方法について詳しくは、[スケジュールを作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。）

バーンダウンチャートでは、半日は考慮されません。 例えば、チームが毎週金曜日に 4 時間働く場合、バーンダウンチャートでは丸 1 日として表されます。

バーンダウンチャートの使用方法について詳しくは、[アジャイルバーンダウンチャートの概要](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)を参照してください。

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
   <td> <p>標準</p> 
   <p>Work またはそれ以上</p> </td> 
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## バーンダウンチャートに代替のチームスケジュールを使用

1. [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)の説明に従って、[!DNL Workfront] 管理者が代替スケジュールをすでに作成していることを確認してください。

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 管理するアジャイルチームを選択します。
1. **[!UICONTROL その他]**&#x200B;メニューをクリックして、「**[!UICONTROL 編集]**」を選択します。

1. 「**[!UICONTROL アジャイル]**」セクションの&#x200B;**[!UICONTROL スケジュール]**&#x200B;領域で、ドロップダウンメニューから新しいスケジュールを選択します。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
