---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 作業とチームのリクエストの管理
description: リクエストは、保留中のタスクまたはイシューの割り当てを表します。ワークリクエストは個人に対して行われ、チームリクエストはチームに対して行われます。
author: Lisa
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: ht
source-wordcount: '504'
ht-degree: 100%

---

# 作業とチームのリクエストの管理

リクエストは、保留中のタスクまたはイシューの割り当てを表します。ワークリクエストは個人に対して行われ、チームリクエストはチームに対して行われます。

>[!NOTE]
>
>アジャイルチームにはチームリクエストはありません。

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
   <td> <p>リクエストの割り当てまたは作業には「レビュー」以上、リクエストの再割り当てには「ワーク」以上を選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランやライセンスの種類を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## チームにリクエストを割り当てる {#assign-a-request-to-a-team}

プロジェクトマネージャとイシュー依頼者は、作業を行うリソースが不明な場合や、誰が作業を完了したかを問わない場合に、作業をチームに割り当てることができます。

チームのユーザーが自発的にリクエストに取り組むまで、チームに割り当てられたタスクは、「[!UICONTROL チームリクエスト]」タブに残ります。

チームのメンバーでないユーザーとチームの両方にリクエストが割り当てられると、そのリクエストは「[!UICONTROL チームリクエスト]」タブとユーザーのワークリクエストエリアの両方に表示されます。チームのメンバーではないユーザーが自発的にタスクに取り組んでいる場合、チームのメンバーが自発的に取り組むまで、そのタスクは「[!UICONTROL チームリクエスト]」に残ります。

チームは、次のいずれかの方法でタスクおよびイシューに割り当てることができます。

* [!UICONTROL ガントチャート]を通じて
* タスクまたはイシューのリスト（個別または一括）から
* タスクまたはイシューが作成または変更されたとき
* リクエストに対するルーティングルール（問題のみ）を通じて

この節で説明するように、チームページからチームにリクエストを手動で割り当てることができます。

チームページからチームにリクエストを手動で割り当てるには、次の手順に従います。

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に「**[!UICONTROL チーム]**」をクリックします。

1. **[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。

1. **[!UICONTROL その他]**&#x200B;アイコン![](assets/more-icon.png)をクリックし、「**[!UICONTROL 作業リクエストを送信]**」を選択します。

   ![](assets/edit-team-settings-350x205.png)

1. 開いたボックスに情報を入力します。
1. 「**[!UICONTROL リクエストを送信]**」をクリックします。\
   チームに新しいタスクが割り当てられ、「チームリクエスト」タブに表示されます。このタスクは、現在プロジェクトに関連付けられていませんが、移動できます。詳しくは、[タスクを移動](../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。

## リクエストを再割り当てする {#reassign-requests}

チームに割り当てられたリクエストを再割り当てすることができます。

1. [!DNL Adobe Workfront]の右上隅で&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**[!UICONTROL チーム]**」の順にクリックします。
1. **[!UICONTROL チームの切り替え]**&#x200B;アイコン![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックして、次にドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。
1. 左側のナビゲーションパネルで、「**[!UICONTROL チームリクエスト]**」を選択します。
1. **[!UICONTROL 再割り当て]**&#x200B;アイコンをクリックします。

1. リクエストの再割り当て先となるユーザー、グループまたはチームの名前を入力しはじめてから、「**[!UICONTROL 割り当てる]**」をクリックします。\
   リクエストが再割り当てされます。
