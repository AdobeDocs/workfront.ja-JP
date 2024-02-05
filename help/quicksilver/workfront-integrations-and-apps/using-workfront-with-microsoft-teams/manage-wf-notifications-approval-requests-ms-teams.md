---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Microsoft]  Teams で  [!DNL Adobe Workfront]  の通知を管理'
description: 承認が必要な項目、与えられた割り当て、または関連付けられている項目に対するコメントや変更について、 [!DNL Adobe Workfront]  から通知を受け取ることができます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7771a7d7-7e20-4b3d-95e7-1050aeb3af67
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 97%

---

# [!DNL Microsoft Teams] で [!DNL Adobe Workfront] の通知を管理

>[!NOTE]
>
>Adobe WorkfrontとMicrosoft Teamsの統合は、現在、クラシックMicrosoft Teamsエクスペリエンスでのみサポートされています。

承認が必要な項目、与えられた割り当て、または関連付けられている項目に対するコメントや変更について、[!DNL Adobe Workfront] から通知を受け取ることができます。

これらの通知には、[!DNL Microsoft Teams] から移動せずに [!DNL Microsoft Teams] 内で実行できる [!DNL Workfront] アクションが含まれています。

>[!NOTE]
>
>[!DNL Microsoft Teams] は、[!DNL Internet Explorer] のサポートを終了しました。[!DNL Adobe Workfront for Microsoft Teams integration] を使用する場合は、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!DNL Microsoft Teams] で [!DNL Workfront] 通知を受信するための前提条件

[!DNL Microsoft Teams] で [!DNL Workfront] 通知を受け取るには、次の条件が満たされている必要があります。

* チーム所有者がチーム用に [!DNL Workfront for Microsoft Teams] をインストールして設定している。
* [!DNL Microsoft Teams] から [!DNL Workfront] にログインしている。
* [!DNL Workfront] でインスタント通知を有効にしている。インスタント通知の有効化について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

[!DNL Workfront for Microsoft Teams] のインストールと [!DNL Workfront from Microsoft Teams] へのログインについては、[ [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) のインストールを参照してください。

## [!DNL Microsoft Teams] での [!DNL Workfront] の通知の管理

[!DNL Workfront for Microsoft Teams] アプリがインストールされると、[!DNL Microsoft Teams] でそのチームのメンバー全員に対して [!DNL Workfront] チャットチャネルが作成されます。[!DNL Workfront] で特定のアクションが実行された場合、[!DNL Microsoft Teams] の [!DNL Workfront] チャットチャネルでそのアクションに関する通知を受信するように [!DNL Workfront for Microsoft Teams] を設定できます。

[!DNL Microsoft Teams] からの [!DNL Workfront] 通知を行う場合は、次の点を考慮してください。

* [!DNL Microsoft Teams] の [!DNL Workfront] 通知は、すべてを受信することはできず、選択した数だけを受信します。
* [!DNL Workfront] から受け取るすべての通知は、[!DNL Workfront] ボットチャットチャネルに表示されます。

  [!DNL Workfront] ボットチャネルのインストールについて詳しくは、[ [!DNL Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) のインストールの記事の [ [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md#logging-in-to-workfront) から  [!DNL Workfront]  へのログインの節を参照してください。

* [!DNL Workfront] で更新が行われてから、その更新に関する通知が [!DNL Microsoft Teams] で受信されるまでに、最大 5 分の遅れが生じる場合があります。
* [!DNL Microsoft Teams] 通知ごとに、メール通知も受け取ります。

[!DNL Microsoft Teams] で受信できる [!DNL Workfront] 通知を管理するには：

1. [!DNL Microsoft Teams] の左側のナビゲーションバーにある&#x200B;**[!UICONTROL その他の追加]**（3 つの点）アプリのアイコンをクリックします。

1. 表示されるリストで [!DNL Workfront] をクリックします。
1. 「**[!UICONTROL 設定]**」タブを選択します。

   ![](assets/ms-teams-settings-tab-350x552.png)

1. 受信しない通知を無効にします。通知のグループ（情報通知や承認通知など）を有効または無効にしたり、通知を個別に管理したりできます。

   すべての通知は、デフォルトで有効になっています。

   [!DNL Workfront for Microsoft] Teams の通知設定は自動的に保存されます。

   >[!NOTE]
   >
   >デフォルトで使用可能な通知に、これ以上通知を追加することはできません。

## [!DNL Workfront] の通知と承認リクエストへの [!DNL Microsoft Teams] での対応

1. [!DNL Microsoft Teams] から [!DNL Workfront] にログインします。\
   [!DNL Workfront] へのログインについては、[インストール [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md)を参照してください。

1. **[!UICONTROL チャット]**&#x200B;エリアに移動し、**[!DNL Workfront]** ボットチャネルをクリックします。\
   このチャネルは、[!DNL Workfront] ボットとの個人的なチャット用です。すべての [!DNL Workfront] 通知がここに表示されます。
1. 受信する通知の種類に応じて、関連するセクションに進みます。

   * [承認通知](#approval-notifications-approval-notifications)
   * [割り当て通知](#assignment-notifications-assignment-notifications)
   * [コメントの通知](#comment-notifications-comment-notifications)
   * [更新通知](#update-notifications-update-notifications)
   * [日付変更の通知](#date-change-notifications-date-change-notifications)

### 承認通知 {#approval-notifications}

タスク、タイムシート、プルーフなどのオブジェクトの承認を求められた場合、承認通知を受け取ります。通知にコメントすることもできます。承認通知から、次のアクションを実行できます。

* **[!UICONTROL 承認]**：クリックしてアイテムを承認します。
* **[!UICONTROL 変更]**：変更を加えたアイテムをクリックして承認します。
* **[!UICONTROL 拒否]**：クリックして項目を却下します。
* **[!UICONTROL コメント]**：クリックしてコメントを入力します。コメントは、通知の対象となるオブジェクトの更新として [!DNL Workfront] にも表示されます。
* **[!UICONTROL プルーフに移動]**：クリックしてプルーフを開きます。その後、プルーフで直接決定できます。詳しくは、[プルーフビューアーでプルーフを決定](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)を参照してください。

>[!NOTE]
>
>承認の決定が完了すると、通知から変更できなくなります。

#### 特定の承認通知で使用可能なアクション：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL Approve]</th> 
   <th>[!UICONTROL Reject]</th> 
   <th> <p>[!UICONTROL Change]</p> </th> 
   <th> <p>[!UICONTROL Go to Proof] </p> </th> 
   <th>[!UICONTROL Comment]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">プロジェクトを承認する必要があります</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">タスクを承認する必要があります</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">イシューを承認する必要があります</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ドキュメントを承認する必要があります</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトへのアクセスを承認する必要があります</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">タイムシートを承認する必要があります</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">誰かがこのプルーフの承認を依頼しています</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">タイムシートが却下されました</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">タイムシートが再開されました</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">リクエストしたドキュメント承認リクエストが承認されました</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">リクエストしたドキュメント承認リクエストが、変更を加えて承認されました</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">リクエストしたドキュメントの承認リクエストが却下されました</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">タイムシートが承認されました</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 割り当て通知 {#assignment-notifications}

割り当て通知は、自分または自分のチームが Workfront のタスクまたはイシューに割り当てられると受け取ります。割り当て通知から、次のアクションを実行できます。

* **[!UICONTROL 作業]**：アイテムに取り組むことをコミットする場合に選択します。新しいアイテムが作業リストに追加されたことを確認する通知が簡潔に表示されます。
* **[!UICONTROL [!DNL Workfront]]** で表示：割り当てられたイシューまたはタスクを Workfront で表示する場合に選択します。新しいタブが開きます。
* **[!UICONTROL 開始]**：アイテムの作業を開始する場合にクリックします。新しいアイテムが作業リストに追加されたことを確認する通知が簡潔に表示されます。
* **[!UICONTROL コメント]**：アイテムにコメントする場合にクリックします。コメントは、Workfront におけるアイテムの更新ストリームにも表示されます。
* **[!UICONTROL ステータス]**：クリックして、ドロップダウンメニューから作業アイテムの新しいステータスを選択します。

#### 特定の割り当て通知で使用可能なアクション：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL Start]</th> 
   <th>[!UICONTROL Comment]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">タスクに割り当てられています</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">イシューに割り当てられています</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">割り当て先のチームがタスクの作業リクエストを受け取ります</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">割り当て先のチームがイシューの作業リクエストを受け取ります</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### コメントの通知 {#comment-notifications}

自分が関連付けられているアイテムに誰かがコメントしたり、誰かが自分を更新に含めたりすると、コミュニケーション通知が届きます。コミュニケーション通知から、次のアクションを実行できます。

* **返信**：コメントまたは[!UICONTROL 更新]に返信する場合にクリックします。返信は、Workfront でコメントが表示される更新ストリームにも表示されます。
* **[!UICONTROL Workfront で表示]**：コメントやアイテムを Workfront に表示する場合に選択します。新しいタブに開かれます。
* **[!UICONTROL ステータス]**：クリックして、コメントや更新の対象となる作業アイテムの新しいステータスを選択します。

#### 特定のコミュニケーション通知で使用できるアクション：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">リクエストに対するコメントが投稿されました</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">作業リクエストに対する返信が投稿されました</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">参加中のスレッドで誰かがコメントしました</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">作業アイテムの 1 つに誰かがコメントしました</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">承認したタイムシートに誰かがコメントしました</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">コメントはユーザープロフィールページに追加されるか、複数のユーザーを一括編集することによって追加されます</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">更新の 1 つにコメントが追加されました</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">タイムシートにコメントが追加されました</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

### 更新通知 {#update-notifications}

関連付けられている項目の更新があるが、その項目に対して何らかのアクションを実行する必要がない場合に、情報通知を受け取ります。情報通知から、次のアクションを実行できます。

* **[!UICONTROL 返信]**：クリックして、[!UICONTROL 更新]に返信します。返信は、Workfront の項目の更新ストリームにも表示されます。
* **Workfront に表示**：選択すると、コメントまたは項目が Workfront に表示され、新しいタブで開きます。
* **[!UICONTROL ステータス]**：クリックして、ドロップダウンメニューから項目の新しいステータスを選択します。

#### 特定の情報通知で使用できるアクション：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th>[!UICONTROL Reply]</th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">購読しているタスク、イシュー、またはプロジェクトが更新された</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">更新を受信する対象者として追加された</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td role="rowheader">チームが [!UICONTROL directed update] として追加されました</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

### 日付変更の通知 {#date-change-notifications}

割り当て先の作業アイテムの日付が変更されると、日付変更通知を受け取ります。日付変更通知から、次のアクションを実行できます。

* **[!UICONTROL コメント]**：クリックして、項目にコメントを追加します。コメントは、Workfront におけるアイテムの更新ストリームにも表示されます。
* **[!UICONTROL ステータス]**：クリックして、ドロップダウンメニューから作業アイテムの新しいステータスを選択します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>通知</th> 
   <th> <p>[!UICONTROL Comment]</p> </th> 
   <th> <p>[!UICONTROL Status]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">割り当てられているタスクの完了予定日が変更になった</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>
