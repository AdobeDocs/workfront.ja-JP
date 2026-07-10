---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Adobe Workfront MCP サーバーの使用
description: Adobe Workfront MCP サーバーを使用して、AI エージェント基盤で自然言語の会話を通じてWorkfrontアイテムを検索、作成、更新、管理します。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 5592c1b93b5e44c732f92d626ed878d2c4647ceb
workflow-type: tm+mt
source-wordcount: '1896'
ht-degree: 2%

---


# Adobe Workfront MCP サーバーの使用

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 プレビューサンドボックス環境でのみ使用できます。</span>

[!DNL Adobe Workfront] MCP サーバーでは、AI エージェント型プラットフォームに自然言語で質問することで、Workfront アイテムを検索、作成、更新、管理できます。 プラットフォームは、呼び出すWorkfront アクションを決定し、Workfrontとの会話を処理します。

>[!IMPORTANT]
>
>現在、Workfront MCP サーバーは、AWSを使用しているお客様のみが利用できます。

## 前提条件

* AI エージェント型プラットフォームとWorkfront MCP サーバー間の接続を設定する必要があります。 設定手順については、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)を参照してください。
* Workfront インスタンスは、Adobe Identity Management システム（IMS）で有効にする必要があります。
* 操作する項目に必要なアクセス レベルとオブジェクト権限を持つWorkfront アカウントが必要です。
* MCPをWorkfront Planningで使用するには、Adobe Workfront Planningを含むWorkfront パッケージに属している必要があります。

この記事では、接続を既に設定していることを前提としています。 設定について詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)を参照してください。

## 利用可能なツール

Workfront MCP サーバーは、AI エージェントプラットフォームがユーザーに代わって呼び出す一連のツールを公開します。 たとえば、Workfrontの検索、項目の作成、フィールドの更新、承認の管理などを行うツールがあります。 完全な参照リストについては、[Adobe Workfront MCP server tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md)を参照してください。

>[!IMPORTANT]
>
>AI エージェント型プラットフォームをWorkfrontに接続すると、Workfront アカウントと権限を使用してWorkfrontで動作します。 プラットフォームのアクションは、Workfront インターフェイスで直接実行するアクションと同じ効果を持ちます。<br>
>
>AI エージェント型プラットフォームのプロバイダーは、Adobe Workfrontにおけるプラットフォームのアクションに責任を負います。 Adobeは、AI エージェント プラットフォームがWorkfront データに加える変更について責任を負いません。<br>
>
>AI エージェント型プラットフォームにリクエストを進める前に、特にデータの変更や削除を行うアクションについて、その意図を理解していることを確認してください。


## 質問する内容の例

連携したら、AI エージェンティックプラットフォームで自然言語のリクエストを入力します。 AI エージェント型プラットフォームは、呼び出すWorkfrontのアクションを決定し、結果を返します。

>[!NOTE]
>
>Workfrontの設定領域の管理者コントロールが原因で、一部のアクションが使用できない場合があります。 例えば、Workfront管理者がMCP サーバーの書き込みアクションを無効にしている場合、項目を作成できない可能性があります。


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

<!--
* *Remove Anna Jones from all approvals in this project, and replace with Sione Carter.*
-->


### プランニングレコードの操作

>[!IMPORTANT]
>
>* MCPをWorkfront Planningで使用するには、Adobe Workfront Planningを含むWorkfront パッケージに属している必要があります。

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


## 考慮事項

Workfront MCP サーバーを使用する場合は、次の点に注意してください。

### AI エージェントプラットフォームは、会話の早い段階で情報を使用する場合があります

AI エージェント型プラットフォームは、Workfrontに最新の情報を依頼するのではなく、会話の早い段階でデータを再利用することがあります。 Workfrontで、AI エージェント型プラットフォームが最後に動作してから何か変化があった場合は、古い情報が表示される可能性があります。

AI エージェントプラットフォームに新しいデータの取得を強制するには、明示的に要求します。 例：

* *Workfrontから最新のデータを取得します。 キャッシュされた結果は使用しません。*

### Workfront MCP サーバーの更新を確認します

Workfront MCP サーバーへの接続を定期的に更新して、最新のツールと機能を使用していることを確認することをお勧めします。

ほとんどの更新は自動的に行われるはずです。 ただし、Workfront リリースノートを定期的に確認することをお勧めします。


## データとセキュリティ

WorkfrontのMCP サーバーツールは、API呼び出しの仕組みと一致しています。 Workfrontには、プロンプト、応答、その他のデータは保存されません。 Workfrontから必要なデータには、Workfrontのプラットフォームからアクセスできます。

アクセスレベルとオブジェクトの権限によって、Workfrontに対してクエリまたは書き込むことができる内容が決まります。 Workfront管理者は、Workfrontの設定領域でMCPの読み取りおよび書き込みアクションを制御できます。

### Workfrontに残るデータ

AI エージェントプラットフォームプロバイダーは、Workfront MCP サーバーを介して操作したWorkfront データにアクセスできます。 詳しくは、AI エージェントプラットフォームプロバイダーにお問い合わせください。


### AI エージェント型プラットフォームプロバイダーによるWorkfrontデータの取り扱い

Workfrontでは、AI エージェンティック プラットフォーム プロバイダーがWorkfront データを処理する方法を制御できません。 詳しくは、AI エージェントプラットフォームプロバイダーにお問い合わせください。

## 日々の業務に関するトラブルシューティング

+++ 展開すると、Workfront MCP サーバーを日常的に使用するためのトラブルシューティングのヒントが表示されます。

| 問題 | 考えられる原因 | 修正 |
| --- | --- | --- |
| AI エージェントプラットフォームは古い情報を提供しています。 | AI エージェント型プラットフォームは、会話の初期段階で収集したデータを再利用しています。 | Workfrontから取得した最新のデータをご確認ください。 |
| Ai エージェント型プラットフォームが、誤ったWorkfront項目からデータを返しました。 | AI エージェントプラットフォームは、あいまいな表現にもとづいて間違った項目を選択しました。 | より具体的な名前、ID、フィルターを使用して、もう一度質問します。 |
| 更新または削除がWorkfrontで有効になりません。 | Workfront管理者がWorkfront MCP サーバーの書き込みアクションを無効にしているか、特定の項目に対してアクションを実行する権限がありません。 | アクションが実行されたAI エージェント型プラットフォームと確認します。 次に、Workfront MCP サーバーに対する書き込みアクションが有効になっており、項目を変更する権限があることを確認します。 |

セットアップと認証の問題について詳しくは、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)の「[ セットアップと認証のトラブルシューティング ](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication)」を参照してください。

+++

## よくある質問

+++ 展開すると、Workfront MCP サーバーの使用に関するよくある質問が表示されます。

### AI エージェント型プラットフォームとは何ですか？

AI エージェントプラットフォームは、企業の代わりにアクションを実行できるAI ツールです
その他のシステムではなく、質問に答えること。 Workfrontに接続すると
mcp サーバーを通じて、Workfrontを検索、作成、更新、削除できます
あなたが自然言語で尋ねたものに基づいてアイテム。 例えば、Claude
デスクトップ、ChatGPT、その他のMCP対応AI クライアント：


### Workfront MCP サーバーを使用するには、Workfront管理者である必要がありますか？

いいえ。 Workfrontのユーザーは、接続されたMCPを介してWorkfront MCP サーバーを使用できます
AI エージェント型プラットフォーム： Workfrontを使用してアクションを実行します
アカウント、アクセスレベル、オブジェクトの権限を管理できるので
Workfrontで直接行うことができます。

### AI エージェントプラットフォームが自分のアイテムを作成、更新、削除できないのはなぜですか？

Workfront管理者は、で許可されるMCP アクションを制御します
Workfront設定エリア。 書き込みアクションが無効な場合、AI エージェンティックプラットフォーム
Workfrontのアイテムを検索して読み取ることができますが、変更を行うことはできません。 あなたも
特定の項目に対する適切なアクセスレベルとオブジェクト権限が必要です
パートナーです。

### AI エージェント型プラットフォームは、Workfrontデータを変更または削除する前に私に尋ねますか？

それは、Workfrontではなく、AI エージェント型プラットフォームに依存します。 主要プラットフォーム
特に削除の場合は、アクションを実行する前に確認するように促します。リクエストを承認する前に、プラットフォームがこれから行うことをお読みください
Workfrontでの変更は、変更した場合と同じように行われます
自分自身をインターフェイスに追加し。

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### AI エージェント型プラットフォームが間違ったWorkfront商品を返すのはなぜですか？

AI エージェントは、使用した単語にもとづいてアイテムを選択します。 最初の
リクエストがあいまいです。例えば、2つのプロジェクトの名前が似ています
間違ったものを選ぶかもしれません。 より具体的な名前、ID、日付で再度質問し，
フィルターを使用して結果を絞り込むこともできます。


### AI エージェントプラットフォームを通じて使用できるWorkfrontのアイテムは何ですか？

Workfrontでアクセスできるすべての項目は、アクセスレベルおよび
オブジェクトの権限： これには、プロジェクト、タスク、イシュー、ドキュメント，
様々な機能を利用できます。

### AI エージェント型プラットフォームと私の会話を他の人に見せることはできますか？

Workfrontに、プロンプトやAI エージェンティックプラットフォームの応答が保存されることはありません。AI エージェント型プラットフォームを提供する誰もが、会話の流れを制御できます
保存または共有されています。 AI エージェント型プラットフォームのプロバイダーに次の項目について確認します
詳細：

### 使用するWorkfront APIまたはMCP ツールを知る必要がありますか？

いいえ。 AI エージェント型プラットフォームは、自然言語のリクエストを
適切なWorkfrontアクションとツールを選ぶことです。 自社が
Workfront APIに慣れ親しんでいると、アクションは，
これは要件ではありません。

### Workfrontのデータは、AI エージェントプラットフォームプロバイダーに送信されるか、プロバイダーによって保存されますか？

詳しくは、この「[ データとセキュリティ ](#data-and-security)」を参照してください
ガイド。

### Workfront MCP サーバーの新しいバージョンがリリースされたときはどうなりますか？

通常、MCP サーバーは自動的に更新されますが、最新のツールや機能を確認するには、MCP サーバーへの接続を頻繁に更新する必要がある場合があります。

### Adobe Identity Management System （IMS）でWorkfront インスタンスが有効になっていない場合、Workfront MCP サーバーを使用できますか？

いいえ。 Workfront MCP サーバーを使用するには、Adobe Identity Management システム（IMS）でWorkfront インスタンスを有効にする必要があります。 インスタンスがIMSで有効になっているかどうかわからない場合は、Workfront管理者にお問い合わせください。


+++
