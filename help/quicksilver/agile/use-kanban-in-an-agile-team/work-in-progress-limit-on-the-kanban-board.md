---
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: かんばんボード上の進行中の作業（WIP）制限の管理
description: かんばんボードの各列に対して、進行中の作業（WIP）の上限を設定できます。WIP の上限は視覚的に警告が表示されるだけで、各ステータス列の項目が設定した上限より多くならないよう制限するものではありません。
author: Lisa
feature: Agile
exl-id: 540880ad-46af-416b-8e0b-5df869555424
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 85%

---

# かんばんボードでの[!UICONTROL 進行中の作業]（WIP）の上限の管理

[かんばんの設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)の記事で説明されているように、[!UICONTROL かんばん]ボードの各列に対し、[!UICONTROL 進行中の作業]（WIP）の上限を設定できます。

WIP の上限は視覚的に警告が表示されるだけで、各ステータス列の項目が設定した上限より多くならないよう制限するものではありません。

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
   <p>ワークまたはそれ以上</p> </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!UICONTROL かんばん]ボードで[!UICONTROL 進行中の作業]（WIP）の上限を表示

アジャイルチームに WIP の上限を設定すると、かんばんボードの各列（[!UICONTROL 完了]」列以外）の右上隅に WIP の上限が表示されます。

[!UICONTROL  かんばん ] ボード上のいずれかの列の上限を超えると、上限が赤でハイライト表示され、メッセージが表示されます。
![WIP の上限](assets/kanban-wip.png)

## [!UICONTROL かんばん]ボードで[!UICONTROL 進行中の作業]（WIP）の上限を更新

[!UICONTROL 編集]権限を持つチームメンバーは、[!UICONTROL かんばん]ボードで直接、各ステータス列の WIP の上限を更新できます。あるいは、[かんばんの設定](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)の記事の説明に従って WIP の上限を更新することもできます。

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、新しい[!UICONTROL かんばん]チームをドロップダウンメニューから選択するか、検索バーでチームを検索します。

1. [!UICONTROL かんばん]ボードで、かんばんボードの各列の右上隅にある WIP 上限を検索します。
1. 変更する WIP の上限をクリックし、新しい上限を指定します。
1. **[!UICONTROL Enter]** を押します。
