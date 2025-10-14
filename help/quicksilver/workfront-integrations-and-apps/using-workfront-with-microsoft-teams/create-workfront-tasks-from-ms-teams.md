---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Microsoft] Teams からの [!DNL Adobe Workfront] タスクの作成'
description: チーム所有者がチームに [!DNL Workfront] for Microsoft Teams をインストールし設定してある場合、Microsoft Teams から Workfront にログインすると、Microsoft Teams から Adobe [!DNL Workfront] に個人タスクを作成できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 940cbfb34f12eacd5ba698f60fb7a3e67eb62b22
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 77%

---

# [!DNL Microsoft Teams] からの [!DNL Adobe Workfront] タスクの作成

>[!IMPORTANT]
>
>[Microsoftが新しい Teams クライアント &#x200B;](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) に移行すると、Classic Teams クライアントは 2025 年 7 月 1 日（PT）以降は使用できなくなります。 Microsoft TeamsとWorkfrontなどの統合アプリを引き続き使用するには、この日付までに New Teams クライアントに移行する必要があります。
>
>更新されたWorkfront統合が利用できるようになり、新しい Teams エクスペリエンスと完全に互換性があります。 ほとんどの場合、ユーザーが移行すると、Workfrontが自動的に表示されます。 そうでない場合は、Microsoft Teams App Storeから手動で統合をインストールできます。 新しい Teams クライアントでWorkfront統合をインストールまたは検証するには、[Microsoft Teams用のインストール  [!DNL Adobe Workfront] &#x200B;](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) を参照してください。

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

## 前提条件

次の条件が満たされた場合、[!DNL Microsoft Teams] から [!DNL Adobe Workfront] に個人タスクを作成できます。

* チーム所有者がチームに [!DNL Workfront for Microsoft Teams] をインストールし設定してある。
* ユーザーが [!DNL Microsoft Teams] から [!DNL Workfront] にログインしている。

>[!NOTE]
>
>[!DNL Microsoft Teams] では [!DNL Internet Explorer] のサポートを終了しました。[!DNL Adobe Workfront for Microsoft Teams] 統合を使用するには、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。

[!DNL Workfront for Microsoft Teams] のインストールと [!DNL Microsoft Teams] からの [!UICONTROL Workfront] へのログインについては、[&#x200B; [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) のインストールを参照してください。

## [!DNL Microsoft Teams] から個人タスクを作成

1. [!DNL Microsoft Teams] から [!DNL Workfront] にログインします。

   [!DNL Workfront] へのログインについては、[&#x200B; [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) のインストールを参照してください。

1. **[!UICONTROL 新規タスク]**&#x200B;カードを開くには

   * [!DNL Workfront] ボットチャットチャネルを使用している場合は、「[!UICONTROL 会話]」フィールドに&#x200B;**[!UICONTROL 新規タスク]**&#x200B;と入力して、新しいタスクを作成します。
   * [!DNL Workfront] ボットチャットチャネル以外のチャットチャネルを使用している場合：

      * 「[!UICONTROL 会話]」フィールドに **[!DNL @workfront]** と入力していき、目的の [!DNL Workfront] ボットチャネルを選択します。
      * 引き続き「[!UICONTROL 会話]」フィールドに&#x200B;**[!UICONTROL 新規タスク]**&#x200B;と入力して、新しいタスクを作成します。

        [!DNL Workfront] ボットチャネルに[!UICONTROL 新規タスク]カードが表示されます。

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. [!UICONTROL Workfront] ボットチャネルの[!UICONTROL 新規タスク]カードで、次の情報を指定します。

   * 「**[!UICONTROL タスクのタイトルをここに書き込みます]**」フィールドにタスク名を入力します。
   * 「**[!UICONTROL タスクの説明を書き込みます]**」フィールドにタスクの説明を入力します。
   * タスクの完了期限の日付を「**[!UICONTROL 期限日]**」フィールドに入力します。

1. 「**[!UICONTROL 保存]」をクリックします。**

   新しい個人タスクが [!DNL Workfront] に作成されます。[!UICONTROL 参照番号]がタスクに割り当てられ、[!UICONTROL 新規タスク]カードに表示されます。

   参照番号については、[&#x200B; [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) のオブジェクトについての記事のオブジェクトの[[!UICONTROL 参照番号]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects)の節を参照してください。

1. （オプション）「**[!UICONTROL 編集]**」をクリックして、タスクの情報をさらに編集します。
1. （オプション）「**[!UICONTROL [!DNL Workfront]]** で表示」をクリックして [!DNL Workfront] の新しいタブにタスクを開き、さらに編集して、プロジェクトに移動するか、他のユーザーに割り当てます。
