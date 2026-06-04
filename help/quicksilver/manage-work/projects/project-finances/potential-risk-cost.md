---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 潜在リスクコストを計算
description: プロジェクトの潜在リスクコストでは、プロジェクトリスクの潜在的なコストと発生する確率が考慮されます。
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
TQID: https://experienceleague.adobe.com/32kwPUhdtWhFeqQ34oReoU8xl2JlaWQeZlq7MI1jqtc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 302
ht-degree: 83%

---

# 潜在リスクコストを計算

プロジェクトの潜在リスクコストでは、プロジェクトリスクの潜在的なコストと発生する確率が考慮されます。

## プロジェクトの潜在リスクコストの概要

Adobe Workfrontでは、次の式を使用してプロジェクトの潜在的なリスクコストを計算します。

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

プロジェクトの潜在的なリスクコストを確認する際には、次の点を考慮してください。

* プロジェクトの予定リスクコストは、潜在リスクコストと同じです。
* 潜在リスクコストは、プロジェクトの予定コストには組み込まれません。 代わりに、純価値を決定するために使用されます。

## プロジェクトの潜在的なリスクコストの特定

Workfront の次のエリアで、プロジェクトのリスクと潜在コストを確認できます。

* プロジェクトの「リスク」タブ内。
* ビジネスケースの概要で。\
  プロジェクトのビジネスケースについて詳しくは、「[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)」の記事を参照してください。
* プロジェクトレポートで、レポートの列に「予定リスクコスト」フィールドを追加する場合。\
  Workfront でのレポート作成について詳しくは、「[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)」の記事を参照してください。

* ポートフォリオオプティマイザーで、プロジェクトがポートフォリオに関連付けられている場合は、「リスク」列に表示されます。\
  ポートフォリオ内のすべてのプロジェクトの潜在リスクコストの合計が、ポートフォリオのリスクに加算されます。\
  ポートフォリオオプティマイザーについて詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)の記事を参照してください。

プロジェクトでリスクを作成する方法について詳しくは、[プロジェクトに関するリスクの作成と編集](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)の記事を参照してください。

プロジェクトのビジネスケースについて詳しくは、[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)の記事を参照してください。
