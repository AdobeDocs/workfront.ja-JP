---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: カードの減少を設定する
description: カードをスケジュールに従ってアーカイブしたり、ボードから外れたりするようにボードを設定できます。
author: Lisa
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '243'
ht-degree: 100%

---

# カードの減少を設定する

カードをスケジュールに従ってアーカイブしたり、ボードから「フォールオフ」したりするようにボードを設定できます。特定の列にカードを設定して、一定の日数または週数でボードから外れるように設定できます。

カードがボードから外れると、そのカードはアーカイブされます。フィルター付きのアーカイブ済みカードを表示できます。詳しくは、[フィルタリングおよびボード内で検索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)を参照してください。

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
   <td> <p>[!UICONTROL Request] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセスを確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## カードの減少を設定する

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![ メインメニュー ](assets/main-menu-icon.png) をクリックして、「**[!UICONTROL ボード]**」をクリックします。
1. ボードにアクセスします。詳しくは、[ボードを作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. ボードの右側の「**[!UICONTROL 設定]**」をクリックして、設定パネルを開きます。
1. 「**[!UICONTROL カード]**」を展開します。
1. **[!UICONTROL ボードからカードを自動的にアーカイブ]**&#x200B;オンにします。

   ![カードの減少設定](assets/card-falloff-switch.png)

1. カードをボードからアーカイブするタイミングを選択します。最大 8 週間または最大 60 日まで選択できます。

   日付は、カードが最後に変更された日から決定されます。

1. カードを削除する列を選択します。
1. 確認メッセージで「**[!UICONTROL 保存]**」をクリックします。
1. 「**[!UICONTROL 設定を非表示]**」をクリックして「[!UICONTROL 設定]」パネルを閉じます。設定は、ボードを更新すると自動的に適用されます。
