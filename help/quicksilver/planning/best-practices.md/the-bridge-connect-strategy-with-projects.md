---
title: Bridgeの構築：戦略的な意図をプロジェクトに結び付ける
description: Adobe Workfront Planning の大まかなプランとAdobe Workfrontでの毎日のワークフロー実行の間に「戦略的スレッド」を作成する方法を説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---


# 橋渡し：戦略的意図をプロジェクトに結び付ける

{{planning-important-intro}}

Adobe Workfront Planning の大まかなプランとWorkfrontでの日々の実行の間で戦略的なスレッドを作成する方法を説明します。 接続を使用して、戦略と実行の間にブリッジを構築できます。

このガイドは、Workfront Planning を実装しているWorkfront管理者および Workspace 管理者を対象としています。

## 実行に対する戦略の関連付けの概要

戦略と日常業務を結び付けることで、ビジョンが現実のものになります。 高レベルのプランが実行と同期している場合は、すべてのプロジェクトとタスクがビジネスを前進させる戦略的スレッドを作成します。

この連携を達成するには、Workfrontの取り組みとWorkfront計画の戦略的レコードを結び付ける一連の技術的リンクとプロセスガードレールが必要です。

計画とアクションのギャップを埋めることで、チームのエネルギーが常に最優先目標に集中できるようにします。

## 接続を作成して基盤を確立する

ワークスペースマネージャーは、計画と実行を橋渡しする前に、接続に適格なレコードタイプを定義する必要があります。

### 接続フィールドの概要

ブリッジは接続フィールドの作成から始まります。

接続フィールドは、レコードタイプ間の技術的なハンドシェイクとして機能します。

このフィールドタイプは、Workfront Planning のすべての関係の背後にあるエンジンです。 特定のレコードタイプ（チャネル戦術など）を、Planning またはWorkfrontに住んでいるかどうかに関係なく、他のオブジェクトタイプにリンクできることを明確にするという意図を表すものです。

詳しくは、[ 接続されたレコードタイプの概要 ](/help/quicksilver/planning/architecture/connect-record-types-overview.md) を参照してください。

### 接続を作成するタイミングを定義

作業を作成する前に、接続を作成する必要があるかどうかを判断するのが理想的です。

接続フィールドを追加することで、個々のレコードが最終的にどのように作成されるかに関係なく、戦略スレッドをサポートするように環境を構築できます。

## 戦略と実行を同期に設定

戦略的レイヤーに焦点を当て続けるために、Workfrontを戦術的な実行に使用しながら、計画記録を全体的な意図に焦点を当てることをお勧めします。

このアプローチでは、次の方法で両方のモジュールの独自の強みを使用します。

* **Workfront計画（戦略的レイヤー）:** はハイレベルのままです。 キャンペーン、チャネル戦術および予算をトラッキングします。 ノイズがなく、エグゼクティブ向けの機能です。

* **Workfront（実行レイヤー）:** 戦術の詳細を管理します。 個々のエクスペリエンスまたはアクティビティを、プロジェクト、タスク、イシューとして管理できます。 これらを所有権に割り当て、実行の承認を作成できます。

## ブリッジをアクティブ化することで、意図から行動に移ります

接続を設定したら、特定の戦略的レコードと実行プロジェクトの間のリンクをアクティブ化する方法を決定する必要があります。

### テーブル主導のパスを使用

ストラテジストやパワーユーザーは、時間の経過と共にプランを調整するワークベンチとしてテーブルビューを使用することがよくあります。

テーブルにレコードを作成しても、デフォルトではWorkfrontへのリンクは確立されません。

実行プロジェクトへの接続は、ユーザーがリンクをアクティベートすると確立されます。

これは、次の方法で行うことができます。

* Workfront Planning の接続フィールド、またはレコードの詳細ビューのオプションの接続ページから、ダウンストリーム接続プロジェクトを手動で作成します。

  手動で作成すると、特定のカスタムフォームのない空のプロジェクトが発生します。

  詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

* より複雑なニーズに対しては、Workfront Planning の自動化を利用して自動で対応します。

  テーブルの行を選択すると、これらの自動化がアクションバーのボタンとして使用できるようになります。

  これにより、人間による監督やプレースホルダーの作成が可能になり、プロジェクトが本当に必要なときにのみワークフロー環境で生成されるようになります。

  詳しくは、[Adobe Workfront計画レコードの自動作成を使用したオブジェクトの作成 ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md) を参照してください。


### 自動アクティベーションの作成

大量のリクエストがある組織や高度な自動化のニーズがある組織の場合、特定のイベントに基づいて、またはリクエストフォームで設定されたフィールド値に基づいて、ブリッジを自動的にアクティブ化できます。

このアプローチには、Adobe Workfront Fusion のライセンスが必要です。

詳しくは、[Workfront Fusion の設定と管理：記事のインデックス ](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc) を参照してください。

* **送信トリガーの使用：** フォームは 1 つのクリーンな送信イベントを提供するので、Fusion の自動化のトリガーとして使用できます。 Fusion シナリオを使用すると、フォームの送信を検出し、Workfrontでリンクされたプロジェクトを直ちに生成できます。

* **フィールド値トリガーの使用：** より深い自動化を行うには、Fusion を設定して、特定のフィールドを監視できます。 たとえば、「Ready for execution」というラベルの付いた単純なチェックボックスを触媒として使用し、チェックがオンになった時点で自動的にブリッジを確立できます。

## サーフェスの表示にルックアップフィールドを追加

プロジェクトをリンクすると、プロジェクトのルックアップフィールドを追加することで、Workfrontのリアルタイムデータを計画レコード内に直接表示できます。

Workspace 管理者は、参照フィールドを設定して、リンクされたプロジェクト（実際の完了日やCreative リードなど）から計画レコードタイプにシステムまたはカスタムフィールドを取り込むことができます。 取得したら、このデータを戦略的階層の複数のレベルからキャンペーンレベルまでロールアップできます。 これにより、マーケティングライフサイクル全体にわたって強力な集計レポートが関係者に提供され、計画環境を離れることなく関係者に情報が提供されます。

## 戦略を行動につなげることで視認性を高める

このブリッジの究極の価値は、リアルタイムの可視性です。

意図を行動に結び付けることで、重要なビジネス上の質問に一目で答えることができます。 これらの質問の例を以下に示します。

* 「26 年度ブランド認知度」キャンペーンは今、積極的に成果を上げていますか。

* 戦略戦術をスケジュールどおりに進めるために、よりクリエイティブなサポートが必要な場所はどこですか？

* 我々は、どのように資源を最優先の戦略柱に合致させているのか。

## ベストプラクティスとヒント

### Dos:

* **「戦略的スレッド」メタファーを使用：** すべてのプロジェクトは戦略的な文字列の「ビーズ」である必要があることをチームに思い出させます。

* **ハンドオフの自動化：** 自動化を使用してプロジェクトの作成をトリガー化することで、時間と労力を節約すると同時に、データの接続性とガバナンスを向上させます。

* **リンク、複製しない：** ルックアップフィールドを使用して、戦略的レコードにリアルタイム実行データ（ステータスや完了日など）を表示します。 これにより、チームが手動で更新しなくても、戦略的なビューが常に正確になります。

### 注意事項：

* **計画レコードをタスクリストとして扱わないでください：** このブリッジは、戦略的意図を実行プロジェクトに結び付けるように設計されています。 計画記録は「何」と「理由」に焦点を当て、タスクとイシューを通じて詳細な「方法」をワークフローモジュールで処理できるようにします。

* **過剰同期を行わない：** すべてのプロジェクトレベルの詳細を Planning に同期する必要はありません。 戦略的レイヤーを高レベルでノイズフリーに保ちます。

* **ブリッジを回避しない：** Planning へのリンクなしでワークフローモジュールで作業が開始された場合、リーダーシップに見えない「シャドウプラン」が作成されています。

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



