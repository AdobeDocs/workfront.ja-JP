---
title: 2025 年第 3 四半期レポートの機能強化
description: 2025 年第 3 四半期プロジェクトの強化
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 7%

---

# 2025 年第 3 四半期レポートの機能強化

このページでは、2025 年第 3 四半期リリースで行われた、プレビュー環境に対するすべてのレポートの機能強化について説明します。 これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2025 年第 3 四半期のリリースサイクルのこの時点で利用できるすべての変更のリストについては、[2025 年第 3 四半期のリリースの概要 ](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md) を参照してください。

## フィルタリング時にユーザーワイルドカードが null 値を含む結果を返さなくなりました

>[!NOTE]
>
>* プレビュー：2025 年 4 月 30 日（PT）
>* 実稼動高速リリース：2025 年 5 月 15 日（PT）
>* すべてのお客様の実稼動：2025 年 7 月 17 日（PT）

レポートをフィルタリングする際に null 値を除外するように、ユーザーワイルドカード動作を更新しました。 この変更により、フィルターは、ユーザーが正しく設定されていない結果（null 結果）を返すのではなく、より正確な結果を生成するのに役立ちます。

以前は、ユーザーのワイルドカードが null 値を生成した場合、レポートには null 値も持つすべてのレコードが表示されていました。

この変更は、次のワイルドカードフィルターに適用されます。

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

