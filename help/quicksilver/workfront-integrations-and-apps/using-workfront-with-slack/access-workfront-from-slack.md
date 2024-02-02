---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: ' [!DNL Slack] から  [!DNL Adobe Workfront]  へのアクセス'
description: ' [!DNL Adobe Workfront]  を  [!DNL Slack]  に統合すると、Slack から  [!DNL Workfront]  にアクセスしたり、スラッシュコマンドを使用して  [!DNL Workfront]  で特定のアクションを実行したりできます。 [!DNL Slack]  モバイルアプリを含め、任意の  [!DNL Slack]  環境から統合を使用できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 5f531217-3bd6-4156-8b9f-eabc95d4df10
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: ht
source-wordcount: '1075'
ht-degree: 100%

---

# [!DNL Slack] から [!DNL Adobe Workfront] へのアクセス

[!DNL Adobe Workfront] を [!DNL Slack] に統合すると、[!DNL Slack] から [!DNL Workfront] にアクセスしたり、スラッシュコマンドを使用して [!DNL Workfront] で特定のアクションを実行したりできます。[!DNL Slack] モバイルアプリを含め、任意の [!DNL Slack] 環境から統合を使用できます。

[!DNL Slack] から [!DNL Workfront] を使用するには、ユーザーまたは [!DNL Slack] 管理者が [!DNL Slack] インスタンスに [!DNL Workfront] アプリをインストールする必要があります。詳しくは、[Adobe Workfront for Slack の設定](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)を参照してください。

## スラッシュコマンドについて {#about-slash-commands}

[!DNL Slack] を使用する場合は、メッセージフィールドの内部にメッセージを入力します。メッセージをスラッシュで開始すると、そのメッセージはコマンドになり、単純なメッセージとは異なる動作をします。このコマンドは、[!DNL Slack] にアクションを実行するように指示します。

[!DNL Workfront] インスタンスには、[!DNL Slack] から、任意の [!DNL Slack] チャネルでスラッシュコマンドを入力することでアクセスできます。

[!DNL Slack] でスラッシュコマンドを使用して [!DNL Workfront] にアクセスする場合は、次の点に注意してください。

* スラッシュコマンドでは、大文字と小文字が区別されます。
* [!DNL Workfront] 用のコマンドは、入力しているチャネルに関係なく、ユーザーにのみ表示されます。
* コマンドは常に `/workfront` または `/wf` で始まり、その後にスペースと [!DNL Workfront] で実行するアクションの名前が続く必要があります。

  これは、コマンドが [!DNL Workfront] アプリ用であることを示しています。[!DNL Workfront] 用のコマンドは、[!DNL Slack] インスタンスで [!DNL Workfront] アプリを既に設定している場合にのみ機能します。

Slack for [!DNL Workfront] から実行できるすべてのコマンドのリストについては、[ [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) でのスラッシュコマンドからのアクセス [!DNL Workfront] を参照してください。

## [!DNL Slack] から [!DNL Workfront] へのログイン {#log-in-to-workfront-from-slack}

Slack のメッセージフィールドにコマンドを入力すると、最初に [!DNL Workfront] にログインするように求められます。\
[!DNL Slack] の [!DNL Workfront] コマンドの完全な一覧については、この記事で、[ [!DNL Slack]](#access-workfront-from-a-slash-command-in-slack-access-workfront-from-a-slash-command-in-slack) でのスラッシュコマンドからのアクセス [!DNL Workfront] の節を参照してください。

[!DNL Slack] から [!DNL Workfront] にログインするには：

1. [!DNL Slack] インスタンスにログインします。
1. 任意のチャネルから、次のいずれかのコマンドを入力します。\
   `/workfront log in`

   または

   `/wf log in`

1. 応答に表示される [!DNL Workfront] **[!UICONTROL ログイン]**&#x200B;リンクをクリックします。\
   新しいタブが開き、[!DNL Workfront] 資格情報のフィールドが表示されます。

1. プロンプトに従い、拡張認証 OAuth 2.0 または Security Assertion Markup Language（SAML）URL を使用して [!DNL Workfront] にログインします。

   >[!NOTE]
   >
   >* [!DNL Workfront] アカウントのホストを入力するように求められたら、*yourCompany&#39;sDomain.my.workfront.com* の形式で入力します。会社のドメインは通常、会社の名前です。
   >* 拡張認証は、[!DNL Workfront] 管理者がこの統合に対して有効にするまで使用できません。


   [!DNL Slack] の [!DNL Workfront] 通知の設定ページが開きます。

1. （オプション）[!DNL Slack] で受信したくない [!DNL Workfront] 通知を無効にします。

   [!DNL Slack] の [!DNL Workfront] 設定の構成については、この記事で[設定を行う](#configure-settings-configure-settings)の節を参照してください。

1. [!DNL Slack] チャネルに戻ります。

   [!DNL Slack] インスタンスから [!DNL Workfront] にログインしています。

## [!DNL Slack] から [!DNL Workfront] へのアクセス

* [スラッシュコマンドについて](#about-slash-commands-about-slash-commands)
* [ [!DNL Slack] の共有リンクから  [!DNL Workfront]  へのアクセス](#access-workfront-from-a-shared-link-in-slack-access-workfront-from-a-shared-link-in-slack)

## [!DNL Slack] のスラッシュコマンドから [!DNL Workfront] へのアクセス {#access-workfront-from-a-slash-command-in-slack}

1. [!DNL Slack] インスタンスにログインし、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインの詳細については、「[  [!DNL Slack]](#log-in-to-workfront-from-slack-log-in-to-workfront-from-slack) から  [!DNL Workfront]  へのログイン」を参照してください。

1. 任意のチャネルから、メッセージフィールドに次のコマンドを入力します。

   `/workfront help`

   または

   `/wf help`

1. 次のコマンドから選択します。

   * `/wf home`

     タスク、イシューおよび承認のリストにアクセスするためのボタンが表示されます。ボタンの 1 つをクリックすると、[!DNL Slack] に、各リストの最初の 20 項目が表示されます。

     [!DNL Slack] からの [!DNL Workfront] 作業アイテムの管理について詳しくは、「[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md) からの作業と承認の管理」を参照してください。

   * `/wf add task <TaskName>`

     [!DNL Workfront] インターフェイスに表示される、タスクの名前を含みます。

     [!DNL Workfront] にタスクをに追加します。

     Slack から [!DNL Workfront] にタスクを追加する方法の詳細については、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md) からのタスクとイシューの作成の「[!DNL Slack] からのタスク作成」の節を参照してください。

   * `/wf add issue <Issue Name>`

     [!DNL Workfront] インターフェイスに表示される、イシューの名前を含みます。

     [!DNL Workfront] にイシューを追加します。

     [!DNL Slack] から [!DNL Workfront] にタスクを追加する方法の詳細については、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/create-tasks-and-issues-from-slack.md) からのタスクとイシューの作成で、「[!DNL Slack] からのタスク作成」の節を参照してください。

   * `/wf favorites`

     [!DNL Workfront] お気に入りのリストを表示します。

     [!DNL Slack] からのお気に入りへのアクセスの詳細については、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md) からのお気に入りと最近のアイテムへのアクセスの [ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-favorites) からの[!UICONTROL お気に入り]リストへのアクセスを参照してください。

   * `/wf recent`

     [!DNL Workfront] で最近アクセスした項目のリストが表示されます。

     [!DNL Slack] からの最近のアイテムへのアクセスの詳細については、 [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md)で、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-favorites-and-recent-items-from-slack.md#accessing-recent-items) section in the [[!UICONTROL Access your favorites]  からの [!UICONTROL 最近のアイテム]リストへのアクセスおよび [!UICONTROL  の最近のアイテムへのアクセスを参照してください。

   * `wf tasks`

     タスクのリストを表示します。

     [!DNL Slack] からのタスクの管理の詳細については、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md) からの作業と承認の管理の [!DNL Slack] からのタスクの管理節を参照してください。

   * `/wf issues`

     イシューのリストを表示します。

     [!DNL Slack] からのイシューの管理の詳細については、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md) からの作業と承認の管理で、「[!DNL Slack] からのイシューの管理」の節を参照してください。

   * `/wf approvals` [!DNL Workfront] の承認を表示します。\

     [!DNL Slack] からのタスクの管理の詳細については、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/manage-your-work-and-approvals-from-slack.md) からの作業と承認の管理の [!DNL Slack] からのタスクの管理節を参照してください。

   * `/wf search <keyword>`

     キーワードを含めます。

     特定のキーワードを検索します。次のタイプのオブジェクトを検索できます。

      * プロジェクト
      * タスク
      * イシュー
      * レポート
      * ユーザー
      * テンプレート
      * ドキュメント
      * ポートフォリオ
      * プログラム
      * ダッシュボード
      * 会社
      * メモ \

        [!DNL Slack] での検索について詳しくは、[Slack からの  [!DNL Adobe Workfront]  項目の検索](../../workfront-integrations-and-apps/using-workfront-with-slack/search-for-wf-items-from-slack.md)を参照してください。
   * `/wf log in`

     [!DNL Slack] から [!DNL Workfront] にログインします。

   * `/wf log out `

     [!DNL Slack] で [!DNL Workfront] からログアウトします。別のアプリケーションの別のブラウザータブで別の [!DNL Workfront] インスタンスを開いている場合は、[!DNL Workfront] にログインしたままになります。
   * `/wf settings`

     [!DNL Slack] で [!DNL Workfront] 設定を行うためのアクセス許可が付与されます。

     Slack での [!DNL Workfront] 設定の構成については、[設定を行う](#configure-settings-configure-settings)を参照してください。

   * `/wf help`
[!DNL Workfront] のコマンドの完全なリストを表示します。


   * `Visit Workfront Help`：[!DNL Workfront] ヘルプサイトの [!UICONTROL Slack] セクションが新しいブラウザータブで開きます。


1. （オプション）コマンドのメッセージを削除するには、コマンドを含む Slack メッセージの右上隅にマウスを置き、「**[!UICONTROL メッセージ アクションを表示]**」、「**[!UICONTROL メッセージを削除]**」の順にクリックします。

1. （オプションおよび条件付き）「**[!UICONTROL 削除]**」をクリックして、このメッセージの削除を確認します。

### [!DNL Slack] の共有リンクから [!DNL Workfront] にアクセス {#access-workfront-from-a-shared-link-in-slack}

[!DNL Slack] で共有されているオブジェクトへのリンクから、[!DNL Workfront] オブジェクトにアクセスできます。

共有リンクから [!DNL Workfront] にアクセスする方法の詳細については、 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-wf-objects-from-shared-linked-in-slack.md) の共有リンクからの [ [!DNL Adobe Workfront]  オブジェクトへのアクセスを参照してください。

## 設定を行う {#configure-settings}

1. [!DNL Slack] メッセージフィールド内に次のコマンドを入力します。

   `/workfront settings`

   または

   `/wf settings`

   すべての設定は、デフォルトで有効になっています。

1. Workfront の設定を無効にするには、次のオプションの選択を解除します。

   * [!UICONTROL Slack] でオブジェクトへの URL を共有するときに、[!DNL Slack] によって [!DNL Workfront] オブジェクトに関する追加情報が追加されないようにするには、**[!UICONTROL 一般設定]**&#x200B;エリアで、「**[!UICONTROL [!DNL Slack] チャンネルに [!DNL Workfront] の URL をペーストする際に、追加の説明、期限、またはリクエスト者名を表示]**」設定を無効にします。

   * **[!UICONTROL 通知設定]**&#x200B;エリア内で、Workfront からの受信を停止する通知を無効にします。\

     [!DNL Slack] で [!DNL Workfront] 通知を受信する方法については、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md) で  [!DNL Adobe Workfront]  通知を受信するを参照してください。

## [!DNL Slack] で [!DNL Workfront] からログアウト

1. [!DNL Slack] メッセージフィールド内に次のコマンドを入力します。\
   `/workfront log out` または\
   `/wf log out`\
   [!DNL Workfront] からログアウトされたことを示す確認メッセージが表示されます。\
   別のアプリケーションの別のブラウザータブで別の [!DNL Workfront] インスタンスを開いている場合は、[!DNL Workfront] にログインしたままになります。
