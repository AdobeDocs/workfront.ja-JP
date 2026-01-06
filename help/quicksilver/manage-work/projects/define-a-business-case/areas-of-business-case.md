---
content-type: overview
navigation-topic: business-case-and-scorecards
title: ビジネスケースのエリアの概要
description: この記事では、プロジェクトのビジネスケースのエリアについて説明します。
author: Becky
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 43%

---

# ビジネスケース領域の概要

<!-- Audited: 4/2025 -->

この記事では、プロジェクトのビジネスケースのエリアについて説明します。

プロジェクトのビジネスケースの作成について詳しくは、[プロジェクトのビジネスケースを作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

プロジェクトに表示される前に、Adobe Workfront管理者またはグループ管理者がビジネスケース内のすべてのセクションを有効にする必要があります（プロジェクト情報セクションを除く）。 「プロジェクト情報」セクションは、デフォルトで有効になっています。

ビジネスケースの領域を有効にする方法については、記事 [&#x200B; システム全体のプロジェクト環境設定の指定 &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) の「ビジネスケース」の節を参照してください。

プロジェクトのビジネスケースに含まれるエリアを次に示します。

* プロジェクト情報
* Goals
* 費用
* リソース予算計上
* リスク
* スコアカード
* カスタムフォーム
* ビジネスケースの概要

## プロジェクト情報

ビジネスケースのプロジェクト情報セクションには、プロジェクトが実際に開始される前のプロジェクトの基本情報が含まれます。

すべてのプロジェクトには、事前に設定されたフィールドを含むビジネスケースのプロジェクト情報エリアがあります。つまり、Workfront管理者は、このエリアに表示するフィールドを設定できません。

次のフィールドの編集を検討してください。

* **説明**: プロジェクトの説明を追加します。

* **プロジェクト所有者**: デフォルトでは、プロジェクトを作成したユーザーはプロジェクト所有者でもあります。 別のアクティブなユーザーをプロジェクトの所有者として選択するには、このフィールドを編集します。

* **プロジェクトスポンサー**: プロジェクトスポンサーになるアクティブなユーザーを選択します。 スポンサーは、ビジネスケースの承認を受けます。

* **Portfolio**: プロジェクトのPortfolioを選択します。 このドロップダウンメニューで選択できるようにするには、Portfolioを作成して「アクティブ」ステータスにする必要があります。

  ポートフォリオについて詳しくは、[Adobe Workfront でのポートフォリオの概要](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)を参照してください。

  ポートフォリオの作成について詳しくは、[ポートフォリオの作成](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)を参照してください。

* **予定利益**：このプロジェクトが完了したときに、組織が予定する金銭上の利益を見積もります。任意の金額の通貨を指定でき、正の値（例：$10,000）にする必要があります。

* **ステータス**：デフォルトでは、プロジェクトリクエストのステータスはアイデアに設定されます。 ステータスを Idea または Planning 以外の値に変更すると、「発行」ボタンが「ビジネス・ケースの要約」領域から消え、ビジネス・ケースを承認用に発行できなくなります。

* **固定開始日**：プロジェクトを開始する日付を指定します。

* **固定終了日**：プロジェクトを終了する日付を指定します。

  >[!NOTE]
  >
  >ビジネスケースの「固定開始日」と「終了日」は、プロジェクトの予定開始日と完了日には影響しません。これらは、プロジェクトが理想的に開発されるタイミングについて、プロジェクト作成者がリクエストした日付を表します。 代わりに、プロジェクトの予定開始日と予定完了日は、プロジェクトのタスクに基づいて、プロジェクトの予定タイムラインを示します。

## Goals

目標は、プロジェクトの目標を定義します。 この領域は、ビジネスケースではデフォルトで有効になっていますが、Workfront管理者は表示しないようにしている場合があります。 このフィールドには、目標が優先順に表示されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>プロジェクトの個々のビジネスケースに関連していない組織の戦略目標を作成できます。戦略的目標を作成するには、Adobe Workfront Goals へのアクセス権が必要です。 その後、ビジネスケース外のプロジェクトに接続できます。Workfront Goals を使用した目標の作成について詳しくは、[Adobe Workfront Goals の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。

プロジェクトでPortfolio Optimizer でスコアを受け取るには、目標の定義はオプションです。 このセクションは、ビジネスケースの唯一のオプションセクションです。ビジネスケースの他のすべてのセクションは、Portfolio Optimizer でプロジェクトにスコアリングする前に完了する必要があります。 目標を作成する際に、目標の優先度レベルを指定できます。

詳しくは、[&#x200B; ビジネスケースの目標の作成 &#x200B;](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md) を参照してください。

## 費用

費用は、プロジェクトの存続中に発生する可能性のある非労務費を表します。 この領域は、ビジネスケースではデフォルトで有効になっていますが、Workfront管理者は表示しないようにすることができます。

ビジネスケースに入力する費用は、プロジェクトの「費用」タブにも予定費用として入力されます。

費用は、プロジェクトの次のフィールドに影響します。

* 予算計上コスト
* 純価

Workfront 管理者はカスタム費用タイプを設定できます。

予算計上コストと純価について詳しくは、[ビジネスケースの財務フィールドの概要](../../../manage-work/projects/define-a-business-case/business-case-finances.md)を参照してください。

費用について詳しくは、[&#x200B; プロジェクト費用の管理 &#x200B;](../../../manage-work/projects/project-finances/manage-project-expenses.md) を参照してください。

カスタム費用タイプの作成について詳しくは、「[&#x200B; カスタム費用タイプの作成 &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md)」を参照してください。

## リソース予算計上

ビジネスケースの「リソース予算計上」エリアでは、次のアクションを実行できます。

* リソースプールをプロジェクトに関連付ける。
* プロジェクトレベルでリソースを予算に計上する。

プロジェクトのリソースに予算計上された時間は、ビジネス・ケースの「リソース予算計上」領域に表示され、プロジェクトの予算計上労力コストが生成されます。 この領域はデフォルトで有効になっています。

ビジネスケースでのプロジェクトのリソース予算計上について詳しくは、[ビジネスケースでのリソースの予算計上](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。

<!--![Business case resource budgeting](assets/business-case-sp-selected-with-choose-button-350x121.png)-->

ビジネスケースの「リソース予算計上」セクションを確認する際は、次の点を考慮してください。

* ここでは、次のツールを使用してリソース情報の予算を計上できます。

   * リソースプランナー

     詳しくは、[リソースプランナーを使用したビジネスケースでのリソースの予算計上](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md)を参照してください。

   * シナリオプランナ

     詳しくは、[シナリオプランナーを使用したビジネスケースでのリソースの予算計上](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)を参照してください。

     シナリオプランナーは、新しい Adobe Workfront エクスペリエンスでのみ使用でき、追加のライセンスが必要です。Workfront シナリオプランナーについて詳しくは、[シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。

* ここに表示される情報は、システムレベルのリソースプランナーやシナリオプランナーにも表示されます。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in NWE only)<br></p>
  -->

* 役割が 1 時間当たりのコスト率に関連付けられている場合、リソースを予算計上すると、プロジェクトの予算計上労力コストが「リソース予算計上」領域に表示されます。 予算計上労力コストは、プロジェクトの通貨で表示されます。

  >[!IMPORTANT]
  >
  >予算計上労力コストは、ユーザーではなく、プロジェクトの担当業務に関連付けられたコストです。ユーザーの予算計上労力コストの合計は、ユーザーに関連付けられた担当業務の予算計上労力コストと等しくなる場合もあれば、異なる場合もあります。

  予算計上労力コストについて詳しくは、[ビジネスケースの財務フィールドの概要](../../../manage-work/projects/define-a-business-case/business-case-finances.md)を参照してください。

  担当業務の作成および 1 時間当たりのコストのレートを担当業務に関連付ける方法について詳しくは、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。

## リスク

リスクとは、プロジェクトが期限や予算を超過せずに完了することを妨げる可能性のある要因のことです。これらの要因の定義は、Portfolio マネージャーまたはプロジェクトスポンサーが、プロジェクトの承認に関して知識に基づいた決定を下すために重要です。 この領域は、ビジネスケースではデフォルトで有効になっていますが、Workfront管理者は表示しないようにすることができます。

発生した場合に備え、潜在的なコストを定義しているリスクに関連付けることができます。 リスクのコストは、プロジェクトの純価に影響します。

Workfront 管理者はカスタムリスクタイプを設定できます。

プロジェクトの純価値の詳細については、[ビジネスケースの財務フィールドの概要](../../../manage-work/projects/define-a-business-case/business-case-finances.md)を参照してください。

リスクの作成の詳細については、「[&#x200B; プロジェクトのリスクの作成と編集 &#x200B;](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)」を参照してください。

カスタム危険タイプの作成および編集の詳細については、「[&#x200B; 危険タイプの編集および作成 &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md)」を参照してください。

## スコアカード

スコアカードは、プロジェクトの整合性を測定します。 この領域は、ビジネスケースではデフォルトで有効になっていますが、Workfront管理者は表示しないようにすることができます。

スコアカードを適用するには、まずWorkfront管理者がスコアカードを作成する必要があります。 ビジネス ケースのスコアカード エリアは、スコアカードが作成されない限り表示されません。

プロジェクトへのスコアカードの適用および整合性スコアの生成について詳しくは、[プロジェクトへのスコアカードの適用および整合性スコアの生成](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)を参照してください。

スコアカードの作成について詳しくは、[&#x200B; スコアカードの作成 &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md) を参照してください。

## カスタムフォーム

ビジネスケースを定義する際に、カスタムFormsをプロジェクトに添付できます。 この領域は、ビジネスケースではデフォルトで有効になっていません。Workfront管理者は、ビジネスケースでこの領域を表示できるようにするには、有効にする必要があります。

カスタムフォームを適用するには、まずWorkfront管理者がカスタムフォームを作成する必要があります。

カスタムフォームを使用して、ビジネスケースの他のフィールドに表示されない追加情報を収集できます。

ビジネスケースのエリアを有効にする方法について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

カスタムフォームの作成について詳しくは、「[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

カスタムフォームの適用について詳しくは、[ビジネスケースへのカスタムフォームの添付](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md)を参照してください。

## ビジネスケースの概要

* [ビジネスケースの概要](#overview-of-the-business-case-summary)
* [ビジネスケースをエクスポート](#export-the-business-case)

### ビジネスケースの概要 {#overview-of-the-business-case-summary}

ビジネスケースの右上隅にあるビジネスケースの概要パネルを使用して、メインプロジェクトの財務の概要と、プロジェクトがスコアカードに合っているかどうかを確認できます。

ビジネスケース概要は、財務フィールドとスコアカードに関連するため、プロジェクトの状態のクイックビューにすぎず、編集することはできません。

ビジネスケースの概要には、次のフィールドが表示されます。

* プロジェクト純価
* プロジェクト予算計上コスト
* 潜在リスクコスト
* 予定利益
* 整合性スコア

これらのフィールドの詳細については、[ビジネスケースの財務フィールドの概要](../../../manage-work/projects/define-a-business-case/business-case-finances.md)を参照してください。

### ビジネスケースをエクスポート {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

ビジネスケースを印刷する必要がある場合や、より圧縮された形式でメールに添付する必要がある場合は、PDF ファイルにエクスポートできます。

詳しくは、[プロジェクトのビジネスケースの書き出し](../../../manage-work/projects/define-a-business-case/export-business-case.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it. </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.  The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>

