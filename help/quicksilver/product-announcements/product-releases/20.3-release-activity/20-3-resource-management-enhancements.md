---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 リソース管理の強化
description: このページでは、実稼動環境の 20.3 リリースでおこなわれたリソース管理のすべての機能強化について説明します。 これらの機能強化は、2020 年 8 月 10 日の週に実稼動環境で公開されました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 リソース管理の強化

このページでは、実稼動環境の 20.3 リリースでおこなわれたリソース管理のすべての機能強化について説明します。 これらの機能強化は、2020 年 8 月 10 日の週に実稼動環境で公開されました。

20.3 リリースで使用可能なすべての変更点の一覧については、 [20.3 リリースの概要](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## ワークロードバランサーの割り当て済み作業領域の問題からの時間数を含めます

担当者のすべてのワークロードの全体像を把握できるように、ワークロードバランサーの割り当て済み作業領域に問題の発生時間を含める設定を導入しました。

ワークロードバランサーでの作業の詳細は、 [ワークロード・バランサのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## ワークロードバランサーの非稼働日の割り当てを調整します

ワークロードバランサーを使用して、非営業日のリソースの割り当てを調整できます。

ワークロード・バランサでの割り当ての管理の詳細は、 [ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## ワークロードバランサーで使用可能な変数フィルター

エクスペリエンスを向上させ、情報を共有する際の柔軟性を高めるために、ワークロードバランサーの変数フィルターを実装しました。 次のフィルターがワークロードバランサーに追加されました。

* 「自分」（ユーザーによるフィルタリングの場合）
* 「自分のプライマリの役割」（役割でフィルタリングする場合）
* 「My Home Team」または「All My Teams」（チームでフィルタリングする場合）。

これらのフィルターは、$$USER.ID、$$USER.roleID、$$USER.homeTeamID および$$USER.teamIDs のワイルドカードフィルター変数を置き換えます

これらのフィルタの 1 つを適用し、ワークロードバランサーを共有したり、ダッシュボードに配置したりすると、他のすべてのユーザーには、それぞれ独自の情報が表示されます。

ワークロード・バランサへのフィルタの適用の詳細は、 [ワークロードバランサーの情報のフィルタリング](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## ワークロードバランサーのプロジェクトの新しいソート

ワークロード・バランサは、最も早い計画開始日に基づいてプロジェクトをソートし、次に、ユーザーが画面に表示する期間中に発生する、プロジェクト内のタスクの最も遅い計画完了日に基づいてプロジェクトをソートするようになりました。 これにより、1 日の作業をより簡単に識別できる、ツリー状の階層に作業を整理できます。

ワークロード・バランサでのプロジェクトと作業項目の表示の詳細は、次を参照してください： [ワークロード・バランサのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## ワークロードバランサーでの実際の作業の進行状況の表示

ワークロードの進行状況を正確に把握できるように、ワークロードバランサーに新しい設定を導入し、タスクと問題の予定日に応じたタイムラインを表示しました。 「予定日を表示」設定を有効にして、予定タイムラインに加えて、作業項目の予測タイムラインを表示できます。

また、この改善により、タスクまたはイシューが計画完了日より前に完了した場合、残りの日から割り当てられた時間が、ユーザーの全体的な配分にカウントされないことを示すために切り替えられます。

ワークロードバランサーの操作と設定の有効化の詳細は、 [ワークロード・バランサのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 20.2 リリースでリリースされたときに伝わったワークロードバランサー機能

* [ワークロードバランサーでの日次および週次の配分を調整](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [ワークロードバランサーでのタスク予定時間の更新](#update-task-planned-hours-in-the-workload-balancer)
* [ワークロードバランサーで割り当てを更新する便利な方法](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### ワークロードバランサーでの日次および週次の配分を調整 {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

リソースの消費を避けるために、ワークロードバランサーを使用して、ユーザーの日別および週別の割り当てを調整できるようになりました。

この機能強化以前は、リソーススケジュールツールを使用した場合にのみ可能でした。

ワークロード・バランサでの割り当ての管理の詳細は、 [ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**次の環境で使用できます。**

* Adobe Workfront Classic
* 新しいAdobe Workfrontエクスペリエンス

### ワークロードバランサーでのタスク予定時間の更新 {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>この機能強化は、2020.2 リリース後間もなく実稼動環境で利用できるようになります。

アクセス・レベルの「リソース管理」領域に新しいオプションが追加され、このアクセス権を持つユーザーは、ワークロード・バランサから計画時間を編集できるようになりました。 ワークロード・バランサで割り当てを調整する場合、1 日の割り当ての合計は、タスクの計画時間数と一致する必要はありません。 割り当てを保存すると、割り当て時間の合計がタスクの予定時間になります。 これは、シンプルな期間タイプを持つタスクでのみ可能です。

ワークロード・バランサでの割り当ての管理の詳細は、 [ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

リソース管理へのアクセス権の付与については、 [リソース管理へのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### ワークロードバランサーで割り当てを更新する便利な方法 {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

ワークロードバランサー内の作業項目に対するユーザーの割り当てを管理しやすくするために、作業項目をダブルクリックできるようになりました。 既存の「割り当てを編集」メニューオプションも引き続き使用できます。 また、割り当ての表示を有効にして更新できるようにする必要はなくなりました。

ワークロード・バランサでの割り当ての管理の詳細は、 [ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
