---
product-area: agile-and-teams;projects;user-management
navigation-topic: scrum-board
title: スクラムボードでのストーリーとイシューの管理
description: ストーリーやイシューをスクラムボードから別のイテレーションやバックログに移動したり、スクラムボードから削除したりできます。ストーリーやイシューを削除すると、30 日間ごみ箱に移動され、システム管理者のみが復元できます。
author: Jenny
feature: Agile
exl-id: 72990251-0264-4e68-83ef-1a9cde5b685c
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 82%

---

# [!UICONTROL スクラム]ボードでのストーリーとイシューの管理

ストーリーやイシューを[!UICONTROL スクラム]ボードから別のイテレーションやバックログに移動したり、[!UICONTROL スクラム]ボードから削除したりできます。ストーリーやイシューを削除すると、30 日間ごみ箱に移動され、システム管理者のみが復元できます。

タスクまたは問題を削除したり、バックログに送信したりせずにイテレーションから削除するには、プロジェクトに移動し、割り当て列からアジャイルチームを削除します。 これにより、スクラムボードからタスクまたはイシューが削除されますが、プロジェクトには残ります。

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
   <td>タスクまたはイシューへの[!UICONTROL Manage]アクセス権 </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!UICONTROL &#x200B; スクラム &#x200B;] ボードからのストーリーまたはイシューの移動

{{step1-to-team}}

1. **[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームの切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューからスクラムチームを選択するか、検索バーでチームを検索します。
1. 左パネルで、「**[!UICONTROL 反復]**」を選択して特定のイテレーションを選択するか、「**[!UICONTROL 進行中の反復]**」を選択します。
1. ストーリーまたはイシューの&#x200B;**[!UICONTROL その他]**&#x200B;アイコンをクリックし、「**[!UICONTROL 指定の場所に移動]**」を選択します。

   ![スクラムボードからのストーリーの削除または移動](assets/scrum-delete-move-story.png)

1. 確認メッセージで、次のいずれかを選択します。

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Another iteration]</strong></td>
        <td>アイテムを別のイテレーションに移動する場合に選択し、ストーリーまたはイシューの移動先のイテレーションを選択します。今後のイテレーションが定義されていない場合は、アイテムを移動できません。</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Backlog]</strong></td>
        <td>ストーリーまたはイシューをチームのバックログに移動する場合に選択します。</td>
    </tr>
   </table>

   >[!NOTE]
   >
   >作業アイテムの[!UICONTROL 予定開始日]と[!UICONTROL 予定完了日]は、[!UICONTROL チームを編集]ページの設定の影響を受けます。詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の記事で[[!UICONTROL 作業アイテムをイテレーションに追加する際に日付を適用する方法の設定]](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)を参照してください。

1. 「**[!UICONTROL 移動]**」をクリックします。

## [!UICONTROL &#x200B; スクラム &#x200B;] ボードからのストーリーまたはイシューの削除

{{step1-to-team}}

1. **[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームの切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューからスクラムチームを選択するか、検索バーでチームを検索します。
1. 左パネルで、「**[!UICONTROL 反復]**」を選択して特定のイテレーションを選択するか、「**[!UICONTROL 進行中の反復]**」を選択します。
1. ストーリーまたはイシューの&#x200B;**[!UICONTROL その他]**&#x200B;アイコンをクリックし、「**[!UICONTROL ストーリーを削除]**」または「**[!UICONTROL 問題の削除]**」を選択します。

   ![スクラムボードからのストーリーの削除または移動](assets/scrum-delete-move-story.png)

1. 確認メッセージで、「**[!UICONTROL はい、削除します]**」をクリックします。
