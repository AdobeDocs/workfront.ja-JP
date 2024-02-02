---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 リソース管理の機能強化
description: このページでは、実稼動環境の 20.3 リリースで行われた、すべてのリソース管理の機能強化について説明します。これらの機能強化は、2020年8月10日（PT）の週に実稼動環境で利用可能になりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: ht
source-wordcount: '837'
ht-degree: 100%

---

# 20.3 リソース管理の機能強化

このページでは、実稼動環境の 20.3 リリースで行われた、すべてのリソース管理の機能強化について説明します。これらの機能強化は、2020年8月10日（PT）の週に実稼動環境で利用可能になりました。

20.3 リリースで利用可能なすべての変更点の一覧については、[20.3 リリースの概要](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md)を参照してください。

## ワークロードバランサーの割り当て済み作業エリアのイシューの時間数を含める

すべての担当者のワークロードの全体像を把握できるように、ワークロードバランサーの割り当て済み作業エリアのイシューの時間数を含める設定を導入しました。

ワークロードバランサーでの作業について詳しくは、[ワークロードバランサーのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)を参照してください。

## ワークロードバランサーの非作業日の割り当てを調整

ワークロードバランサーを使用して、非作業日のリソースの割り当てを調整できます。

ワークロードバランサーの割り当ての管理について詳しくは、[ワークロードバランサーのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

## ワークロードバランサーで使用可能な変数フィルター

エクスペリエンスを向上させ、情報を共有する際の柔軟性を高めるために、ワークロードバランサーに変数フィルターを実装しました。以下のフィルターがワークロードバランサーに追加されました。

* 「自分」（ユーザーによるフィルタリングの場合）
* 「自分の主要役割」（役割でフィルタリングする場合）
* 「自分のホームチーム」または「すべての自分のチーム」（チームでフィルタリングする場合）。

これらのフィルターは、$$USER.ID、$$USER.roleID、$$USER.homeTeamID および$$USER.teamIDs のワイルドカードフィルター変数を置き換えます

これらのフィルターの 1 つを適用し、ワークロードバランサーを共有したり、ダッシュボードに配置したりすると、他のすべてのユーザーには、それぞれ独自の情報が表示されます。

ワークロードバランサーへのフィルターの適用ついて詳しくは、[ワークロードバランサーの情報のフィルタリング](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)を参照してください。

## ワークロードバランサーのプロジェクトの新しいソート

ワークロードバランサーは、まず最も早い予定開始日に基づいてプロジェクトを並べ替え、次に、ユーザーが画面に表示する期間中に発生する、プロジェクト内のタスクの最も遅い予定完了日に基づいてプロジェクトを並べ替えるようになりました。これにより、1 日の作業をより簡単に識別できる、ツリー状の階層に作業を整理することができます。

ワークロードバランサーでのプロジェクトと作業アイテムの表示について詳しくは、[ワークロードバランサーのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)を参照してください。

## ワークロードバランサーでの実際の作業の進行状況を表示

ワークロードの進行状況を正確に把握できるように、ワークロードバランサーに新しい設定を導入し、タスクと問題の見込み日に応じたタイムラインを表示できるようにしました。「見込み日を表示」の設定を有効にして、予定タイムラインに加えて、作業アイテムの見込みタイムラインを表示できます。

また、この改善により、タスクまたは問題が予定完了日より前に完了した場合、残りの日数から割り当てられた時間には取り消し線が引かれ、ユーザーの全体的な割り当てにはカウントされないことが示されます。

ワークロードバランサーのナビゲートと設定の有効化について詳しくは、[ワークロードバランサーのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)を参照してください。

## 以前 20.2 リリースでリリースされるとして通知されていた Workload Balancer の機能

* [ワークロードバランサーでの日次および週次の配分の調整](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [ワークロードバランサーでのタスクの予定時間数の更新](#update-task-planned-hours-in-the-workload-balancer)
* [ワークロードバランサーで割り当てを更新するためのより便利な方法](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### ワークロードバランサーでの日次および週次の配分の調整 {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

リソースのバーンアウトを避けるために、ワークロードバランサーを使用して、ユーザーの日次および週次の作業の配分が調整できるようになりました。

この機能強化以前は、この調整はリソーススケジュールツールを使用した場合にのみ可能でした。

ワークロードバランサーでの割り当て管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

**利用可能な環境：**

* Adobe Workfront Classic
* 新しい Adobe Workfront エクスペリエンス

### ワークロードバランサーでのタスクの予定時間数の更新 {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>この機能強化は、2020.2 リリース後間もなく実稼動環境で利用できるようになります。

アクセスレベルのリソース管理エリアに新しいオプションが追加され、このアクセス権を持つユーザーが、ワークロードバランサーから予定時間数を編集できるようになりました。ワークロードバランサーで割り当てを調整する場合、1 日の割り当ての合計は、タスクの予定時間数と一致する必要はありません。割り当てを保存すると、割り当て時間の合計がタスクの予定時間数になります。これは、シンプルな期間タイプを持つタスクでのみ可能です。

ワークロードバランサーでの割り当て管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

リソース管理へのアクセス権の付与について詳しくは、[リソース管理へのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)を参照してください。

### ワークロードバランサーで割り当てを更新するためのより便利な方法 {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

ワークロードバランサー内の作業アイテムに対するユーザーの割り当てを管理しやすくするために、作業アイテムをダブルクリックできるようになりました。既存の「割り当てを編集」メニューオプションも引き続き使用できます。また、割り当てを更新するために、割り当ての表示を有効にする必要もなくなりました。

ワークロードバランサーでの割り当て管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。
