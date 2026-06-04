---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Microsoft]  Teams から  [!DNL Adobe Workfront]  にアクセス'
description: Workfront ボットチャネルまたは他のチームチャネルのいずれかでコマンドを入力することで、 [!DNL Microsoft Teams]  から  [!DNL Adobe Workfront]  にアクセスして、 [!DNL Workfront]  で複数のアクションを実行できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: a12277e8-2c2e-4b53-990f-6ee9a6541492
TQID: https://experienceleague.adobe.com/ztTWhJ3wias0xujQofaN-PZZfSM1BHNnCajJnruzdO8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: a7ef0b24-c866-4849-a368-53678af2dfe5
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 516
ht-degree: 94%

---

# [!DNL Microsoft Teams] から [!DNL Adobe Workfront] にアクセス

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>[Microsoft が New Teams クライアントに移行すると](https://learn.microsoft.com/ja-jp/microsoftteams/teams-classic-client-end-of-availability)、Classic Teams クライアントは 2025年7月1日（PT）以降は使用できなくなります。 Microsoft Teams や Workfront などの統合アプリを引き続き使用するには、この日付までに New Teams クライアントに移行する必要があります。
>
>アップデートされた Workfront 統合が利用可能になりました。この統合には、New Teams エクスペリエンスとの完全な互換性があります。 ほとんどの場合、ユーザーが移行すると、Workfront が自動的に表示されます。 表示されない場合は、Microsoft Teams App Store から手動で統合をインストールできます。 New Teams クライアントで Workfront 統合をインストールまたは検証するには、Workfront for Microsoft Teams[&#128279;](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) のインストール [!DNL Adobe Workfront] を参照してください。


[!DNL Workfront] ボットチャネルまたはその他のチームチャネルにいずれかにコマンドを入力することで、[!DNL Microsoft Teams] から [!DNL Adobe Workfront] にアクセスして、[!DNL Workfront] で複数のアクションを実行できます。

[!DNL Microsoft Teams] から [!DNL Workfront] で次の操作を実行できます。

* プロジェクト、タスクまたはイシューを検索する
* 個人用タスクを作成する
* 通知に返信する
* ドキュメント承認を管理する

これらのアクションを実行するために [!DNL Microsoft Teams] から使用するコマンドは、どのチャネルから [!DNL Workfront] にアクセスするかによって異なります。

>[!NOTE]
>
>[!DNL Microsoft Teams] は、[!DNL Internet Explorer] のサポートを終了しました。 [!DNL Adobe Workfront for Microsoft Teams integration] を使用する場合は、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。

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
   <p>Work またはそれ以上</p> </td> 
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

   項目の検索について詳しくは、[&#x200B; [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) での  [!DNL Microsoft Teams][&#128279;](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) in the article Search for and share [!DNL Adobe Workfront]  項目の  [!DNL Adobe Workfront]  項目を検索および共有を参照してください。

1. 「**[!UICONTROL ここに質問を入力]**」フィールドをクリックします。

   ![ms_teams_type_your_questions_here_and_what_can_I_do_fields.png](assets/ms-teams-type-your-questions-here-and-what-can-i-do-fields-350x71.png)

1. 次のいずれかの操作を行います。

   * 「**[!UICONTROL 何ができますか？]**」をクリックすると、**[!UICONTROL ログイン]**&#x200B;または&#x200B;**[!UICONTROL ログアウト]**/[!DNL Workfront]の後、**[!UICONTROL 新しいタスク]** （個人タスク）を[!DNL Workfront]に作成するか、使用可能なコマンドを一覧表示して&#x200B;**[!UICONTROL ヘルプ]**&#x200B;を取得します。

   * 「**[!UICONTROL ここに質問を入力]**」フィールドにコマンドを入力して、[!DNL Workfront] に直接アクセスします。

     コマンドでは大文字と小文字が区別されません。

     [!DNL Workfront] ボットは、[!DNL Workfront] ボットチャットチャネルのリクエストで返信します。

## チームチャネルから [!DNL Workfront] にアクセス

Workfront にログインしている必要があります。

1. チームチャネルを開き、**@[!DNL Workfront]** を入力して、**[!DNL Workfront]を選択します。**

1. 「**[!UICONTROL 検索]**」をクリックして、プロジェクト、タスクまたはイシューを検索します。

   項目の検索について詳しくは、 [!DNL Microsoft Teams][&#128279;](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) 記事に記載される  [!DNL Microsoft Teams][&#128279;](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) section in the Search for and share [!DNL Adobe Workfront]  項目での項目の検索と共有 [!DNL Adobe Workfront] を参照してください。

1. 次のいずれかのコマンドを入力して、Workfront でこれらのアクションを実行します。\
   コマンドでは大文字と小文字が区別されません。

   * **[!UICONTROL ログイン]** で [!DNL Workfront] にログインする
   * **[!DNL Log out]** で Workfront からログアウトする
   * **[!DNL New task]** で新しい個人の仕事を作成する

     [!DNL Microsoft Teams] からのタスクの作成について詳しくは、[&#x200B; [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/create-workfront-tasks-from-ms-teams.md) から  [!DNL Adobe Workfront]  タスクを作成を参照してください。

   * **[!UICONTROL ヘルプ]**&#x200B;で使用できるすべてのコマンドのリストを表示します。

     [!DNL Workfront] ボットは、[!DNL Workfront] ボットチャットチャネルのリクエストで返信します。

1. [!DNL Workfront] ボットチャットチャネルに移動し、[!DNL Workfront] にアクセスしてリクエストを完了します。
