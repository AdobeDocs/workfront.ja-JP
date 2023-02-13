---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 投資利益率 (ROI) の計算
description: 投資利益率 (ROI) はAdobe Workfrontの指標で、ポートフォリオ管理者は、プロジェクトの当初の計画されたメリットと予算に基づくコストに対するプロジェクトのパフォーマンスをすばやく確認できます。
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 投資利益率 (ROI) の計算

投資利益率 (ROI) はAdobe Workfrontの指標で、ポートフォリオ管理者は、プロジェクトの当初の計画されたメリットと予算に基づくコストに対するプロジェクトのパフォーマンスをすばやく確認できます。

## プロジェクトの概要投資利益率 (ROI)

Workfrontは次の式を使用して ROI を計算します。

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

次のフィールドは、プロジェクトの ROI に影響します。

* **プロジェクト計画特典**:これは、ビジネスケースの「プロジェクト情報」領域を完了する際に、プロジェクト所有者が指定する手動エントリです。 これは、プロジェクト所有者として、プロジェクトを完了した場合にプロジェクトのメリットが生じる可能性があると考える、ユーザーの推定値です。 これは特定の金額の通貨で、正の値にする必要があります。\
   プロジェクトの計画的利益の詳細については、この記事の「プロジェクト情報」の節を参照してください [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **プロジェクトの予算コスト**：プロジェクトを初めて起動したときの推定プロジェクトに関連する合計コストです。

   この **予算コスト** は **予算労務費** ビジネス・ケースの「生産資源予算編成」領域で計算される値で、「生産資源プランナ」の製造オーダー・ロールに予算された時間数と、各製造オーダー・ロールの「時間単価」レートが考慮されます。\
   詳しくは、 [予算コストの計算](../../../manage-work/projects/project-finances/budgeted-cost.md).

## プロジェクトの投資収益率 (ROI) を見つける

Workfrontの次の領域で、プロジェクトの ROI の値を確認できます。

* Portfolioの最適化で、プロジェクトがポートフォリオに関連付けられているかどうか

   >[!NOTE]
   >
   >すべてのプロジェクトの ROI 値の合計は、ポートフォリオの ROI です。

   Optimizer の詳細については、「Portfolio・オプティマイザ」を参照してください。 [Portfolio最適化の概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* 次のリストとレポートの「プロジェクトの ROI 」フィールド： 

   * プロジェクト
   * タスク
   * 問題
   * プロジェクト（財務データ）
   Workfrontでのレポート作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
