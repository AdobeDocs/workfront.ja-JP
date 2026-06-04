---
title: 2025年第3四半期レポートの機能強化
description: 2025年第3四半期プロジェクトの機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/XN5rfSeje0azVxpC4uBSDn5mg2C9Oyik2awD5pQy3Jo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 5%

---

# 2025年第3四半期レポートの機能強化

このページでは、2025年第3四半期リリースでプレビュー環境に加えられたすべてのレポート機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2025年第3四半期のリリースサイクルで現時点で利用可能なすべての変更のリストについては、[2025年第3四半期のリリースの概要](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)を参照してください。

## レポート配信のセキュリティ強化

* プレビュー：2025年6月26日（PT）
* 実稼動：2025年6月26日から2025年7月9日まで段階的に展開

Workfront通知がメール許可リストで承認されたメールドメインにのみ送信されるように、スケジュールされたレポートの配信を強化しました。

以前は、Workfront通知の電子メールドメインに制限を定義していた場合、電子メールが追加されている際に、この電子メールドメインに対してチェックを実行していました。

現在は、入力されたメールアドレスがメール送信許可リストに加えるに準拠していることを確認するために、メールの送信中にチェックも行います。 この改善されたチェックは、ユーザーに関連付けられたメールアドレスと、レポート受信者リストに追加されたアドホックメールの両方に適用されます。

詳しくは、[自動レポート配信のスケジュール &#x200B;](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)を参照してください。


## ユーザーワイルドカードは、フィルタリング時にnull値を持つ結果を返さなくなりました

>[!NOTE]
>
>* プレビュー：2025年4月30日（PT）
>* プロダクション高速リリース：2025年5月15日（PT）
>* すべての顧客の本番環境：2025年7月17日

レポートをフィルタリングする際のnull値を除外するように、ユーザーのワイルドカード動作を更新しました。 この変更は、ユーザーが正しく設定されていない結果（null結果）を返すのではなく、フィルターがより正確な結果を生成するのに役立ちます。

以前は、ユーザーのワイルドカードでnull値が生成された場合、null値を持つすべてのレコードがレポートに表示されていました。

この変更は、次のワイルドカードフィルターに適用されます。

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
