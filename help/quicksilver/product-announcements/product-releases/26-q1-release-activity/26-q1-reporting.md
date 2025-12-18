---
title: 2026 年第 1 四半期レポートの機能強化
description: 2026 年第 1 四半期レポートの機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: bed931281d7d0b3184914ed7649d9cb889bcf39a
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 4%

---

# 2026 年第 1 四半期レポートの機能強化

このページでは、2026 年第 1 四半期リリースで行われた、プレビュー環境に対するレポートの機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2026年第 1 四半期リリースサイクルの現時点で利用可能なすべての変更のリストについて詳しくは、[2026年第 1 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)を参照してください。

<!--

## Currency updates in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We have made the following updates for currency fields:

* When multiple currencies are defined in Workfront, you can now choose a default currency for the dashboard during creation. 

* When creating a report, you can lock a currency field. This ensures that the dashboard-level currency preference does not affect the display of these values.

* When viewing a dashboard, users can toggle between any defined currencies in Workfront. These changes apply to the entire dashboard with the exception of locked currency fields.

-->

<!--

## Quick search table results in Canvas Dashboards

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast release: January 14, 2026 
>Production for everyone: January 15, 2026 

We have added a quick search to Table reports. This search works across all pages, so you can find data even if it's not currently visible.

-->

## 新しい「円グラフに合計を表示」オプション

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

円グラフをドーナツグラフに変換する、新しい「合計を表示」オプションが導入されました。 この機能を使用すると、グラフ内のすべてのセグメントの合計を表す一元的な値を表示できます。

* カウント集計タイプの場合、表示される中央の値は、グラフのすべてのセグメントのカウントです。
* 合計集計タイプの場合、表示される中央値は、数値または通貨値の集計合計です。
* 平均、最大、最小の集計タイプの場合、中央値には、それに応じて平均、最大、最小の値が表示されます。

ユーザーは、合計のラベルを表示または非表示にしたり、カスタムラベル値を指定したりすることもできます。

詳しくは、[ キャンバスダッシュボードでのグラフレポートの作成 ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) を参照してください。

## キャンバスダッシュボードの円グラフ用の新しい設定オプション

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

円グラフ用に、次の 2 つの新しい設定オプションが導入されました。

* セグメントラベルを非表示にする：円グラフのセグメントラベルが長すぎてグラフの読みやすさに影響する場合に、円グラフでセグメントラベルを非表示にするように選択できるようになりました。
* グラフの凡例の非表示と再配置：円グラフの凡例を非表示にするように選択できるようになりました。 凡例の位置は、グラフの右（デフォルト）、左、上、下に設定することもできます。

詳しくは、[ キャンバスダッシュボードでのグラフレポートの作成 ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) を参照してください。

## キャンバスダッシュボードのグループ化数の改善

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

キャンバスダッシュボードのグループ化バーを更新して、現在のページのレコード数とすべてのページにわたるグループ化の全体的なレコード数を表示しました。

例えば、グループ化バーには「3/7」または「83/21032」が表示され、グループ化内のデータ配分が明確に表示されます。

以前は、グループ化バーにはこの詳細なカウント情報が表示されなかったので、複数のページを移動する際に、グループ内の合計レコード数を理解するのが困難でした。

## キャンバスダッシュボードのレポートの新しい参照線機能

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

棒グラフ、列グラフ、折れ線グラフで参照線を定義して、系列ベースのレポートのターゲットまたはしきい値 4 を設定できるようになりました。

注記：参照線は動的ではなく、複数の参照線は適用できません。 将来の機能強化については検討していますが、当面の計画はありません。

詳しくは、[ キャンバスダッシュボードでのグラフレポートの作成 ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) を参照してください。

## キャンバスダッシュボードのチャートレポートの軸ラベルのカスタマイズ

>[!NOTE]
>
>プレビュー：2025 年 12 月 18 日（PT）
>実稼動高速リリース：2026 年 1 月 14 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

グラフレポートの軸ラベルをカスタマイズできるようになりました。 この新機能を使用すると、デフォルトのオブジェクトおよびフィールド パスの代わりに表示する置き換え軸ラベルを入力できます。 また、軸ラベル全体を非表示にすることもできます。

詳しくは、[ キャンバスダッシュボードでのグラフレポートの作成 ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) を参照してください。

## キャンバスダッシュボードでのレポートの複製

>[!NOTE]
>
>プレビューリリース：2025年10月23日（PT）
>実稼動版（すべてのお客様向け）：2025年10月23日（PT）
>[!BADGE 予定外 ]{type=Neutral}

キャンバスダッシュボードで KPI、テーブル、またはグラフレポートを作成後に複製できるようになりました。 複製したら、必要に応じてレポートを編集してから保存できます。

## レポートフィルターからのフィールドオプションの削除

>[!NOTE]
>
>プレビュー：2025 年 11 月 6 日（PT）
>実稼動高速リリース：2025 年 11 月 13 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

レポートにフィルターを適用する際に以前使用できた次のフィールドオプションを削除しました。

* その他のグループ ID
* その他の役割 ID
* その他のチーム ID

これらは、「次に等しくない」および「空である」演算子に関連する問題により削除されました。 これらのフィールドのいずれかを使用する既存のフィルターがある場合、そのフィルターは引き続き期待どおりに動作します。 または、これらのフィールドを <code>textmode で引き続き使用することもできます。</code>ただし、その際は「次と等しくない」または「空である」演算子の使用は避けることをお勧めします。

次のフィールドオプションが代替値として使用できます。

* その他のグループ：ID
* その他の役割：ID
* その他のチーム：ID

## キャンバスダッシュボードでのグループ化数の表示を改善しました

>[!NOTE]
>
>プレビュー：2025 年 11 月 6 日（PT）
>実稼動高速リリース：2025 年 11 月 13 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

表レポートに結果の複数のページがあり、表がグループ化で構成されている場合、表には、現在のページのレコード金額と、すべてのページの全体的なレコード数の両方が表示されるようになりました。 例えば、テーブルレポートに 7 つのグループがあり、最初のページに 3 が表示されている場合、テーブルには 3/7 が表示されます。


## キャンバスダッシュボードの読み込み時間を改善する新しいガードレール

>[!NOTE]
>
>プレビュー：2025 年 11 月 6 日（PT）
>実稼動高速リリース：2025 年 11 月 13 日（PT）
>すべてのユーザー向けの実稼動：2026 年 1 月 15 日（PT）

キャンバスダッシュボードで読み込み時間の遅延を回避し、全体的なパフォーマンスを向上させるために、1 つのダッシュボードに追加できるダッシュボードコンポーネントの数に制限を適用しました。

* ダッシュボードあたりのレポート数：25 件の制限
* テーブルビューのグループ化：5 つの制限
* レポートの基本オブジェクトからの距離：10 limit
* テーブル表示の列：25 個の制限
* ダッシュボードレベルのフィルタープロンプト：10 個の制限




