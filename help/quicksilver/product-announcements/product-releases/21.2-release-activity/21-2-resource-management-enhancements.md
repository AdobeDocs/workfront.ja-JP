---
content-type: release-notes
keywords: メモ、四半期、アップデート、リリース
navigation-topic: 2021-2-release-activity
title: 21.2 リソース管理の機能強化
description: このページでは、プレビュー環境の 21.2 リリースで行われたリソース管理のすべての機能強化について説明します。 これらの機能強化は、2021年5月10日（PT）の週に本番環境で利用可能になる予定です。 21.2 リリースで使用できるすべての変更点のリストについては、21.2 リリースの概要を参照してください。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
TQID: https://experienceleague.adobe.com/cAM0R2azvfhRW25brnRKCUXZ5f2ZLGeBVd19okbdBpU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 575
ht-degree: 100%

---

# 21.2 リソース管理の機能強化

このページでは、プレビュー環境の 21.2 リリースで行われたリソース管理のすべての機能強化について説明します。 これらの機能強化は、2021年5月10日（PT）の週に本番環境で利用可能になる予定です。 21.2 リリースで使用可能なすべての変更点の一覧については、[21.2 リリースの概要](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md)を参照してください。

## ワークロードバランサーの月レベルの表示

リソースの割り当てをより長期間管理できるよう、ワークロードバランサーの月レベルの表示を実装しました。 一度に 3 か月まで表示し、月別のリソース割り当てをアップデートできます。 この変更以前は、1 日または 1 週間のみでワークロードバランサーを表示できました。

詳しくは、[ワークロードバランサーのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)を参照してください。

## シナリオプランナー、ワークロードバランサー、タスクリスト間の接続

>[!NOTE]
>
>新しい Adobe Workfront エクスペリエンスでのみ使用できます。

プロジェクトの戦略的計画に役立ち、シナリオプランナーの大きな構想に合わせるために、プロジェクトに新しいエリアを作成しました。その領域には、イニチアチブからの担当業務要件と、プロジェクト作業アイテムで予測される予定時間数が表示されます。 この領域は、プロジェクトレベルのワークロードバランサーと、新しい Workfront エクスペリエンスのタスクリストで使用できます。 従来のエクスペリエンスでは、プロジェクトのワークロードバランサーでのみ使用できます。

詳しくは、次の記事を参照してください。

* [プロジェクトとイニシアチブ間でのリソース割り当て調整の概要](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md)。
* [ワークロードバランサーの操作](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>この新しい機能は、新しい Workfront エクスペリエンスと従来の Workfront エクスペリエンスの両方で、すべてのユーザーに表示されます。 これは、Workfront Scenario Planner ライセンスを購入していない顧客にも表示されます。

## リソースプランナーの純価を計算する際に予定時間数を使用

リソースプランナーの新しい設定を使用すると、正味価値の計算に予定時間数を使用できます。

この機能強化の前は、Workfront は予算計上時間数のみを使用して正味価値を計算しました。 正味価値には、利用可能時間数と予算計上時間数または予定時間数、FTE、コストとの差が表示されます。 正味価値を計算する場合、予算計上時間数は依然としてデフォルト設定です。

詳しくは、[リソースプランナーのプロジェクトビューと役割ビューでの時間数、FTE、コスト情報の概要](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)を参照してください。

## ワークロードバランサーの 12 週間表示

ワークロードバランサーで最大 12 週間分の情報を表示できるようになりました。 この機能強化がおこなわれる前は、2 週間、4 週間、6 週間の情報を表示できました。

ワークロードバランサーの表示について詳しくは、[ワークロードバランサーのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)ワークロードバランサーのナビゲートを参照してください。

## ワークロードバランサーの未割り当てエリアでの担当業務フィルターの動作方法を変更

ワークロードバランサーでの担当業務フィルターの動作を改善し、ユーザーの期待に応えるために、未割り当てエリアでのフィルターの機能を変更しました。 フィルターで指定した担当業務に割り当てられた時間のみを表示できるようになりました。

この強化が行われる前は、未割り当てエリアに担当業務フィルターを適用すると、ワークロードバランサーは、担当業務に割り当てられた作業アイテムに関連するすべての時間数を表示していました。

ワークロードバランサーでの情報のフィルタリングについて詳しくは、[ワークロードバランサーのフィルターの管理](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)を参照してください。
