---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP サーバーの設定
description: WorkfrontインスタンスとAI アシスタントを設定することで、自然言語の会話を通じてWorkfrontと作業できるようになります。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 5%

---


# Adobe Workfront MCP サーバーの設定

[!DNL Adobe Workfront] MCP サーバーを使用すると、ClaudeやChatGPTなどのサポート対象AI アシスタントで、自然言語の会話を通じてWorkfront データを操作できます。

AI アシスタントをWorkfrontに接続する前に、Workfront管理者がWorkfront インスタンスでMCP サーバーアクセスを有効にする必要があります。 AI アシスタントを連携させる手順は、サポートされるAI アシスタントごとに異なります。

Workfront MCP サーバーについて詳しくは、[Adobe Workfront MCP サーバーの概要](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)を参照してください。

## サポートされているAI アシスタント

Workfront MCP サーバーは現在、次のAI アシスタントをサポートしています。

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

WorkfrontをAI アシスタントに接続する前に、次のことをおこなう必要があります。

* 操作するデータにアクセスする権限を持つアクティブな[!DNL Adobe Workfront] アカウントを持っています。
* [!DNL Claude]のようなAI アシスタントにアクセスできます。

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### 管理者の前提条件

MCP サーバーアクセスは、2人の別々の管理者によってゲートされます。 接続する前に、両方ともアクセスを有効にする必要があります。

* **Workfront管理者**&#x200B;は、Workfront インスタンスでMCP サーバーアクセスを有効にする必要があります。

* エンタープライズ版のAI アシスタントを使用する場合、AI アシスタント管理者は、組織の[!DNL Adobe Workfront] コネクタを有効にする必要があります。


## WorkfrontとClaudeの連携

Workfrontへの接続は、[!DNL Claude] アカウントごとに1回です。 接続によって特定のWorkfront インスタンスが認証され、切断するまで接続が維持されます。


>[!IMPORTANT]
>
>[!DNL Claude] Enterpriseを使用している場合、**お使いの[!DNL Claude] Enterprise管理者**&#x200B;はお使いの組織で[!DNL Adobe Workfront] コネクタを有効にする必要があります。 それまでは、[!DNL Claude]で検索しても[!DNL Adobe Workfront] コネクタは表示されません。 最初に[!DNL Claude]管理者にお問い合わせください。


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

### 接続を確認

[!DNL Claude]がWorkfrontに接続されていることを確認するには、[!DNL Claude]に対して、Workfront MCP サーバーで使用可能なアクションの一覧を表示するように依頼します。 例：

* *Workfrontでどのようなアクションを実行できますか？*
* *アクセスできるWorkfront ツールを一覧表示します。*

[!DNL Claude]は、使用可能なアクションのリストを返します。

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### 別のWorkfront インスタンスへの切り替え

各接続は、1つのWorkfront インスタンスに[!DNL Claude]を認証します。 別のインスタンスを使用するには、接続を解除して再接続します。

別のWorkfront インスタンスに接続するには：

1. [!DNL Claude]で、[!DNL Adobe Workfront] コネクタを切断します。
1. コネクタを再接続します。
1. 新しいWorkfront インスタンスに認証します。

>[!NOTE]
>
>[!DNL Claude]からログアウトしても、Workfront インスタンスは切り替わりません。 コネクタを切断して再接続する必要があります。

## Claudeの行動をスキルでカスタマイズする

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude]は、スキルと呼ばれるユーザー作成の命令セットをサポートしています。 Workfrontでは、スキルを使用して[!DNL Claude]の動作をカスタマイズできます。 例えば、以前の結果に頼るのではなく、常にWorkfrontから新しいデータを取得するように[!DNL Claude]に指示するスキルを作成できます。

## セットアップと認証のトラブルシューティング

| 問題 | 考えられる原因 | 修正 |
|---|---|---|
| [!DNL Adobe Workfront] コネクタが[!DNL Claude]に見つかりません。 | [!DNL Claude]管理者が有効にしていません。 | [!DNL Claude]管理者（Workfront管理者ではない）に連絡し、[!DNL Adobe Workfront] コネクタを有効にするように依頼します。 |
| 連携はしていますが、データを見ることはできません。 | 間違ったWorkfront インスタンスに対して認証されました。 | コネクタを取り外し、再接続して、正しいインスタンスに認証します。 |
| 認証に失敗したか、接続が機能しなくなりました。 | 認証セッションの有効期限が切れているか、接続エラーが発生しています。 | コネクタを取り外して再接続します。 |
| 別のWorkfrontインスタンスに切り替える場合。 | 1つの接続で1つのインスタンスに関連付けられます。 | 新しいインスタンスの接続を解除して、再接続し、認証します。 |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

接続後の日々のトラブルシューティング（例：古い結果や予期しない動作）については、[Adobe Workfront MCP サーバーの使用](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)を参照してください。

## セットアップに関するよくある質問

### 一度に複数のWorkfront インスタンスに接続できますか？

いいえ。 各接続は、AI アシスタントを1つのWorkfrontインスタンスに結び付けます。 切り替えるには、切断して再接続し、新しいインスタンスに認証します。

### これはClaude ProまたはClaude Teamで機能しますか、それともClaude Enterpriseでのみ機能しますか？

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### どの管理者がこれを有効にしますか？

Workfront管理者とAI アシスタント管理者の両方が対象です。 Workfront管理者は、Workfront側でMCP サーバーアクセスを有効にします。 AI アシスタント管理者は、AI アシスタント側でWorkfrontへのアクセスを有効にします。 [!DNL Claude]の場合、[!DNL Claude] Enterprise管理者は[!DNL Adobe Workfront] コネクタを有効にします。
