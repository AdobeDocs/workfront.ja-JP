---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: ストーリー情報を編集
description: かんばんボード上のストーリータイルを表示する場合、ストーリータイルから直接、インラインで編集できる情報があります。
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# ストーリー情報を編集

## 表示および編集できる情報を理解する {#understand-what-information-can-be-viewed-and-edited}

ストーリータイルを表示するとき ( [!UICONTROL かんばん] ボードの場合は、次の表の情報を使用できます。 ほとんどの情報は、ストーリータイルから直接、インラインで編集できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>情報</strong> </th> 
   <th><strong>表示</strong> </th> 
   <th><strong>編集可能なインライン</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>タスクまたはイシューへの直接リンクを含むストーリー名</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクトに直接リンクされたプロジェクト名</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>ストーリーの完了ポイント数または完了時間数と、ストーリーに割り当てられたポイント数または時間数<br>これらの数値は、各ストーリーの「完了率」の計算と表示に使用されます。</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>各ストーリーおよびイシューの [!UICONTROL パーセント完了 ]。<br>[!UICONTROL 反復の完了率は、各ストーリーの [!UICONTROL 完了率 ] に基づいて計算されます。<br></p> <p>ストーリーまたはイシューの [!UICONTROL パーセント完了 ] を更新する際に、0 ～ 100 の任意の数を選択できます。</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>ストーリーの担当者</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>タイルの色またはカテゴリ</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>「アジャイルビューの作成とカスタマイズ」( <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">表示の概要 ( [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以降</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者は、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## ストーリータイルの情報の表示と編集

1. 次をクリック： *[!UICONTROL *メインメニュー]**アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL チーム]**.

1. （オプション） **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)」をクリックし、ドロップダウンメニューから新しいかんばんチームを選択するか、検索バーでチームを検索します。

1. 次に移動： [!UICONTROL かんばん] ボード。
1. ストーリータイルを展開して、ストーリーに関連するすべてのフィールドを表示します。

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. （オプション）フィールドを編集するには、フィールドをクリックして、変更を加えます。\
   必ず [!UICONTROL 編集] ストーリータイルを編集するためのタスクまたはイシューに対する権限\
   各フィールドと編集可能かどうかについて詳しくは、 [表示および編集できる情報を理解する](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>次の手順で [!UICONTROL 完了率]に値を入力する場合は、0 ～ 100 の数値を入力する必要があります。 このフィールドは、動かすことのできるスライダーではありません。
