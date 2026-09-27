---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: ワークストリームでのイテレーションの作成
description: イテレーションとは、作業の完了のために予約された一定時間のことです。 アジャイルチームの中には、イテレーションをスプリントと呼ぶものもあります。
author: Courtney
feature: Agile
exl-id: 37b8810d-8439-4a7a-89d5-7c2560422ace
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/t1BOO1GO5uTeqd45ZwNPJC6GXVQWi9sivHwisw2zuFY'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 92%
---
# ワークストリームでイテレーションを作成

>[!IMPORTANT]
>
>ワークストリームは、特定の顧客グループのみが使用できます。

イテレーションとは、作業の完了のために予約された一定時間のことです。 アジャイルチームの中には、イテレーションをスプリントと呼ぶものもあります。

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
   <p>コントリビューター以上</p> 
   <p>リクエスト以上</p>
   </td> 
  </tr>  
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ワークストリームでイテレーションを作成

{{step1-to-boards}}

1. イテレーションを追加するワークストリームを開きます。 ワークストリームを開くには、[!UICONTROL **ワークストリームを表示**]&#x200B;をクリックします。
1. 次のいずれかの方法を使用して、イテレーションを作成します。

   * イテレーションビューの「カードリスト」タブで、「[!UICONTROL **イテレーションを作成**]」をクリックします。
   * リストビューの「カードリスト」タブで、「[!UICONTROL **イテレーションを作成**]」をクリックします。
   * 「ボード」タブで、「[!UICONTROL **ボードを追加**]」をクリックし、「[!UICONTROL **イテレーションプロセス**]」をボードテンプレートとして選択します。 次に、イテレーションボードを開き、「[!UICONTROL **イテレーションを設定**]」をクリックします。

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
      <td>イテレーションが開始される日付。 終了日は、イテレーションの長さに基づいて自動的に入力されます。</td> 
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
