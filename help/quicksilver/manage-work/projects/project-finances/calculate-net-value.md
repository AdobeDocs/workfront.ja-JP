---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 正味値の計算
description: プロジェクト純価は、利益を計算してコストを削除した後の、プロジェクトの期待値の合計です。
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
TQID: https://experienceleague.adobe.com/Bj8-Lz2cRE0HeMF7xGryTucaqddQW25DzyPpbzWQR94
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
source-wordcount: 402
ht-degree: 56%

---

# 正味値の計算

プロジェクト純価は、利益を計算してコストを削除した後の、プロジェクトの期待値の合計です。

## プロジェクト純価の概要

Adobe Workfrontでは、次の式を使用してプロジェクトの純価値を計算します。

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

次のフィールドは、プロジェクト純価の値に影響を与える可能性があります。

* **予定利益**：これは、ビジネスケースの&#x200B;**プロジェクト情報**&#x200B;エリアに入力する際にプロジェクト所有者が指定する手動エントリです。\
  プロジェクトの予定利益の詳細については、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)の[プロジェクト情報](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)の節を参照してください。

* **予算計上コスト**：これは、プロジェクトの初回起動時に見積もられた、プロジェクトに関連付けられた総コストです。

  **予算計上コスト**&#x200B;は、ビジネスケースのリソース予算領域で計算される&#x200B;**予算計上された労力コスト**&#x200B;の値を使用し、リソースプランナーの担当業務に対する予算計上された時間と各担当業務の時間当たりのコスト率を考慮します。\
  予算コストは、プロジェクトの&#x200B;**正味値**&#x200B;に影響します。 予算計上コストの計算方法について詳しくは、[予算計上コストの計算](../../../manage-work/projects/project-finances/budgeted-cost.md)を参照してください。

* **潜在リスクコスト**：これは、ビジネスケースやプロジェクトの「リスク」タブで定義されている、プロジェクト上の任意のリスクに関連するコストです。\
  プロジェクトの潜在リスクコストの計算について詳しくは、[潜在リスクコストの計算](../../../manage-work/projects/project-finances/potential-risk-cost.md)を参照してください。



## プロジェクト純価を見つけます。

プロジェクト純価は、Workfront の次のエリアにあります。

* ビジネスケースの概要エリア\
  ビジネスケースの概要エリアについて詳しくは、記事「[&#x200B; プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md) [&#x200B; プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)」の「ビジネスケースの概要について」の節を参照してください。

  ![&#x200B; ビジネスケースの純額](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* Portfolio Optimizerで、プロジェクトがポートフォリオに関連付けられている場合

  >[!TIP]
  >
  >すべてのプロジェクト純価の合計は、ポートフォリオの純価です。

  ポートフォリオオプティマイザーについて詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)を参照してください。

* 次のリストおよびレポートの「プロジェクト純値」フィールドで、

   * プロジェクト
   * タスク
   * イシュー
   * プロジェクト（財務データ）

  レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。
