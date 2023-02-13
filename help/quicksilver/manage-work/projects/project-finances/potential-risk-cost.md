---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 潜在的なリスクコストの計算
description: プロジェクトの潜在的なリスクコストでは、プロジェクトのリスクの潜在的なコストと発生する確率が考慮されます。
author: Alina
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 潜在的なリスクコストの計算

プロジェクトの潜在的なリスクコストでは、プロジェクトのリスクの潜在的なコストと発生する確率が考慮されます。

## プロジェクトの潜在的なリスクコストの概要

Adobe Workfrontは、次の式を使用してプロジェクトの潜在的リスクコストを計算します。

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

プロジェクトの潜在的なリスクコストを見直す際は、次の点を考慮してください。

* プロジェクトの計画リスクコストは、潜在的リスクコストと同じです。 
* 潜在的なリスクコストは、プロジェクトの計画コストには組み込まれません。 代わりに、その正味値を決定するために使用されます。.

## プロジェクトの潜在的なリスクコストを見つける

Workfrontの次の領域で、プロジェクトのリスクと潜在的なコストを確認できます。

* （プロジェクトの「リスク」タブ）。
* 「ビジネス事例の概要」で、\
   プロジェクトのビジネス事例の詳細については、「 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* プロジェクトレポートで、「計画リスクコスト」フィールドをレポートの列に追加する場合。\
   Workfrontでのレポート作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Portfolio・オプティマイザで、プロジェクトがPortfolioに関連付けられている場合は、[ リスク ] 列に表示されます。\
   ポートフォリオ内のすべてのプロジェクトの潜在的なリスクコストの合計は、Portfolioのリスクに加算されます。\
   Adobe Manager の詳細については、「Portfolio・オプティマイザ」を参照してください。 [Portfolio最適化の概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

プロジェクトでのリスク作成の詳細については、「 [プロジェクトのリスクの作成と編集](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

プロジェクトのビジネス事例の詳細については、「 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).
