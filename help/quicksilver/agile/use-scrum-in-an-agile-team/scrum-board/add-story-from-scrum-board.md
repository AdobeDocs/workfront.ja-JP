---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: スクラムボードからのストーリーと問題の追加
description: 新しいストーリーやイシューは、スクラムボードから直接作成することも、ボードから既存のストーリーやイシューを追加することもできます。
author: Lisa
feature: Agile
exl-id: d4eec3c5-8cea-467f-b1b4-3f9fab57b10f
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 次の場所からストーリーと問題を追加： [!UICONTROL スクラム] ボード

新しいストーリーやイシューは、スクラムボードから直接作成することも、ボードから既存のストーリーやイシューを追加することもできます。

>[!NOTE]
>
>作業項目 [!UICONTROL 計画開始日] および [!UICONTROL 計画完了日] が [!UICONTROL チームの編集] ページ。 詳しくは、 [[!UICONTROL 設定] 作業項目を反復に追加する際に日付を適用する方法](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) 記事内 [スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

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
   <td> <p>[!UICONTROL Worker] 以降</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>タスクまたは問題が発生しているプロジェクトへの [!UICONTROL 管理 ] アクセス</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## スクラムボードから新しいストーリーやイシューを作成する

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL チーム]**.
1. （オプション） **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。
1. 左のパネルで、「 」を選択します。 **[!UICONTROL 反復]** 特定の反復を選択するには、または **[!UICONTROL 現在の反復]**.
1. クリック **[!UICONTROL 追加]** スクラムボードの右側で、を選択します。 **[!UICONTROL 新しいストーリー]** または **[!UICONTROL 新しい問題]**.
1. 内 **[!UICONTROL 新規]** ダイアログボックスに次の情報を追加します。

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL 名前 ]</strong></td>
        <td>（必須）ストーリーまたはイシューの名前。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 説明 ]</strong></td>
        <td>項目の説明。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 予測 ]</strong></td>
        <td>品目の推定時間数またはポイント数。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL 親プロジェクト ]</strong></td>
        <td>（必須）新しいストーリーまたはイシューを保存するプロジェクトです。 プロジェクトの名前を入力し、リストに表示されたら選択します。</td>
    </tr>
   </table>

1. クリック **[!UICONTROL ストーリーを追加]** または **[!UICONTROL 問題を追加]**.

## 既存のストーリーまたはイシューを [!UICONTROL スクラム] ボード

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL チーム]**.
1. （オプション） **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。
1. 左のパネルで、「 」を選択します。 **[!UICONTROL 反復]** 特定の反復を選択するには、または **[!UICONTROL 現在の反復]**.
1. クリック **[!UICONTROL 追加]** スクラムボードの右側で、を選択します。 **[!UICONTROL 既存のストーリー]** または **[!UICONTROL 既存の問題]**.
1. 内 **[!UICONTROL バックログから既存を追加]** ダイアログボックスにストーリーまたはイシューの名前を入力し、リストに表示されたら選択します。
1. クリック **[!UICONTROL ストーリーを追加]** または **[!UICONTROL 問題を追加]**.
