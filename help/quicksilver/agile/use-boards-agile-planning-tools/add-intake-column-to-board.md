---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: ボードへの取り込み列の追加
description: オプションで、タスクとイシューが Workfront に追加されると、定義したフィルターに基づいて、接続されたカードとしてタスクとイシューを自動的に取り込み列をボードに追加できます。
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 0c0c1f538cfd12e18c504fcb42ee424789d1cde8
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 86%

---

# ボードへの取り込み列の追加

オプションで、タスクとイシューが [!DNL Workfront] に追加されると、定義したフィルターに基づいて、接続されたカードとしてタスクとイシューを自動的に取り込み列をボードに追加できます。取り込み列は、かんばんチームのバックログ列として、サポートチームがリクエストキューに追加されたイシューを確認するための取り込み場所として、またはその他の必要な目的として機能します。

1 つのボード上で許可される取り込み列は 1 つだけで、常に一番左の列として表示されます。

取り込み列は、動的ボードでは使用できません。 ただし、動的なボードに取り込むカードを定義するフィルターを更新できます。 動的ボードでこれらのフィルターを変更すると、Workfrontのタスクやイシューに含まれていないカード設定（タグなど）はリセットされます。

>[!NOTE]
>
>セキュリティ上の理由から、設定パネルでボードフィルターを変更できるのはボードの所有者のみです。

取り込み列は、300 タスクと 300 イシューに制限されます。取り込み列の項目のデフォルトの順序は次のとおりです。

タスク：

* プライマリの順序：プロジェクト名
* セカンダリの順序：作業分類構造

イシュー：

* プライマリの順序：プロジェクト名
* セカンダリの順序：参照番号

>[!IMPORTANT]
>
>複数のユーザーがボードで同時に作業している場合は、ボードを頻繁に更新することをお勧めします。 ページを更新すると、ボード上の視覚的な変更を最新の状態に保つことができ、重複カードが取り込み列からボードに移動されるなどの問題を防ぐことができます。
>
>Workfrontと同期し、新しいタスクや問題をボードまたは取り込み列に追加するには、ボード名の横にある **[!UICONTROL 詳細]** メニュー ![[!UICONTROL &#x200B; 詳細メニュー &#x200B;]](assets/more-icon-spectrum.png) をクリックし、**[!UICONTROL 接続済み項目を同期]** を選択します。

列について詳しくは、[ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。接続されたカードについて詳しくは、[ボードで接続済みカードを使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> 
   <p>新規：[!UICONTROL Contributor]以上</p> 
   <p>または</p>
   <p>現在：[!UICONTROL Request] 以上</p>
   </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## シンプルなフィルターを使用して取り込み列を作成する

{{step1-to-boards}}

1. ボードにアクセスします。詳しくは、[ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. ボードの右側の「**[!UICONTROL 設定]**」をクリックして、設定パネルを開きます。
1. 「**[!UICONTROL ボード]**」を展開します。
1. **[!UICONTROL ボードに項目を動的に取り込む]**&#x200B;をオンにします。

   ![取り込み列のシンプルフィルターオプション](assets/intake-column-simple-filters.png)

   取り込み列は、ボードの左側に追加されます。フィルターを適用するまで空白のままです。

1. （オプション）[!DNL Workfront] [!UICONTROL **プロジェクト**]&#x200B;を検索して選択します。
1. （オプション）ユーザーまたはチーム&#x200B;[!UICONTROL **割り当て**]&#x200B;を検索して選択します。
1. 「[!UICONTROL **完了した作業を含める**]」を選択すると、取り込み列に完了ステータスのタスクとイシューが表示されます。

   >[!NOTE]
   >
   >このオプションを選択しない場合、他のステータスのカードが完了とマークされると、そのカードはボードから「外れ」、表示されなくなります。

1. 「[!UICONTROL **適用**]」をクリックします。

   すべてのオブジェクトは、接続されたカードとしてボード取り込み列に表示されます。

   ![取り込み列](assets/intake-column-added3.png)

## 詳細フィルターを使用して取り込み列を作成する

{{step1-to-boards}}

1. ボードにアクセスします。詳しくは、[ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. ボードの右側の「**[!UICONTROL 設定]**」をクリックして、設定パネルを開きます。
1. 「**[!UICONTROL ボード]**」を展開します。
1. **[!UICONTROL ボードに項目を動的に取り込む]**&#x200B;をオンにします。

   取り込み列は、ボードの左側に追加されます。フィルターを適用するまで空白のままです。

1. 「[!UICONTROL **詳細フィルターを使用**]」をクリックします。
1. 「**[!UICONTROL フィルターソースを追加]**」をクリックし、「**[!UICONTROL タスク]**」または「**[!UICONTROL イシュー]**」を選択します。

   ![取り込み列の詳細フィルターオプション](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >取り込み列をフィルタリングして、タスクとイシューの両方を含めることができますが、オブジェクトタイプごとに個別にフィルターを設定する必要があります。
   >
   >また、保存済みフィルターとシステムのデフォルトフィルターを選択することもできます。

1. フィルターパネルで、「**[!UICONTROL 新規フィルター]**」をクリックして開始します。

   ![「新しいフィルター」をクリック](assets/intake-filter-dialog5.png)

1. フィルターを作成して、「**[!UICONTROL 新規として保存]**」をクリックします。

   ![フィルタービルダー](assets/intake-filter-dialog6.png)

   この例は、ステータスが[!UICONTROL 新規]または[!UICONTROL 処理中]である特定のプロジェクトのタスクのフィルターを示しています。

   >[!NOTE]
   >
   >ログインユーザーのタスクやイシューが常に表示されるとは限らないので、ボードフィルターでは「自分」（ログインユーザー）ワイルドカードを使用しないことをお勧めします。ボードに正しいタスクとイシューを設定したら、ボードをフィルタリングして特定の割り当て先のアイテムを表示できます。詳しくは、[フィルタリングおよびボード内で検索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)を参照してください。

   フィルターの作成について詳しくは、[ [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md) でのフィルターの作成または編集の記事の「標準ビルダーでのフィルターの作成または編集」の節を参照してください。

1. フィルターに名前を付け、「**[!UICONTROL 保存]**」をクリックします。

   ![フィルターへの名前の入力](assets/intake-filter-dialog7.png)

   フィルターに一意の名前を付けると、後で検索できます。

1. 保存されたフィルターのリストにフィルターが表示され、自動的に取り込み列に適用されます。フィルターパネルの上部にある「X」をクリックして閉じます。

   ![保存済みフィルター](assets/intake-filter-dialog8.png)

1. （オプション）フィルターを他のユーザーと共有するには、保存されているフィルターにポインタを合わせて、**[!UICONTROL その他]** メニュー ![その他のメニューアイコン](assets/more-icon-spectrum.png) をクリックし、「**[!UICONTROL 共有]**」を選択します。「フィルター共有」ボックスで、共有するユーザーまたはチームを選択します。詳しくは、[フィルター、ビュー、グループ化の共有](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)を参照してください。
1. （オプション）取り込み条件の列にタスクとイシューの両方を含めるには、**[!UICONTROL ソースをフィルター]**&#x200B;をクリックし、他のオブジェクトを選択して別のフィルターを作成します。
1. フィルターの追加が完了したら、取り込み列を確認して、正しいタスクとイシューが表示されることを確認します。

   ![取り込み列](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >フィルターは、設定パネルを開き、「**[!UICONTROL ソースをフィルター]**」をクリックし、「**[!UICONTROL タスク]**」または「**[!UICONTROL イシュー]**」を選択することで、いつでも更新できます。

## 取り込み列の使用

取り込み列のカードは、他のボード列に移動するまで編集できません。カードをクリックして読み取り専用ビューで開くか、「![タスクまたはイシューを開く](assets/boards-launch-icon.png)」をクリックして、タスクまたはイシューを新しいブラウザータブで開きます。

取り込み列の項目は、手動で並べ替えることができます。

取り込み列の右上にあるアイコンは、現在列にあるカードの数と、適用されているフィルターの数を示します。

1. （オプション）取り込み列で項目を検索するには、列の![検索アイコン](assets/search-icon.png)をクリックします。
1. （オプション）取り込み列から別の列にカードを移動するには、カードを表示したい位置にドラッグ&amp;ドロップします。

   または

   カード上の&#x200B;**[!UICONTROL 詳細]**&#x200B;メニュー ![詳細メニュー](assets/more-icon-spectrum.png) をクリックしてから、「**[!UICONTROL 移動]**」を選択します。次に、「**[!UICONTROL 項目の移動]**」ボックスで、別の列を選択し、「**[!UICONTROL 移動]**」を選択します。

1. （オプション）取り込み列を削除するには、**[!UICONTROL その他]**&#x200B;メニュー ![その他のメニューアイコン](assets/more-icon-spectrum.png) を選択し、「**[!UICONTROL 削除]**」を選択します。
