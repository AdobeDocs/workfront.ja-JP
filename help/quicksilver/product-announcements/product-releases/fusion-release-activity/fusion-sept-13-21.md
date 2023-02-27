---
title: Workfront Fusion リリースアクティビティ：&nbsp;2021 年 9 月 13 日の週
description: Workfront Fusion リリースアクティビティ：&nbsp;2021 年 9 月 13 日の週
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: d9056d6f-a62d-4516-930e-4c3f4fbaec3e
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Workfront Fusion リリースアクティビティ： 2021 年 9 月 13 日の週

このページでは、2021 年 9 月 23 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。

最近のすべての変更の一覧については、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion の最近のバグ修正の一覧については、 [Workfrontメンテナンスの更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) ページを開き、 Workfront Fusion メンテナンスアップデートというラベルの付いたアップデートがないか確認します。

## Workfront Fusion シナリオ実行履歴のフィルターと並べ替え

特定のシナリオ実行を見つけやすくするために、シナリオ実行履歴の他のフィールドでフィルタリングできるようにしました。 既存のフィルターに加えて、次の条件でフィルタリングできるようになりました。

* 実行期間
* 操作数
* 転送されたデータの量
* アクションタイプ（実行または更新）

以前は、実行履歴は開始時刻またはステータスでのみフィルタリングできました。

また、シナリオ実行履歴の並べ替えも可能にしました。 次の値で並べ替えることができます。

* 実行開始時間
* 実行ステータス
* 実行期間
* 操作数
* 転送されたデータの量

実行履歴のフィルタリングと並べ替えについて詳しくは、 [Adobe Workfront Fusion でシナリオの実行履歴を表示します](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Fusion のヘルプリンクが特定の記事にリードするようになりました。

必要な情報を簡単に見つけられるように、Fusion のヘルプリンクを更新し、作業中の Fusion の領域に関する記事に直接アクセスできるようにしました。

Fusion の任意の領域でヘルプアイコンをクリックすると、その領域に関する記事に移動できます。 例えば、シナリオ設定パネルのヘルプリンクはシナリオ設定パネルを説明する記事に、WorkfrontモジュールのヘルプリンクはWorkfrontモジュールの設定方法を説明する記事になります。 また、説明テキスト内でハイライト表示されたリンクをクリックすると、サポートされている日付と時刻の形式のリストなど、説明テキストに関連する記事が表示されます。

以前は、Fusion ヘルプリンクはWorkfront Fusion のドキュメントを開き、必要なトピックを検索できました。

## 詳細が使用可能な場合、シナリオ実行履歴に「詳細」ボタンのみが表示されます

シナリオ実行テーブルでより明確にするために、詳細を持つ実行に対してのみ「詳細」ボタンを表示するようにしました。 実行の詳細がアーカイブされたかどうかを一目で確認できるようになりました。 「詳細」ボタンの機能は変更されていません。

以前は、すべての実行に「詳細」ボタンが表示されていたので、ユーザーが詳細情報をクリックしただけで、詳細情報がないことがありました。

詳しくは、 [Adobe Workfront Fusion でシナリオの実行履歴を表示します](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## SDL Managed Translation Connector のタイムアウトが 120 秒に増加

SDL Managed Translation Connector のタイムアウトを短縮するために、タイムアウト時間を 120 秒に増やしました。

以前は、SDL Managed Translation は、Workfront Fusion のタイムアウトガードレールである 40 秒に従っていました。
