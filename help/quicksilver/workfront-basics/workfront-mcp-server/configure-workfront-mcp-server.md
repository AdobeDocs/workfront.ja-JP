---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP サーバーの設定
description: WorkfrontインスタンスとAI エージェント型プラットフォームを設定することで、自然言語の会話を通じてWorkfrontと連携できます。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---


# Adobe Workfront MCP サーバーの設定

[!DNL Adobe Workfront] MCP サーバーを使用すると、ClaudeやChatGPTなどのサポートされているAI エージェント型プラットフォームで、自然言語の会話を通じてWorkfront データを操作できます。

AI エージェント型プラットフォームをWorkfrontに接続する前に、Workfront管理者がWorkfront インスタンスでMCP サーバーアクセスを有効にする必要があります。 AI エージェント型プラットフォームを接続する正確な手順は、サポートされているAI エージェント型プラットフォームごとに異なります。

Workfront MCP サーバーについて詳しくは、[Adobe Workfront MCP サーバーの概要](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)を参照してください。

## サポートされているAI エージェント型プラットフォーム

Workfront MCP サーバーは現在、次のAI エージェント プラットフォームをサポートしています。

* [!DNL Claude]
* [!DNL ChatGPT]

## 前提条件

WorkfrontをAI エージェント型プラットフォームに接続する前に、次の手順を実行する必要があります。

* 操作するデータにアクセスする権限を持つアクティブな[!DNL Adobe Workfront] アカウントを持っています。
* [!DNL Claude]のようなAI エージェンティック プラットフォームにアクセスできます。

### 管理者の前提条件

MCP サーバーアクセスは、2人の別々の管理者によってゲートされます。

* **Workfront管理者**&#x200B;は、Workfront インスタンスのMCP サーバーアクセスを制御します。 システム環境設定では、アクセスはデフォルトで有効になっているので、管理者が無効にするように選択していない限り、アクションは必要ありません。<!-- TODO: link to the System Preferences AI preferences article once the Enable MCP toggle is documented there. -->

* エンタープライズ版のAI エージェント型プラットフォームを使用する場合、そのプラットフォームの管理者は、組織の[!DNL Adobe Workfront] コネクタを有効にする必要があります。


## WorkfrontとClaudeの連携

Workfrontへの接続は、[!DNL Claude] アカウントごとに1回です。 接続によって特定のWorkfront インスタンスが認証され、切断するまで接続が維持されます。

### Connectors ディレクトリから接続する

+++ 展開すると、Workfrontを[!DNL Claude]に接続するための手順が表示されます。

Workfrontを[!DNL Claude]に接続するには：

1. [!DNL Claude] を開きます。.

1. コネクタ領域に移動します。

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. コネクタリストで&#x200B;**[!DNL Adobe Workfront]**&#x200B;を検索します。

   表示されない場合は、この記事の「[管理者の前提条件](#admin-prerequisites)」を参照してください。

1. 「**接続**」をクリックします。

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. プロンプトが表示されたら、Workfront インスタンスにログインします。

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. 認証が完了したら、接続されます。

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

+++

### URLへの接続

+++ 展開すると、URLを使用してWorkfrontを[!DNL Claude]に接続するための手順ごとの手順が表示されます。

URLを使用してWorkfrontを[!DNL Claude]に接続するには：

1. 資格情報を使用して[Claude](https://claude.ai)にログインします。
1. 左側のメニューで、**カスタマイズ** アイコンを選択します。
1. **コネクタ**&#x200B;を選択し、**+** アイコンを選択してコネクタを追加します。
1. 「**アプリを作成**」ボタンを選択します。
1. コネクタに目的の名前（「Workfront」など）を付け、目的のMCP Server URLを入力します：`https://mcp.workfront.adobe.com/mcp/v1/workfront`

1. コネクタを作成すると、ログインウィンドウがポップアップ表示されます。 Adobe IDの認証情報を使用して認証します。 複数に属している場合は、必ず目的のWorkfront インスタンスを選択してください。

+++

### Claudeの行動をスキルでカスタマイズする

[!DNL Claude]は、スキルと呼ばれるユーザー作成の命令セットをサポートしています。 Workfrontでは、スキルを使用して[!DNL Claude]の動作をカスタマイズできます。 例えば、以前の結果に頼るのではなく、常にWorkfrontから新しいデータを取得するように[!DNL Claude]に指示するスキルを作成できます。

[!DNL Claude] スキルについて詳しくは、[Claude ユーザードキュメント &#x200B;](https://code.claude.com/docs/en/skills)を参照するか、Claudeにスキルに関するヘルプを依頼してください。

## ChatGPTへの接続

1. 資格情報を使用して[ChatGPT](https://chatgpt.com)にログインします。
1. 左下で、**あなたの名前** → **設定**&#x200B;を選択します。
1. **アプリ**&#x200B;を選択し、**開発者モード**&#x200B;を有効にします。
1. 「**アプリを作成**」ボタンを選択します。
1. アプリに目的の名前（「Workfront」など）を付け、目的のMCP Server URLを入力します：`https://mcp.workfront.adobe.com/mcp/v1/workfront`
1. 認証が&#x200B;**OAuth** （デフォルトで設定）に設定されていることを確認し、「承認」チェックボックスをオンにして続行します。
1. アプリが作成されると、ログインウィンドウがポップアップ表示されます。 Adobe IDの認証情報を使用して認証します。 複数に属している場合は、必ず目的のWorkfront インスタンスを選択してください。

### カスタム GPTでChatGPTの動作をカスタマイズ

ChatGPTは、カスタム GPTと呼ばれるユーザー作成アシスタントをサポートしています。 カスタム GPTを使用して、ChatGPTがコネクタでどのように動作するかをカスタマイズできます。 例えば、以前の結果に頼るのではなく、接続されたサービスから常に新しいデータを取得するようにChatGPTに指示するカスタム GPTを作成できます。

カスタム GPTについて詳しくは、[ChatGPT ユーザードキュメント &#x200B;](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)を参照するか、カスタム GPTのヘルプをChatGPTに依頼してください。

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
>ログアウトしても、Workfront インスタンスは切り替わりません。 コネクタを切断して再接続する必要があります。

<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
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
|---|---|---|
| [!DNL Adobe Workfront] コネクタが[!DNL Claude]に見つかりません。 | [!DNL Claude]管理者が有効にしていません。 | [!DNL Claude]管理者（Workfront管理者ではない）に連絡し、[!DNL Adobe Workfront] コネクタを有効にするように依頼します。 |
| 連携はしていますが、データを見ることはできません。 | 間違ったWorkfront インスタンスに対して認証されました。 | コネクタを取り外し、再接続して、正しいインスタンスに認証します。 |
| 認証に失敗したか、接続が機能しなくなりました。 | 認証セッションの有効期限が切れているか、接続エラーが発生しています。 | コネクタを取り外して再接続します。 |
| 別のWorkfrontインスタンスに切り替える場合。 | 1つの接続で1つのインスタンスに関連付けられます。 | 新しいインスタンスの接続を解除して、再接続し、認証します。 |
| Workfrontに接続できないか、MCP サーバーアクセスが無効になっていることを示すメッセージが表示されます。 | Workfront管理者は、インスタンスのMCP サーバーアクセスをオフにしています。 | Workfront管理者に連絡し、システム環境設定でMCP サーバーアクセスを有効にするように依頼します。 |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

接続後の日々のトラブルシューティング（例：古い結果や予期しない動作）については、[Adobe Workfront MCP サーバーの使用](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)を参照してください。


+++


<!--
+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at once?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++

-->