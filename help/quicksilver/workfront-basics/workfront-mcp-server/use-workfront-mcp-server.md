---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP サーバーの使用
description: Adobe Workfront MCP サーバーを使用して、AI アシスタントで自然言語の会話を通じてWorkfrontアイテムを検索、作成、更新、管理します。
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 2%

---


# Adobe Workfront MCP サーバーの使用

[!DNL Adobe Workfront] MCP サーバーでは、AI アシスタントに簡単な英語で質問することで、Workfrontのアイテムを検索、作成、更新、管理できます。 AI アシスタントが、Workfrontのどのアクションを呼び出すかを決定し、Workfrontとのやり取りを処理します。

現在、サポートされているAI アシスタントは[!DNL Claude]のみですが、この記事の例とパターンは、Workfront MCP サーバーをサポートしているすべてのAI アシスタントに適用されます。

この記事では、接続を既に設定していることを前提としています。 設定について詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)を参照してください。 Workfront MCP サーバーについて詳しくは、[Adobe Workfront MCP サーバーの概要](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)を参照してください。



## Workfront MCP サーバーを通じて使用可能なアクション

Workfront MCP サーバーは、承認、計画、ワークフローをまたいだアクションをカバーします。

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>Workfront アカウントと権限を使用して、WorkfrontでAI アシスタントが動作します。 AI アシスタントプロバイダーは、AI アシスタントが代わりに実行するアクションに責任を負います。 AI アシスタントが何をしようとしているかを確認してから先へ進めます。


## AI アシスタントのアクションに対する責任

AI アシスタントをWorkfrontに接続すると、AI アシスタントは、Workfront アカウントと権限を使用してWorkfrontで動作します。 AI アシスタントのアクションは、Workfront インターフェイスで直接実行するアクションと同じ効果を持ちます。

WorkfrontでAI アシスタントが実行するアクションは、お客様とAI アシスタントプロバイダーが責任を負います。 Adobeは、AI アシスタントがWorkfront データに加えた変更について責任を負いません。

AI アシスタントにリクエストを進める前に、特にデータの変更や削除を行うアクションについて、その意図を理解していることを確認してください。

### 主要アクション

Workfront MCP サーバーには、次のコアアクションが含まれています。

| アクション | 機能 |
|---|---|
| 作成 | Workfrontで新しい項目を作成します。 |
| 検索 | Workfrontから項目を検索して取得します。 |
| 更新 | Workfrontの既存の項目を変更します。 |
| 削除 | Workfrontから項目を削除します。 |
| フィールド名を解決 | AI アシスタントがデータに対する正確なリクエストを作成できるように、正しいWorkfrontフィールド名を検索します。 |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### 承認アクション

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### アクションの計画

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### ワークフローのアクション

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## 質問する内容の例

接続したら、AI アシスタントに自然言語のリクエストを入力します。 AI アシスタントは、呼び出すWorkfront アクションを決定し、結果を返します。

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### 作品の検索と表示

AI アシスタントに対して、Workfrontで目的に一致する商品を検索するように依頼します。 例：

* *ブランドマーケティングチームのすべてのアクティブなプロジェクトを表示します。*
* *Joan Harrisに割り当てられているすべてのタスクを確認します。*
* *「テクニカル」カテゴリの「Web サイトの再設計」プロジェクトのすべての問題を表示します。*

### 新しい項目を作成

プロジェクト、タスク、その他のWorkfront アイテムの作成をAI アシスタントに依頼します。 例：

* *3月10日から4月30日までの期間に「Q2 Innovation Sandbox」という名前の空白プロジェクトを作成します。 所有者として私を設定してください。*
* *ランディングページ QAという新しいタスクをプロジェクトに追加し、4月22日から4月26日までスケジュールします。*
* *Summer Sale 2026という新しいキャンペーンレコードを作成します。&quot;*

### 既存の項目を更新

Workfront内の既存の項目に変更を加えるように、AI アシスタントに依頼します。 例：

* *4月18日に完了するように「デザインレビュー」タスクを更新し、クリエイティブチームに割り当てます。*
* *「Lucent AI Launch - NA」プロジェクトの場合、4月中旬に終了をプッシュし、予算を$150Kに増やします。*
* *「サマーキャンペーン」レコードの予算フィールドを$75,000に更新します。*

### 項目を削除

AI アシスタントに、Workfrontの項目を削除するように依頼します。 例：

* *「Q1 Test Campaign」という名前のプロジェクトを削除します。*
* *プロジェクトから「アセット制作の印刷」タスクを削除します。*
* *「古いプロモーション」という名前のキャンペーンレコードを削除します。*

>[!WARNING]
>
>AI アシスタントを使用してWorkfrontの項目を削除することは、Workfront インターフェイスで項目を削除することと同じです。 AI アシスタントが削除しようとしているものを確認してから続行します。

### 承認の操作

AI アシスタントに、ドキュメントとアセットの承認を管理するように依頼します。 例：

* *現在の文書にSarah ChenとMiguel Alvarezを承認者として追加します。*
* *応答していないアセット「Spring Campaign Video」の承認者にリマインダーを送信します。*
* *アセット「Spring Campaign Video」に「Marketing Launch」承認テンプレートを適用します。*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### プランニングレコードの操作

AI アシスタントに、プランニングレコードの管理を依頼します。 例：

* *ブランドマーケティングチームの「Q2 マーケティングプラン」という新しいプランニングレコードを作成します。*
* *計画レコードに「ソーシャルメディア監査」という新しいタスクを追加します。*
* *4月18日に終了するように「ソーシャルメディア監査」タスクを更新し、クリエイティブ チームに割り当てます。*

### ワークフローの操作

AI アシスタントにワークフロー管理を依頼する。 例：

* *第2四半期イノベーション サンドボックス プロジェクトをイノベーション レビュー委員会にルーティングします。*
* *サマーキャンペーンのレコードを「準備完了」ステータスに更新します。*
* *「サマーキャンペーン」レコードを承認します。*


### 会話でのリクエストのチェーン

1回の会話でリクエストをチェーン化できます。 AI アシスタントはコンテキストを保持するため、各リクエストは前のリクエストの上に構築できます。 例：

1. AI アシスタントに一連の項目を検索するように依頼します：*期限切れのタスクを検索します。*
1. AI アシスタントがリストを返したら、その結果に基づいて処理するように依頼します。*すべての結果を次の金曜日に更新します。*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## 考慮事項

Workfront MCP サーバーを使用する場合は、次の点に注意してください。

### AI アシスタントは、会話の初期段階にある情報を使用して

AI アシスタントは、Workfrontに最新の情報を依頼するのではなく、会話の早い段階でデータを再利用することがあります。 AI アシスタントが最後に表示してからWorkfrontで何かが変更された場合は、古い情報が表示される可能性があります。

AI アシスタントに新しいデータの取得を強制するには、明示的に要求します。 例：

* *Workfrontから最新のデータを取得します。 キャッシュされた結果は使用しません。*

### Workfront MCP サーバーは自動的に更新されます

Adobeが新しいバージョンのWorkfront MCP サーバーをリリースすると、AI アシスタントは新しいバージョンを自動的に使用します。 システムに再接続したり、変更を加えたりする必要はありません。

## データとセキュリティ

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Workfrontに残るデータ

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### AI アシスタントプロバイダーによるWorkfrontデータの扱い方

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### AI アシスタントの相違点

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## 日々の業務に関するトラブルシューティング

セットアップと認証の問題について詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)の「[&#x200B; セットアップと認証のトラブルシューティング &#x200B;](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)」を参照してください。

| 問題 | 考えられる原因 | 修正 |
|---|---|---|
| AI アシスタントが古い情報を提供しています。 | AI アシスタントは、会話の早い段階で収集したデータを再利用しています。 | AI アシスタントに、Workfrontから新しいデータを取得するように依頼します。 |
| AI アシスタントが間違ったWorkfront項目からデータを返しました。 | AI アシスタントは、あいまいな表現にもとづいて間違った項目を選択しました。 | より具体的な名前、ID、フィルターを使用して、もう一度質問します。 |
| 更新または削除がWorkfrontで有効になりません。 | AI アシスタントがまだアクションを呼び出していないか、権限で許可されていません。 | アクションが実行されたことをAI アシスタントに確認してから、Workfrontの権限を確認します。 |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## よくある質問

### AI アシスタントを通じて使用できるWorkfrontの項目は何ですか？

アクセスレベルとオブジェクト権限を介してWorkfrontでアクセスできる項目。

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Workfrontのデータは、AI アシスタントプロバイダーに送信されるか、プロバイダーによって保存されますか？

詳しくは、この記事の「[&#x200B; データとセキュリティ &#x200B;](#data-and-security)」を参照してください。

### Workfront MCP サーバーの新しいバージョンがリリースされたときはどうなりますか？

MCP サーバーが自動的に更新されます。 何かを再接続したり変更したりする必要はありません。

### Workfront MCP サーバーを使用するには、Workfront APIを知る必要がありますか？

いいえ。 AI アシスタントは、自然言語のリクエストをWorkfrontでの適切なアクションに変換します。 Workfront APIに慣れ親しんでいる場合、そのアクションに慣れていると感じられるかもしれませんが、必須ではありません。
