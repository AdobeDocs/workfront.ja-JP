---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP サーバーの設定
description: WorkfrontインスタンスとAI エージェント型プラットフォームを設定することで、自然言語の会話を通じてWorkfrontと連携できます。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 6ee4dc992b62ce2602bab0b75d8a27fa6a01acc2
workflow-type: tm+mt
source-wordcount: '1935'
ht-degree: 0%

---


# Adobe Workfront MCP サーバーの設定

[!DNL Adobe Workfront] MCP サーバーを使用すると、サポートされているAI エージェント プラットフォームで自然言語の会話を通じてWorkfront データを操作できます。

AI エージェント型プラットフォームをWorkfrontに接続する前に、Workfront管理者がWorkfront インスタンスでMCP サーバーアクセスを有効にする必要があります。 AI エージェント型プラットフォームを接続する正確な手順は、サポートされているAI エージェント型プラットフォームごとに異なります。

## サポートされているAI エージェント型プラットフォーム

Workfront MCP サーバーは、Model Context Protocol （MCP）をサポートするあらゆるAI エージェント プラットフォームで動作します。

この記事では、次の接続手順について説明します。

* [!DNL Claude]
* [!DNL ChatGPT]

別のMCP互換AI エージェンティック プラットフォーム（例：[!DNL Gemini]または[!DNL Microsoft Copilot]）を使用している場合は、そのプラットフォームのドキュメントの手順に従って、カスタム MCP サーバーを追加します。 MCP サーバーのURLの入力を求められたら、次のように入力します。

```
https://mcp.workfront.adobe.com/mcp/v1/workfront
```

## 前提条件

WorkfrontをAI エージェント型プラットフォームに接続する前に、次の手順を実行する必要があります。

* 操作するデータにアクセスする権限を持つアクティブな[!DNL Adobe Workfront] アカウントを持っている
* [!DNL Claude]のようなAI エージェンティック プラットフォームにアクセスする
* Workfront インスタンスは、Adobe Identity Management システム（IMS）で有効にする必要があります。
* MCPをWorkfront Planningで使用するには、Adobe Workfront Planningを含むWorkfront パッケージに属している必要があります。


### 管理者の前提条件

MCP サーバーアクセスは、2人の別々の管理者によってゲートされます。

* Workfront管理者は、システム環境設定の&#x200B;**読み取り専用MCP ツール** （デフォルトで有効）と&#x200B;**書き込みMCP ツール** （デフォルトで無効）の2つのトグルを使用して、Workfront インスタンスのMCP サーバーアクセスを制御します。 AI エージェントを使用してWorkfront アイテムを見つけることができるが、作成、更新、または削除できない場合は、Workfront管理者に書き込みアクションを有効にするように依頼してください。

  詳しくは、[&#x200B; システム環境設定の設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。

* エンタープライズ版のAI エージェント型プラットフォームを使用する場合、そのプラットフォームの管理者は、組織の[!DNL Adobe Workfront] コネクタを有効にするか、Workfront MCP サーバーに接続するためのカスタム URL アクセス権を付与する必要があります。


## WorkfrontとClaudeの連携

Workfrontへの接続は、[!DNL Claude] アカウントごとに1回です。 接続によって特定のWorkfront インスタンスが認証され、切断するまで接続が維持されます。

* [Connectors ディレクトリからClaude デスクトップに接続します](#connect-to-claude-desktop-from-the-connectors-directory)
* [URLを使用してClaudeに接続](#connect-to-claude-with-a-url)
* [Claudeの行動をスキルでカスタマイズする](#customize-claude-behavior-with-skills)

### Connectors ディレクトリからClaude デスクトップに接続します

+++ 展開すると、Workfrontを[!DNL Claude]に接続するための手順が表示されます。

Workfrontを[!DNL Claude]に接続するには：

1. [!DNL Claude] を開きます。.

1. コネクタ領域に移動します。



1. コネクタリストで&#x200B;**[!DNL Adobe Workfront]**&#x200B;を検索します。

   表示されない場合は、この記事の「[管理者の前提条件](#admin-prerequisites)」を参照してください。

1. 「**接続**」をクリックします。



1. プロンプトが表示されたら、Workfront インスタンスにログインします。


1. 認証が完了したら、接続されます。



+++

### URLを使用してClaudeに接続

+++ 展開すると、URLを使用してWorkfrontを[!DNL Claude]に接続するための手順ごとの手順が表示されます。

>[!NOTE]
>
>この手順を実行するには、エンタープライズクラウド環境の所有者である必要があります。
>
>所有者の要件に関するClaudeのステートメントについては、Claude ドキュメントの「[&#x200B; カスタムコネクタを追加](https://support.claude.com/en/articles/11175166-get-started-with-custom-connectors-using-remote-mcp#:~:text=Note%3A%20While,has%20access%20to)」を参照してください。

URLを使用してWorkfrontを[!DNL Claude]に接続するには：

1. 資格情報を使用して[Claude](https://claude.ai)にログインします。
1. 左側のメニューで、**カスタマイズ** アイコンを選択します。
1. **コネクタ**&#x200B;を選択し、**+** アイコンを選択してコネクタを追加します。
1. 「**アプリを作成**」ボタンを選択します。
1. コネクターに目的の名前（「Workfront」など）を付け、MCP サーバーのURLを入力します。

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront
   ```

1. コネクタを作成すると、ログインウィンドウがポップアップ表示されます。 Adobe IDの認証情報を使用して認証します。 複数に属している場合は、必ず目的のWorkfront インスタンスを選択してください。

+++

### Claudeの行動をスキルでカスタマイズする

[!DNL Claude]は、スキルと呼ばれるユーザー作成の命令セットをサポートしています。 Workfrontでは、スキルを使用して[!DNL Claude]の動作をカスタマイズできます。 例えば、以前の結果に頼るのではなく、常にWorkfrontから新しいデータを取得するように[!DNL Claude]に指示するスキルを作成できます。

[!DNL Claude] スキルについて詳しくは、[Claude ユーザードキュメント &#x200B;](https://code.claude.com/docs/en/skills)を参照するか、Claudeにスキルに関するヘルプを依頼してください。

## ChatGPTへの接続

Workfront MCP サーバーとChatGPTを接続する手順は、ChatGPT デスクトップとCodex、またはWeb上のChatGPTのどちらを使用しているかによって異なります。

* [ChatGPT デスクトップまたはChatGPT コーデックスへの接続](#connect-to-chatgpt-desktop-or-chatgpt-codex)
* [Web上でChatGPTに接続する](#connect-to-chatgpt-on-the-web)
* [カスタム GPTでChatGPTの動作をカスタマイズ](#customize-chatgpt-behavior-with-custom-gpts)

### ChatGPT デスクトップまたはChatGPT コーデックスへの接続

1. ChatGPTで、**設定**&#x200B;を開きます。
1. 左側のナビゲーションで「**プラグイン**」をクリックします。
1. ウィンドウの右上付近にある「**サーバーを追加**」をクリックします。
1. サーバーの名前を入力します。
1. タイプに「**ストリーマブル HTTP**」を選択します。
1. MCP サーバーのURLを設定します。

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront
   ```

1. 「**保存**」をクリックします。
1. 表示されるリストで、追加するMCP サーバーの&#x200B;**Authenticate**&#x200B;をクリックします。
1. Workfrontにログインします。
1. ChatGPTでは、MCP サーバーリストで、新しいMCP サーバーの右側のトグルがオンのままであることを確認します。


### Web上でChatGPTに接続する

1. 資格情報を使用して[ChatGPT](https://chatgpt.com)にログインします。
1. 左下で名前を選択し、**設定**&#x200B;を選択します。
1. 左側のナビゲーションで、**セキュリティとログイン**&#x200B;を選択します。
1. https://chatgpt.com/pluginsのChatGPT プラグインページに移動します。
1. プラグインページの右上付近にあるプラスアイコンをクリックします。
1. 「**名前**」フィールドに、MCP サーバーの名前を入力します。
1. **接続** フィールドで、**サーバーURL**&#x200B;を選択し、MCP サーバーURLを入力します。

   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront
   ```

1. 認証が&#x200B;**OAuth**&#x200B;に設定されていることを確認します（デフォルトで設定）。
1. リスクメッセージを読み、チェックボックスにチェックを入れて、読んだことを示します。
1. 「**作成**」をクリックします。
1. アプリを作成すると、Workfront ログインウィンドウが表示されます。 Adobe IDの認証情報を使用して認証します。 複数に属している場合は、必ず目的のWorkfront インスタンスを選択してください。


### カスタム GPTでChatGPTの動作をカスタマイズ

ChatGPTは、カスタム GPTと呼ばれるユーザー作成アシスタントをサポートしています。 カスタム GPTを使用して、ChatGPTがコネクタでどのように動作するかをカスタマイズできます。 例えば、以前の結果に頼るのではなく、接続されたサービスから常に新しいデータを取得するようにChatGPTに指示するカスタム GPTを作成できます。

カスタム GPTについて詳しくは、[ChatGPT ユーザードキュメント &#x200B;](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)を参照するか、カスタム GPTのヘルプをChatGPTに依頼してください。

## WorkfrontとCopilotの連携

Workfront MCPが接続できるカスタム Copilot エージェントを構築するには、Copilot Studioを使用します。

1. Copilot Studioで、**空のエージェントを作成**&#x200B;をクリックします。
1. エージェントに名前を付け、**作成**&#x200B;をクリックします。
エージェントのウィンドウが開きます。

1. 「**手順**」フィールドに、エージェントに対して何をさせるかを記述します。 既存のプロセスやWorkfrontの使用方法などの情報を含めます。 大量の詳細を提供することをお勧めします。
1. 上部のナビゲーションで「**ツール**」をクリックし、「**ツールを追加**」をクリックします。
1. **モデル コンテキスト プロトコル** タイルを選択します。
1. 表示されるパネルで、この接続の名前と説明を入力します。
1. 「サーバーURL」フィールドに、次のURLを入力します。

```
https://mcp.workfront.adobe.com/mcp/v1/workfront`
```

1. 承認の場合は、**OAuth 2.0**&#x200B;を選択し、**Dynamic discovery**&#x200B;を選択します。
1. パネルの下部にある「**作成**」をクリックします。

   アプリが登録されました。

1. アプリが登録されたら、表示されるパネルで「**未接続**」をクリックし、「**新しい接続を作成**」をクリックしてから「**作成**」をクリックします。
1. 表示されるログインパネルで、Workfrontにログインし、使用するWorkfront インスタンスが表示されたら&#x200B;**続行**&#x200B;を選択します。
1. サーバーを表示するパネルで、**追加して設定**&#x200B;をクリックします。

   これで、MCP サーバーのツールの使用と設定を開始できます。
1. ツールを設定してテストする場合は、**公開**&#x200B;をクリックします。

   公開する権限がない可能性があります。 そのような場合は、Copilotの管理者にお問い合わせください。

## Workfrontをカスタム MCP ソリューションに接続する

独自のカスタムアプリケーションやエージェントを構築する場合は、Workfront MCP サーバーに直接接続できます。

連携させる方法は2つあります。

* [サービストークンへの接続](#connect-with-a-service-to-service-token)
* [OAuthへの接続](#connect-with-oauth)

### サービストークンへの接続

1. Adobe Developer Consoleを使用してサービス資格情報を作成します。 詳しくは、[&#x200B; サーバー間の認証](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/)を参照してください。
1. 次の情報を使用して、Workfront MCP サーバーに接続します。

   * **URL**：`https://mcp.workfront.adobe.com/mcp/v1/workfront`
   * **ヘッダー**:

     * `Authorization: Bearer <access_token>`
     * `wf-url: <your_subdomain>.my.workfront.com` （資格情報が複数のWorkfront インスタンス （プレビューや実稼動環境など）にアクセスできる場合は必須）。

### OAuthへの接続

カスタム OAuth統合のセルフサービスサポートは、Workfrontではまだ利用できません。

## 接続を確認

AI エージェント型プラットフォームがWorkfrontに接続されていることを確認するには、AI エージェント型プラットフォームに、Workfront MCP サーバーで使用可能なアクションのリストを依頼します。 例：

* *Workfrontでどのようなアクションを実行できますか？*
* *アクセスできるWorkfront ツールを一覧表示します。*

また、[Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)でツールの完全な一覧を表示することもできます。

## 利用可能なツール

Workfront MCP サーバーは、接続されたAI エージェント型プラットフォームがユーザーに代わって呼び出す一連のツールを公開します。例えば、Workfrontの検索、項目の作成、フィールドの更新、承認の管理を行うツールなどです。 Workfront領域でグループ化された完全な参照リストについては、[Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)を参照してください。

## 別のWorkfront インスタンスへの切り替え

各コネクションは、1つのWorkfront インスタンスに対してAI エージェントプラットフォームを認証します。 別のインスタンスを使用するには、接続を解除して再接続します。

別のWorkfront インスタンスに接続するには：

1. AI エージェント型プラットフォームで、Workfront MCP サーバーを切断します。
1. コネクタを再接続します。
1. 新しいWorkfront インスタンスに認証します。

>[!NOTE]
>
>* ログアウトしても、Workfront インスタンスは切り替わりません。 コネクタを切断して再接続する必要があります。


<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server:  
   ```
   https://mcp.workfront.adobe.com/mcp/v1/workfront|
   
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## セットアップと認証のトラブルシューティング

+++ 展開して、Workfront MCP サーバーのセットアップと認証に関するトラブルシューティングのヒントを表示します。

| 問題 | 考えられる原因 | 修正 |
| --- | --- | --- |
| [!DNL Adobe Workfront] コネクタが[!DNL Claude]に見つかりません。 | [!DNL Claude]管理者が有効にしていません。 | [!DNL Claude]管理者（Workfront管理者ではない）に連絡し、[!DNL Adobe Workfront] コネクタを有効にするように依頼します。 |
| 連携はしていますが、データを見ることはできません。 | 間違ったWorkfront インスタンスに対して認証されました。 | コネクタを取り外し、再接続して、正しいインスタンスに認証します。 |
| 認証に失敗したか、接続が機能しなくなりました。 | 認証セッションの有効期限が切れているか、接続エラーが発生しています。 | コネクタを取り外して再接続します。 |
| 別のWorkfrontインスタンスに切り替える場合。 | 1つの接続で1つのインスタンスに関連付けられます。 | 新しいインスタンスの接続を解除して、再接続し、認証します。 |
| Workfrontに接続できないか、MCP サーバーアクセスが無効になっていることを示すメッセージが表示されます。 | Workfront管理者は、インスタンスのMCP サーバーアクセスをオフにしています。 | Workfront管理者に連絡し、システム環境設定でMCP サーバーアクセスを有効にするように依頼します。 |
| AI エージェント型プラットフォームは、Workfrontのアイテムを見つけることはできますが、作成、更新、削除することはできません。 | Workfront管理者が、Workfront MCP サーバーの書き込みアクションを無効にしています。 | Workfront管理者に連絡し、システム環境設定で書き込みアクションを有効にするように依頼します。 |

接続後の日々のトラブルシューティング（例：古い結果や予期しない動作）については、[Adobe Workfront MCP サーバーの使用](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)を参照してください。


+++

## セットアップに関するよくある質問

+++ 展開すると、Workfront MCP サーバーの設定に関するよくある質問が表示されます。

* [複数のWorkfront インスタンスに同時に接続できますか？](#can-i-connect-to-multiple-workfront-instances-at-the-same-time)
* [どの管理者がこれを有効にしますか？](#which-administrator-enables-this)
* [Adobe Identity Management System （IMS）でWorkfront インスタンスが有効になっていない場合、Workfront MCP サーバーを使用できますか？](#can-i-use-the-workfront-mcp-server-if-my-workfront-instance-isnt-enabled-on-adobe-identity-management-system-ims)

### 複数のWorkfront インスタンスに同時に接続できますか？

いいえ。 各コネクションは、AI エージェント型プラットフォームを1つのWorkfrontインスタンスに結び付けます。 切り替えるには、切断して再接続し、新しいインスタンスに認証します。

### どの管理者がこれを有効にしますか？

Workfrontの管理者とAI エージェントプラットフォームの管理者の両方。 Workfront管理者は、Workfront側でMCP サーバーアクセスを有効にします。 AI エージェントプラットフォームの管理者は、そのプラットフォームの側でWorkfrontへのアクセスを有効にします。 [!DNL Claude]の場合、[!DNL Claude] Enterprise管理者は[!DNL Adobe Workfront] コネクタを有効にします。

### Adobe Identity Management System （IMS）でWorkfront インスタンスが有効になっていない場合、Workfront MCP サーバーを使用できますか？

いいえ。 Workfront MCP サーバーを使用するには、Adobe Identity Management システム（IMS）でWorkfront インスタンスを有効にする必要があります。 インスタンスがIMSで有効になっているかどうかわからない場合は、Workfront管理者にお問い合わせください。

+++ 

