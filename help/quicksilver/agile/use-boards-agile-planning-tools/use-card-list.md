---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: カードリストを使用
description: ワークストリーム上にカードリストを作成し、カードを繰り返しに追加できます。
author: Lisa
feature: Agile
source-git-commit: 8c02f5364154bdc343512416d0c7e38ef563a170
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---

# カードリストを使用

ワークストリーム上にカードリストを作成し、カードを繰り返しに追加できます。

カードリストは、ワークストリームの作業のバックログとして機能することができます。

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
   <td> <p>[!UICONTROL リクエスト ] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

## カードリストへのカードの追加

{{step1-to-boards}}

1. ワークストリームを開くには、 [!UICONTROL **ワークストリームを表示**].
1. 次をクリック： [!UICONTROL **カードリスト**] タブをクリックします。
1. クリック [!UICONTROL **カードを追加**].
1. 内 [!UICONTROL **カードを作成/編集**] ダイアログで、次の情報を追加します。

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL 名前 ]</strong></td> 
      <td>カードの名前。</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL 説明 ]</strong></td> 
      <td>カードの説明。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 推定 ]</strong></td> 
      <td>カードが完了するまでの推定時間数。 これは手動のエントリのみです。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL ステータス ]</strong></td> 
      <td>カードのステータスを選択します。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 反復 ]</strong></td> 
      <td>カードを割り当てる反復を選択します。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 担当者 ]</strong></td> 
      <td><p>カードを割り当てるには、検索フィールドに名前を入力し始め、カードがリストに表示されたら選択します。 個人とチームの両方を追加し、1 つのカードに複数の人またはチームを割り当てることができます。</p><p>割り当て先は、ワークストリーム上のメンバーである必要があります。メンバーでない場合、選択リストに表示されません。</p></td> 
     </tr>
    </tbody> 
   </table>

1. 「[!UICONTROL **保存**]」をクリックします。
1. カードリストを作成するまで、引き続きカードを追加します。

## カードを表示

ワークストリームのすべてのカードを 1 つのリストに表示するには、 [!UICONTROL **リスト表示**] 」をクリックします。

繰り返しごとにグループ化されたワークストリームのすべてのカードを表示するには、 [!UICONTROL **反復表示**]. 計画外のカードは、それぞれのグループに表示されます。

既存のカードを編集するには、リストからカードを選択し、 [!UICONTROL **編集**].

カードを削除するには、リストでカードを選択し、 [!UICONTROL **削除**].

### カードをフィルター

カードは、イテレーションボードからのみアーカイブできます。 カードをアーカイブすると、フィルターを適用してアーカイブされたカードを表示しない限り、カードはカードリストに表示されません。 カードのアーカイブについて詳しくは、 [ボードからのカードの削除またはアーカイブ](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md).

1. ワークストリームのカードリストにアクセスします。
1. クリック [!UICONTROL **フィルター**] を選択し、 [!UICONTROL **すべて**], [!UICONTROL **アクティブなカード**]&#x200B;または [!UICONTROL **アーカイブしたカード**].

   デフォルト以外のフィルターがカードリストに適用されると、フィルターアイコンにインジケーターが表示されます ![適用されたフィルター](assets/boards-filterapplied-30x30.png).

### カードリストでの検索

1. ワークストリームのカードリストにアクセスします。
1. クリック [!UICONTROL **検索**] 検索語句を入力します。 次に、Enter キーを押します。

   検索語句を含むすべてのカードが表示されます。
「 X 」をクリックして検索をクリアします。

   ![ボード内のカードの検索](assets/boards-searchbox.png)

## カードを反復に追加

>[!NOTE]
>
>カードを追加する前に、イテレーションを作成する必要があります。 詳しくは、 [ワークストリームでの反復の作成](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. ワークストリームのカードリストにアクセスします。
1. を選択します。 [!UICONTROL **反復表示**] を使用して、反復に割り当てられているカードと予期しないカードを確認します。
1. リストから予期しないカードを選択し、 [!UICONTROL **編集**].
1. でイテレーションを選択 [!UICONTROL **反復**] フィールドに入力します。
1. ストーリーポイントを使用する場合は、 [!UICONTROL **推定**] フィールドに入力します。
1. 「[!UICONTROL **保存**]」をクリックします。

   カードは反復に移動し、反復指標はカード数とポイント数を反映します。

   また、予期しないカードグループからイテレーションにカードをドラッグ&amp;ドロップするか、 [!UICONTROL **カードを追加**] をクリックして、新しいカードをイテレーションに追加します。

>[!TIP]
>
>イテレーションプロセスボードを作成した場合は、カードリストの予期しないカードがすべてに [!UICONTROL バックログ] 列。 カードが別の列に移動すると、そのカードはアクティブな反復の一部になります。 カードリストで繰り返しに追加するカードは、ステータスに基づいて列に追加されます。

