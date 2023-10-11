---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: ワークストリームでの反復の作成
description: 繰り返しとは、作業の完了に必要な一定時間のことです。 アジャイルチームの中には、反復をスプリントと呼ぶものもあります。
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 1%

---

# ワークストリームでの反復の作成

>[!IMPORTANT]
>
>ワークストリームは、特定の顧客グループのみが使用できます。

繰り返しとは、作業の完了に必要な一定時間のことです。 アジャイルチームの中には、反復をスプリントと呼ぶものもあります。

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

## ワークストリームでの反復の作成

{{step1-to-boards}}

1. 繰り返しを追加するワークストリームを開きます。 ワークストリームを開くには、 [!UICONTROL **ワークストリームを表示**].
1. 次のいずれかの方法を使用して、反復を作成します。

   * [ カード一覧 ] タブの反復表示で、 [!UICONTROL **反復を作成**].
   * [ カード一覧 ] タブの一覧表示で、 [!UICONTROL **反復を作成**].
   * 「ボード」タブで、 [!UICONTROL **ボードを追加**] を選択し、 [!UICONTROL **反復処理**] をボードテンプレートとして使用します。 次に、イテレーションボードを開き、 [!UICONTROL **繰り返しの設定**].

1. [ 反復詳細 ] ダイアログで、次の情報を追加します。

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL 反復名 ]</strong></td> 
      <td>繰り返しの名前（「Sprint 1」など）。</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL 反復の長さ ]</strong></td> 
      <td>反復の長さ（日、週、月）。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL 開始日 ]</strong></td> 
      <td>繰り返しが開始される日付。 終了日は、繰り返しの長さに基づいて自動的に入力されます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「[!UICONTROL **保存**]」をクリックします。

   これで、カードリストの反復表示と、反復ボードの指標領域に反復が表示されます。

   カードをイテレーションに追加するには、 [カードリストを使用](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

## 既存の反復を編集

1. ワークストリームを開くには、 [!UICONTROL **ワークストリームを表示**].
1. 次のいずれかの方法で繰り返しを開きます。

   * [ カード一覧 ] タブの反復表示で、 [!UICONTROL **反復の詳細**] アイコン ![反復の詳細](assets/iteration-details-button.png).
   * イテレーションボードで、 [!UICONTROL **反復の詳細**] アイコン ![反復の詳細](assets/iteration-details-button.png) 」と表示されます。

1. Adobe Analytics の [!UICONTROL 反復設定] パネルで、必要に応じてイテレーションを編集します。
1. イテレーション名を変更するには、を展開します。 [!UICONTROL **反復の詳細**].

   イテレーションが開始された後は、イテレーション名のみを変更でき、日付やイテレーションの長さは変更できません。

<!--   

1. <span class="preview">To add goals to the iteration, expand [!UICONTROL **Goals**].</span>
1. <span class="preview">Click [!UICONTROL **Add goal**], and type the goal name.</span>

   <span class="preview">As goals are completed during the iteration, you can select the check box to mark them complete, or click the **Delete** icon ![Delete icon](assets/delete.png) to delete a goal. The metrics area on the top right of the iteration shows how many goals exist and how many have been completed.</span>

<div class="preview">

## Assign cards to the next iteration

Use the [!UICONTROL Next Iteration] column to move cards from the current iteration to the next iteration, without sending them to the backlog first.

1. Move a card to the [!UICONTROL **Next Iteration**] column, or add a new card directly in the column.
1. Access the next iteration by clicking the [!UICONTROL **Next Iteration**] column title, or by clicking the up-pointing arrow next to the iteration name on the top of the screen.

   The cards that you marked to come over to the next iteration are placed in the columns that correspond with their status.

</div>
-->

## 繰り返しの削除

1. 次をクリック： [!UICONTROL **カードリスト**] 」タブをクリックし、イテレーションビューを開きます。
1. 次をクリック： **削除** アイコン ![削除アイコン](assets/delete.png) をクリックします。
1. クリック [!UICONTROL **繰り返しを削除**] をクリックします。
