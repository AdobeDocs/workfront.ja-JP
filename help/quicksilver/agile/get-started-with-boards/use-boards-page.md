---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードダッシュボードの使用
description: この [!UICONTROL ボード] 「ダッシュボード」には、自分が作成したボードや追加したボードなど、アクセス権のあるボードの一覧が表示されます。
author: Lisa
feature: Agile
exl-id: bb275f4f-efaf-4dcc-b184-40e015f089b6
source-git-commit: 16e96d55932116cb475eecbe8b6ebfd4661eb494
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# ボードダッシュボードの使用

{{highlighted-preview}}

ボードダッシュボードには、作成したボードや追加したボードを含む、アクセス権のあるボードやワークストリームのリストが表示されます。 アクセス権を持つ個々のボードは、最初にワークストリームに含まれていません。

>[!NOTE]
>
>ワークストリームはプレビュー環境で、実稼動環境では初期の機能オプトインから次のように使用できます。 [!UICONTROL [!DNL Workfront] ボード]. 詳しくは、 [Adobe Workfrontボードの初期機能のオプトイン](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

ダッシュボードでは、ボードとワークストリームに対して次の操作を実行できます。

* ボードのアーカイブ <span class="preview">または workstream</span>
* ボードをフィルター <span class="preview">およびワークストリーム</span>
* ボード名または変更日でボードリストを並べ替え
* ボードまたはワークストリームの検索
* ボードまたはワークストリームの削除

新しいボードの作成や既存のボードの編集について詳しくは、 [ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md). 新しいワークストリームの作成について詳しくは、 [ワークストリームの管理](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL リクエスト ] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## フィルターボード <span class="preview">およびワークストリーム</span> {#filter-boards}

ボードダッシュボードにフィルターを適用して、アクティブなボード、アーカイブされたボード、またはすべてのボードやワークストリームを表示できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. クリック [!UICONTROL **フィルター**] 「ボード」領域または「ワークストリーム」領域で、 **[!UICONTROL すべて]**, **[!UICONTROL アクティブ]**&#x200B;または **[!UICONTROL アーカイブ済み]**.

   デフォルト以外のフィルターがダッシュボードに適用されると、フィルターアイコンにインジケーターが表示されます ![ダッシュボードに適用するフィルター](assets/boards-filterapplied-30x30.png).

## ボードを並べ替え

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. ボードのリストを並べ替えるには、 [!UICONTROL **並べ替え**]. ページのデフォルトの並べ替えオプションは次のとおりです。 **[!UICONTROL 変更日]**. また、ページをボードで並べ替えることもできます **[!UICONTROL 名前]**.

   選択 **[!UICONTROL 逆順]** をクリックして、変更日または名前の逆の順序でボードを並べ替えます。 並べ替えアイコンの矢印が上を向くと、逆順が適用されます。 矢印が下を向くと、標準の順序が適用されます。

   デフォルト以外の並べ替えがダッシュボードに適用されると、並べ替えアイコンにインジケーターが表示されます ![適用された並べ替え](assets/sort-applied-boards.png).

## ボードまたはワークストリームの検索

「ボード」領域で特定のボードを検索したり、「ワークストリーム」領域で特定のワークストリームを検索したりできます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. クリック [!UICONTROL **検索**] 検索語句を入力します。 次に、Enter キーを押します。

   タイトルに検索語を含むすべてのボードまたはワークストリームが表示されます。

   「 X 」をクリックして検索をクリアします。

   ![ダッシュボードでのボードの検索](assets/boards-searchbox.png)

## ボードのアーカイブ <span class="preview">またはワークストリーム</span>

ボードまたはワークストリームをアーカイブすると、アーカイブに送信され、後で復元できます。

>[!NOTE]
>
>ボードをアーカイブすると、そのボードはすべてのボードメンバー用にアーカイブされます。
>
>ワークストリームをアーカイブすると、そのすべてのボードがアーカイブされます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. 次をクリック： **[!UICONTROL 詳細]** メニュー ![その他のメニュー](assets/more-icon-spectrum.png) を選択します。 **[!UICONTROL アーカイブ]**.

   ワークストリームでは、右側のメニューが「 [!UICONTROL **ワークストリームを表示**] 」ボタンをクリックします。

   An [!UICONTROL アーカイブ] アイコン ![アーカイブ](assets/archive-icon-spectrum-25x20.png) は、ボードまたはワークストリームに表示されます。 アーカイブしたボードやワークストリームは編集できません。

   アーカイブした項目は、表示するフィルターを適用しない限り、ボードダッシュボードでは非表示になります。 詳しくは、 [[!UICONTROL フィルターボード]](#filter-boards) 」の節を参照してください。

1. アーカイブされたボードまたはワークストリームを復元するには、 **[!UICONTROL 詳細]** メニュー ![その他のメニューアイコン](assets/more-icon-spectrum.png) を選択します。 **[!UICONTROL 復元]**.

## ボードまたはワークストリームの削除

ボードを削除すると、そのボードは次の場所から永久に削除されます： [!DNL Workfront] 復元することはできません。 ボード上のカードもボードと一緒に削除されます。

ワークストリームを削除すると、ワークストリーム内のすべてのボードも削除されます。

>[!NOTE]
>
>削除できるのは、自分で作成したボードとワークストリームのみで、追加したボードとワークストリームは削除できません。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. 次をクリック： **[!UICONTROL 詳細]** メニュー ![[!UICONTROL その他のメニュー]](assets/more-icon-spectrum.png) を選択します。 **[!UICONTROL 削除]**.

   ワークストリームでは、右側のメニューが「 [!UICONTROL **ワークストリームを表示**] 」ボタンをクリックします。

1. クリック **[!UICONTROL ボードを削除]** または [!UICONTROL **ワークストリームを削除**] をクリックします。

## ワークストリームへのボードの移動

スタンドアロン・ボードをワークストリーム内に移動したり、あるワークストリームから別のワークストリームにボードを移動したりできます。

>[!NOTE]
>
>移動できるのは自分で作成したボードのみで、自分が追加したボードは移動できません。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. 次をクリック： **[!UICONTROL 詳細]** メニュー ![[!UICONTROL その他のメニュー]](assets/more-icon-spectrum.png) を選択し、 [!UICONTROL **ワークストリームに移動**].
1. ボードを追加するワークストリームを選択し、 [!UICONTROL **移動**].

   ボードがワークストリーム内に移動され、 [!UICONTROL ボード] 領域
まだワークストリームを作成していない場合は、ボードを移動するワークストリームを作成するように求められます。
