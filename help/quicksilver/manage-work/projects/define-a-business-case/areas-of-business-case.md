---
content-type: overview
navigation-topic: business-case-and-scorecards
title: ビジネス事例の領域の概要
description: この記事では、プロジェクトのビジネス事例の領域について説明します。
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1604'
ht-degree: 2%

---

# ビジネス事例の領域の概要

この記事では、プロジェクトのビジネス事例の領域について説明します。

プロジェクトのビジネスケースの作成については、 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Adobe Workfront管理者またはグループ管理者は、プロジェクト情報セクションを除き、ビジネスケース内のすべてのセクションを有効にしてから、プロジェクトに表示する必要があります。 「プロジェクト情報」セクションは、デフォルトで有効になっています。

ビジネスケースの領域を有効にする方法について詳しくは、  [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

プロジェクトのビジネス事例に含まれる領域を次に示します。

* プロジェクト情報
* 目標
* 費用
* リソース予算計上
* 危険
* スコアカード
* カスタムフォーム
* ビジネス ケース概要

## プロジェクト情報

この **プロジェクト情報** ビジネスケースの領域は、Workfront管理者が設定できません。 すべてのプロジェクトには、ビジネスケース内に「プロジェクト情報」領域があります。 

ビジネスケースの「プロジェクト情報」セクションには、プロジェクトが実際に開始される前の、プロジェクトの基本情報が含まれます。

次のフィールドの編集を検討してください。

* **説明**:プロジェクトの説明を指定します。
* **プロジェクト所有者**

   デフォルトでは、プロジェクトを作成するユーザーもプロジェクト所有者です。 このフィールドを編集し、別のアクティブなユーザーをプロジェクトの所有者として指定できます。

* **プロジェクト スポンサー**

   プロジェクトのスポンサーとして、プロジェクト所有者以外のユーザーを追加することを検討します。 スポンサーはビジネスケースの承認を受けます。 

* **Portfolio**:プロジェクトのPortfolioを指定します。 Portfolioを作成し、 **アクティブ** このドロップダウンメニューで選択できるようになる前に。

   ポートフォリオについて詳しくは、 [Adobe WorkfrontのPortfolioの概要](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

   Portfolioの作成について詳しくは、 [ポートフォリオの作成](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **計画済み特典**:このプロジェクトが完了したときに、組織に対してどのような金銭上の利益が計画されるかを見積もります。 任意の金額の通貨を指定でき、正の値にする必要があります。 例：$10,000。
* **ステータス**:デフォルトでは、プロジェクトリクエストのステータスはに設定されています **アイデア**.

   「ステータス」を「アイデア」または「計画」以外に変更した場合、「 **送信** 」ボタンが「ビジネス・ケース要約」領域に表示されなくなり、ビジネス・ケースを承認用に送信できなくなります。 

* **固定開始日**:プロジェクトを開始する日付を指定します。
* **固定終了日**:プロジェクトを終了する日付を指定します。

   >[!NOTE]
   >
   >ビジネス・ケースの「固定開始日」と「終了日」は、プロジェクトの計画開始日と完了日には影響しません。 これらは、プロジェクトが理想的に開発される時期に、プロジェクト作成者がリクエストした日付を表します。 代わりに、プロジェクトの「計画開始日」と「計画完了日」に、プロジェクト上のタスクに基づくプロジェクトの計画タイムラインが表示されます。

## 目標

目標は、プロジェクトの目標を定義します。 この領域はビジネスケースではデフォルトで有効になっていますが、Workfrontの管理者が表示しないように選択する場合があります。 このフィールドには、目標が優先順に表示されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
プロジェクトの個々のビジネスケースに関連していない組織の戦略目標を作成できます。 戦略的目標を作成するには、Adobe Workfront目標にアクセスできる必要があります。 その後、ビジネスケース外のプロジェクトに接続できます。 Workfront目標を使用した目標の作成について詳しくは、 [Adobe Workfront目標の概要](../../../workfront-goals/goal-management/wf-goals-overview.md).

目標の定義は、Portfolio・オプティマイザでスコアを受け取るプロジェクトに対してオプションです。 このセクションは、ビジネスケースの唯一のオプションセクションです。 ビジネス・ケースのその他のセクションは、Portfolio・オプティマイザでプロジェクトのスコアリングを行う前に完了する必要があります。 目標の作成時に、目標の優先度を指定できます。

目標について詳しくは、  [ビジネスケース目標の作成](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## 費用

費用は、プロジェクトの存続中に発生する可能性のある非労務費を表します。 この領域はビジネスケースではデフォルトで有効になっていますが、Workfrontの管理者が表示しないように選択する場合があります。 

ビジネス・ケースに入力する費用は、「計画費用」として、プロジェクトの「費用」タブにも入力されます。

費用は、プロジェクトの次のフィールドに影響します。

* 予算計上コスト
* 純価

予算原価と正味値の詳細は、次を参照してください： [ビジネス事例の財務分野の概要](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

費用について詳しくは、  [プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

Workfront管理者がカスタム費用タイプを設定できます。

カスタム費用タイプの作成の詳細については、 [カスタム経費タイプを作成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## リソース予算計上

ビジネス・ケースの「生産資源予算編成」領域では、次の処理を実行できます。

* リソースプールをプロジェクトに関連付けます。
* プロジェクトレベルでリソースを予算化します。

プロジェクト上の生産資源の予算時間は、ビジネス・ケースの「生産資源予算」領域に表示され、プロジェクトの予算労務費が生成されます。 ビジネスケースのこの領域は、デフォルトで有効になっています。

ビジネス事例のプロジェクトの予算リソースの詳細は、 [ビジネス事例の予算リソース](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

ビジネス・ケースの「生産資源予算編成」セクションを表示する際は、次の点を考慮してください。

* ここでは、次のツールを使用してリソース情報を予算できます。

   * リソースプランナー

      詳しくは、 [リソース・プランナを使用したビジネス・ケースの予算リソース](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * シナリオプランナー（会社がシナリオプランナーの追加ライセンスを購入している場合）

      詳しくは、 [シナリオ・プランナを使用したビジネス・ケースの予算生産資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      シナリオプランナーは、新しいAdobe Workfrontエクスペリエンスでのみ使用でき、追加のライセンスが必要です。 Workfront Scenario Planner の詳細は、 [シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md).

* ここに表示される情報は、システム・レベルの生産資源プランナまたはシナリオ・プランナにも表示されます。 

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* 役割が時間単価の原価率に関連付けられている場合は、生産資源を予算化した後、「生産資源予算」領域にプロジェクトの予算労務費が表示されます。 予算労務費は、プロジェクトの通貨で表示されます。

   >[!IMPORTANT]
   予算労務費は、ユーザーではなく、プロジェクト上の役割に関連する原価です。 ユーザーの全予算労務費の合計は、ユーザーに関連付けられたジョブ・ロールの予算労務費と等しくなる場合と異なる場合があります。 

   予算労務費の詳細は、 [ビジネス事例の財務分野の概要](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

   ジョブの役割を作成し、それらに時間単価を関連付ける方法の詳細は、 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## 危険

リスクとは、プロジェクトが予定通りに完了しない、または予算に達しない可能性のある要因です。 これらの要因を定義することは、Portfolioマネージャーまたはプロジェクトスポンサーが、プロジェクトの承認に関する教育を受けた決定を下すうえで重要です。 この領域はビジネスケースではデフォルトで有効になっていますが、Workfrontの管理者が表示しないように選択する場合があります。

潜在的なコストを、発生した場合に定義するリスクに関連付けることができます。 プロジェクトのリスクに伴うコストは、プロジェクトの正味価値に影響します。 

プロジェクトの純価値の詳細については、 [ビジネス事例の財務分野の概要](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

リスクの作成の詳細については、  [プロジェクトのリスクの作成と編集](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Workfront管理者がカスタムリスクタイプを設定できます。

カスタムリスクタイプの作成と編集の詳細については、 [リスクタイプの編集と作成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## スコアカード

スコアカードは、プロジェクトの整列を測定します。 この領域はビジネスケースではデフォルトで有効になっていますが、Workfrontの管理者が表示しないように選択する場合があります。

プロジェクトへのスコアカードの適用と線形スコアの生成の詳細については、 [プロジェクトにスコアカードを適用し、線形スコアを生成する](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

スコアカードを適用するには、Workfront管理者がスコアカードを作成する必要があります。 この **スコアカード** スコアカードを作成しない限り、ビジネス・ケースの領域は表示されません。

スコアカードの作成の詳細については、「  [スコアカードの作成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## カスタムフォーム

ビジネスケースを定義する際に、カスタムFormsをプロジェクトに添付できます。 ビジネス事例では、この領域はデフォルトで有効になっていません。 Workfrontの管理者が、ビジネスケースに表示するために有効にする必要があります。

ビジネス事例の領域を有効にする方法について詳しくは、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

カスタムフォームを適用するには、Workfront管理者が最初にカスタムフォームを作成する必要があります。

カスタムフォームの作成について詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

カスタムフォームを使用して、ビジネスケースの他のフィールドに表示されない追加情報を収集できます。

カスタムフォームの適用について詳しくは、 [ビジネス事例にカスタムフォームを添付する](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## ビジネス ケース概要

* [ビジネス事例の概要](#overview-of-the-business-case-summary)
* [ビジネスケースのエクスポート](#export-the-business-case)

### ビジネス事例の概要 {#overview-of-the-business-case-summary}

主なプロジェクトの財務状況の概要と、プロジェクトがスコアカードと一致しているかどうかの概要は、ビジネスケースの右上隅にあるビジネスケースの概要パネルで確認できます。

ビジネス事例サマリは編集できません。 これは、財務分野とスコアカードに関連する、プロジェクトの状態のクイックビューに過ぎません。 \
 

次のフィールドが「ビジネス事例サマリ」に表示されます。

* プロジェクトの正味の値
* プロジェクトの予算コスト
* 潜在的なリスクコスト
* 計画済み給付金
* 線形スコア

これらのフィールドについて詳しくは、 [ビジネス事例の財務分野の概要](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### ビジネスケースのエクスポート {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

ビジネスケースを印刷したり、より簡潔な形式で E メールに添付したりする必要がある場合は、ビジネスケースをPDFファイルに書き出すことができます。 

詳しくは、 [プロジェクトのビジネス事例のエクスポート](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
