---
title: Adobe Workfront計画のためのアイデア創出スペースの基本を学ぶ
description: Adobe Workfront Planningでは、キャンペーンを開始する前にアイデアを立案するための機能が追加されました。 AIを活用して、データと直接入力を具体的な計画に変換し、情報にもとづいた出発点を空白ページの代わりに提供します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 2%

---


# Adobe Workfront Planningのアイデア創出スペースの基本を学ぶ

<!--
Should we add a new Feature to ExL for "Strategic Ideation"?
-->

<!--information in this article come from this document, in addition to my notes for this project up to August 31, 2026:

https://adobe-my.sharepoint.com/:w:/r/personal/alinaw_adobe_com/_layouts/15/Doc.aspx?sourcedoc=%7B513DE769-B70B-4040-8C9E-6A9B8E3167BB%7D&file=getting-started-catalyze.docx&action=default&mobileredirect=true
-->

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 これは、**アイデア創出スペース Beta** プログラムの一部としてのみ使用できます。</span>\
</span>

{{planning-important-intro}}

Adobeのアイデア創出スペースは、Workfront Planningに直接ビルトインされた、AdobeのAIを活用した戦略的アイデア出し機能です。 これにより、マーケティング部門は、データにもとづいた体系化されたキャンペーン戦略の出発点を得ることができます。手作業による調査や推測は、組織の実際のパフォーマンス履歴にもとづいてAIが生成したブリーフに置き換えることができます。

Workfront Planningからのみアクセスできるアイデア創出スペースは、キャンペーンのライフサイクルの最前線にあり、計画、制作、配信の前に配置され、チームが作業を計画および実行するWorkfront計画ワークスペースに直接送られます。

## 製品の可用性

変更される可能性のあるアイデア立案スペースのリリース予定タイムラインには、次のマイルストーンが含まれます。

* **終了したBeta:** 2026年7月にリリースされ、少数のお客様が含まれています。
* **2026年9月を目標とするBeta:**&#x200B;を開きます。 これはオプトインオファーであり、顧客はオプションを積極的にオプトアウトするのではなく、オプションをオンにして設定する必要があります。
* **一般公開：** 2026年後半の予定です。

## 必要な製品

組織と同時に次のパッケージにアクセスできる場合は、アイデア創出スペースにアクセスできます。

* Workfront計画パッケージを含むAdobe Workfront Workflow パッケージ

  または

  スタンドアロン製品としてのAdobe Workfront計画

  >[!NOTE]
  >
  >アイデア創出スペースには、Adobe Planningからのみアクセスできます。 アイデア創出スペースにアクセスするために個別のログインは必要ありません。 Workfront Planningにログインできる場合は、すぐに使用できます。

* Adobe GenStudio for Performance Marketing

<!-- only required for closed beta, see below: * Adobe Customer Journey Analytics-->

アイデア出しスペースを使用するために必要なアクセスについて詳しくは、「[&#x200B; アイデア出しスペースを使用するために必要なアクセス &#x200B;](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md)」を参照してください。

上記の要件に加えて、Closed Beta プログラムに参加するには、次の条件を満たす必要があります。

* キャンペーンのトラッキングを設定したアクティブなAdobe Customer Journey Analytics（CJA）アカウントを持つ
* 反復可能な計画プロセスによるマルチチャネル施策を実施している
* マーケティングオペレーションにWorkfrontプランニングを活用する
* 主要なアイデア創出スペースユーザーとなる、少なくとも1人の特定された戦略家またはアイデア創出ユーザーがいる

## オーディエンスとユースケース

アイデア創出スペースは、キャンペーン戦略の策定とキャンペーンブリーフの作成を担当する、製品マーケターやブランドマーケター向けに設計されています。

<!--
Too much: 

| Role | Primary job to be done |
|---|---|
| Brand Marketer | Identify messaging, trends, and cultural shifts that resonate with target audiences |
| Product Marketer | Launch insight-driven, culturally relevant campaigns that deliver business impact |
| Collaborators | Internal creative studios, external agencies, media planners/managers, and executives who need visibility into strategic direction |
-->

ワークスペース管理者は、次の手順に従って、アイデア創出スペースを使用してWorkfront Planningでレコードを作成できます。

* レコードの作成または編集を開始する際に、Planningからアイデア創出スペースでブリーフを作成します。
* AI プロンプトを使用して、システム内またはweb上の他のレコードから詳細を収集し、アイデア創出の概要を作成できます。
* ブリーフからプランニングレコードタイプを作成します。
* アイデア創出の概要を改善し、Planningの既存のレコードタイプを更新できます。

アイデア出しスペースの使用例を次に示します。

* **過去のパフォーマンスを使用して以前のキャンペーンを更新する**

  * 例えば、新しい四半期、シーズン、または製品のモーメントの既存のキャンペーンを更新できます。
  * これにより、過去の実績に基づいて、何が残るのか、何が変化するのか、そしてその理由を説明した「デルタブリーフ」を作成します。

* **過去のパフォーマンスを使用して最新のキャンペーンを作成**

  * 例えば、キャンペーン履歴を直接示すことなく、新しい製品、セグメント、イニシアチブを立ち上げる際にキャンペーンを作成できます。
  * これにより、ガイド付きのアイデア出し、推奨されるチャネルミックス、初期のコンセプトやメッセージの方向性を通じて、まったく新しいブリーフを作成できます。

## アイデア創出スペースへのアクセス

アイデア創出スペースにアクセスするには、次の操作を行います。

1. この記事の「[製品要件](#product-requirements)」の節で説明されているように、製品要件を満たしていることを確認してください。
1. Adobeのアカウント担当者に連絡して、クローズドBetaへの参加に関心を示すか、Open Betaの待機リストに参加してください。
1. 最初のキャンペーンを特定する：最近リフレッシュするキャンペーンか、ゼロから作成する新しいキャンペーンです。

アイデア出しスペースの使用について詳しくは、次の記事も参照してください。

* [アイデア創出スペースの利用に必要なアクセス](/help/quicksilver/planning/ideation/access-needed-to-use-ideation-space.md)
* [アイデア立案スペースの概要からプランニングレコードを作成](/help/quicksilver/planning/ideation/create-records-in-ideation-space-for-planning.md)
* [アイデア創出スペースでブリーフを作成する](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md)

## アイデア創出スペースの概要

アイデア創出スペースは、ブランド企業と製品マーケターが、より緊密なキャンペーンをより迅速に、より緊密に連携して構築するための、戦略的なマーケティングアイデア創出ツールです。 過去のブリーフ、パフォーマンスデータ、オーディエンスインサイト、ブランドガイドライン、既存のキャンペーンアセットなど、リアルタイムのマーケティングのコンテキストにAIの提案を基にして、結果は汎用的なものではなく、関連性のあるものです。

ブリーフを作成する際に、アイデア出しを最大限に活用する方法の例を以下に示します。

* ドキュメントやソーシャルリスニングインサイトのアップロード
* 作成する概要に関連するweb コンテンツにアクセスします
* キャンペーン目標の定義
* オーディエンスインサイトの概要を取得
* オーディエンスのペルソナの生成
* キャンペーンメッセージの立案
* AI プロンプトを使用して、テキスト、画像、ファイル、チャート、insightカードを生成し、大規模なビジュアルキャンバスで作業できます
* カードを整理、修正、拡張し、最終的にキャンペーンブリーフに変換します
* ブリーフが完成する前に、アイデアを追加したり、特定のキャンバス項目にコメントを残したり、付箋を使ってフリーフォームのアイデアを書き出したりできる、複数のユーザーと共同作業を行うことができます
* アイデア出しスペースを使用する場合は、次のベストプラクティスをお勧めします。

  * **具体的であること**。 より豊富なキャンペーン説明により、より関連性が高く、より根拠のあるカードを生み出すことができます。
  * **確定する前に確認**。 AIで生成された回答は不正確である可能性があるため、レコードを確定する前に、常にカードの&#x200B;**ソース**&#x200B;を確認し、リンクされたソースと確認してください。
  * **実際のレコードでAI カードを組み合わせる**。 実際のレコードをアイデア創出スペースにドラッグ&amp;ドロップできます。

## Adobe CX Coworkerのアイデア創出スペース

アイデア創出スペースでは、AdobeのCX Coworkerを通じて、対話型コミュニケーションもサポートしています。

利用者は、たった一発の結果を得るのではなく、フォローアップで質問し、会話で概要を絞り込むことができます。

ブリーフがWorkfront Planningのライブ接続に関連付けられている場合、Coworkerはブリーフの上書きを控え、基礎となるプランを維持します。

<!--
**************** CONSIDER INCLUDING THIS INFORMATION FROM JESH BARLOW ABOUT COWORKER IN CATALYZE?? - https://adobecorpdev.slack.com/archives/C091C0Y735W/p1788917610365089?thread_ts=1788917251.550099&cid=C091C0Y735W

Catalyze Coworker needs — panel inside Catalyze, not a rail from Unified ShellWhy this matters. Catalyze is AI-first. You can't use it without a prompt, so the prompting surface can't be something you open and close from Unified Shell. Coworker's rail was built to bolt onto apps that already work fine without AI. We need the opposite.

What we need

* Coworker embedded as a panel inside Catalyze (the Photoshop/Illustrator model), always present, minimized or expanded, never fully closeable.
* Not the Unified Shell rail that slides in, pushes the app, and only opens and closes from the shell.
* Quick terminology flag, since Coworker inverts it. By "panel" we mean embedded in the app. Their team uses "panel" for the shell version, so we have to be explicit every time.


Must-haves

* Minimized and expanded prompt bar states that live inside Catalyze, not tied to the shell.
* Minimize, never close. There's no state where the prompt disappears.
* Full UI control over how the prompt behaves.
* Headless Coworker so the panel can always sit on the canvas.


Where it stands (Aug 20 Shell/Catalyze sync with Stephen Gould)

* Headless is technically possible. Coworker can be hosted in Catalyze's own front-end.
* But Horia's team has no capacity to build or own an in-app rail. Deeper embedding means Catalyze eng builds the panel and owns it going forward.
* The open question is ownership, one-time integration vs owning the panel long-term. Still unresolved, and it's the thing that decides this.


Worth noting

* Experience Workspace and Brand Visibility (AM) already run Coworker without the shell, so headless isn't net-new. Let's learn how they did it before anyone calls it infeasible.
* Next step everyone agreed on is getting clarity from Horia's team and Joshua on rail ownership.

*************************************
-->

## 追加のリソース

* [Adobe Workfront Campaign Planning](https://business.adobe.com/jp/products/workfront/campaign-planning.html)
* [Adobe Workfront計画ドキュメント](/help/quicksilver/planning/planning-information.md)
* [Adobe GenStudioの概要](https://business.adobe.com/jp/products/genstudio.html)
* [Adobe Customer Journey Analytics](https://business.adobe.com/jp/products/adobe-analytics/customer-journey-analytics.html)


<!--

Not sure if we should disclose this: 

## The problem the Ideation space solves

Before the Ideation space, campaign strategy relied on two slow, manual processes:

- **Gathering insights** — fragmented, time-consuming, and difficult when no prior audience data exists
- **Aligning stakeholders** — without a shared, data-backed "hook," executives, creatives, and channel partners often work from different assumptions, causing rework and delays

The Ideation space automates insight synthesis and generates a structured brief that gives everyone a shared starting point.
-->

<!--
## What's included, phase by phase

| Phase | Timeline | What's included |
|---|---|---|
| Closed Beta | July 2026 | Limited customers/users/campaigns; core agent skills (strategy framing, messaging ideation, audience definition, data ingestion, brief generation); CJA data integration |
| Open Beta | ~Sept 2026 (planned) | Quality/performance improvements; CJA integration refinements; Workfront Planning handoff; data visualization; Planning workspace structure ingestion; Unity/Conversational UI integration |
| General Availability | H2 2026 (planned) | Bring Your Own Data Source (BYODS); Workfront/Workfront Planning data integration; audience data integration; social data integration; workflow ingestion; strategy testing capabilities |

At GA, the Ideation space is also expected to be accessible through the GenStudio Home conversational UI, running as part of Adobe's Agent Orchestrator suite of agents.
-->