---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 投資回収率（ROI）の計算
description: 投資回収率（ROI）は、ポートフォリオマネージャーがプロジェクトの元の予定利率と予算計上コストに対するプロジェクトのパフォーマンスをすばやく確認するための Adobe Workfront の指標です。
author: Lisa
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
TQID: https://experienceleague.adobe.com/x7MGrAZbtlDd0oTePPgRdLQfUg8-M4GkkQdeWXUTyh4
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
source-wordcount: 348
ht-degree: 74%

---

# 投資回収率（ROI）の計算

投資回収率（ROI）は、ポートフォリオマネージャーがプロジェクトの元の予定利率と予算計上コストに対するプロジェクトのパフォーマンスをすばやく確認するための Adobe Workfront の指標です。

## プロジェクト投資回収率（ROI）の概要

Workfront は次の式を使用して ROI を計算します。

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

次のフィールドは、プロジェクトの ROI に影響します。

* **プロジェクト予定利益**：これは、ビジネスケースのプロジェクト情報エリアに入力する際にプロジェクト所有者が指定する手動エントリです。 これは、プロジェクトを完了した場合にプロジェクトに生じる利益のプロジェクト所有者による推定値です。 これは特定の金額の通貨で、正の値にする必要があります。\
  プロジェクトの予定利益について詳しくは、[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)の記事の「プロジェクト情報」の節を参照してください。

* **プロジェクト予算計上コスト**：これは、プロジェクトの初回起動時に見積もられた、プロジェクトに関連付けられた総コストです。

  **予算計上コスト**&#x200B;は、ビジネスケースのリソース予算領域で計算される&#x200B;**予算計上された労力コスト**&#x200B;の値を使用し、リソースプランナーの担当業務に対する予算計上された時間と各担当業務の時間当たりのコスト率を考慮します。\
  詳しくは、[予算計上コストの計算](../../../manage-work/projects/project-finances/budgeted-cost.md)を参照してください。

## プロジェクト投資回収率（ROI）の検索

Workfront の次のエリアで、プロジェクトの ROI の値を表示できます。

* Portfolio Optimizerで、プロジェクトがポートフォリオに関連付けられている場合

  >[!NOTE]
  >
  >すべてのプロジェクトの ROI 値の合計は、ポートフォリオの ROI です。

  ポートフォリオオプティマイザーについて詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)の記事を参照してください。

* 次のリストとレポートの「プロジェクト ROI」フィールドで、

   * プロジェクト
   * タスク
   * イシュー
   * プロジェクト（財務データ）

  Workfront でのレポート作成について詳しくは、「[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)」の記事を参照してください。
