---
title: 2025年第 2 四半期のリリース期間中におけるその他の機能強化
description: 2025年第2四半期のリリース期間中のその他の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 30%

---

# 2025年第 2 四半期のリリース期間中におけるその他の機能強化

このページでは、2025年第2四半期リリースで行われたプレビュー環境への機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2025年第 2 四半期のリリースサイクルにおける現時点で利用可能なすべての変更点のリストについては、[2025年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md)を参照してください。

## バージョンのアップグレードエンドポイントを使用して、新しいイベントサブスクリプションバージョンにアップグレードします

>[!NOTE]
>
>実稼動（すべてのお客様向け）：2025年3月6日（PT)

Workfrontに、イベントサブスクリプションのバージョンが追加されました。 新バージョンはWorkfront APIに対する変更ではなく、イベントサブスクリプション機能に対する変更です。

イベント登録のアップグレードまたはダウングレード機能により、イベントの構造に変更が加えられても既存の登録には影響せず、イベント登録を中断することなく新しいバージョンのテストとアップグレードができます。

2つのバージョンの違いの詳細については、[イベントサブスクリプションのバージョン管理](/help/quicksilver/wf-api/general/event-subs-versioning.md)を参照してください。

バージョン間でイベントサブスクリプションをアップグレードまたはダウングレードするために使用されるエンドポイントの詳細については、Event Subscription APIの記事の[イベントサブスクリプションバージョン管理](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning)を参照してください。

## Adobe Admin Consoleユーザーの変更を、Workfrontアップデートフィードで「System」として表示します。

>[!NOTE]
>
>プレビューリリース：2025年1月23日、高速リリースのプロダクション：25.2リリース（2025年2月13日）、四半期リリースのプロダクション：25.4リリース（2025年4月）

Adobe Admin Consoleの管理者がWorkfrontユーザーのユーザー情報に変更を加えると、Workfrontはその変更を「システム」に属するものとして、ユーザーのアップデートエリアの「システムアクティビティ」タブに記録します。 これは、Adobe Admin Console管理者を指します。

このアップデートの前は、システムの管理者が行ったユーザー変更は、WorkfrontのメインAdmin Console管理者が行った変更として記録されていました。

Adobe Admin Consoleでのユーザーの管理について詳しくは、[Adobe Admin Consoleでのユーザーの管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください
