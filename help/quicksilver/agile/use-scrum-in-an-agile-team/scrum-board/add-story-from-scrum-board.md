---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: スクラムボードからのストーリーとイシューの追加
description: スクラムボードから直接新しいストーリーやイシューを作成することも、ボードから既存のストーリーやイシューを追加することもできます。
author: Courtney
feature: Agile
exl-id: d4eec3c5-8cea-467f-b1b4-3f9fab57b10f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/CapWxR-tjybMrL03dQVmq4La0hsYrEMncixYSLGnxr0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 415
ht-degree: 98%

---

# [!UICONTROL スクラム]ボードからのストーリーとイシューの追加

スクラムボードから直接新しいストーリーやイシューを作成することも、ボードから既存のストーリーやイシューを追加することもできます。

>[!NOTE]
>
>作業アイテムの[!UICONTROL 予定開始日]と[!UICONTROL 予定完了日]は、[!UICONTROL チームの編集]ページの設定に影響されます。 詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の、[[!UICONTROL 作業アイテムをイテレーションに追加する際に、日付を適用する方法を設定]](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)の節を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p> 
   または
   <p>現在：[!UICONTROL Work] 以上</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>タスクまたはイシューが発生しているプロジェクトへの [!UICONTROL Manage] アクセス権 </td> 
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## スクラムボードからのストーリーやイシューの新規作成

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。
1. 左パネルで、「**[!UICONTROL 反復]**」を選択して特定の反復を選ぶか、「**[!UICONTROL 進行中の反復]**」を選択します。
1. スクラムボードの右側にある「**[!UICONTROL 追加]**」をクリックし、「**[!UICONTROL 新規ストーリー]**」または「**[!UICONTROL 新規イシュー]**」を選択します。
1. **[!UICONTROL 新規]**&#x200B;ダイアログボックスで、次の情報を追加します。

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Name]</strong></td>
        <td>（必須）ストーリーまたはイシューの名前。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Description]</strong></td>
        <td>アイテムの説明。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Estimate]</strong></td>
        <td>アイテムの推定時間数または推定ポイント数。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Parent Project]</strong></td>
        <td>（必須）新しいストーリーまたはイシューを保存するプロジェクト。 プロジェクト名を入力していき、リストに表示されたら選択します。</td>
    </tr>
   </table>

1. 「**[!UICONTROL ストーリーを追加]**」または「**[!UICONTROL イシューを追加]**」をクリックします。

## [!UICONTROL スクラム]ボードへの既存のストーリーまたはイシューの追加

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。
1. 左パネルで、「**[!UICONTROL 反復]**」を選択して特定の反復を選ぶか、「**[!UICONTROL 進行中の反復]**」を選択します。
1. スクラムボードの右側にある「**[!UICONTROL 追加]**」をクリックし、「**[!UICONTROL 既存ストーリー]**」または「**[!UICONTROL 既存イシュー]**」を選択します。
1. **[!UICONTROL バックログから既存項目を追加]**&#x200B;ダイアログボックスで、ストーリーまたはイシューの名前を入力し始めて、リストに表示されたら選択します。
1. 「**[!UICONTROL ストーリーを追加]**」または「**[!UICONTROL イシューを追加]**」をクリックします。
