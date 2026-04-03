---
title: 2025年第 2 四半期のリリース期間中におけるその他の機能強化
description: 2025年第2四半期リリース期間のその他の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 30%

---

# 2025年第 2 四半期のリリース期間中におけるその他の機能強化

このページでは、プレビュー環境に対する2025年第2四半期リリースで行われた機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2025年第 2 四半期のリリースサイクルにおける現時点で利用可能なすべての変更点のリストについては、[2025年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md)を参照してください。

## バージョンアップグレードエンドポイントを使用して、新しいイベントサブスクリプションバージョンにアップグレードする

>[!NOTE]
>
>実稼動（すべてのお客様向け）：2025年3月6日（PT)

Workfrontには、イベントサブスクリプションのバージョンが追加されました。 新しいバージョンは、Workfront APIの変更ではなく、イベントサブスクリプション機能の変更です。

イベント登録のアップグレードまたはダウングレード機能により、イベントの構造に変更が加えられても既存の登録には影響せず、イベント登録を中断することなく新しいバージョンのテストとアップグレードができます。

2つのバージョンの違いについて詳しくは、[&#x200B; イベント サブスクリプションのバージョン管理](/help/quicksilver/wf-api/general/event-subs-versioning.md)の記事を参照してください。

バージョン間でイベントサブスクリプションをアップグレードまたはダウングレードするために使用されるエンドポイントについて詳しくは、「イベントサブスクリプション API」の「[&#x200B; イベントサブスクリプションのバージョン管理](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning)」の節を参照してください。

## Workfrontの更新フィードでAdobe Admin Console ユーザーの変更を「システム」として表す

>[!NOTE]
>
>プレビューリリース：2025年1月23日（PT）、高速リリースの実稼動：25.2 リリース（2025年2月13日（PT））、四半期リリースの実稼動：25.4 リリース（2025年4月）

現在、Adobe Admin Consoleの管理者がWorkfront ユーザーのユーザー情報に変更を加えた場合、Workfrontは、ユーザーの更新領域の「システム」アクティビティ タブに、この変更を「システム」に属するものとして記録します。 これは、Adobe Admin Console管理者を指します。

このアップデートの前は、Workfrontの管理者が行ったユーザーの変更は、メインのAdmin Consoleの管理者が行ったように記録されていました。

Adobe Admin Consoleでのユーザーの管理について詳しくは、[Adobe Admin Consoleでのユーザーの管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください
