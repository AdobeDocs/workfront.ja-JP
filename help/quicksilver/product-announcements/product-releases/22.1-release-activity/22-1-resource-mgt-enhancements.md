---
title: 22.1 リソース管理の強化
description: 22.1 リソース管理の強化
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 513e0831-5571-4432-ade3-4f11b7e97266
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# 22.1 リソース管理の強化

このページでは、プレビュー環境の 2.1 リリースでおこなわれたすべてのリソース管理の機能強化について説明します。 これらの機能強化は、実稼動環境で利用できるようになります

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

2022 年 1 月 17 日の週。

22.1 リリースで使用可能なすべての変更点の一覧については、 [22.1 リリースの概要](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## 設定パネルの改善と、ワークロードバランサーでのプロジェクトとタスクのカラーコード機能の改善

ワークロードバランサーを使用する際のエクスペリエンスを向上させるために、次の機能強化が導入されました。

* 設定パネルのデザインが一新され、以前ツールバーにあったオプションが含まれるようになりました。 これにより、ツールバーのスペースが使いやすくなります。
* プロジェクトごとにカラーテーマをカスタマイズする機能が追加されました。 プロジェクトで色分けを選択すると、各プロジェクトとその作業項目が同じ色で表示されます。 色は各プロジェクトに固有です。 この機能強化の前は、プロジェクトステータス別のカラーコードのみを表示できました。

詳しくは、 [ワークロード・バランサのナビゲート](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## ワークロードバランサーを使用して作業を一括で割り当て

スケジューリングツールを廃止し、ワークロードバランサーに置き換える取り組みを続ける中で、割り当てを一括で管理する機能を追加しました。 複数の作業項目を一度に複数のユーザーに割り当てたり、複数の作業項目のユーザーを他のユーザーに置き換えたり、複数の項目のユーザーを一度に割り当て解除したりできるようになりました。 ワークロードバランサーの新しい一括割り当て機能を使用すると、これらすべてを 1 回のアクションで実行できます。

この機能強化がおこなわれるまでは、手動またはドラッグ&amp;ドロップで 1 人のユーザーを 1 つの作業項目に割り当てることができました。

新しい一括割り当てには、名前に加えて、プロジェクトステータスとタスクステータス別の新しいフィルタリング機能も含まれます。

詳しくは、 [ワークロードバランサーでの作業割り当ての概要](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

スケジュールツールの廃止について詳しくは、 [Adobe Workfrontのリソーススケジュールツールの廃止](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

## ジョブの役割を管理する際の通貨の上書き

グローバル組織全体のコストと請求率を簡単に管理できるように、ジョブロールの通貨の上書きを実装しました。 この機能を使用して、ジョブロールの場所に一致する通貨でジョブロールのコストと請求率を設定できるようになりました。 これにより、ジョブロールのすべての財務計算でシステム通貨が上書きされます。

詳しくは、 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

