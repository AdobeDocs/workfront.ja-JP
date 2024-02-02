---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 投資回収率（ROI）の計算
description: 投資回収率（ROI）は、ポートフォリオマネージャーがプロジェクトの元の予定利率と予算計上コストに対するプロジェクトのパフォーマンスをすばやく確認するための Adobe Workfront の指標です。
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '348'
ht-degree: 100%

---

# 投資回収率（ROI）の計算

投資回収率（ROI）は、ポートフォリオマネージャーがプロジェクトの元の予定利率と予算計上コストに対するプロジェクトのパフォーマンスをすばやく確認するための Adobe Workfront の指標です。

## プロジェクト投資回収率（ROI）の概要

Workfront は次の式を使用して ROI を計算します。

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

次のフィールドは、プロジェクトの ROI に影響します。

* **プロジェクト予定利益**：これは、ビジネスケースのプロジェクト情報エリアに入力する際にプロジェクト所有者が指定する手動エントリです。これは、プロジェクトを完了した場合にプロジェクトに生じる利益のプロジェクト所有者による推定値です。これは特定の金額の通貨で、正の値にする必要があります。\
  プロジェクトの予定利益について詳しくは、[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)の記事の「プロジェクト情報」の節を参照してください。

* **プロジェクトの予算計上コスト**：プロジェクトの立ち上げ当初に見積もった、プロジェクトに関連する合計コストです。

  **予算計上コスト**&#x200B;は、ビジネスケースのリソース予算計上のエリアで計算された&#x200B;**予算計上労力コスト**&#x200B;の値を使用します。この値には、リソースプランナーで担当業務に予算計上された時間と、それぞれの担当業務の 1 時間あたりのコストが考慮されます。\
  詳しくは、[予算計上コストの計算](../../../manage-work/projects/project-finances/budgeted-cost.md)を参照してください。

## プロジェクト投資回収率（ROI）の検索

Workfront の次のエリアで、プロジェクトの ROI の値を表示できます。

* ポートフォリオオプティマイザー（プロジェクトがポートフォリオに関連付けられている場合）

  >[!NOTE]
  >
  >すべてのプロジェクトの ROI 値の合計は、ポートフォリオの ROI です。

  ポートフォリオオプティマイザーについて詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)の記事を参照してください。

* 次のリストとレポートに「プロジェクト ROI」フィールドがあります。

   * プロジェクト
   * タスク
   * イシュー
   * プロジェクト（財務データ）

  Workfront でのレポート作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)の記事を参照してください。
