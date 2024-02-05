---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: カードリストを使用
description: ワークストリーム上にカードリストを作成し、カードをイテレーションに追加できます。
author: Lisa
feature: Agile
exl-id: 2976f7e8-be84-4d27-9d70-8430392d5331
source-git-commit: d44eb048103e469bc072cc5287947fea471668b3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 98%

---

# カードリストを使用

>[!IMPORTANT]
>
>一部のお客様は、ワークストリームを利用できません。

ワークストリーム上にカードリストを作成し、カードをイテレーションに追加できます。

カードリストは、ワークストリームの作業のバックログとして機能できます。

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

## カードリストにカードを追加

{{step1-to-boards}}

1. ワークストリームを開くには、[!UICONTROL **ワークストリームを表示**]&#x200B;をクリックします。
1. 「[!UICONTROL **カードリスト**]」タブをクリックします。
1. 「[!UICONTROL **カードを追加**]」をクリックします。
1. [!UICONTROL **カードを作成／編集**]&#x200B;ダイアログで、次の情報を追加します。

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Name]</strong></td> 
      <td>カードの名前。</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Description]</strong></td> 
      <td>カードの説明。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Estimation]</strong></td> 
      <td>カードが完了するまでの推定時間数。これは手動のエントリのみです。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Status]</strong></td> 
      <td>カードのステータスを選択します。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Iterations]</strong></td> 
      <td>カードを割り当てるイテレーションを選択します。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Assignees]</strong></td> 
      <td><p>カードを割り当てるには、検索フィールドに名前を入力していき、リストに候補が表示されたら選択します。個人とチームの両方を追加し、1 つのカードに複数のユーザーまたはチームを割り当てることができます。</p><p>担当者はワークストリームのメンバーである必要があります。メンバーでない場合は、選択リストに表示されません。</p></td> 
     </tr>
    </tbody> 
   </table>

1. 「[!UICONTROL **保存**]」をクリックします。
1. カードリストを作成するまで、カードの追加を続行します。

## カードを表示

ワークストリームのすべてのカードを 1 つのリストに表示するには、「カードリスト」タブの「[!UICONTROL **リスト表示**]」をクリックします。

イテレーションごとにグループ化されたワークストリームのすべてのカードを表示するには、「[!UICONTROL **イテレーション表示**]」をクリックします。予定外のカードは、独自のグループに表示されます。

既存のカードを編集するには、リストからカードを選択し、「[!UICONTROL **編集**]」をクリックします。

カードを削除するには、リストからカードを選択し、「[!UICONTROL **削除**]」をクリックします。

### カードをフィルター

カードは、イテレーションボードからのみアーカイブできます。 カードをアーカイブすると、フィルターを適用してアーカイブされたカードを表示しない限り、カードはカードリストに表示されません。カードのアーカイブについて詳しくは、[ボードからのカードを削除またはアーカイブ](/help/quicksilver/agile/get-started-with-boards/delete-board-items.md)を参照してください。

1. ワークストリームのカードリストにアクセスします。
1. 「[!UICONTROL **フィルター**]」をクリックし、「[!UICONTROL **すべて**]」、「[!UICONTROL **アクティブなカード**]」、「[!UICONTROL **アーカイブ済みカード**]」から選択します。

   デフォルト以外のフィルターがカードリストに適用されている場合、![フィルターが適用された](assets/boards-filterapplied-30x30.png)フィルター アイコンにインジケーターが表示されます。

### カードリストでの検索

1. ワークストリームのカードリストにアクセスします。
1. 「[!UICONTROL **検索**]」をクリックし、検索語を入力します。 次に、Enter キーを押します。

   検索語を含むすべてのカードが表示されます。
「 X 」をクリックして検索をクリアします。

   ![ボード内のカードを検索](assets/boards-searchbox.png)

## カードをイテレーションに追加

>[!NOTE]
>
>カードを追加する前に、イテレーションを作成する必要があります。 詳しくは、[ワークストリームでイテレーションを作成](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)を参照してください。

1. ワークストリームのカードリストにアクセスします。
1. 「[!UICONTROL **イテレーション表示**]」を選択して、どのカードがイテレーションに割り当てられているか、どのカードが予定外であるかを確認します。
1. リストから予定外のカードを選択し、「[!UICONTROL **編集**]」をクリックします。
1. 「[!UICONTROL **イテレーション**]」フィールドでイテレーションを選択します。
1. ストーリーポイントを使用する場合は、「[!UICONTROL **推定**]」フィールドに値を入力します。
1. 「[!UICONTROL **保存**]」をクリックします。

   カードはイテレーションに移動し、イテレーション指標はカード数とポイント数を反映します。

   また、予定外のカードグループからイテレーションにカードをドラッグ＆ドロップするか、「[!UICONTROL **カードを追加**]」をクリックして、新しいカードをイテレーションに追加します。

>[!TIP]
>
>イテレーションプロセスボードを作成した場合は、カードリストの予定外のカードはすべて[!UICONTROL バックログ]列に表示されます。別の列に移動されたカードはアクティブなイテレーションの一部になります。カードリストでイテレーションに追加するカードは、ステータスに基づいて列に追加されます。
