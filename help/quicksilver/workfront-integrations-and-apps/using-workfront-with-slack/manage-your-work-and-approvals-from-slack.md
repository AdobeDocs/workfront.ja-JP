---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: 作業と承認を Slack から管理
description: ホームのワークリストにアクセスし、タスクやイシューに対して確認、同意して、Slack から直接承認を確認あるいは決定できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: ht
source-wordcount: '902'
ht-degree: 100%

---

# [!DNL Slack] から作業と承認を管理

[!DNL Adobe Workfront for Slack] をインストールした後には、以下の操作を実行できます。

* [!DNL Slack] から[!UICONTROL ホーム]項目にアクセス
* [!DNL Slack] からタスクとイシューに関する作業を確認し、同意
* [!DNL Slack] から、承認を確認および決定

[!DNL Slack] を用いた [!DNL Workfront] の設定に関して詳しくは、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) を設定を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] プラン</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 前提条件

[!DNL Slack] から作業と承認を管理するには、以下の操作が必要です。

* [!DNL Workfront for Slack] を設定\
  [!DNL Workfront for Slack] の設定の手順については、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

## [!DNL Slack] から作業を管理

1. お使いの [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインに関して詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスにある「[!DNL Slack]から [!DNL Workfront] へのログイン」の節を参照してください。

1. 任意のチャネルから、メッセージフィールドに次のコマンドを入力します。

   `/workfront home`

   >[!NOTE]
   >
   >* コマンドでは大文字と小文字が区別されます。
   >* `/workfront` の代わりに `/wf` でコマンドを開始できます。

   タスク、イシューおよび承認のリストにアクセスできるボタンが表示されます。ボタンのうちの 1 つをクリックすると、[!DNL Slack] 内の各リストの最初の 20 項目が表示されます。

1. （オプション）「**[!UICONTROL タスク]**」をクリックして、すべてのタスクを表示します。

   [!DNL Slack] でのタスク管理の詳細に関して詳しくは、[ [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack) からのタスクの管理を参照してください。

1. （オプション）「**[!UICONTROL イシュー]**」をクリックして、すべてのイシューを表示します。

   [!DNL Slack] でのイシューの管理に関して詳しくは、[ [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack) からのイシューの管理を参照してください。

1. （オプション）「**[!UICONTROL 承認]**」をクリックして、決定を待機しているすべての承認を表示します。\
   [!DNL Slack] での承認の管理に関して詳しくは、[ [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack) から承認を管理を参照してください。

## [!DNL Slack] からタスクを管理 {#manage-your-tasks-from-slack}

1. お使いの [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインに関する詳細情報は、 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から [ アクセス [!DNL Adobe Workfront] にある「[!DNL Slack] から [!DNL Workfront] へのログイン」を参照してください。

1. 任意のチャネルから、メッセージフィールドに次のいずれかのコマンドを入力します。

   `/workfront home`、「**[!UICONTROL タスク]**」の順にクリックします。

   または

   `/workfront tasks`

   >[!NOTE]
   >
   >* コマンドでは大文字と小文字が区別されます。
   >* `/workfront` の代わりに `/wf` でコマンドを開始できます。

   リストの最初の 20 件のタスクが表示されます。

1. 「**[!UICONTROL +`<remaining number>`その他]**」をクリックして、追加のタスクを表示します。
1. 作業アイテムに関する以下の情報を考慮してください。

   * **[!UICONTROL 名前]**
   * **[!UICONTROL プロジェクト名]**&#x200B;または **[!DNL Parent Object Name]**

   * 作業アイテムの **[!DNL Planned Completion Date]**。
   * **[!DNL Assigned By Name]**：タスクを割り当ててきたたユーザーの名前です。
   * **[!UICONTROL ステータス]**

1. （オプション）項目の名前をクリックして、別の「ブラウザー」タブの Workfront で開きます。
1. （オプション）**[!UICONTROL ステータス]**&#x200B;フィールドで、新しいステータスを選択します。
1. （オプション）「**[!UICONTROL 時間を記録]**」をクリックし、項目に記録する&#x200B;**[!UICONTROL 時間タイプ]**&#x200B;および時間数を選択します。

   >[!NOTE]
   >
   >* 記録できるのは、1 時間または 30 分単位、最大 12 時間 30 分までです。
   >* 記録した時間数のエントリ日は今日になっています。[!DNL Slack] から過去または未来の日付の時間を記録することはできません。

   時間が記録されたことを示す確認メッセージが表示されます。

1. （オプション）「**[!UICONTROL 作業をする]**」をクリックして、タスクの作業を承認します。「[!UICONTROL 作業をする]」ボタンが表示されなくなります。

## [!DNL Slack] からイシューを管理 {#manage-your-issues-from-slack}

1. お使いの [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインに関して詳しくは、 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) の [ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront]  から [!DNL Workfront]  へのログインを参照してください。

1. 任意のチャネルから、メッセージフィールドに次のいずれかのコマンドを入力します。

   `/workfront home`、**[!UICONTROL イシュー]**&#x200B;の順にクリック

   または

   `/workfront issues`

   >[!NOTE]
   >
   >* コマンドでは大文字と小文字が区別されます。
   >* `/workfront` の代わりに `/wf` でコマンドを開始できます。

   リストの最初の 20 件のイシューが表示されます。

1. 「**[!UICONTROL + 残り `<number>`]**」をクリックして、追加の項目を表示します。
1. 作業アイテムに関する以下の情報を考慮してください。

   * **[!UICONTROL 名前]**
   * **[!UICONTROL プロジェクト]**&#x200B;名または親オブジェクト名
   * **[!UICONTROL 期限]**&#x200B;日付：これは、作業アイテムの予定完了日です。
   * **[!DNL Requested by]**&#x200B;名前：これは、プライマリ連絡先（イシューの場合）または割り当てを行ったユーザー（タスクの場合）です。

1. （オプション）イシューの名前をクリックして、別の「ブラウザー」タブの Workfront で開きます。
1. （オプション）**[!DNL Work on it]** をクリックして、まだ受け入れていないイシューの作業を開始します。

   「[!UICONTROL 作業をする]」ボタンが表示されなくなります。

## 作業と承認を [!DNL Slack] から管理 {#manage-your-approvals-from-slack}

1. [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインに関して詳しくは、 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から [ へのアクセス [!DNL Adobe Workfront] にある「[!DNL Slack] から [!DNL Workfront] へのログイン」の節を参照してください。

1. 任意のチャネルから、メッセージフィールドに次のいずれかのコマンドを入力します。

   `/workfront home`、「**[!UICONTROL 承認]**」の順にクリック

   または

   `/workfront approvals`

   >[!NOTE]
   >
   >* コマンドでは大文字と小文字が区別されます。
   >* `/workfront` の代わりに `/wf` でコマンドを開始できます。

   **[!UICONTROL 承認]**&#x200B;リストの最初の 20 項目が表示されます。項目をリクエストしたユーザーの名前や、項目が属するプロジェクトの名前などの、項目に関する追加情報も表示されます。

1. 「**[!UICONTROL + 残り `<number>`]**」をクリックして、追加の項目を表示します。

1. 以下のオブジェクトの承認の管理を考慮します。

   * **プロジェクト**

     「**[!UICONTROL 承認]**」または「**[!UICONTROL 却下]**」をクリックし、プロジェクトのステータスの変更を許可または却下します。

   * **タスク**

     「**[!UICONTROL 承認]**」または「**[!UICONTROL 却下]**」をクリックし、プロジェクトのステータスの変更を許可または却下します。

   * **イシュー**

     「**[!UICONTROL 承認]**」または **[!DNL Reject]** をクリックし、イシューのステータスの変更を許可または却下します。

   * **ドキュメント**

     「**[!UICONTROL 承認]**」をクリックしてドキュメントを承認、「**[!UICONTROL 却下]**」をクリックしてドキュメントを却下、あるいは「**[!UICONTROL 変更]**」をクリックして、承認はするがドキュメントに追加の変更が必要であることを示します。\
     （オプション）ドキュメントのサムネールの上にマウスを移動して、虫眼鏡アイコンをクリックし、ドキュメントをプレビューします。

   * **プルーフ**：プルーフ名をクリックして別タブの[!DNL Workfront]でプルーフを開き、承認を管理します。
   * **アクセスリクエスト**

     「**[!UICONTROL アクセス権の付与]**」をクリックして、リクエストされたオブジェクトに対する拡張権限を与えるか、「**[!UICONTROL 無視]**」をクリックして、追加のアクセス権のリクエストを無視します。

1. （オプション）承認用に送信されたオブジェクトの名前をクリックして、新しい「ブラウザー」タブの [!DNL Workfront] で開きます。
