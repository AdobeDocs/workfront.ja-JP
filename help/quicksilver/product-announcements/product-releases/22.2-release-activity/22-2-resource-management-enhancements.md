---
title: 22.2 リソース管理の強化
description: 22.2 リソース管理の強化
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 22.2 リソース管理の強化

このページでは、プレビュー環境の 2.2 リリースでおこなわれたリソース管理のすべての機能強化について説明します。 これらの機能強化は、実稼動環境で利用できるようになります

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022 年 4 月 4 日の週。

22.2 リリースで使用可能なすべての変更点の一覧については、 [22.2 リリースの概要](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## ワークロードバランサーのナビゲーションの改善

ワークロードバランサーを使用する際のエクスペリエンスを向上させるために、次の機能強化が導入されました。

* 割り当て調整時の [ キャンセル ] ボタンと [ 保存 ] ボタンは、画面に表示される期間より長い場合や [ 概要 ] パネルが表示された場合でも、固定されるようになりました。
* ユーザー名と作業項目名を表示する左側のパネルが固定され、長い期間水平にスクロールでき、パネルに一覧表示される項目名を読み取れるようになりました。
* ユーザーレベルやプロジェクトレベルではなく、1 回のクリックで、左側のパネルに表示されるすべての項目を折りたたんだり展開したりできます。
* 左側のパネルもサイズ変更可能になりました。
* ワークロードバランサーにフルスクリーンモードが追加されました。

ワークロード・バランサのナビゲーションの詳細は、 [ワークロード・バランサのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## ワークロード・バランサでの高度な割り当てへのアクセス

作業項目の割り当てをより簡単かつ正確に行うために、ワークロードバランサーで作業項目を手動で割り当てる際に、高度な割り当てを行うことができるようになりました。 この機能強化がおこなわれる前は、項目の編集時、項目のヘッダーから、またはリストで、[ 高度な割り当て ] にアクセスできました。

詳しくは、 [ワークロードバランサーを使用して作業を手動で割り当てる](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## 「デフォルトのスケジュール」環境設定が選択されている場合にユーザーの可用性を計算する新しい数式

リソース管理ツールに関するより正確な情報を提供するために、Workfront管理者が「リソース管理環境設定」で「デフォルトのスケジュール」を選択した場合に、Workfrontがユーザーの可用性を計算するために使用する式を変更しました。 新しい更新に伴い、Workfrontは次の数式を使用してユーザーの可用性を計算します。

ユーザー使用可能時間= （デフォルトの予定時間 — 例外） &#42; FTE — 時間外

この更新以前は、Workfrontでは次の数式を使用して「デフォルトのスケジュール」が選択されている場合のユーザーの可用性を計算していました。

ユーザー使用可能時間= ( デフォルトの予定時間 — （予定例外+時間外）) &#42; ユーザー FTE 値

詳しくは、 [リソース管理環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

