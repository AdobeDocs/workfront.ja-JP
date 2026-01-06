---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 正味値の計算
description: プロジェクト純価は、利益を計算してコストを削除した後の、プロジェクトの期待値の合計です。
author: Lisa
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 56%

---

# 正味値の計算

プロジェクト純価は、利益を計算してコストを削除した後の、プロジェクトの期待値の合計です。

## プロジェクト純価の概要

Adobe Workfrontは、次の式を使用してプロジェクトの純価を計算します。

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

次のフィールドは、プロジェクト純価の値に影響を与える可能性があります。

* **予定利益**：これは、ビジネスケースの&#x200B;**プロジェクト情報**&#x200B;エリアに入力する際にプロジェクト所有者が指定する手動エントリです。\
  プロジェクトの予定利益の詳細については、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)の[プロジェクト情報](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)の節を参照してください。

* **予算コスト**：これは、プロジェクトを最初に起動したときに見積もられた、プロジェクトに関連するコストの合計です。

  **予算計上コスト** では、ビジネス ケースのリソース予算計上エリアで計算された **予算計上労力コスト** の値を使用し、リソース プランナの担当業務に予算計上された時間と、各担当業務の時間当たりのコスト率が考慮されます。\
  予算コストはプロジェクトの **純価** に影響します。 予算コストの計算方法の詳細については、「[ 予算コストの計算 ](../../../manage-work/projects/project-finances/budgeted-cost.md)」を参照してください。

* **潜在リスクコスト**：これは、ビジネスケースやプロジェクトの「リスク」タブで定義されている、プロジェクト上の任意のリスクに関連するコストです。\
  プロジェクトの潜在リスクコストの計算について詳しくは、[潜在リスクコストの計算](../../../manage-work/projects/project-finances/potential-risk-cost.md)を参照してください。



## プロジェクト純価を見つけます。

プロジェクト純価は、Workfront の次のエリアにあります。

* ビジネスケース概要エリア\
  「ビジネスケースの概要」領域について詳しくは、[ プロジェクトのビジネスケースを作成 ](../../../manage-work/projects/define-a-business-case/create-business-case.md)[ プロジェクトのビジネスケースを作成 ](../../../manage-work/projects/define-a-business-case/create-business-case.md) の「ビジネスケースの概要について」の節を参照してください。

  ![ ビジネスケースの純価 ](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* Portfolioオプティマイザー（プロジェクトがポートフォリオに関連付けられている場合）

  >[!TIP]
  >
  >すべてのプロジェクト純価の合計は、ポートフォリオの純価です。

  ポートフォリオオプティマイザーについて詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)を参照してください。

* 次のリストおよびレポートの「プロジェクト純値」フィールド：

   * プロジェクト
   * タスク
   * イシュー
   * プロジェクト（財務データ）

  レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。
