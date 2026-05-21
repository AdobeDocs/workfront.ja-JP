---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP サーバーの使用
description: Adobe Workfront MCP サーバーを使用して、AI エージェント基盤で自然言語の会話を通じてWorkfrontアイテムを検索、作成、更新、管理します。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 1%

---


# Adobe Workfront MCP サーバーの使用

[!DNL Adobe Workfront] MCP サーバーを使用すると、AI エージェント型プラットフォームに簡単な英語で質問して、Workfront アイテムを検索、作成、更新、管理できます。 プラットフォームは、呼び出すWorkfront アクションを決定し、Workfrontとの会話を処理します。

現在、[!DNL Claude]はサポートされているAI エージェント型プラットフォームですが、この記事の例とパターンは、Workfront MCP サーバーをサポートする任意のAI エージェント型プラットフォームに適用されます。

この記事では、接続を既に設定していることを前提としています。 設定について詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)を参照してください。 Workfront MCP サーバーについて詳しくは、[Adobe Workfront MCP サーバーの概要](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)を参照してください。

## 利用可能なツール

Workfront MCP サーバーは、AI エージェント型プラットフォームがユーザーに代わって呼び出す一連のツールを公開します。例えば、Workfrontの検索、項目の作成、フィールドの更新、承認の管理を行うツールがあります。 Workfront領域でグループ化された完全な参照リストについては、[Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)を参照してください。

>[!IMPORTANT]
>
>AI エージェント型プラットフォームをWorkfrontに接続すると、Workfront アカウントと権限を使用してWorkfrontで動作します。 プラットフォームのアクションは、Workfront インターフェイスで直接実行するアクションと同じ効果を持ちます。
>
>AI エージェント型プラットフォームのプロバイダーは、Adobe Workfrontにおけるプラットフォームのアクションに責任を負います。 Adobeは、AI エージェントによるWorkfront データの変更について責任を負いません。
>
>AI エージェント型プラットフォームにリクエストを進める前に、特にデータの変更や削除を行うアクションについて、その意図を理解していることを確認してください。


## 質問する内容の例

連携したら、AI エージェンティックプラットフォームで自然言語のリクエストを入力します。 AI エージェント型プラットフォームは、呼び出すWorkfrontのアクションを決定し、結果を返します。

### 作品の検索と表示

Workfrontで、お探しの商品と一致する商品を検索するには、次の質問を行います。

* *ブランドマーケティングチームのすべてのアクティブなプロジェクトを表示します。*
* *Joan Harrisに割り当てられているすべてのタスクを確認します。*
* *「テクニカル」カテゴリの「Web サイトの再設計」プロジェクトのすべての問題を表示します。*

### 新しい項目を作成

プロジェクト、タスク、またはその他のWorkfront アイテムを作成するには、次の質問を行います。

* *3月10日から4月30日までの期間に「Q2 Innovation Sandbox」という名前の空白プロジェクトを作成します。 所有者として私を設定してください。*
* *ランディングページ QAという新しいタスクをプロジェクトに追加し、4月22日から4月26日までスケジュールします。*
* *Summer Sale 2026という新しいキャンペーンレコードを作成します。&quot;*

### 既存の項目を更新

Workfront内の既存の項目に変更を加えるには、次の操作を行います。

* *4月18日に完了するように「デザインレビュー」タスクを更新し、クリエイティブチームに割り当てます。*
* *「Lucent AI Launch - NA」プロジェクトの場合、4月中旬に終了をプッシュし、予算を$150Kに増やします。*
* *「サマーキャンペーン」レコードの予算フィールドを$75,000に更新します。*

### 項目を削除

Workfrontのアイテムを削除するには、次の質問を行います。

* *「Q1 Test Campaign」という名前のプロジェクトを削除します。*
* *プロジェクトから「アセット制作の印刷」タスクを削除します。*
* *「古いプロモーション」という名前のキャンペーンレコードを削除します。*

>[!WARNING]
>
>AI エージェントプラットフォームを介してWorkfrontのアイテムを削除することは、Workfront インターフェイスでアイテムを削除することと同じです。 AI エージェント型プラットフォームが削除しようとしているものを確認してから、先に進めます。

### 承認の操作

ドキュメントとアセットの承認を管理するには、次の質問を行います。

* *現在の文書にSarah ChenとMiguel Alvarezを承認者として追加します。*
* *応答していないアセット「Spring Campaign Video」の承認者にリマインダーを送信します。*
* *アセット「Spring Campaign Video」に「Marketing Launch」承認テンプレートを適用します。*


### プランニングレコードの操作

プランニングレコードを管理するには、次の質問を行います。

* *ブランドマーケティングチームの「Q2 マーケティングプラン」という新しいプランニングレコードを作成します。*
* *計画レコードに「ソーシャルメディア監査」という新しいタスクを追加します。*
* *4月18日に終了するように「ソーシャルメディア監査」タスクを更新し、クリエイティブ チームに割り当てます。*

### ワークフローの操作

ワークフローを管理するには、次の質問を行います。

* *第2四半期イノベーション サンドボックス プロジェクトをイノベーション レビュー委員会にルーティングします。*
* *サマーキャンペーンのレコードを「準備完了」ステータスに更新します。*
* *「サマーキャンペーン」レコードを承認します。*


### 会話でのリクエストのチェーン

1回の会話でリクエストをチェーン化できます。 AI エージェント型プラットフォームはコンテキストを保持するため、各リクエストは前のリクエストの上に構築できます。 例：

1. 一連のアイテムを要求：*期限切れのタスクを検索します。*
1. リストを取得したら、次の結果に対するアクションを求めます。*すべての結果を次の金曜日に更新します。*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## 考慮事項

Workfront MCP サーバーを使用する場合は、次の点に注意してください。

### AI エージェントプラットフォームは、会話の早い段階で情報を使用する場合があります

AI エージェント型プラットフォームは、Workfrontに最新の情報を依頼するのではなく、会話の早い段階でデータを再利用することがあります。 Workfrontで、AI エージェント型プラットフォームが最後に動作してから何か変化があった場合は、古い情報が表示される可能性があります。

AI エージェントプラットフォームに新しいデータの取得を強制するには、明示的に要求します。 例：

* *Workfrontから最新のデータを取得します。 キャッシュされた結果は使用しません。*

### Workfront MCP サーバーは自動的に更新されます

Adobeが新しいバージョンのWorkfront MCP サーバーをリリースすると、AI エージェンティックプラットフォームは新しいバージョンを自動的に使用します。 システムに再接続したり、変更を加えたりする必要はありません。

## データとセキュリティ

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Workfrontに残るデータ

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### AI エージェント型プラットフォームプロバイダーによるWorkfrontデータの取り扱い

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### AI エージェントプラットフォームの違い

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## 日々の業務に関するトラブルシューティング

+++ 展開すると、Workfront MCP サーバーを日常的に使用するためのトラブルシューティングのヒントが表示されます。

| 問題 | 考えられる原因 | 修正 |
|---|---|---|
| AI エージェントプラットフォームは古い情報を提供しています。 | AI エージェント型プラットフォームは、会話の初期段階で収集したデータを再利用しています。 | Workfrontから取得した最新のデータをご確認ください。 |
| Ai エージェント型プラットフォームが、誤ったWorkfront項目からデータを返しました。 | AI エージェントプラットフォームは、あいまいな表現にもとづいて間違った項目を選択しました。 | より具体的な名前、ID、フィルターを使用して、もう一度質問します。 |
| 更新または削除がWorkfrontで有効になりません。 | AI エージェント型プラットフォームがまだアクションを呼び出していないか、権限で許可されていません。 | アクションが実行されたAI エージェント型プラットフォームで確認し、Workfront権限を確認します。 |

セットアップと認証の問題について詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)の「[&#x200B; セットアップと認証のトラブルシューティング &#x200B;](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)」を参照してください。

+++

## よくある質問

+++ 展開すると、Workfront MCP サーバーの使用に関するよくある質問が表示されます。

### AI エージェントプラットフォームを通じて使用できるWorkfrontのアイテムは何ですか？

アクセスレベルとオブジェクト権限を介してWorkfrontでアクセスできる項目。

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Workfrontのデータは、AI エージェントプラットフォームプロバイダーに送信されるか、プロバイダーによって保存されますか？

詳しくは、この記事の「[&#x200B; データとセキュリティ &#x200B;](#data-and-security)」を参照してください。

### Workfront MCP サーバーの新しいバージョンがリリースされたときはどうなりますか？

MCP サーバーが自動的に更新されます。 何かを再接続したり変更したりする必要はありません。

### Workfront MCP サーバーを使用するには、Workfront APIを知る必要がありますか？

いいえ。 AI エージェント型プラットフォームは、自然言語のリクエストを適切なWorkfrontアクションに変換します。 Workfront APIに慣れ親しんでいる場合、そのアクションに慣れていると感じられるかもしれませんが、必須ではありません。

+++
