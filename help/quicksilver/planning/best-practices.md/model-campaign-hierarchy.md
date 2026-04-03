---
title: 成功を設計する：キャンペーン階層のモデル化
description: 「重心」とマルチワークスペースアーキテクチャを使用して、複雑なビジネスプロセスをスケーラブルで管理されたキャンペーン階層に変換する方法を説明します。
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 2%

---

# 成功を設計する：キャンペーン階層のモデル化

<!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfront の追加機能である Adobe Workfront Planning に関するものです。
>
>この記事で推奨されている機能をサポートするには、Workfront Planning Prime以降のパッケージが必要です。
>
>Workfront Planning へのアクセス要件のリストについて詳しくは、[Adobe Workfront Planning へのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。
> 
>Workfront計画の一般的な詳細については、[Adobe Workfront計画の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)を参照してください。

Adobe Workfront Planningの重心とマルチワークスペースアーキテクチャを使用して、複雑なビジネスプロセスを拡張性の高い管理されたキャンペーン階層に変換する方法を説明します。

このガイドは、Workfront Planningで環境のアーキテクチャを実装および設計しているWorkfront管理者およびPower Usersを対象としています。

## 成功アーキテクチャの概要

マーケティング業務の成熟度が高まるにつれて、データの複雑さも高まります。 明確な設計図がなければ、マーケティング記録システムは、分断されたレコード、矛盾する用語、レポートのサイロ化といったジャンク引き出しになってしまいます。

成功のアーキテクチャを構築する際には、Workfront Planningでキャンペーン階層をモデリングするためのフレームワークを確立します。 スプレッドシートの混乱を解消し、あらゆるチームが同じ言葉を使いながら、実行に必要な俊敏性を維持できる、管理されたオブジェクト指向モデルを導入できます。

## 階層を構築し、購買の意思を明確化

Workfront計画では、明確さと拡張性を維持するために、実績のあるコアパスから始めて、ワークフローを設計することをおすすめします。

それをもとに、アーキテクチャのレベルを上げて、戦略を強化します。

### 中心となるパス：戦略からアクションにつなげる方法

組織は、業務ニーズの進化に合わせてこの階層を拡大できますが、最初に以下の3つのレベルで説明することで、戦略と実行の間に強力な橋渡しができます。

調査結果から、Workfront計画の成功した実装のほとんどが、計画とWorkfrontの両方にまたがる、クリーンで3層モデルで成功していることに気づきました。

以下は、Planningの実装を成功させるためのレベルと、プロセスをサポートするために作成することを検討する可能性のあるアーティファクトです。

* **レベル 1: キャンペーン （Workfront計画）**

   * **フォーカス：**&#x200B;長期的な戦略的支柱と年間の取り組みを定義します。 例えば、「FY26 グローバルブランド認知」という組織のイニシアチブを定義します。 特定の期間における優先事項です。 この取り組みを支援する施策を構築します。

   * このレベルの&#x200B;**ペルソナ：**&#x200B;の関係者は、マーケティング責任者、マーケティング担当バイスプレジデント、またはその他の戦略的リードです。

  詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

* **レベル 2: チャネル戦術（Workfront計画）**

   * **フォーカス：**&#x200B;特定のチャネルに対する「何を」概要を説明する運用概要を定義します。 これは、戦略的意図を示す最後のレイヤーとなり、作業が始まります。 例えば、「第1四半期ソーシャルメディアブリッツ」戦術を策定します。 それをキャンペーンと組み合わせることができます。

   * **ペルソナ：**&#x200B;主な関係者は、マーケティングオペレーションリーダー、チャネルリーダー、キャンペーンマネージャーです。

* **レベル 3: プロジェクト（計画およびWorkfront）**

   * **フォーカス：**&#x200B;最終的に取り組みを達成するエクスペリエンスやアクティビティを正確に実行します。 成果物の中には、ソーシャル投稿、メール、web ページなど、特定のものもあります。

   * **実装：** Planningで戦術を作成し、それらをWorkfrontの&#x200B;**プロジェクト**&#x200B;に直接リンクできます。この場合、個々の成果物はタスクと問題として管理されます。

   * **ペルソナ：**&#x200B;主な関係者は、クリエイター、個人貢献者、イニシアチブをサポートする作業を担当する人です。

### 戦略的な拡大：レベルを上げる方法

コアパスを確立したら、特定のビジネスの複雑さを慎重に検討した後、さらにレイヤーを追加することもできます。

次の追加項目を作成すると便利な場合があります。

* **チャネルプラン：** キャンペーンと戦術の間のレイヤーで、部門横断的な戦略をグループ化します。 例えば、「デジタル戦略」という計画があります。

* **アクティビティ：**&#x200B;小規模な環境で作業している場合（年間5,000件以下の成果物がある場合があります）、一部のチームでは、Workfront プロジェクトになる前に、個々のエクスペリエンスをWorkfront プランニングレコードとして追跡することを好む場合があります。

>[!IMPORTANT]
>
>年間5,000以上のアクティビティを制作している場合は、個々の成果物をWorkfrontに保管しましょう。
>
>Planningで膨大なエクスペリエンス記録を管理すると、データが蓄積され、戦略的な可視性が不明瞭になる可能性があります。
>効率を最大化するための広範なガイドラインを以下に示します。
>
>* 「なぜ」と「何」に対するプランニングの使用
>* Workfrontを使用して、大量の「方法」を作成します。

## 重心を理解してアーキテクチャを構築

エンタープライズグレードのマーケティング記録システムは、単一のワークスペースに構築されていません。 レコードタイプを自然な重心で管理する「ハブアンドスポーク」アーキテクチャを使用します。

詳細については、「[戦略的ホームをロールアウト：30日間のランチパッド ](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md)」を参照してください。

ハブアンドスポーク方式でアーキテクチャを構築するには、次の要素を作成する必要があります。

* 分類ハブ
* 戦略的プランニングワークスペース
* 機能スポーク

### 分類として分類ハブを構築する

まず、グローバル分類のための一元化されたワークスペースを確立し、組織内の全員が理解しなければならない主な概念を定義する必要があります。 例えば、一元化されたワークスペースに、ブランド、地域、製品、ペルソナのレコードタイプを作成できます。

詳しくは、次を参照してください。

* [レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)

* [クロスワークスペースのレコードタイプの概要](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

分類を作成する際には、次の点を確認します。

* **プライマリの場所：** プライマリワークスペースを選択します。 作成するレコードタイプの信頼できる唯一の情報源である必要があります。

* **メリット：**&#x200B;これらの定義をビジネスの他の部分とシンジケートすることで、「地域：EMEA」などの概念がすべてのチームにとって同じことを意味することを明確に解決できます。

### 戦略的プランニングワークスペースをエグゼクティブセンターとして作成する

エグゼクティブセンターには、上位レベルのキャンペーン（および任意のチャネルプラン）が公開されます。

* **プライマリの場所：**&#x200B;これは重心のエグゼクティブセンターであり、戦略的な意思決定にノイズのない環境を提供します。

* **メリット：**&#x200B;経営陣は、日々の戦術的な雑音を聞くことなく、キャンペーンのポートフォリオを管理できます。

### チームのワークスペースとして機能スポークを定義します

機能部門（ソーシャル、Creative、メール）には、戦術を管理するための独自のワークスペースがあります。

* **プライマリの場所：**&#x200B;これらのワークスペースは、ローカルチームが実行するための個別の重心です。

* **メリット：** チームは、独自のローカルオブジェクトを維持しながら、ハブからのグローバルキャンペーンと分類を利用します。

  例えば、チームは中央ワークスペースのキャンペーンレコードタイプをチームのワークスペースに追加し、そのワークスペースだけに関連するキャンペーンを作成できます。 キャンペーンの例としては、「メディアのコンセント」または「使用権限」があります。

## 名詞ベースのガバナンスアプローチを用いる

アーキテクチャをプレッシャー下で維持できるように、名詞ベースのガバナンスの原則に従ってください。

Workfront Planningでエンティティを作成する場合は、次をお勧めします。

* **動詞ではなく名詞を使用：**&#x200B;実行するアクションではなく、トラッキング対象のアクションの後にレコードタイプの名前を付けます（「Campaign」または「Tactic」という名前を付けます）（「Campaign」または「Planning」という名前は付けません）。

* **正規表現を標準化：**&#x200B;すべてのワークスペースで同じ名前を使用します。 これにより、エグゼクティブレポート用にポートフォリオ全体のデータを集計できます。

## 既存のポートフォリオとプログラムについて

成熟した企業にとってよくある質問は、Workfrontで既に構築されているポートフォリオやプログラムをどのように処理するかということです。 これまで、これらのオブジェクトは戦略的プランニングを模倣するために使用されることがよくありました。

ここでは、Workfront計画に移行することをお勧めします。これは、計画に対する戦略的アプローチと自然に一致します。

### ポートフォリオとプログラムをレコードタイプに置き換える

多くの組織では、ポートフォリオは上位レベルのブランドや事業部門を表すために使用され、プログラムは戦略的テーマを表します。

Workfront Planningでは、これらは分類ハブのレコードタイプとして最もよくモデル化されます。

ブランドや事業部をレコードタイプとして扱うことで、企業全体でキャンペーンや戦術にリンクさせ、静的なPortfolioのプログラム構造よりもはるかに柔軟なレポートを提供できます。

### レポートブリッジ戦略の使用

Workfront計画は戦略的インテントの未来ですが、Canvas ダッシュボードを介したネイティブレポートはまだ成熟しています。

多くの企業は、依然として、Workfrontの従来のPortfolioやプログラム構造に関連する強力なレポート機能を利用しています。

以下をお勧めします。

* ポートフォリオとプログラムは削除しないでください。
* プランニングの自動化を利用して、レコードタイプとポートフォリオやプログラムをつなぎ合わせることができます。

  Workfront Planningで戦術またはキャンペーンが作成されると、そのレコードは対応するPortfolioまたはプログラムをWorkfrontで生成できます。

  詳しくは、[Adobe Workfront Planning レコードの自動処理を使用したオブジェクトの作成](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)を参照してください。

これにより、次のことが可能になります。

* タイムラインとカレンダーを利用して、Workfront Planningの優れた戦略的ビジュアライゼーションを活用できます。

* まだCanvasに移行する準備ができていない関係者については、Workfrontで従来のレポートを管理します。

## ベストプラクティスとヒント

### ドス

* **パス優先のコアアプローチに従う：**&#x200B;複雑さを増す前に、キャンペーンから戦術、プロジェクトのフローを確立します。

* **プライマリワークスペースを指定：**&#x200B;各レコードタイプに、レポート用の集計器として機能するホームワークスペースが1つあることを確認します（重心を考慮してください）。

* **受け入れプロセスのリクエストフォームに優先順位を付ける：** Workfront Planningの難易度の低いグループには、レコードフォームを使用して、メタデータの整合性を確保します。

  >[!CAUTION]
  >
  >パワーユーザーは、テーブルビューでの直接データ入力からメリットを得られる場合がありますが、これは慎重にアプローチする必要があります。
  >テーブルの一括変更は、ほかの関係者のデータに頭痛の種を簡単に作成できます。

### わからない

* **一般化を使用しない：**&#x200B;例えば、「コア」環境について説明する代わりに、実行について説明する際は、Workfrontとプロジェクトオブジェクトを具体的に参照します。

* **複雑すぎない：**&#x200B;階層の追加レベルごとに管理税が加算されます。 現在は回答できないビジネス上の質問に対してのみレベルを追加してください。

* **サイロを作成しないでください：** チームが同じデータを再入力しないように、レコードタイプがワークスペース間で共有されていることを確認します。


<!--
original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->