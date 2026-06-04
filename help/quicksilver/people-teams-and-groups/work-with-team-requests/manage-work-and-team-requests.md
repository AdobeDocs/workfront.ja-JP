---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: 作業リクエストとチームリクエストの管理
description: リクエストは、保留中のタスクまたはイシューの割り当てを表します。 ワークリクエストは個人に対して行われ、チームリクエストはチームに対して行われます。
author: Courtney
feature: People Teams and Groups, Work Management
exl-id: ef96e520-0d5f-4180-a27a-1fbbffff8f2b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/h9ebMyu8AQNPQTzfYkEMbEbHtghIj-wegaml3cM3RMY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: be65ef36-43e4-48e1-a062-caa3778e15beid: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 488
ht-degree: 96%

---

# 作業とチームのリクエストの管理

リクエストは、保留中のタスクまたはイシューの割り当てを表します。 ワークリクエストは個人に対して行われ、チームリクエストはチームに対して行われます。

>[!NOTE]
>
>アジャイルチームにはチームリクエストはありません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>リクエストを割り当てたり作業したりするには：
   <p>明るいまたはそれ以上</p>
  <p>レビュー以上</p>
   <p>リクエストを再割り当てするには：
   <p>標準</p>
   <p>Work またはそれ以上</p></td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## チームにリクエストを割り当てる {#assign-a-request-to-a-team}

プロジェクトマネージャとイシュー依頼者は、作業を行うリソースが不明な場合や、誰が作業を完了したかを問わない場合に、作業をチームに割り当てることができます。

チームのユーザーが自発的にリクエストに取り組むまで、チームに割り当てられたタスクは、「[!UICONTROL チームリクエスト]」タブに残ります。

チームのメンバーでないユーザーとチームの両方にリクエストが割り当てられると、そのリクエストは「[!UICONTROL チームリクエスト]」タブとユーザーのワークリクエストエリアの両方に表示されます。 チームのメンバーではないユーザーが自発的にタスクに取り組んでいる場合、チームのメンバーが自発的に取り組むまで、そのタスクは「[!UICONTROL チームリクエスト]」に残ります。

チームは、次のいずれかの方法でタスクおよびイシューに割り当てることができます。

* [!UICONTROL ガントチャート]を通じて
* タスクまたはイシューのリスト（個別または一括）から
* タスクまたはイシューが作成または変更されたとき
* リクエストに対するルーティングルール（問題のみ）を通じて

この節で説明するように、チームページからチームにリクエストを手動で割り当てることができます。

チームページからチームにリクエストを手動で割り当てるには、次の手順に従います。

{{step1-to-team}}

1. **[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。

1. **[!UICONTROL その他]**&#x200B;アイコン![](assets/more-icon.png)をクリックし、「**[!UICONTROL 作業リクエストを送信]**」を選択します。

   ![](assets/edit-team-settings-350x205.png)

1. 開いたボックスに情報を入力します。
1. 「**[!UICONTROL リクエストを送信]**」をクリックします。\
   チームに新しいタスクが割り当てられ、「チームリクエスト」タブに表示されます。 このタスクは、現在プロジェクトに関連付けられていませんが、移動できます。詳しくは、[タスクを移動](../../manage-work/tasks/manage-tasks/move-tasks.md)を参照してください。

## リクエストを再割り当てする {#reassign-requests}

チームに割り当てられたリクエストを再割り当てすることができます。

{{step1-to-team}}

1. **[!UICONTROL チームの切り替え]**&#x200B;アイコン![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックして、次にドロップダウンメニューから新しいチームを選択するか、検索バーでチームを検索します。
1. 左側のナビゲーションパネルで、「**[!UICONTROL チームリクエスト]**」を選択します。
1. **[!UICONTROL 再割り当て]**&#x200B;アイコンをクリックします。

1. リクエストの再割り当て先となるユーザー、グループまたはチームの名前を入力しはじめてから、「**[!UICONTROL 割り当てる]**」をクリックします。\
   リクエストが再割り当てされます。
