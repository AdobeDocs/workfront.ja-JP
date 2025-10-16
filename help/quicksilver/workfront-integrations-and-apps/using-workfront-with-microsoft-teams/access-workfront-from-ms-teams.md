---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Microsoft]  Teams から  [!DNL Adobe Workfront]  にアクセス'
description: Workfront ボットチャネルまたは他のチームチャネルのいずれかでコマンドを入力することで、 [!DNL Microsoft Teams]  から  [!DNL Adobe Workfront]  にアクセスして、 [!DNL Workfront]  で複数のアクションを実行できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: a12277e8-2c2e-4b53-990f-6ee9a6541492
source-git-commit: 4cf780aa1b1221cd6ff8e6ce58fbb7d3621f7fa9
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 77%

---

# [!DNL Microsoft Teams] から [!DNL Adobe Workfront] にアクセス

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>[Microsoftが新しい Teams クライアント ](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) に移行すると、Classic Teams クライアントは 2025 年 7 月 1 日（PT）以降は使用できなくなります。 Microsoft TeamsとWorkfrontなどの統合アプリを引き続き使用するには、この日付までに New Teams クライアントに移行する必要があります。
>
>更新されたWorkfront統合が利用できるようになり、新しい Teams エクスペリエンスと完全に互換性があります。 ほとんどの場合、ユーザーが移行すると、Workfrontが自動的に表示されます。 そうでない場合は、Microsoft Teams App Storeから手動で統合をインストールできます。 新しい Teams クライアントでWorkfront統合をインストールまたは検証するには、[Microsoft Teams用のインストール  [!DNL Adobe Workfront] ](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) を参照してください。


[!DNL Workfront] ボットチャネルまたはその他のチームチャネルにいずれかにコマンドを入力することで、[!DNL Microsoft Teams] から [!DNL Adobe Workfront] にアクセスして、[!DNL Workfront] で複数のアクションを実行できます。

[!DNL Microsoft Teams] から [!DNL Workfront] で次の操作を実行できます。

* プロジェクト、タスクまたはイシューを検索する
* 個人用タスクを作成する
* 通知に返信する
* ドキュメント承認を管理する

これらのアクションを実行するために [!DNL Microsoft Teams] から使用するコマンドは、どのチャネルから [!DNL Workfront] にアクセスするかによって異なります。

>[!NOTE]
>
>[!DNL Microsoft Teams] は、[!DNL Internet Explorer] のサポートを終了しました。[!DNL Adobe Workfront for Microsoft Teams integration] を使用する場合は、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>ワークまたはそれ以上</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

次の条件が満たされた場合、[!DNL Microsoft Teams] から [!DNL Adobe Workfront] に個人タスクを作成できます。

* チーム所有者がチームに [!DNL Workfront for Microsoft Teams] をインストールし設定してある。
* [!DNL Microsoft Teams] から [!DNL Workfront] にログインしています。

## [!DNL Workfront] ボットチャットチャネルから [!DNL Workfront] にアクセス

Workfront にログインしている必要があります。

1. **[!DNL Workfront]** ボットチャットチャネルを開きます。
1. テキストフィールドの下の **[!DNL Workfront]** アイコンをクリックして、検索ボックスを表示します。

   ![teams_search_box_in_the_bot_channel.PNG](assets/teams-search-box-in-the-bot-channel-350x456.png)

1. プロジェクト、タスクまたはイシューの名前を入力します。

   項目の検索について詳しくは、[ [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) での  [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) in the article [Search for and share [!DNL Adobe Workfront]  項目の  [!DNL Adobe Workfront]  項目を検索および共有を参照してください。

1. 「**[!UICONTROL ここに質問を入力]**」フィールドをクリックします。

   ![ms_teams_type_your_questions_here_and_what_can_I_do_fields.png](assets/ms-teams-type-your-questions-here-and-what-can-i-do-fields-350x71.png)

1. 次のいずれかの操作を行います。

   * **[!UICONTROL 何ができますか？]**&#x200B;をクリックしてから、[!DNL Workfront] に&#x200B;**[!UICONTROL ログイン]**&#x200B;または&#x200B;**[!UICONTROL ログアウト]**&#x200B;して、[!DNL Workfront] に&#x200B;**[!UICONTROL 新規タスク]**（個人のタスク）を作成するかまたは使用可能なコマンドをリストして&#x200B;**[!UICONTROL ヘルプ]**&#x200B;に問い合わせます。

   * 「**[!UICONTROL ここに質問を入力]**」フィールドにコマンドを入力して、[!DNL Workfront] に直接アクセスします。

     コマンドでは大文字と小文字が区別されません。

     [!DNL Workfront] ボットは、[!DNL Workfront] ボットチャットチャネルのリクエストで返信します。

## チームチャネルから [!DNL Workfront] にアクセス

Workfront にログインしている必要があります。

1. チームチャネルを開き、**@[!DNL Workfront]** を入力して、**[!DNL Workfront]を選択します。**

1. 「**[!UICONTROL 検索]**」をクリックして、プロジェクト、タスクまたはイシューを検索します。

   項目の検索について詳しくは、 [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) 記事に記載される  [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) section in the [Search for and share [!DNL Adobe Workfront]  項目での項目の[検索と共有 [!DNL Adobe Workfront] を参照してください。

1. 次のいずれかのコマンドを入力して、Workfront でこれらのアクションを実行します。\
   コマンドでは大文字と小文字が区別されません。

   * **[!UICONTROL ログイン]** で [!DNL Workfront] にログインする
   * **[!DNL Log out]** で Workfront からログアウトする
   * **[!DNL New task]** で新しい個人の仕事を作成する

     [!DNL Microsoft Teams] からのタスクの作成について詳しくは、[ [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/create-workfront-tasks-from-ms-teams.md) から  [!DNL Adobe Workfront]  タスクを作成を参照してください。

   * **[!UICONTROL ヘルプ]**&#x200B;で使用できるすべてのコマンドのリストを表示します。

     [!DNL Workfront] ボットは、[!DNL Workfront] ボットチャットチャネルのリクエストで返信します。

1. [!DNL Workfront] ボットチャットチャネルに移動し、[!DNL Workfront] にアクセスしてリクエストを完了します。
