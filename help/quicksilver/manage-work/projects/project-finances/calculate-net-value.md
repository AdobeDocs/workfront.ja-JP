---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 正味値の計算
description: プロジェクト純価は、利益を計算してコストを削除した後の、プロジェクトの期待値の合計です。
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '397'
ht-degree: 100%

---

# 正味値の計算

プロジェクト純価は、利益を計算してコストを削除した後の、プロジェクトの期待値の合計です。 

## プロジェクト純価の概要

Adobe Workfront では、次の式を使用してプロジェクト純価を計算します。

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

次のフィールドは、プロジェクト純価の値に影響を与える可能性があります。

* **予定利益**：これは、ビジネスケースの&#x200B;**プロジェクト情報**&#x200B;エリアに入力する際にプロジェクト所有者が指定する手動エントリです。\
  プロジェクトの予定利益の詳細については、[ビジネスケースのエリアの概要](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)の[プロジェクト情報](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)の節を参照してください。

* **予算計上コスト**：プロジェクトを初めて立ち上げる際に推定される、プロジェクトに関連する合計コストです。

  **予算計上コスト**&#x200B;は、ビジネスケースのリソース予算エリアで計算された&#x200B;**予算計上労力コスト**&#x200B;の値を使用します。この値では、リソースプランナーで担当業務に予算計上された時間と、それぞれの担当業務の 1 時間あたりのコストを考慮します。\
  予算計上コストはプロジェクト&#x200B;**純価**&#x200B;に影響します。予算計上コストの計算について詳しくは、[予算計上コストの計算](../../../manage-work/projects/project-finances/budgeted-cost.md)を参照してください。

* **潜在リスクコスト**：これは、ビジネスケースやプロジェクトの「リスク」タブで定義されている、プロジェクト上の任意のリスクに関連するコストです。\
  プロジェクトの潜在リスクコストの計算について詳しくは、[潜在リスクコストの計算](../../../manage-work/projects/project-finances/potential-risk-cost.md)を参照してください。

   

## プロジェクト純価を見つけます。

プロジェクト純価は、Workfront の次のエリアにあります。

* ビジネスケースのビジネスケースの概要領域 \
  ビジネスケースの概要領域の詳細については、[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)の「[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)」の節を参照してください。

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* ポートフォリオオプティマイザー（プロジェクトがポートフォリオに関連付けられている場合）

  >[!TIP]
  >
  >すべてのプロジェクト純価の合計は、ポートフォリオの純価です。

  ポートフォリオオプティマイザーについて詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)を参照してください。

* 次のリストおよびレポートの「プロジェクト純価」フィールド：

   * プロジェクト
   * タスク
   * イシュー
   * プロジェクト（財務データ）

  レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。
