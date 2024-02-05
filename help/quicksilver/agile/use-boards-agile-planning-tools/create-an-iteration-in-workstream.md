---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: ワークストリームでイテレーションを作成
description: イテレーションとは、作業の完了のために予約された一定時間のことです。アジャイルチームでは、イテレーションをスプリントと呼ぶ場合もあります。
author: Lisa
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 97%

---

# ワークストリームでイテレーションを作成

>[!IMPORTANT]
>
>ワークストリームは、特定の顧客グループのみが使用できます。

イテレーションとは、作業の完了のために予約された一定時間のことです。アジャイルチームでは、イテレーションをスプリントと呼ぶ場合もあります。

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

## ワークストリームでイテレーションを作成

{{step1-to-boards}}

1. イテレーションを追加するワークストリームを開きます。ワークストリームを開くには、[!UICONTROL **ワークストリームを表示**]&#x200B;をクリックします。
1. 次のいずれかの方法を使用して、イテレーションを作成します。

   * イテレーションビューの「カードリスト」タブで、「[!UICONTROL **イテレーションを作成**]」をクリックします。
   * リストビューの「カードリスト」タブで、「[!UICONTROL **イテレーションを作成**]」をクリックします。
   * 「ボード」タブで、「[!UICONTROL **ボードを追加**]」をクリックし、「[!UICONTROL **イテレーションプロセス**]」をボードテンプレートとして選択します。次に、イテレーションボードを開き、「[!UICONTROL **イテレーションを設定**]」をクリックします。

1. イテレーションの詳細ダイアログで、次の情報を追加します。

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td><strong>[!UICONTROL Iteration name]</strong></td> 
      <td>イテレーションの名前（「Sprint 1」など）。</td> 
     </tr> 
     <tr> 
      <td><strong>[!UICONTROL Iteration length]</strong></td> 
      <td>イテレーションの長さ（日、週、月）。</td> 
     </tr>
     <tr> 
      <td><strong>[!UICONTROL Start date]</strong></td> 
      <td>イテレーションが開始される日付。終了日は、イテレーションの長さに基づいて自動的に入力されます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「[!UICONTROL **保存**]」をクリックします。

   これでイテレーションが、カードリストのイテレーションビューと、イテレーションボードの指標領域に表示されます。

   イテレーションにカードを追加するには、[カードリストを使用](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)を参照してください。

## 既存のイテレーションを編集

1. ワークストリームを開くには、「[!UICONTROL **ワークストリームを表示**]」をクリックします。
1. 次のいずれかの方法で、イテレーションを開きます。

   * イテレーションビューの「カードリスト」タブで、[!UICONTROL **イテレーションの詳細**]&#x200B;アイコン ![イテレーションの詳細](assets/iteration-details-button.png) をクリックします。
   * イテレーションボードで、右上の指標領域に表示される&#x200B;[!UICONTROL **イテレーションの詳細**]&#x200B;アイコン ![イテレーションの詳細](assets/iteration-details-button.png) をクリックします。

1. [!UICONTROL イテレーション設定]パネルで、必要に応じてイテレーションを編集します。
1. イテレーション名を変更するには、「[!UICONTROL **イテレーションの詳細**]」を展開します。

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

## イテレーションを削除

1. ワークストリームの「[!UICONTROL **カードリスト**]」タブをクリックし、イテレーションビューを開きます。
1. イテレーションの横にある&#x200B;**削除**&#x200B;アイコン ![削除アイコン](assets/delete.png) をクリックします。
1. 確認メッセージで「[!UICONTROL **イテレーションを削除**]」をクリックします。
