---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: ホームエリアで作業とチームのリクエストを管理
description: 作業用タスクとタスクが割り当てられると、タスクとタスクは [!UICONTROL 作業用リスト] 内 [!UICONTROL ホーム] 領域 リクエストの表示、再割り当て、返信、操作、削除を行うことができます。 での作業リクエスト [!UICONTROL ホーム] 領域は、リクエストキューに関連する問題に限定されません。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# での作業およびチームリクエストの管理 [!UICONTROL ホーム] 領域

作業用タスクとタスクが割り当てられると、タスクとタスクは [!UICONTROL 作業用リスト] 内 [!UICONTROL ホーム] 領域 リクエストの表示、再割り当て、返信、操作、削除を行うことができます。 での作業リクエスト [!UICONTROL ホーム] 領域は、リクエストキューに関連する問題に限定されません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>タスクと問題への [!UICONTROL 編集 ] アクセス</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>作業が必要なタスクや問題に、権限以上を貢献する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 作業リクエストの表示

自分に割り当てられた作業要求は、 [!UICONTROL ホーム]. どのリクエストを [!UICONTROL ホーム] の上部にあるフィルターの使用 [!UICONTROL 作業用リスト].

作業の準備ができた項目または現在作業中の項目を表示するフィルタを選択できます。

この記事では、 [!UICONTROL ホーム] 現在作業中の項目を表示する領域、または作業を開始する予定の項目。 詳しくは、 [!UICONTROL ホーム] 領域： [作業リストの項目を [!UICONTROL ホーム] 領域](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. 次をクリック： **[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png) 右上隅で、「 **[!UICONTROL ホーム]**.
1. 次をクリック： **[!UICONTROL フィルター]** ドロップダウンメニュー。

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. タスクに対して、次のいずれかのオプションまたは両方をクリックします。

   **[!UICONTROL 開始準備完了]:** 開始する準備ができたタスクと問題のみを表示します。 次のステートメントの両方が真である必要があります。

   * タスクとその親には、作業を妨げる先行タスクやタスクの制約はありません。
   * この [!UICONTROL 計画開始日] タスクや問題の数は、過去または 2 週間以内の将来の数です。

   **[!UICONTROL 準備ができていません]**:まだ開始する準備ができていないタスクと問題のみを表示します。 次のいずれかのステートメントが true である必要があります。

   * タスクとその親には、作業を妨げる先行タスクやタスクの制約がある場合があります。
   * タスクまたは問題には [!UICONTROL 計画開始日] それは 2 週間以上先です。



1. クリック **[!UICONTROL 作業]** under [!UICONTROL タスク] または [!UICONTROL 問題] 現在作業中のタスクと問題を表示します。
1. クリック **[!UICONTROL リクエスト]** under [!UICONTROL 問題] :（自分が割り当てられている）自分からリクエストされたが、まだ作業を承認していない問題を表示する場合。

## チームリクエストへのアクセス

チームに割り当てられたリクエストには、 [!UICONTROL ホーム] 領域 チームリクエストについて詳しくは、 [チームリクエストの概要](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. 次をクリック： **[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png) 右上隅で、「 **[!UICONTROL ホーム]**.
1. 内 **[!UICONTROL 作業用リスト]** 領域、クリックして展開 **[!UICONTROL チームリクエスト]** グループ化。

   チームにリクエストが割り当てられていない場合は、グループ化は表示されません。

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. チーム名をクリックします。\
   この **[!UICONTROL チームリクエスト]** 「 」セクションには、チームに割り当てられているすべてのリクエストが表示されます。 チームリクエストの操作について詳しくは、 [作業とチームのリクエストを管理](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## リクエストの再割り当て

1. 次をクリック： **[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png) 右上隅で、「 **[!UICONTROL ホーム]**.
1. 内 **[!UICONTROL 作業用リスト]** 「 」領域で、再割り当てするリクエストを選択します。

1. をクリックします。 **[!UICONTROL 割り当て]** ウィジェットを使用してリクエストから自分を削除し、リクエストを再割り当てするユーザーの名前を入力します。

   >[!TIP]
   >
   >作業リクエストがまだ「開始準備完了」または「準備完了」の状態の場合、 **[!UICONTROL 再割り当て]** ボタン **[!UICONTROL 詳細]** メニュー [!UICONTROL 作業用リスト].\
   >![再割り当てボタン](assets/reassign-in-left-panel-350x204.png)

1. タスクのステータスが [!UICONTROL 新規] または [!UICONTROL 処理中] タスクが完了したら、ユーザーの割り当てを解除し、タスクを保存してから、タスクを再割り当てして、タスクをホームの作業リストに再度表示する必要があります。

## リクエストに返信

リクエストに返信して、リクエストをより明確にしたり、新しい日付を提案したりできます。

1. 次をクリック： **[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png) 右上隅で、「 **[!UICONTROL ホーム]**.
1. 内 **[!UICONTROL 作業用リスト]** 「 」領域で、返信先のリクエストを選択します。
1. 自分にリクエストを割り当てた個人を見つけます。

   この情報は、 [!UICONTROL 更新] タスクのタブ 次のオプションを必ず選択してください。 **[!UICONTROL システム更新を表示]** が有効になっている。

1. クリック **[!UICONTROL 新しい更新を開始]** 返信を入力し始めます。
1. 受信者の名前を **[!UICONTROL 通知]** ボックスに移動し、 **[!UICONTROL 更新]**.

   >[!TIP]
   >
   >作業リクエストが「開始準備完了」になっているか、 [!UICONTROL 準備ができていません] 州、 **[!UICONTROL 返信]** ボタン **[!UICONTROL 詳細]** メニュー [!UICONTROL 作業用リスト].\
   >![[!UICONTROL 返信ボタン]](assets/reassign-in-left-panel-350x204.png)   >

## リクエストの処理

この [!UICONTROL 作業] ボタンをクリックすると、リクエストを送信したユーザーと、リクエストの処理を開始するリクエストに割り当てられる可能性のある他のユーザーに対して表示されます。 リクエストの操作について詳しくは、  [作業とチームのリクエストを管理](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. 次をクリック： **[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png) 右上隅で、「 **[!UICONTROL ホーム]**.
1. 内 **[!UICONTROL 作業用リスト]** 「 」領域で、作業対象のリクエストを選択し、 **[!UICONTROL 作業]**.\
   問題に関する情報が右側のパネルに表示されます。

## リクエストの削除

リクエストで作業を行わない場合は、タスクを変換するか、リクエストに問い合わせるか、リストから削除します。

1. 次をクリック： **[!UICONTROL メインメニュー]** ![](assets/main-menu-icon.png) 右上隅で、「 **[!UICONTROL ホーム]**.
1. 内 **[!UICONTROL 作業用リスト]**&#x200B;の上にマウスポインターを置いて、作業を待機している項目を指定します。
1. 次をクリック： **[!UICONTROL 割り当て]** ウィジェットを使用して自分を削除します。 これにより、作業項目が作業リストから削除されます。 リクエストが他のユーザーに割り当てられていない場合、または別のチームやジョブの役割に割り当てられていない場合、リクエストは未割り当てのままになります。

   または

   次をクリック： **[!UICONTROL 詳細]** メニューアイコン ![](assets/more-icon.png) を [!UICONTROL ホームワーク] リスト。

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. 次のオプションから選択します。

   * **[!UICONTROL 作業要求に変換]:** 作業項目を作業要求に変換するには、このオプションを選択します。\

      作業項目はリクエストに切り替えられ、リクエストに割り当てられたままになります。\
      後で「 **[!UICONTROL 作業]** 再び

   * **[!UICONTROL 削除]:** このオプションを選択して、 [!UICONTROL 作業用リスト].\

      リクエストから割り当てが解除され、リクエストは、 [!DNL Adobe Workfront].\
      リクエストが他のユーザーに割り当てられていない場合、または別のチームやジョブの役割に割り当てられていない場合、リクエストは未割り当てのままになります。
