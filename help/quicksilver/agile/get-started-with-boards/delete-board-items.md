---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードからのカードの削除またはアーカイブ
description: ボードからカードを削除すると、そのカードは完全に削除され、復元できません。カードをアーカイブすると、アーカイブに送信され、後でボードに復元できます。
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 67%

---

# ボードからカードを削除またはアーカイブする

ボードからアドホックカードを削除すると、そのカードは完全に削除され、復元できなくなります。 接続されたカードは、削除された後、手動でボードに再度追加できます。

接続されたカードを動的ボードから削除すると、このボードタイプが特定のプロジェクトからすべてのタスクと問題を取り込むため、ボードを更新した際に再び表示されます。 カードを削除するには、接続されたタスクまたはイシューをWorkfront プロジェクトから削除する必要があります。

取り込み列を持つ他のボードタイプから接続されたカードを削除すると、接続されたタスクまたは問題がまだ完了とマークされていない場合、ボードを更新したときにカードが取り込み列に再び表示されます。 取り込み列について詳しくは、[ ボードへの取り込み列の追加 ](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md) を参照してください。

カードをアーカイブすると、アーカイブに送信され、後でボードに復元できます。

アーカイブしたカードが、Workfrontのタスクおよび問題と同期されない。 カードを復元すると、再度同期されます。

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

## ボードからのカードを削除する

{{step1-to-boards}}

1. ボードにアクセスします。詳しくは、[ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. カード上の&#x200B;**[!UICONTROL 詳細]**&#x200B;メニュー![詳細メニュー](assets/more-icon-spectrum.png)をクリックしてから、「**[!UICONTROL 削除]**」を選択します。
1. 確認メッセージで「**[!UICONTROL 削除]**」をクリックします。

## ボードからのカードをアーカイブする

1. ボードにアクセスします。
1. カード上の&#x200B;**[!UICONTROL 詳細]**&#x200B;メニュー![詳細メニュー](assets/more-icon-spectrum.png)をクリックしてから、「**[!UICONTROL アーカイブ]**」を選択します。

   アーカイブしたカードは、表示するフィルターを適用しない限り、ボードに表示されません。詳しくは、[ボードをフィルタリングしてアーカイブされたカードを表示](#filter-a-board-to-show-archived-cards)を参照してください。

   [!UICONTROL アーカイブ]アイコン ![ アーカイブ ](assets/archive-icon-spectrum-25x20.png) は、アーカイブされたカードに表示されます。アーカイブしたカードは編集できませんが、削除したり、別の列に移動したりすることはできます。

1. アーカイブしたカードを復元するには、**[!UICONTROL その他]**&#x200B;メニュー ![ その他のメニュー ](assets/more-icon-spectrum.png) をクリックし、「**[!UICONTROL 復元]**」を選択します。

## ボードをフィルタリングしてアーカイブされたカードを表示する

デフォルトでは、アクティブなカードのみがボードに表示されます。ボードをフィルタリングして、アーカイブしたカードも表示できます。

1. ボードにアクセスします。
1. ボードの右側の「[!UICONTROL **設定**]」をクリックして、設定パネルを開きます。
1. 「[!UICONTROL **カード**]」を展開します。
1. 「[!UICONTROL **ボードにアーカイブされたカードを表示**]」をオンにします。
1. 「[!UICONTROL **フィルター**]」をクリックし、「[!UICONTROL アーカイブされたカード]」セクションを展開して、**[!UICONTROL アーカイブされたカード]**&#x200B;を選択してアーカイブされたカードを表示します。

   フィルターには、アーカイブされたカードの数が表示されます。

   ![アーカイブされたカードをフィルター](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >アーカイブされたカードを表示する設定をオンにしていない場合、「[!UICONTROL アーカイブされたカード]」セクションはフィルターで使用できません。詳しくは、[カードに表示するフィールドのカスタマイズ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)を参照してください。

1. 「**[!UICONTROL アーカイブされたカード]**」を再び選択し、オプションをクリアして、アクティブなカードのみを表示します。
