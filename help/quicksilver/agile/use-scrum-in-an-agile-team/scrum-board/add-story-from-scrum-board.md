---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: スクラムボードからストーリーとイシューを追加
description: スクラムボードから直接新しいストーリーやイシューを作成することも、ボードから既存のストーリーやイシューを追加することもできます。
author: Lisa
feature: Agile
exl-id: d4eec3c5-8cea-467f-b1b4-3f9fab57b10f
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: ht
source-wordcount: '485'
ht-degree: 100%

---

# [!UICONTROL スクラム]ボードからのストーリーとイシューの追加

スクラムボードから直接新しいストーリーやイシューを作成することも、ボードから既存のストーリーやイシューを追加することもできます。

>[!NOTE]
>
>作業アイテムの[!UICONTROL 予定開始日]と[!UICONTROL 予定完了日]は、[!UICONTROL チームの編集]ページの設定に影響されます。詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の、[[!UICONTROL 作業アイテムをイテレーションに追加する際に、日付を適用する方法を設定]](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)の節を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以上</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>タスクまたはイシューが発生しているプロジェクトへの [!UICONTROL Manage] アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトのアクセスのリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## スクラムボードからのストーリーやイシューの新規作成

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、**[!UICONTROL チーム]**&#x200B;の順にクリックします。
1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。
1. 左パネルで、「**[!UICONTROL イテレーション]**」を選択して特定のイテレーションを選ぶか、「**[!UICONTROL 進行中のイテレーション]**」を選択します。
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
        <td>（必須）新しいストーリーまたはイシューを保存するプロジェクト。プロジェクト名を入力していき、リストに表示されたら選択します。</td>
    </tr>
   </table>

1. 「**[!UICONTROL ストーリーを追加]**」または「**[!UICONTROL イシューを追加]**」をクリックします。

## [!UICONTROL スクラム]ボードへの既存のストーリーまたはイシューの追加

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**[!UICONTROL ボード]**」の順にクリックします。
1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。
1. 左パネルで、「**[!UICONTROL イテレーション]**」を選択して特定のイテレーションを選ぶか、「**[!UICONTROL 進行中のイテレーション]**」を選択します。
1. スクラムボードの右側にある「**[!UICONTROL 追加]**」をクリックし、「**[!UICONTROL 既存ストーリー]**」または「**[!UICONTROL 既存イシュー]**」を選択します。
1. **[!UICONTROL バックログから既存項目を追加]**&#x200B;ダイアログボックスで、ストーリーまたはイシューの名前を入力し始めて、リストに表示されたら選択します。
1. 「**[!UICONTROL ストーリーを追加]**」または「**[!UICONTROL イシューを追加]**」をクリックします。
