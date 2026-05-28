---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP サーバーの概要
description: Adobe Workfront MCP サーバーの機能と、AI エージェント型プラットフォームで自然言語の会話を通じてWorkfrontを使用する方法について説明します。
author: Courtney
feature: Get Started with Workfront
source-git-commit: f96afd17e9f4e726ac545a9cb0c54ace5a4fcffe
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Adobe Workfront MCP サーバーの概要

{{highlighted-preview-article-level}}

[!DNL Adobe Workfront] MCP サーバーは、Workfront インスタンスを[!DNL Claude]や[!DNL ChatGPT]などのAI エージェント プラットフォームに接続します。 Ai エージェント基盤から、自然言語のリクエストを行うことで、Workfrontアイテムを検索、作成、更新、管理できます。

例えば、次のように求めることができます。

* *ブランドマーケティングチームのすべてのアクティブなプロジェクトを表示します。*
* *4月18日に完了するように、「デザインレビュー」タスクを更新します。*
* *応答していないアセット「Spring Campaign Video」の承認者にリマインダーを送信します。*

Workfront APIや、MCP サーバーがWorkfront MCP サーバーを使用する仕組みを知る必要はありません。

>[!IMPORTANT]
>
>現在、Workfront MCP サーバーは、AWSを使用しているお客様の米国のお客様のみが利用できます。

## MCP サーバーとは

MCP サーバーは、AI エージェンティックプラットフォームを別のシステムと連携させる接続ポイントです。 Workfront MCP サーバーは、AI エージェント型プラットフォームの接続先であり、Workfrontデータを読み取り、代わりに処理することができます。

MCPとは、Model Context Protocolの略。 これは、AI エージェントプラットフォームと外部システムが互いにどのように連携するかを定義する標準です。

## 接続の設定

Workfront MCP サーバーは、[!DNL Claude]や[!DNL ChatGPT]など、MCPと互換性のあるAI エージェンティック プラットフォームで動作します。 使用する前に、次のことが必要です。

* Workfront管理者は、Workfront インスタンスでMCP サーバーアクセスを有効にする必要があります。
* お客様（または管理者）は、AI エージェントプラットフォームをWorkfrontに接続する必要があります。

詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)を参照してください。

## Workfront MCP サーバーの使用を開始する

Workfrontを設定したら、AI エージェントに自然言語でアセットの検索、作成、更新、管理を依頼できます。

リクエストの例、念頭に置くべきこと、データとセキュリティに関する詳細については、[Adobe Workfront MCP サーバーの使用](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)を参照してください。