---
title: 成功のアーキテクト：キャンペーン階層のモデリング
description: 「重心」とマルチワークスペースアーキテクチャを使用して、複雑なビジネスプロセスをスケーラブルで管理されたキャンペーン階層に翻訳する方法を説明します。
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 1%

---

# 成功のアーキテクト：キャンペーン階層のモデリング

<!--see the file again for additional comments from Seth and others-->

{{planning-important-intro}}

Adobe Workfront Planning で重心とマルチワークスペースアーキテクチャを使用して、複雑なビジネスプロセスをスケーラブルで管理されたキャンペーン階層に変換する方法について説明します。

このガイドは、Workfront Planning で環境のアーキテクチャを実装および設計するWorkfront管理者およびパワーユーザーを対象としています。

## 成功のアーキテクチャの概要

マーケティング業務の成熟に伴い、データは複雑になります。 明確なブループリントがなければ、マーケティングレコードのシステムは、切断されたレコード、矛盾する用語、レポートサイロの迷惑ドロワーになる可能性があります。

成功のアーキテクチャを構築する際には、Workfront Planning でキャンペーン階層をモデリングするためのフレームワークを確立します。 スプレッドシートの混乱から、管理されたオブジェクト指向モデルに移行し、すべてのチームが必要な俊敏性を維持しながら同じ言語を話せるようにします。

## 階層を構築して、インテントのレベルを定義します

明確さと拡張性を維持するために、Workfront Planning でワークフローを設計する際には、実証済みのコアパスから始めることをお勧めします。

そこから、アーキテクチャにレベルを追加することで、戦略を拡大できます。

### コアパス：戦略から行動を起こす方法

組織は、運用ニーズの変化に合わせてこの階層を拡大できますが、以下の節で説明する 3 つのレベルに始まり、戦略と実行の間の強力なブリッジを確保します。

調査結果から、Workfront Planning の導入が成功した大半は、Planning とWorkfrontの両方にまたがるクリーンな 3 層モデルで行われていることに気がつきました。

Planning の実装が成功したレベルと、プロセスでサポートするために作成を検討するアーティファクトを次に示します。

* **レベル 1：キャンペーン（Workfront計画）**

   * **焦点：** 長期的な戦略的な柱と年間の取り組みを定義します。 例えば、組織の「FY26 Global Brand Awareness」というイニシアチブを定義します。 これは、特定の時間枠に対するフォーカスです。 このイニシアチブをサポートするキャンペーンを作成します。

   * **ペルソナ：** このレベルの関係者は、マーケティング責任者、マーケティング担当副社長、その他の戦略的リードなどです。

  詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

* **レベル 2：チャネル戦術（Workfront計画）**

   * **フォーカス：** 特定のチャネルの「何」の概要を説明する運用概要を定義します。 これは、作業を開始する前の戦略的な意図の最後のレイヤーです。 例えば、「Q1 ソーシャルメディア Blitz」戦術を作成します。 その後、キャンペーンとペアにすることができます。

   * **ペルソナ：** 主な関係者は、マーケティング運用リーダー、チャネルリーダーまたはキャンペーンマネージャーです。

* **レベル 3：プロジェクト（Planning およびWorkfront）**

   * **フォーカス：** 最終的にイニシアチブを達成する正確なエクスペリエンスまたはアクティビティを実行します。 配信物の一部は特定のものです（ソーシャル投稿、メール、web ページなど）。

   * **導入：** 計画中に戦術を作成し、Workfrontの **プロジェクト** に直接リンクできます。そこでは、個々の成果物がタスクおよびイシューとして管理されます。

   * **ペルソナ：** 主なステークホルダーは、クリエイティブ担当者、個々のコントリビューター、イニシアチブを支援するための作業を行う責任がある人です。

### 戦略的拡張：さらにレベルを追加する方法

コアパスを確立したら、ビジネス固有の複雑さを慎重に考慮した後、追加のレイヤーを追加することを選択できます。

次の追加アイテムを作成すると便利です。

* **チャネルプラン：** キャンペーンと戦術の間のレイヤーを統合して、部門横断的な戦略をグループ化します。 例えば、「デジタル戦略」と呼ばれるプランです。

* **アクティビティ：** 作業量が少ない環境（年間の成果物の数が 5,000 件以下）で作業する場合、一部のチームは、Workfront プロジェクトになる前に、Workfront Planning のレコードとして個人のエクスペリエンスをトラッキングする方を好む場合があります。

>[!IMPORTANT]
>
>年間 5,000 を超えるアクティビティを生成する組織の場合は、個々の成果物のトラッキングをWorkfrontに移行する必要があります。
>
>計画で大量のエクスペリエンスレコードを管理すると、戦略的な可視性を不明瞭にするデータ蓄積につながる可能性があります。
>効率を最大限に高めるには、次の広範なガイドラインをお勧めします。
>
>* 「理由」と「内容」に計画を使用する
>* 大量の「方法」を得るには、Workfrontを使用します。

## 重心を把握してアーキテクチャを構築

エンタープライズグレードのレコードのマーケティングシステムは、単一のワークスペースでは構築されません。 レコードの種類を自然な重心で管理する「ハブアンドスポーク」アーキテクチャを使用します。

詳しくは、[ 戦略的なホームのロールアウト：30 日間のランチパッド ](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md) を参照してください。

ハブアンドスポーク方式を使用してアーキテクチャを構築するには、次の手順を作成する必要があります。

* 分類のハブ
* 戦略的計画ワークスペース
* 機能スポーク

### 分類として分類ハブを作成します

最初に、グローバル分類に対して 1 つの一元化されたワークスペースを確立して、組織内の全員が理解する必要がある主な概念を定義する必要があります。 例えば、中央のワークスペースに、ブランド、地域、製品、ペルソナのレコードタイプを作成します。

詳しくは、[リクエストタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

分類を作成する際は、次の事項を確立します。

* **プライマリの場所：** プライマリ ワークスペースを選択します。 このワークスペースは、作成するレコードタイプの信頼できる情報源となる必要があります。

* **メリット：** これらの定義をビジネスの他の部分にシンジケートすることで、「地域：EMEA」のような概念がすべてのチームに対して同じことを意味することを明確にします。

### エグゼクティブセンターとしての戦略的計画ワークスペースの作成

エグゼクティブセンターには、ハイレベルなキャンペーン（および任意のチャネルプラン）が開催されます。

* **プライマリの場所：** これはエグゼクティブの重心で、戦略的な意思決定に騒音を使用しません。

* **メリット：** リーダーシップは、日々の戦術的なノイズに耳を傾けることなく、キャンペーンのポートフォリオを管理できます。

### 機能スポークをチームのワークスペースとして定義します

機能ユニット（ソーシャル、Creative、メール）には、戦術を管理するための独自のワークスペースがあります。

* **プライマリの場所：** これらのワークスペースは、ローカル チームの実行用の個々の重心です。

* **メリット：** チームは、独自のローカルオブジェクトを維持しながら、ハブからグローバルなキャンペーンと分類を消費します。

  例えば、チームはセントラルワークスペースからチームのワークスペースにキャンペーンレコードタイプを追加できますが、自分のワークスペースにのみ関連するキャンペーンを作成できます。 キャンペーンの例としては、「メディアアウトレット」や「使用権限」があります。

## 名詞ベースのガバナンスアプローチを使用

アーキテクチャがプレッシャーの中でも動かないようにするには、名詞ベースのガバナンスの原則に従います。

Workfront Planning でエンティティを作成する場合は、次の操作をお勧めします。

* **動詞ではなく名詞を使用：** 追跡するものにちなんでレコードタイプに名前を付けます（「キャンペーン」や「戦術」という名前を付けます）。実行するアクションには名前を付けません（「キャンペーン」や「計画」という名前は付けません）。

* **用語を標準化：** すべてのワークスペースで同じ名前を使用します。 これにより、エグゼクティブレポート用に、ポートフォリオ全体でデータを集計できます。

## 既存のポートフォリオとプログラムはどうですか？

成熟した組織に共通する問題は、Workfrontで既に作成したポートフォリオとプログラムの処理方法です。 以前は、これらのオブジェクトは、戦略的計画を模倣するためによく使用されていました。

今は、そのアプローチをWorkfrontプランニングに移行することをお勧めします。これは、プランニングへの戦略的アプローチに自然に適合します。

### ポートフォリオとプログラムをレコードタイプに置き換える

多くの組織では、ポートフォリオは高レベルのブランドまたはビジネスユニットを表すために使用され、プログラムは戦略的テーマを表します。

Workfront Planning では、これらは分類ハブのレコードタイプとしてモデル化するのが最適です。

ブランドまたはビジネスユニットをレコードタイプとして扱うことで、それらを企業全体のキャンペーンや戦術にリンクでき、静的なPortfolio - プログラム構造よりもはるかに柔軟なレポートを提供できます。

### レポートブリッジ戦略の使用

Workfront Planning は戦略的な意図の未来ですが、Canvas Dashboard を介したネイティブレポートはまだ成熟しています。

多くの組織は、Workfrontの従来のPortfolioとプログラム構造に結び付いた堅牢なレポート機能に依然として依存しています。

以下をお勧めします。

* ポートフォリオとプログラムを削除しないでください。
* 計画の自動化を使用すると、レコードタイプとポートフォリオおよびプログラムを橋渡しすることができます。

  Workfront Planning で戦術またはキャンペーンが作成されると、そのレコードで対応するPortfolioまたはプログラムがWorkfrontで生成されます。

  詳しくは、[Adobe Workfront計画レコードの自動作成を使用したオブジェクトの作成 ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md) を参照してください。

これにより、次のことが可能になります。

* タイムラインとカレンダーを使用して、Workfrontプランニングの優れた戦略的ビジュアライゼーションをご覧ください。

* キャンバスに移行する準備がまだ整っていない関係者のために、Workfrontで従来のレポートを管理します。

## ベストプラクティスとヒント

### Dos

* **コアパスファーストのアプローチに固執する：** 複雑さを増す前に、キャンペーンから戦術をプロジェクトに至るフローを確立します。

* **プライマリワークスペースの指定：** 各レコードタイプに、レポートのアグリゲータとして機能するホームワークスペースが 1 つ（重心であると見なします）あることを確認します。

* **取り込みプロセスのリクエストフォームの優先順位を付ける：** Workfront Planning で、洗練度の低いグループのレコードフォームを使用して、メタデータの整合性を確保します。

  >[!CAUTION]
  >
  >パワーユーザーには、テーブル表示での直接データ入力のメリットがありますが、この方法には注意が必要です。
  >テーブルを一括で変更すると、他の関係者のデータに関する頭痛の種になりやすい場合があります。

### してはいけない

* **一般化を使用しない：** 例えば、「コア」環境については説明せず、実行については特にWorkfrontとプロジェクトオブジェクトを参照してください。

* **複雑にしすぎない：** 階層レベルを追加するたびに管理税が追加されます。 現在回答できないビジネス上の質問に回答するレベルのみを追加します。

* **サイロを作成しない：** レコードタイプがワークスペース間で共有されるので、チームが同じデータを再入力しないようにします。


<!--original content:


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