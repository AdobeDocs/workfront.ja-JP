---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: ボード上の進行中の作業（WIP）の制限の管理
description: ボード上の各列に対して進行中の作業（WIP）の制限を設定できます。
author: Lisa
feature: Agile
exl-id: 7901c6e7-75a4-41e4-b288-d527c4a6d031
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 89%

---

# ボードでの[!UICONTROL 進行中の作業]（WIP）の制限の管理

ボード上の各列に対して[!UICONTROL 進行中の作業]（WIP）の制限を設定できます。

WIP の制限は単に視覚的な警告であり、各列に設定した制限よりも多くの項目が表示されることを制限しません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>投稿者以上</p> 
   <p>リクエスト以上</p>
   </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## WIP の制限を列に設定

{{step1-to-boards}}

1. ボードにアクセスします。詳しくは、[ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. WIP 制限を追加する列を見つけます。

   新しい列を追加するには、[ボード列の管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。

1. 列の&#x200B;**[!UICONTROL 詳細]**&#x200B;メニューをクリックして、「**[!UICONTROL 編集]**」を選択して設定エリアを開きます。
1. [!UICONTROL 列ポリシー]で、**[!UICONTROL 進行中の作業]制限**&#x200B;ポリシーを有効にして、列に追加できるカードの数を制限します。
1. 制限値を「**[!UICONTROL 制限を設定]**」フィールドに入力します。

   ![列の WIP 制限](assets/boards-wip-limit-in-column.png)

   カードの数と制限が列の上部に表示されます。列に制限を超えるカードが含まれている場合、カウンターが赤に変わります。

   ![WIP 制限カウンター](assets/boards-wip-limit-counter.png)

1. 「**[!UICONTROL 閉じる]**」をクリックして[!UICONTROL 設定]エリアを終了し、列とそのカードを表示します。
