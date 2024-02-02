---
title: 22.2 リソース管理の機能強化
description: 22.2 リソース管理の機能強化
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '373'
ht-degree: 100%

---

# 22.2 リソース管理の機能強化

このページでは、プレビュー環境での 22.2 リリースで行われた、リソース管理のすべての機能強化について説明します。これらの機能強化は、

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022年4月4日（PT）の週に実稼動環境で公開されます。

22.2 リリースで利用可能なすべての変更点の一覧については、[22.2 リリースの概要](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md)を参照してください。

## ワークロードバランサーへのナビゲーションの改善

ワークロードバランサーを使用する際のエクスペリエンスを向上させるために、次の機能強化が導入されました。

* 配分調整時の「キャンセル」ボタンと「保存」ボタンは、タスクが画面に表示される期間より長い場合や、概要パネルが表示された場合でも、固定されるようになりました。
* ユーザー名と作業アイテム名を表示する左側のパネルが固定され、長い期間を水平にスクロールでき、パネルに一覧表示される項目名を読み取れるようになりました。
* ユーザーレベルやプロジェクトレベルではなく、1 回のクリックで、左側のパネルに表示されるすべての項目を折りたたんだり展開したりできます。
* 左側のパネルもサイズ変更可能になりました。
* ワークロードバランサーにフルスクリーンモードが追加されました。

ワークロードバランサーのナビゲーションについて詳しくは、[ワークロードバランサーのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)を参照してください。

## ワークロードバランサーでの高度な割り当てへのアクセス

作業アイテムの割り当てをより簡単かつ正確に行うために、ワークロードバランサーで作業アイテムを手動で割り当てる際に、高度な割り当てができるようになりました。この機能強化が行われるまでは、アイテムの編集時や、アイテムのヘッダーから、またはリストで高度な割り当てにアクセスできました。

詳しくは、[ワークロードバランサーを使用した作業の手動割り当て](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md)を参照してください。

## デフォルトのスケジュール環境設定が選択されている場合に新しい数式を使用してユーザーの空き時間を計算

リソース管理ツールでより正確な情報を提供するため、Workfront 管理者がリソース管理環境設定でデフォルトのスケジュールを選択した場合に、Workfront でユーザーの空き時間の計算に使用する式を変更しました。新しいアップデートに伴い、Workfront は次の数式を使用してユーザーの空き時間を計算します。

ユーザーの空き時間数 =（デフォルトのスケジュール時間数 - 例外）&#42; FTE - 休暇時間数

このアップデート以前は、Workfront では次の数式を使用して、デフォルトのスケジュールが選択されている場合のユーザーの空き時間を計算していました。

ユーザーの空き時間数 =（デフォルトのスケジュール時間数 -（スケジュール例外 + 休暇時間数））&#42; ユーザーの FTE 値

詳しくは、[リソース管理の環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

