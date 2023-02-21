---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: アクセス [!DNL Adobe Workfront] から [!DNL Slack]
description: 統合 [!DNL Adobe Workfront] と [!DNL Slack] を使用して、 [!DNL Workfront] Slackから、または [!DNL Workfront] スラッシュコマンドを使用します。 統合は、任意の [!DNL Slack] 環境 ( [!DNL Slack] モバイルアプリを使用します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 1%

---

# アクセス [!DNL Adobe Workfront] から [!DNL Slack]

統合 [!DNL Adobe Workfront] と [!DNL Slack] を使用して、 [!DNL Workfront] から [!DNL Slack]または [!DNL Workfront] スラッシュコマンドを使用します。 統合は、任意の [!DNL Slack] 環境 ( [!DNL Slack] モバイルアプリを使用します。

自分または自分の [!DNL Slack] 管理者は、 [!DNL Workfront] アプリ内 [!DNL Slack] インスタンスを使用する前に [!DNL Workfront] から [!DNL Slack]. 詳しくは、 [Adobe WorkfrontをSlack用に設定](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## スラッシュコマンドについて {#about-slash-commands}

を使用する場合 [!DNL Slack]の場合、メッセージフィールドの内部にメッセージを入力します。 メッセージをスラッシュで開始すると、そのメッセージはコマンドになり、単純なメッセージとは異なる動作をします。 コマンドは、 [!DNL Slack] をクリックしてアクションを実行します。

次にアクセス： [!DNL Workfront] インスタンスから [!DNL Slack] 任意の [!DNL Slack] チャネル。

でスラッシュコマンドを使用する場合は、次の点に注意してください。 [!DNL Slack] アクセスする [!DNL Workfront]:

* スラッシュコマンドでは、大文字と小文字が区別されます。
* のコマンド [!DNL Workfront] は、入力しているチャネルに関係なく、ユーザーにのみ表示されます。
* コマンドは常に次の文字で始まる必要があります。 `/workfront` または `/wf`に続いて、スペースと、で実行するアクションの名前が表示されます。 [!DNL Workfront].

   これは、コマンドが [!DNL Workfront] アプリを使用します。 のコマンド [!DNL Workfront] は、 [!DNL Workfront] アプリを [!DNL Slack] インスタンス。

Slackで実行できるすべてのコマンドの一覧 [!DNL Workfront]を参照してください。 [アクセス [!DNL Workfront] のスラッシュコマンドから [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack).

## にログインします。 [!DNL Workfront] から [!DNL Slack] {#log-in-to-workfront-from-slack}

[Slack] の [ メッセージ ] フィールドに任意のコマンドを入力すると、にログインするよう求められます。 [!DNL Workfront] 1 つ目は\
の完全なリスト [!DNL Workfront] コマンド [!DNL Slack]を参照し、 [アクセス [!DNL Workfront] のスラッシュコマンドから [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) 」の節を参照してください。

にログインするには [!DNL Workfront] から [!DNL Slack]:

1. にログインします。 [!DNL Slack] インスタンス。
1. 任意のチャネルから、次のいずれかのコマンドを入力します。\
   `/workfront log in`

   または

   `/wf log in`

1. 次をクリック： [!DNL Workfront] **[!UICONTROL ログイン]** 応答に表示されるリンク。\
   新しいタブが開き、次のフィールドが表示されます。 [!DNL Workfront] 資格情報。

1. 画面の指示に従ってにログインします。 [!DNL Workfront] 拡張認証、OAuth 2.0、または Security Assertion Markup Language(SAML)URL を使用する。

   >[!NOTE]
   >
   >* のホストを入力するよう求められたら、 [!DNL Workfront] アカウントに次の形式で入力します。 *yourCompany&#39;sDomain.my.workfront.com*. 会社のドメインは通常、会社の名前です。
   >* 拡張認証は、 [!DNL Workfront] 管理者がこの統合に対して有効にします。



   の設定ページ [!DNL Workfront] 通知 [!DNL Slack] が開きます。

1. （オプション）任意の [!DNL Workfront] 受信しない通知 [!DNL Slack].

   設定に関する情報 [!DNL Workfront] 設定 [!DNL Slack]を参照し、 [設定を構成](#configure-settings-configure-settings) この記事の節

1. に戻ります。 [!DNL Slack] チャネル。

   次にログインしています： [!DNL Workfront] から [!DNL Slack] インスタンス。

## アクセス [!DNL Workfront] から [!DNL Slack]

* [スラッシュコマンドについて](#about-slash-commands-about-slash-commands)
* [アクセス [!DNL Workfront] 共有リンクから [!DNL Slack]](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## アクセス [!DNL Workfront] のスラッシュコマンドから [!DNL Slack] {#access-workfront-from-a-slash-command-in-slack}

1. にログインします。 [!DNL Slack] インスタンスとログイン [!DNL Workfront] から [!DNL Slack].\
   へのログインの詳細 [!DNL Workfront] から [!DNL Slack]を参照してください。 [にログインします。 [!DNL Workfront] から [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack)

1. 任意のチャネルから、メッセージフィールドに次のコマンドを入力します。

   `/workfront help`

   または

   `/wf help`

1. 次のコマンドからを選択します。

   * `/wf home`

      タスク、タスクおよび承認のリストにアクセスするためのボタンが表示されます。 ボタンの 1 つをクリックすると、 [!DNL Slack].

      管理の詳細 [!DNL Workfront] 作業項目 [!DNL Slack]を参照してください。 [作業と承認を次の場所から管理 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf add task <TaskName>`

      タスクが [!DNL Workfront] インターフェイス。

      タスクをに追加します [!DNL Workfront].

      タスクを [!DNL Workfront] Slackから、「 [!DNL Slack]」セクション内の [タスクとタスクの作成元 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf add issue <Issue Name>`

      イシューの名前を、 [!DNL Workfront] インターフェイス。

      に問題を追加しました [!DNL Workfront]

      に問題を追加する方法の詳細 [!DNL Workfront] から [!DNL Slack](「 [!DNL Slack]」セクション内の [タスクとタスクの作成元 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md).

   * `/wf favorites`

      次のリストを表示： [!DNL Workfront] お気に入り。

      お気に入りへのアクセス方法の詳細 [!DNL Slack]を参照し、 [へのアクセス [!UICONTROL お気に入り] リスト元 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) セクション [お気に入りと最近使用した項目へのアクセス [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 記事。

   * `/wf recent`

      最近アクセスした項目のリストを表示します。 [!DNL Workfront].

      最近使用した項目にアクセスする方法の詳細 [!DNL Slack]を参照し、 [へのアクセス [!UICONTROL 最近使用した項目] リスト元 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites] および [!UICONTROL 最近の項目 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) 記事。

   * `wf tasks`

      タスクのリストを表示します。

      タスク管理の詳細 [!DNL Slack]詳しくは、「 [!DNL Slack]」セクション内の [からの作業と承認の管理 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf issues`

      問題のリストを表示します。

      次の場所での問題管理の詳細 [!DNL Slack]詳しくは、 [!DNL Slack]」セクション内の [からの作業と承認の管理 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf approvals` 次を表示： [!DNL Workfront] 承認。\

      次の場所での承認の管理に関する詳細 [!DNL Slack]詳しくは、「 [!DNL Slack]」セクション内の [作業と承認を次の場所から管理 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md).

   * `/wf search <keyword>`

      キーワードを含めます。

      特定のキーワードを検索する。 次のタイプのオブジェクトを検索できます。

      * プロジェクト
      * タスク
      * 問題
      * レポート
      * ユーザー
      * テンプレート
      * ドキュメント
      * ポートフォリオ
      * プログラム
      * ダッシュボード
      * 会社
      * メモ  \

         での検索の詳細 [!DNL Slack]を参照してください。 [を検索 [!DNL Adobe Workfront] Slackの項目](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md).
   * `/wf log in`

      にログインします。 [!DNL Workfront] から [!DNL Slack].

   * `/wf log out `

      からログアウトします。 [!DNL Workfront] から [!DNL Slack]. ログインしたまま [!DNL Workfront] 別の [!DNL Workfront] インスタンスは、別のアプリケーションの別のブラウザータブで開きます。
   * `/wf settings`

      次の設定にアクセスできます： [!DNL Workfront] の設定 [!DNL Slack].

      設定に関する情報 [!DNL Workfront] Slackの設定： [設定を構成](#configure-settings-configure-settings).

   * `/wf help`
次のコマンドの完全なリストを表示します： [!DNL Workfront].


   * `Visit Workfront Help`:を開きます。 [!UICONTROL Slack] セクション [!DNL Workfront] 新しいブラウザタブのヘルプサイト。


1. （オプション）任意のコマンドのメッセージを削除するには、そのコマンドが含まれているSlackメッセージの右上隅にマウスを移動し、次に、「 」をクリックしま&#x200B;す&#x200B;**[!UICONTROL メッセージアクションを表示]**&#x200B;を選択し、「 **[!UICONTROL メッセージを削除]**.

1. （オプションおよび条件付き）「 **[!UICONTROL 削除]** をクリックして、このメッセージの削除を確認します。

### アクセス [!DNL Workfront] 共有リンクから [!DNL Slack] {#access-workfront-from-a-shared-link-in-slack}

次にアクセスできます： [!DNL Workfront] リンクから、 [!DNL Slack].

へのアクセスについて詳しくは、 [!DNL Workfront] 共有リンクから、 [アクセス [!DNL Adobe Workfront] 内の共有リンクのオブジェクト [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md).

## 設定を構成 {#configure-settings}

1. 内部 [!DNL Slack] message フィールドに、次のコマンドを入力します。

   `/workfront settings`

   または

   `/wf settings`

   すべての設定は、デフォルトで有効になっています。

1. Workfrontの設定を無効にするには、次のオプションの選択を解除します。

   * 内 **[!UICONTROL 一般設定]** 領域、無効 **[!UICONTROL 貼り付け時 [!DNL Workfront] 内の URL [!DNL Slack] チャネル、追加の説明、期限、または要求者名を表示]**&#x200B;を設定&#x200B;します。 [!DNL Slack] を追加するには、 [!DNL Workfront] オブジェクトを使用します。 [!UICONTROL Slack].

   * 内 **[!UICONTROL 通知設定]** エリア内で、Workfrontからの受信を停止する通知を無効にします。\

      受信に関する情報 [!DNL Workfront] 通知 [!DNL Slack]を参照してください。 [受信 [!DNL Adobe Workfront] 通知 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## からログアウト [!DNL Workfront] から [!DNL Slack]

1. 内部 [!DNL Slack] message フィールドに、次のコマンドを入力します。\
   `/workfront log out` または\
   `/wf log out`\
   次のページからログアウトしたことを示す確認メッセージが表示されます： [!DNL Workfront].\
   ログインしたまま [!DNL Workfront] 別の [!DNL Workfront] インスタンスは、別のアプリケーションの別のブラウザータブで開きます。
