---
title: 2025 年第 2 四半期のリリース期間中のその他の機能強化
description: 2025 年第 2 四半期のリリース期間中のその他の機能強化
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: d603edee0099b6ce3e4f8d3414d1b31f94209196
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 12%

---

# 2025 年第 2 四半期のリリース期間中のその他の機能強化

このページでは、2025 年第 2 四半期リリースでプレビュー環境に加えられた機能強化について説明します。 これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2025年第 2 四半期のリリースサイクルにおける現時点で利用可能なすべての変更点のリストについては、[2025年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md)を参照してください。

## バージョン アップグレード エンドポイントを使用して、新しいイベント サブスクリプション バージョンにアップグレードします

>[!NOTE]
>
>実稼動（すべてのお客様向け）：2025年3月6日（PT)

Workfrontに、イベント購読のバージョンが追加されました。 新しいバージョンはWorkfront API に対する変更ではなく、イベント購読機能に対する変更です。

イベント購読をアップグレードまたはダウングレードする機能により、イベントの構造に変更が加えられても既存の購読が壊れずに、イベント購読に隙間なく新しいバージョンのテストとアップグレードが可能になります。

2 つのバージョンの違いについて詳しくは、「イベント購読のバージョン管理 [&#x200B; を参照してください &#x200B;](/help/quicksilver/wf-api/general/event-subs-versioning.md)。

バージョン間でイベント購読をアップグレードまたはダウングレードするために使用されるエンドポイントについて詳しくは、Event subscription API の節 [&#x200B; イベント購読のバージョン管理 &#x200B;](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) を参照してください。

## Adobe Admin Console ユーザーの変更をWorkfront更新フィードの「システム」として表す

>[!NOTE]
>
>プレビューリリース：2025 年 1 月 23 日（PT）、高速リリースの実稼動：25.2 リリースの実稼動（2025 年 2 月 13 日（PT））、四半期リリースの実稼動：25.4 リリースの実稼動（2025 年 4 月）

Workfrontの管理者がWorkfront ユーザーのユーザー情報に変更を加えると、Adobe Admin Consoleは、ユーザーの更新領域にある「システム」アクティビティ タブで、この変更を「システム」に属するものとして記録するようになりました。 これはAdobe Admin Console管理者を指します。

このアップデート以前は、Workfrontの管理者によるユーザーの変更内容は、Admin Consoleのメインのシステム管理者による変更内容として記録されていました。

Adobe Admin Consoleでのユーザーの管理については、[Adobe Admin Consoleでのユーザーの管理 &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) を参照してください。
