---
title: 2026年第3四半期リリース期間中のその他の機能強化
description: 2026年第3四半期リリース期間中のその他の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 937b49b44f102fee6c9847ab950eb2b274aee89b
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 1%

---

# 2026年第3四半期リリース期間中のその他の機能強化

このページでは、2026年第3四半期リリースのプレビュー環境に対する機能強化について説明します。 これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2026年第3四半期のリリースサイクルで現時点で利用可能なすべての変更のリストについては、[2026年第3四半期のリリースの概要](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-release-overview.md)を参照してください。

## Workfront MCP コネクタの更新

Workfront MCP コネクタに次の更新を行いました。

* MCP サーバーを拡張して、EU<!-- and US instances that are not on AWS. Each MCP server can only connect to one instance, but are no longer limited to US instances on AWS-->内のインスタンスで動作するようにしました。
* Workfront MCP コネクタの柔軟性を拡大するために、Claudeを接続する機能を追加しました。 これで、ClaudeのコネクタのリストにWorkfrontが表示されるか、URLを使用して直接接続できます。

詳細と手順については、[Adobe Workfront MCP サーバーの設定](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md)を参照してください。


## コメント通知メールのルックアンドフィールを更新しました

>[!NOTE]
>
>お客様向け実稼動リリース：2026年7月16日（PT）から段階的に展開

「更新」領域のコメントに関するメール通知は、より広範なAdobeのメールデザインに合った新しい外観になります。

更新されたメール形式には、次のものが含まれます。

* 以前のWorkfrontのブランドに代わる新しいAdobe Workfront ヘッダー。
* 最新のコメントに焦点を当てた合理化されたレイアウト。
* プライマリ **アイテムを直接開くには、「Workfront**」ボタンで確認してください。

前のコメントのスレッドは、メール本文に含まれなくなりました。 アイテムに関する以前のコメントを表示するには、**Workfront**&#x200B;で表示して、Workfrontで会話を開きます。

この変更は段階的にお客様に展開されます。 このページは、ロールアウトスケジュールが確認されると更新されます。

![ コメント通知メールを更新しました.png](assets/email-look-and-feel-update.png)

## Workfront MCP ServerでWorkfrontをAI ツールに接続する

>[!NOTE]
>
>プレビュー：2026年5月28日>実稼動版の迅速なリリース：2026年6月11日>全員の実稼動：2026年7月16日

チームのオペレーションのコンテキストはWorkfrontに反映されます。 Adobe Workfront MCP Serverなら、既に使用しているAI ツールからコンテキストを取得し、施策につなげることができます。

Workfrontは、Claude、ChatGPT、Copilot、Geminiなど、MCPと互換性のあるあらゆるAI プラットフォームと連携し、自然言語を使用して、任意のAI ツールを離れることなく、Workfrontアイテムを検索、作成、更新、管理できます。 期限切れのタスクの確認、プロジェクトの終了日のプッシュ、承認者へのリマインダーの送信、キャンペーン予算の更新など、AI基盤がWorkfrontで作業を支援します。

さらに、ClaudeのAI スキルとスケジュールされたタスクにより、Adobe Workfrontのライブデータに対して積極的に実行される定期的なワークフローを自動化することができます。 たとえば、月曜日の朝のプロジェクトブリーフィング、毎週のキャパシティレポート、月次のキャンペーンヘルスチェックなどを1回設定するだけで、AIが運用の包括的なコンテキストに基づいて自動的に処理します。

これがエージェンティック作業管理システムの基礎となり、AIが豊富な業務データの中に組み込まれ、人間とAIが協力して作業をフルベロシティで進めることができます。

>[!IMPORTANT]
>
>現在、Workfront MCP サーバーは、AWSを使用しているお客様の米国のお客様のみが利用できます。

詳しくは、[Adobe Workfront MCP サーバーの概要](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md)を参照してください。

## 強化されたリスト更新

>[!NOTE]
>
>プレビュー：2026年5月28日>実稼動版の迅速なリリース：2026年6月11日>全員の実稼動：2026年7月16日

拡張リストの複数のフィールドタイプが更新され、キーボードナビゲーションやその他の機能強化が含まれるようになりました。

拡張リストの割り当て先フィールドにキーボードナビゲーションが追加されました。

* キーボードの上向き矢印と下向き矢印を使用して、ユーザーのリスト内を移動します。
* スペースバーを押して人物を選択するか、\&lt;削除\>して選択した人物を削除します。

拡張リストの単一選択フィールドと複数選択フィールドの場合：

* フィールド操作がキーボードでアクセスできるようになりました。 これには、タグ、検索オプション、上向き矢印と下向き矢印を使用したリスト間のナビゲーションが含まれます。 スペースバーを押して項目を選択するか、\&lt;削除\>して選択した項目を削除します。
* 結果が見つからないときに、エディターから新しいオプションを直接作成できます。 この機能は、一部のリストでは利用できない場合があります。

タイプアヘッドや外部参照フィールドなどの参照フィールドには、インターフェイスの強化が行われています。

また、列をドラッグ&amp;ドロップできるリスト上で列をドラッグ&amp;ドロップする操作の操作性が視覚的に向上しました。

詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。
