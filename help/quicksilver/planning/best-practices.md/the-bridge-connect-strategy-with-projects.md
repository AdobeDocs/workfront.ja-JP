---
title: Bridgeの構築：戦略的インテントをプロジェクトに結び付ける
description: Adobe Workfront Planningの上位レベルの計画とAdobe Workfrontでの日々のワークフローの実行との間に「戦略的スレッド」を作成する方法について説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 3%

---


# 橋渡しをする：戦略的な意図をプロジェクトに結びつける

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfront の追加機能である Adobe Workfront Planning に関するものです。
>
>この記事で推奨されている機能をサポートするには、Workfront Planning Prime以降のパッケージが必要です。
>
>Workfront Planning へのアクセス要件のリストについて詳しくは、[Adobe Workfront Planning へのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。
> 
>Workfront計画の一般的な詳細については、[Adobe Workfront計画の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)を参照してください。

Adobe Workfront Planningの上位レベルの計画とWorkfrontでの日々の実行との間に戦略的な糸を張る方法について説明します。 接続を使用して、戦略と実行の間にブリッジを構築できます。

このガイドは、Workfront Planningを導入しているWorkfront管理者およびワークスペース管理者を対象としています。

## 戦略と実行の整合の概要

戦略を日々の作業に結びつけることで、ビジョンが現実のものになります。 上位レベルの計画が実行と一致している場合は、あらゆるプロジェクトとタスクがビジネスを確実に前進させるための戦略的スレッドを作成します。

この連携を実現するには、Workfrontの取り組みとWorkfront計画の戦略的記録を結びつける、一連の技術的リンクとプロセスのガードレールが必要です。

計画と行動の間のギャップを埋めることで、チームのエネルギーを常に最も優先順位の高い目標に集中させることができます。

## つながりを築き、基盤を確立する

プランニングと実行を橋渡しする前に、ワークスペースマネージャーとして、接続の対象となるレコードタイプを定義する必要があります。

### 接続フィールドの概要

ブリッジは、接続フィールドの作成から始まります。

接続フィールドは、レコードタイプ間の技術的なつながりとして機能します。

このフィールドタイプは、Workfront Planningのすべての関係の背後にあるエンジンです。 これは、特定のレコードタイプ（チャネル戦術など）が、PlanningまたはWorkfrontに存在する場合を問わず、他のオブジェクトタイプにリンクできることを示す、意図の表明です。

詳しくは、[接続されたレコードタイプの概要](/help/quicksilver/planning/architecture/connect-record-types-overview.md)を参照してください。

### 接続を作成するタイミングを定義

理想的には、どのような作業も作成する前に、接続を作成する必要があるかどうかを決める必要があります。

接続フィールドを追加することで、個々のレコードが最終的にどのように作成されるかに関係なく、戦略的スレッドをサポートするように環境を設計できます。

## 戦略と実行を同期

戦略レイヤーに焦点を当て続けるために、Workfrontを戦術的な実行に使用しながら、計画記録を高レベルの意図に焦点を当てることをお勧めします。

このアプローチでは、次の方法で両方のモジュールの独自の強みを使用します。

* **Workfront計画（戦略的レイヤー）:**&#x200B;は上位レベルに留まります。 キャンペーン、チャネル戦術、予算を追跡します。 ノイズフリーで経営陣の賛同を得ることができます。

* **Workfront （実行レイヤー）:**&#x200B;戦術的な詳細を管理します。 個々のエクスペリエンスやアクティビティを、プロジェクト、タスク、イシューとして管理できます。 所有権を割り当てて、実行の承認を組み込むことができます。

## ブリッジをアクティブ化して、意図からアクションへ

接続を設定したら、特定の戦略的レコードと実行プロジェクトの間のリンクをアクティブ化する方法を決定する必要があります。

### テーブル主導のパスを使用

ストラテジストやパワーユーザーは、多くの場合、テーブルビューをワークベンチとして使用し、時間をかけてプランを洗練させます。

テーブルにレコードを作成しても、デフォルトではWorkfrontへのリンクは確立されません。

実行プロジェクトへの接続は、ユーザーがリンクをアクティブ化することを決定したときに確立されます。

これは、次の方法で実行できます。

* ダウンストリーム接続されたプロジェクトを、Workfront Planningの接続フィールドから直接作成するか、レコードの詳細ビューのオプションの接続ページから手動で作成します。

  手動で作成すると、特定のカスタムフォームを使用しない空白のプロジェクトになります。

  詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

* Workfront Planningの自動化機能を使用すれば、より複雑なニーズに対応できます。

  これらの自動処理は、表の行を選択するときに、アクションバーのボタンとして使用できます。

  これにより、人間による管理やプレースホルダーの作成が可能になり、プロジェクトが本当に必要なときにのみワークフロー環境で生成されるようになります。

  詳しくは、[Adobe Workfront Planning レコード自動処理を使用したオブジェクトの作成](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)を参照してください


### 自動アクティベーションの構築

大量のリクエストや高度な自動化が必要な組織の場合、特定のイベントに基づいて、またはリクエストフォームで設定されたフィールド値に基づいて、ブリッジを自動的にアクティブ化できます。

このアプローチには、Adobe Workfront Fusionのライセンスが必要です。

詳しくは、[Workfront Fusionの設定と管理：記事インデックス &#x200B;](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc)を参照してください。

* **送信トリガーを使用：** フォームは1つのクリーンな送信イベントを提供するので、Fusion自動処理のトリガーとして使用できます。 Fusion シナリオでは、フォーム送信を検出し、Workfrontでリンクされたプロジェクトを即座に生成できます。

* **フィールド値トリガーを使用：**&#x200B;より詳細な自動化を行うには、Fusionを設定して特定のフィールドを監視できます。 例えば、「実行準備完了」というラベルの付いた単純なチェックボックスが触媒として機能し、チェックされた瞬間にブリッジが自動的に確立されます。

## ルックアップフィールドを追加して表示

プロジェクトをリンクすると、プロジェクトからルックアップフィールドを追加して、Workfrontから直接Planning レコード内にリアルタイムデータを表示できます。

ワークスペース管理者は、ルックアップフィールドを設定して、リンクされたプロジェクト（実際の完了日やCreative リードなど）から任意のシステムまたはカスタムフィールドをプランニングレコードタイプに取り込むことができます。 いったんキャプチャされると、このデータは、キャンペーンレベルまで、複数のレベルの戦略的階層を通じてロールアップできます。 これにより、マーケティングライフサイクル全体にわたって関係者に強力な集計レポートを提供し、計画環境から離れることなく関係者に情報を提供できます。

## 戦略と行動を結び付けて可視性を向上

橋の究極の価値はリアルタイムの可視性である。

意図を行動につなげることで、重要なビジネス上の質問に一目で答えることができます。 例えば、次の質問に答えます。

* 「26年度ブランド認知度」施策は、現在、積極的に成果を上げているか？

* スケジュール通りに進めるために、より多くのクリエイティブサポートが必要な戦略的戦術は、どこでしょうか？

* リソースを最も優先度の高い戦略ピラーとどのように整合させるのか？

## ベストプラクティスとヒント

### 導入の相談：

* **戦略的スレッドの比喩を使う：**&#x200B;すべてのプロジェクトは戦略的な文字列の「ビーズ」にする必要があることをチームに思い出させます。

* **引き継ぎを自動化：**&#x200B;自動化機能を使用してプロジェクトの作成をトリガー化し、時間と労力を削減しながら、データの接続性とガバナンスを向上させます。

* **リンク、重複なし：**&#x200B;参照フィールドを使用して、戦略的レコードにリアルタイムの実行データ（ステータスや完了日など）を表示します。 これにより、チームの手による更新を必要とせずに、戦略的なビューを常に正確に保つことができます。

### 悪い例：

* **計画記録をタスク リストとして扱わない：** ブリッジは、戦略的インテントを実行プロジェクトに結びつけるように設計されています。 プランニングのレコードでは、「何」と「なぜ」に焦点を当て、タスクと問題を通じて詳細な「方法」をワークフローモジュールで処理できるようにします。

* **過度に同期しない：**&#x200B;すべてのプロジェクトレベルの詳細をPlanningに同期する必要はありません。 戦略的レイヤーは高レベルでノイズフリーに保ちます。

* **ブリッジをバイパスしない：** ワークフローモジュールで作業が開始され、プランニングへのリンクが表示されない場合は、経営陣には見えない「シャドープラン」が作成されています。

<!--
original content:

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



