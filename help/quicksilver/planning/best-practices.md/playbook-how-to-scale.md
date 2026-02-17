---
title: 初めての勝利を持続可能な勢いに変える：マネージドスケーリングのプレイブック
description: 最初に実装が成功した後にAdobe Workfront Planning を展開する方法を説明します。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 54df36b3-01a3-4fd3-b2d3-64ffb2fe5918
source-git-commit: 699add479d958b9f3fc01ae30513ddf6689620f1
workflow-type: tm+mt
source-wordcount: '2483'
ht-degree: 0%

---

# 初めての勝利を持続可能な勢いに変える：マネージドスケーリングのプレイブック

{{planning-important-intro}}


初めて成功したAdobe Workfront計画のユースケースを紹介するのは、需要の急増、新しいチームのアクセスの要望、リーダーシップの下での企業全体の可視化の可能性など、画期的な瞬間です。

しかし、これは採用の最も脆弱な段階でもあります。厳格なガバナンスに素早く移行しすぎると、チームがスプレッドシートに戻るリスクが生じます。あまりにも緩く移行すると、解決するために設定した非常に無秩序な状態が再現されます。

このプレイブックでは、最初に可視性を優先し、地域の革新を可能にし、早期に導入するのではなく、実際の運用上の成功から企業の標準を引き出せる調整エンジンとしてWorkfront計画を使用する方法について、バランスの取れたアプローチを概要を説明します。

以下は、アドビの経験から学んだこと、および注意すべき点に関するいくつかのヒントです。

## &#x200B;1. サクセストラップ

Workfront計画の導入で最も危険な段階は、最初に成功したユースケースまたは概念実証の直後のように感じる場合があります。 熱意は高いものの、技術的負債と行政の無秩序な拡大の恐れは、次の 2 つの同じように悪影響を及ぼす対応につながる可能性があります。

* **ガバナンスの超過**：システムをロックすることでシステムが非常に厳重になるため、新しいチームはスプレッドシートに戻されます。

* **ゼロガバナンス**：各チームが独自のフィールドとレコードタイプを作成し、従来の環境に見られる断片化されたメタデータの拡散を再現します。

## 2.基本理念：和解のエンジンとしてのWorkfront計画

チームの違いを止めるのではなく、Workfrontプランニングを、チームの違いを紐付けできるよう可視化する場所と位置づけています。

この取り組みをサポートするには、次の点を考慮してください。

* **導入速度の管理**：既存の環境を最適化する前に、新しいツールに拡張することに慎重になるのは当然です。 最初にシンプル化を選択すると、高度に管理された基盤が提供されますが、連携の準備が整ったチームの価値創出を遅らせる可能性があります。 この変化を導く最も効果的な方法は、可視性がステップ 1 であることを認識することだと考えています。共有されたエンタープライズ対応ツール（プレゼンテーションやスプレッドシートの無秩序な増加から脱却する）への勢いが、最終的に長期目標の妨げとなるのです。

  最初にクリーンアップを実行する代わりに、継続的なメンテナンスに少ないリソースを割り当て、差し迫ったビジネスニーズを解決する際に大幅に多くのリソースを割り当てることをお勧めします。

  例えば、1 年を「一掃」する分類だけに費やすと、増分値はほとんどありません。 ただし、クロスチームの表示を提供すると、関係者が必要とする変革的な価値が提供されると同時に、環境を経時的に管理するために必要な統合データ構造が提供されます。

  統合されたエンタープライズカレンダーや統合された Go-to マーケットロードマップを通じて、チーム間の可視性を実現できます。

* **現実を認識**：独立したチームは、当然のことながら独自のプロセスを開発しますが、多くの場合、サイロ化されたスプレッドシートに隠されたままになります。 これらのプロセスを共有環境で表示することにより、最終的に対処して改善できる場所にプロセスを配置できます。

  >[!IMPORTANT]
  >
  >Workfront Planning への移行によって混乱が生じることはありません。すでに存在する移行に光を当てます。


* **進捗の兆候を認識**：チームが独自のフィールドを要求しても、「無秩序に拡大」しません。 それを採用の兆候と考えてください。 つまり、チームにはWorkfront Planning がワークスペースとして表示されます。

* **負債の管理、非表示にしない**：後で異なる分類をクリーンアップするために必要な労力を気にするのは当然です。 しかし、厳格な基準を早く導入しすぎるという代替策により、チームはスプレッドシートに戻され、そこでプロセス（および負債）が隠されたままになっていることがよくあります。 チームが現在の分類からWorkfront Planning で開始できるようにすることで、その負債を目に見える管理された環境に移行します。 これにより、最終的な調整は、単一の圧倒的な移行プロジェクトではなく、反復的なタスクになります。

## 3.自律型ガバナンスモデル

道路上の車線とローカルの遊び場（または管理された既定値とテンプレート）を定義し、チームがそれらの中で独自のパスを柔軟に選択できるようにします。

ガイド付き自律型ガバナンスモデルの次のコンポーネントについて考えてみます。

* [グローバルレーン](#the-global-lanes)
* [地元の遊び場](#the-local-playgrounds-or-the-spokes)

詳しくは、次も参照してください。

* [戦略的なホームの展開：30 日間のランチパッド](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md)
* [成功のアーキテクト：キャンペーン階層のモデリング](/help/quicksilver/planning/best-practices.md/model-campaign-hierarchy.md)

### グローバルレーン

グローバル レーンの特性は次のとおりです。

* **制御オブジェクト**：すべてのチームがエンタープライズレポートに使用する必要があるオブジェクト（`Strategic Pillar`、`Region`、`Fiscal Quarter` など）。

* **管理者**：中核的な拠点またはマーケティング業務管理者。

* **ルール**：これらのフィールドは共有されており、必須です。

### 地元の遊び場（または「スポーク」）

その地域の遊び場の特徴を以下に示します

* **実験的なオブジェクト**：チームの戦術的ニーズに固有のフィールドまたはレコードタイプ（ソーシャルチームの `Influencer Handle` や web チームの `URL Slug` など）。

* **管理者**：チームリード（ライトガイダンス付き）。

* **ルール**：チームはここでイノベーションを行うことができます。 ローカルフィールドを 3 つ以上のチームが採用した場合は、グローバルレーンに昇格させることができます。

## &#x200B;4. ガバナンスのパラドックスについて考える。まずチームを選び、標準に従います

Workfrontプランニングの拡張における一般的な課題は、エンタープライズガバナンスとチームの運用面での整合性のどちらが優先されるかを決定することです。

この問題を解決する最も効果的な方法は、企業価値が双方向の道で構築されていることを認識することです。

* **チームには関連性が必要**：企業は、チームがアクティブに実行されている場合にのみ価値を実現します。 したがって、ガバナンスは、チームの既知の運用ニーズをサポートする構造を提供することで、チームにサービスを提供する必要があります。

* **企業には可視性が必要**：データが集約できるほどクリーンな場合にのみ、リーダーシップは十分な情報に基づいた意思決定を行うことができます。 したがって、チームは、ポートフォリオの表示に必要な最小限の実行可能なメタデータを提供することで、企業に貢献する必要があります。

マネージドスケーリングの目標は、可視性を提供するのに十分な標準化によって、これら 2 つのニーズの積集合を見つけることです。ただし、チームの実行を停止させるほどではありません。

ガバナンスモデルを構築する際に、次の段階を考慮します。

* [優先度の調整：データとビジュアライゼーションの比較](#align-priorities-data-vs-visualization)
* [サービス主導の観測段階](#the-service-led-observation-phase)
* [遡及調和](#retroactive-harmonization)

### 優先度の調整：データとビジュアライゼーションの比較

拡大縮小する場合は、値の定義がペルソナ間で異なることを表していることを認識します。

* **管理者または製品所有者** は、統合された分類や分類を重視します。 彼らの目標は、長期的なスケーラビリティをサポートするクリーンなデータアーキテクチャです。

* **関係者またはリーダー** の値ビジュアライゼーションと、グローバルカレンダーまたはポートフォリオタイムラインに取り込むことができるinsight。 目標は、データを実用的にする稲妻の瞬間を特定することです。

>[!NOTE]
>
>この戦略は、関係者のビジュアライゼーションのニーズを、チームが管理者のデータ標準規格のニーズを満たすインセンティブとして使用することです。 リーダーシップが必要とするカレンダーを提供することで、統一された分類を得ることができます。


### サービス主導の観測段階

初期のスケールアップ段階では、管理者の役割は、チームと企業の間でのこの交換を容易にすることです。

管理者は、次の操作を行うことで、この交換を容易にすることができます。

* **標準化よりも運用の優先順位を付ける**：グローバルな定義の欠如によって立ち往生するよりも、サイロ化されたワークスペースでチームが積極的に計画を立てる方が良いでしょう。 このアクティビティは、健全な実際の標準を構築するために必要な生データです。

* **表示の最小値の特定**：リーダーシップと連携して、エンタープライズレポートにクリーンにする必要がある 3～5 個のフィールド（`Strategic Alignment`、`Start Date`、`Budget` など）を特定します。 表示の最小フィールドにのみ適用エネルギーを集中させます。

### サービスとしてのガバナンス

チーム間で既知のニーズのパターンが発生したら、企業は、それらのパターンをグローバルサービスに統合するために移行できます。 これは、サービスとしてのガバナンスです。

サービスとしてのガバナンスを達成するには、以下の手順を実行します。

* **成功したパターンを観察**：チームが既に構築し、採用した勝者の分類を特定します。

* **共同で握手を交わす**：チームチャンピオンを集めて、各地域での成功を共通のエンタープライズ標準に磨き上げます。

* **サービスとしてのデプロイ**：新しいグローバルレーンを制限としてではなく、作業を行うユーザーのレポートとチーム間の連携を簡素化する方法として展開します。

>[!IMPORTANT]
>
>ガバナンスは、運用の成功に対する対応であって、そのための前提条件ではないことに注意してください。

## &#x200B;5. フィールド管理のためのスケーリング機構

### パターンベースのフィールド成長モデル

この哲学を適用するには、データ構造に対する思慮深いアプローチが必要です。 ガバナンスの無秩序な拡散を避けるために、個々のリクエストごとにグローバルなフィールドを構築したいという衝動に抵抗してください。

代わりに、次のフィールド成熟度パスを使用して、実際の使用状況にエンタープライズ標準をガイドさせることができます。

* **レベル 1：ローカル実験**：チーム A がワークスペースにカスタムフィールドを作成します。

* **レベル 2：パターン認識**：管理者は、チーム B とチーム C が類似のフィールドを使用または要求していることに気づきます。

* **レベル 3：企業の標準化**：管理者は、グローバル分類Workspaceでレコードタイプとしてフィールドの標準化された単一バージョンを作成し、チームに同時配信します。

### フィールドの廃止方法

フィールドが関係しなくなり、廃止する必要が生じた時点に到達します。

Workfront Planning には現在、フィールドのネイティブ・アーカイブ機能がないので、ローカル・フィールドを廃止する場合に、UI を混乱させずに履歴データを保持するには、意図的なソフト廃止プロセスが必要です。

フィールドを廃止するには：

1. データ移行を実行します。 テーブルビュー（または Fusion）を使用して、ローカルシャドウフィールドから新しいグローバルレーンフィールドに値を一括コピーします。 この移動中に、データが検証され、消去されていることを確認します。

2. 非推奨のフィールド名を変更：ローカルフィールドの名前を `[DEPRECATED]` や `z_` などのプレフィックス（例：`z_Language (Old)`）に変更します。 これにより、フィールドがフィールドピッカーの下部にプッシュされ、信頼できるソースではなくなったことをユーザーに知らせます。

3. すべてのレコードフォームから非推奨フィールドを削除します。 これが最も重要な手順です。 これにより、必要に応じて既存のテーブルビューやレポートに古いデータを表示したまま、新しいデータが入力されるのを防ぐことができます。

4. 移行中にデータが失われないように、廃止されたフィールド（プレフィックスが付けられ、フォームから削除された）を 30～60 日間保持して、日没期間を開始します。 この期間を過ぎると、グローバルレーン内でデータが完全に紐付けされた場合、ローカルフィールドをワークスペースから削除できます。

## &#x200B;6. Workfrontのドリフトを回避する

Planning が乱雑にならないようにするには、次の手順を実行します。

* **抽象化レイヤーについて**:Planning のすべてのフィールドは、戦略的な質問に答える必要があります。 フィールドが戦術的なトラッキングにのみ使用される場合（例えば、フィールドが「このプルーフは承認されましたか」などの質問に回答する場合）、Workfrontに保持します。

* **最初に統合を実行**：チームが新しいメタデータフィールドを必要としている場合は、まずグローバル分類を確認するようにチームを招待します。 これには、チームのリードにグローバル分類ワークスペースへの読み取り専用アクセスを許可する必要があります（セクション 7 を参照）。 戦術的なニーズを既存の戦略的フィールドにマッピングすることで、不要な重複を防ぎ、レポートの整合性を維持できます。

## 7.読み取り専用アクセス表示モデル

チームがグローバル分類ワークスペースに読み取り専用でアクセスして、どのような概念が独自のワークフローに適用される可能性があるかを確認できるようにすることで、サイロ化された作業のノイズなしでサイロ化された感情を解決できます。

次の点に注意してください。

* **問題**:（スポーク内の）チームは、自分のレコードしか表示されないので孤立していると感じます。

* **修正点**：共有レコードタイプのプライマリとして指定されたワークスペースへの読み取り専用アクセス権をチームに付与します。

  詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。

* **結果**：チームは、インスピレーションと連携のためにより広いエンタープライズコンテキストを確認できますが、ローカルワークスペースはクリーンなままで、特定のタスクに焦点を当てています。

## 8.ワークショップを通じた成長管理

Workfront計画の拡大は、技術的な課題と同じくらい文化的な課題です。 ターゲットを絞ったワークショップを使用してガバナンスギャップを埋める。

以下は、ワークショップのアイデアです。

* [「必要な混乱」発見ワークショップ](#the-necessary-mess-discovery-workshop)
* [「戦略的な可視性」の連携セッション](#the-strategic-visibility-alignment-session)
* [「Spoke-to-global」ショーケース](#the-spoke-to-global-showcase)
* [「継続的なサポート」営業時間](#the-ongoing-support-office-hours)

### 「必要な混乱」発見ワークショップ

* **対象読者**：地域のマーケティングリードや Ops チャンピオン。

* **目標**：現在のサイロ化された現実や、実際の断片化された運用データを文書化します。

* **メッセージ**:「フィールドを削除する権限がありません。 それらがグローバル戦略にどのように結び付いているかを理解するために、私たちはここにいます」

* **成果**：地域の戦術分野をグローバルな戦略的レーンにマッピングする草案。

### 「戦略的な可視性」の連携セッション

* **対象読者**：マーケティングの大まかな関係者（リーダーシップ役割の人物など）。

* **目標**：シンプルなファーストの不安の枠組みを変えます。

* **メッセージ**:「開始するのに、完璧な分類は必要ありません。 私たちは、完璧な分類を構築するための環境としてWorkfrontプランニングを使用しています。」

* **結果**:Workfrontが現在の状態のままである間に、紐付けエンジンとしてWorkfront Planning に進むための承認。

### 「Spoke-to-global」ショーケース

* **対象読者**:Workfrontの計画を検討する新しいチーム。

* **目標**：サイロ化された感情を軽減します。

* **メッセージ**:「チーム A のローカル作業が、指定されたプライマリのWorkspaceをどのように自動的にフィードするかを確認します。 自分の作業に対しても、同じ可視性を持つことができます。」

* **結果**：地域の独立性を失うことなく接続のメリットを確認している新しい部門からオプトインします。

### 「継続的なサポート」営業時間

* **対象読者**：すべてのWorkfront Planning ユーザー（現在および将来のユーザー）。

* **目標**：トラブルシューティングや戦術的なガイダンスのために、低コストの繰り返し環境を提供します。

* **メッセージ**:「間違った質問はありません。 お客様が特定の計画上の課題をリアルタイムで解決できるよう、アドビがサポートします。」

* **結果**：ユーザーの信頼の向上、技術的摩擦の迅速な解決、国際的な標準化が必要となる可能性のある新しいパターンの特定。

## 9.規模に応じた人材の確保：役割・責任

マネージドスケーリングモデルの成功には、単なるツール設定以上のものが必要です。 グローバル チームとスポーク チームに明確な役割を分散させる必要があります。

以下のサブセクションでは、スケールモデルの管理に関する主なプレーヤーのアイデアを見つけることができます。

### エンタープライズアーキテクト（センターオブエクセレンスまたはマーケティングオペレーション）

* **焦点**：企業の整合性、システムパフォーマンス、統合データ分類。

* **責務**:

   * グローバル分類Workspaceを管理します。

   * ローカルでの成功をグローバル標準に昇格させることで、フィールド成熟度パスを促進します。

   * エグゼクティブレポート用にWorkspaceのプライマリビューを維持します。

   * ワークスペース全体で毎月のセマンティック監査をリードします。

### スポーク チャンピオン （チーム プロセス オーナー）

* **焦点**：チームの関連性と導入の速度。

* **責務**:

   * 部門チームの単一の連絡窓口として機能します。

   * ローカルワークスペース構造とカスタムフィールド実験を管理します。

   * チームがデータ入力に管理ゲートウェイ Formsを使用できるようにします。

   * ハーモナイゼーション中に協調ハンドシェイクに参加します。

### エグゼクティブスポンサー（マーケティングリーダーシップ）

* **フォーカス**：戦略的な連携、OKR の可視性およびポートフォリオビジュアライゼーション（グローバルカレンダーなど）。

* **責務**:

   * グローバル分類ワークスペースでエンタープライズマーケティング OKR を定義します。

   * [ 表示設定 ] [ 手順 1] の値を他の引出線に対して支持します。

   * 80/20 リソース割り当てを強制的に行います（クリーンアップに対する値）。

### イネーブルメントリード（変更管理）

* **フォーカス**：文化のシフトとスキルの開発。

* **責務**:

   * Office Hours およびディスカバリーワークショップの定期的なタッチポイントをホストします。

   * 内部の成功事例ショーケースを維持します。

   * 解決するエンタープライズアーキテクトの技術的な摩擦ポイントを特定します。

## 10.次のチームの拡大に向けたチェックリスト

実装の成功から得られるすべての学習は、さらなる実装に使用できるチェックリストを生成する必要があります。

チェックリストに含まれる内容の例を以下に示します。

* [ ]&#x200B;**チャンピオンの特定**：この新しいチームのプロセスオーナーまたはチャンピオンは誰ですか？

* [ ]&#x200B;**ローカル差分の定義**：このチームでは、グローバル標準で現在提供されていない 2 ～ 3 個のフィールドのうち、必要なものはどれですか？

* [ ]&#x200B;**グローバルレーンへのマッピング**：既存のグローバルフィールドで、将来のチームのニーズの 80% を満たすことができますか？

* [ ]&#x200B;**グローバルな表示の許可**:1 日目に、関連するプライマリワークスペースとグローバルな分類ワークスペースへの読み取り専用アクセス権を付与します。

* [ ]&#x200B;**ハンドオフの確立**：その作業が関連するプライマリワークスペースにどのように反映されるか。 例えば、作業はグローバルレコードタイプや特定の検索フィールドを使用して、関連するプライマリワークスペースにフィードする場合があります。

<!--original content: 

**Version**: 1.0 

**Context**: "We've landed our first use case, and now everyone wants in." 

 

## 1. The "Success Trap" 

Sometimes it can feel like the most dangerous phase of WFP adoption is immediately after the first successful use case or POC. Enthusiasm is high, but the fear of "technical debt" and "administrative sprawl" can lead to two equally damaging responses: 

1.  **Over-Governance**: Locking down the system so tightly that new teams revert to spreadsheets. 

2.  **Zero-Governance**: Letting every team create their own fields and record types, recreating the fragmented metadata sprawl found in legacy environments. 

 

## 2. The Core Philosophy: WFP as the "Reconciliation Engine" 

Instead of trying to stop teams from being different, we position WFP as the place where those differences are **made visible so they can be reconciled**. 

 

*   **Managing Adoption Velocity**: It is natural to feel cautious about expanding into a new tool before "cleaning up" existing environments. While choosing to **Simplify First** provides a highly governed foundation, it can delay time-to-value for teams ready to align. We believe the most effective way to lead through this change is to recognize that **visibility is Step 1**. Momentum toward a shared, enterprise-ready tool (moving away from the sprawl of PPTs and spreadsheets) is what ultimately unblocks long-term goals.  

 

    **Recommendation**: Instead of a "Clean Up First" mandate, we recommend allocating a smaller portion of resources to ongoing maintenance and a significantly larger portion to solving pressing business needs. For example, spending a year solely on "cleaning up" taxonomies yields little incremental value. However, delivering **cross-team visibility** (e.g., through a Unified Enterprise Calendar or a consolidated GTM roadmap) provides the transformative value your stakeholders need, while providing the unified data structure you need to govern the environment over time. 

*   **Acknowledge the Reality**: Independent teams naturally develop their own processes, which often stay hidden in siloed spreadsheets. Transitioning to WFP doesn't create a mess; it shines a light on the one that already exists. By making these processes visible in a shared environment, you put them in the one place where they can finally be addressed and improved. 

*   **The Progress Signal**: When a team asks for their own fields, it's not "sprawl"—it's **Adoption**. It means they see WFP as their workspace. 

*   **Manage Debt, Don't Hide It**: It is natural to be concerned about the effort required to clean up divergent taxonomies later. However, the alternative—forcing strict standards too early—often drives teams back to spreadsheets where their processes (and their debt) remain hidden. By allowing teams to begin in WFP with their current classifications, you are moving that debt into a visible, governed environment. This makes the eventual reconciliation an iterative task rather than a single, overwhelming migration project. 

 

## 3. The "Lanes on a Road" Governance Model 

Scale without debt by defining "Global Lanes" and "Local Playgrounds." 

 

### A. The Global Lanes 

*   **Controlled Objects**: Objects that every team must use for enterprise reporting (e.g., `Strategic Pillar`, `Region`, `Fiscal Quarter`). 

*   **Managed By**: The Central COE/Marketing Ops Admin. 

*   **Rule**: These fields are "Shared" and mandatory. 

 

### B. The Local Playgrounds (Spokes) 

*   **Experimental Objects**: Fields or record types specific to a team's tactical needs (e.g., a Social team's `Influencer Handle` or a Web team's `URL Slug`). 

*   **Managed By**: The Team Lead (with light guidance). 

*   **Rule**: Teams can innovate here. If a "Local" field is adopted by >3 teams, it is "Promoted" to a Global Lane. 

 

## 4. The Governance Paradox: Teams First, Standards Follow 

A common challenge in scaling WFP is deciding which comes first: **Enterprise Governance** or **Team Operational Alignment**.  

 

We believe the most effective way to navigate this is to recognize that enterprise value is built on a two-way street: 

1.  **Teams need relevance**: The enterprise only realizes value when its teams are actively executing. Therefore, governance must **serve the teams** by providing structure that supports their known operational needs. 

2.  **The Enterprise needs visibility**: Leadership can only make informed decisions when data is clean enough to aggregate. Therefore, the teams must **serve the enterprise** by providing the minimum viable metadata required for portfolio visibility. 

 

The goal of "Managed Scaling" is to find the intersection of these two needs—standardizing enough to provide visibility, but not so much that you stall team execution. 

 

### A. Aligning Priorities: Data vs. Visualization 

When scaling, recognize that the definition of "Value" differs between personas: 

*   **The Admin/Product Owner**: Values **unified taxonomies and classifications**. Their goal is a clean data architecture that supports long-term scalability. 

*   **The Stakeholder/Leader**: Values **visualization and insight** (e.g., a Global Calendar or a Portfolio Timeline). Their goal is the "Lightning Moment" that makes the data actionable. 

 

**The Strategy**: Use the stakeholder's need for visualization as the *incentive* for the team's compliance with the admin's need for data standards. You get the unified taxonomy by delivering the "Super Calendar" that leadership demands. 

 

### B. The "Service-Led" Observation Phase 

During early scale-up, the Admin's role is to facilitate this exchange between teams and the enterprise. 

*   **Prioritize Operation over Standardization**: It is better to have teams actively planning in siloed workspaces than to have them stalled by a lack of global definitions. This activity is the "raw data" required to build healthy, real-world standards. 

*   **Identify the "Visibility Minimums"**: Work with leadership to identify the 3-5 fields that *must* be clean for enterprise reporting (e.g., `Strategic Alignment`, `Start Date`, `Budget`). Focus your enforcement energy ONLY here. 

 

### B. Retroactive Harmonization (Governance as a Service) 

Once a pattern of "known needs" emerges across teams, the enterprise can move to consolidate those patterns into a global service. 

1.  **Observe Successful Patterns**: Identify the "winning" taxonomies that teams have already built and adopted. 

2.  **The Collaborative Handshake**: Bring team champions together to refine their local successes into a shared enterprise standard. 

3.  **Deploy as a Service**: Roll out the new global lanes not as a "restriction," but as a way to simplify reporting and cross-team alignment for the people doing the work. 

 

**Key Takeaway**: Governance should be a response to operational success, not a prerequisite for it.  

 

## 5. Scaling Mechanics: The Pattern-Based Growth Model 

Applying this philosophy requires a thoughtful approach to data structure. To avoid "Governance Sprawl," resist the urge to build global fields for every individual request. Instead, use the **Field Maturity Path** to let real-world usage guide your enterprise standards: 

 

1.  **Level 1: Local Experiment**: Team A creates a custom field in their workspace. 

2.  **Level 2: Pattern Recognition**: The Admin notices Teams B and C are using or asking for a similar field. 

3.  **Level 3: Enterprise Standardization**: The Admin creates a single, standardized version of that field as a record type in the **Global Taxonomy Workspace** and syndicates it to teams. 

 

### The Mechanics of "Soft Retirement" 

Because WFP does not currently have a native "Archive" feature for fields, retiring a local field requires a deliberate "Soft Retirement" process to preserve historical data without cluttering the UI: 

 

1.  **Data Migration**: Use a table view (or Fusion) to bulk-copy values from the local "Shadow" field into the new Global Lane field. Ensure the data is validated and cleaned during this move. 

2.  **Rename for Deprecation**: Rename the local field with a prefix like `[DEPRECATED]` or `z_` (e.g., `z_Language (Old)`). This pushes the field to the bottom of field pickers and signals to users that it is no longer the "Source of Truth." 

3.  **Form Removal**: **This is the most critical step.** Remove the deprecated field from all **Record Forms**. This prevents new data from being entered while keeping the old data visible in existing table views or reports if needed. 

4.  **The "Sunset" Period**: Keep the deprecated field (prefixed and off-form) for 30-60 days to ensure no data was missed during migration. After this period, if the data is fully reconciled in the Global Lane, the local field can be deleted from the workspace. 

 

## 6. Avoiding the "Core Drift" (The Abstraction Rule) 

To prevent Planning from becoming as cluttered as Core: 

*   **The Abstraction Layer**: Every field in WFP should answer a **Strategic Question**. If a field is only used for tactical tracking (e.g., "Was this proof approved?"), keep it in Core. 

*   **Consolidation First**: If a team wants a new metadata field, invite them to check the Global Taxonomy first. This requires granting team leads **Read-Only access** to the Global Taxonomy workspace (see Section 7). By mapping their tactical needs to an existing strategic field, you prevent unnecessary duplication and maintain reporting integrity. 

 

## 7. The "Read-Only Access" Visibility Model 

Solve the "Siloed" feeling without the noise of "Siloed" work. 

*   **The Problem**: Teams in spokes feel isolated because they only see their own records. 

*   **The Fix**: Grant teams **Read-Only access to the workspaces designated as 'Primary' for those shared record types**.  

*   **The Result**: They can see the broader enterprise context for inspiration and alignment, but their local workspace remains clean and focused on their specific tasks. 

 

## 8. Managing Growth through Workshops 

Scaling WFP is as much a cultural challenge as a technical one. Use targeted workshops to bridge the "Governance Gap." 

 

### A. The "Necessary Mess" Discovery Workshop 

*   **Audience**: Regional Marketing Leads and Ops Champions. 

*   **Goal**: Document the current "Siloed Reality" (the fragmented operational data). 

*   **The Message**: "We aren't here to delete your fields. We're here to understand how they link to the global strategy." 

*   **Outcome**: A draft mapping of local tactical fields to global strategic lanes. 

 

### B. The "Strategic Visibility" Alignment Session 

*   **Audience**: High-level Marketing Stakeholders (leadership). 

*   **Goal**: Reframe the "Simplify First" anxiety. 

*   **The Message**: "We don't need a perfect taxonomy to start. We are using WFP as the environment to *build* the perfect taxonomy." 

*   **Outcome**: Approval to move forward with WFP as the reconciliation engine while Core remains in its current state. 

 

### C. The "Spoke-to-Global" Showcase 

*   **Audience**: New teams exploring WFP. 

*   **Goal**: Reduce the "siloed" feeling. 

*   **The Message**: "See how Team A's local work automatically feeds the designated Primary Workspace? You can have that same visibility for your work too." 

*   **Outcome**: Opt-in from new departments who see the benefit of being "connected" without losing their local independence. 

 

### D. The "Ongoing Support" Office Hours 

*   **Audience**: All WFP users (current and prospective). 

*   **Goal**: Provide a recurring, low-stakes environment for troubleshooting and tactical guidance. 

*   **The Message**: "There are no wrong questions. We are here to help you solve your specific planning challenges in real-time." 

*   **Outcome**: Increased user confidence, faster resolution of technical friction, and the identification of new patterns that might warrant global standardization. 

 

## 9. Staffing for Scale: Roles and Responsibilities 

Success in a managed scaling model requires more than just tool configuration; it requires a clear distribution of roles across the Global and Spoke teams. 

 

### A. The Enterprise Architect (Central COE/Marketing Ops) 

*   **Focus**: Enterprise integrity, system performance, and **unified data taxonomy**. 

*   **Responsibilities**: 

    *   Manages the **Global Taxonomy Workspace**. 

    *   Facilitates the **Field Maturity Path** (promoting local successes to global standards). 

    *   Maintains the **Primary Workspace** views for executive reporting. 

    *   Leads the monthly **Semantic Audit** across workspaces. 

 

### B. The Spoke Champion (Team Process Owner) 

*   **Focus**: Team relevance and adoption velocity. 

*   **Responsibilities**: 

    *   Acts as the single point of contact for the functional team. 

    *   Owns the local workspace structure and custom field experiments. 

    *   Ensures the team uses the **Governed Gateway** (Forms) for data entry. 

    *   Participates in the **Collaborative Handshake** during harmonization. 

 

### C. The Executive Sponsor (Marketing Leadership) 

*   **Focus**: Strategic alignment, OKR visibility, and **portfolio visualization (e.g., Global Calendaring)**. 

*   **Responsibilities**: 

    *   Defines the enterprise **Marketing OKRs** in the Global Taxonomy workspace. 

    *   Champions the value of "Visibility Step 1" to other leaders. 

    *   Reinforces the 80/20 resource allocation (Value over Cleanup). 

 

### D. The Enablement Lead (Change Management) 

*   **Focus**: Cultural shift and skill development. 

*   **Responsibilities**: 

    *   Hosts recurring **Office Hours** and **Discovery Workshops**. 

    *   Maintains the internal "Success Story" showcase. 

    *   Identifies technical friction points for the Enterprise Architect to resolve. 

 

## 10. Checklist for Scaling the Next Team 

* [ ] **Identify the Champion**: Who is the "Process Owner" or "Champion" of this new team? 

* [ ] **Define the "Local Delta"**: What 2-3 fields does this team need that the Global standard doesn't currently provide? 

* [ ] **Map to Global Lanes**: Which existing Global fields can satisfy 80% of their needs? 

* [ ] **Grant Global Visibility**: Give them Read-Only access to the relevant Primary Workspaces and the Global Taxonomy workspace on Day 1. 

* [ ] **Establish the Handoff**: How does their work "feed" the relevant Primary Workspaces? (e.g., via a Global Record Type or a specific lookup).

-->