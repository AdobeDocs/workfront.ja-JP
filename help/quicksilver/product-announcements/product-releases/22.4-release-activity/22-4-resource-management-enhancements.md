---
title: 22.4 リソース管理の強化
description: 22.4 リソース管理の強化
author: Luke
draft: Probably
feature: Product Announcements
exl-id: cd026fc9-e3be-4cff-8d85-4f50fae9dd77
source-git-commit: e0a8093be33773a8b801567cfbe90f67701f9ff3
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# 22.4 リソース管理の強化

このページでは、プレビュー環境の 22.4 リリースでおこなわれたリソース管理のすべての機能強化について説明します。 これらの機能強化は、2022 年 10 月 3 日の週に提供されます。

22.4 リリースで使用可能なすべての変更点の一覧については、 [22.4 リリースの概要](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## プロジェクトのワークロードバランサーのすべてのユーザーを表示

プロジェクトのワークロードバランサーを離れることなく、システム内のすべてのユーザーとその容量を表示できるように、「すべてのユーザーを表示」オプションを追加しました。 有効にすると、プロジェクトのワークロードバランサーに、割り当てられた作業領域にシステム内のすべてのユーザーが表示されます。 この機能強化により、「未割り当ての作業」領域に表示される作業に割り当てる必要があるユーザーを容易に特定できます。

詳しくは、 [ドラッグ&amp;ドロップによりワークロードバランサーで作業を割り当てる](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3412873/){target=_blank}

## 作業を一括で割り当てる際に、選択したジョブロールを持つすべてのユーザーをワークロードバランサーに表示します

ジョブの役割をワークロードバランサー内のユーザーに一括で置き換える際に、適切な担当者を見つけやすくするため、使用可能なユーザーのリストの入力方法を改善しました。 これで、同じユーザーリスト内の 2 つの異なる領域で、選択した役割を果たすシステム内のすべてのユーザーを表示できます。

* 最初の領域（「提案割当」）には、「スマート割当」論理で識別されるユーザーが表示されます。 詳しくは、 [スマート割り当ての概要](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

* 2 つ目の領域（「その他の割り当て」）には、選択した役割を果たすことができるすべてのユーザーが表示されます。

この機能強化の前は、スマート割り当てロジックに従って割り当てに使用できるユーザーのリストのみを表示できました。

ワークロードバランサーを使用した一括割り当ての詳細は、 [ワークロードバランサーを使用して作業を一括で割り当て](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

[この機能のデモビデオを表示](https://video.tv.adobe.com/v/3412874/){target=_blank}

## ワークライセンスユーザーと問題設定用のワークロードバランサーの強化

スケジューリングツールの廃止に備えて、ワークロードバランサーに次の機能が追加されました。

* ワークライセンスユーザーは、プロジェクトのワークロードバランサーを使用する際に割り当てを調整できるようになりました

* 「問題からの時間を含む」設定を有効にすると、問題は未割り当ての作業領域に表示されます

これらの機能強化がおこなわれる前は、割り当てられた作業領域にのみ表示されるユーザーの割り当てと問題を調整できるのは、Plan-license ユーザーのみです。

詳しくは、次の記事を参照してください。

* [ワークロード・バランサのナビゲート](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* [ワークロードバランサーでのユーザー割り当ての管理](/help/quicksilver/resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

