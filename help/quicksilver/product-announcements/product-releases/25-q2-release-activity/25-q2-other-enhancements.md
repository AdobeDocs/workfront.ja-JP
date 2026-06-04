---
title: 2025年第 2 四半期のリリース期間中におけるその他の機能強化
description: 2025年第2四半期リリース期間のその他の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/s8T1ziXqzEOn8yipB5UdM-nShwJhYbCPNfIycC3GjYw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 335
ht-degree: 36%

---

# 2025年第 2 四半期のリリース期間中におけるその他の機能強化

このページでは、プレビュー環境に対する2025年第2四半期リリースで行われた機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2025年第 2 四半期のリリースサイクルにおける現時点で利用可能なすべての変更点のリストについては、[2025年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md)を参照してください。

## バージョンアップグレードエンドポイントを使用して、新しいイベントサブスクリプションバージョンにアップグレードする

>[!NOTE]
>
>実稼動（すべてのお客様向け）：2025年3月6日（PT)

Workfrontには、イベントサブスクリプションのバージョンが追加されました。 新しいバージョンは Workfront API に対する変更ではなく、イベント登録機能に対する変更です。

イベント登録のアップグレードまたはダウングレード機能により、イベントの構造に変更が加えられても既存の登録には影響せず、イベント登録を中断することなく新しいバージョンのテストとアップグレードができます。

2つのバージョンの違いについて詳しくは、[ イベント サブスクリプションのバージョン管理](/help/quicksilver/wf-api/general/event-subs-versioning.md)の記事を参照してください。

バージョン間でイベントサブスクリプションをアップグレードまたはダウングレードするために使用されるエンドポイントについて詳しくは、「イベントサブスクリプション API」の「[ イベントサブスクリプションのバージョン管理](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning)」の節を参照してください。

## Workfrontの更新フィードでAdobe Admin Console ユーザーの変更を「システム」として表す

>[!NOTE]
>
>プレビューリリース：2025年1月23日（PT）、高速リリースの実稼動：25.2 リリース（2025年2月13日（PT））、四半期リリースの実稼動：25.4 リリース（2025年4月）

現在、Adobe Admin Consoleの管理者がWorkfront ユーザーのユーザー情報に変更を加えた場合、Workfrontは、ユーザーの更新領域の「システム」アクティビティ タブに、この変更を「システム」に属するものとして記録します。 これは、Adobe Admin Console管理者を指します。

このアップデートの前は、Workfrontの管理者が行ったユーザーの変更は、メインのAdmin Consoleの管理者が行ったように記録されていました。

Adobe Admin Consoleでのユーザーの管理について詳しくは、[Adobe Admin Consoleでのユーザーの管理](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)を参照してください
