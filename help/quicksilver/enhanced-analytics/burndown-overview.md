---
title: 拡張分析でのバーンダウンビジュアライゼーションの表示
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: バーンダウンビジュアライゼーションは、特定のプロジェクトのバーンダウンの推移を示し、プロジェクト状況、速度および残り時間（日数）の間の関係を理解するのに役立ちます。
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 95%

---

# 拡張分析でのバーンダウンビジュアライゼーションの表示

>[!IMPORTANT]
>
>Enhanced Analytics は、5 月 27 日（PT）にWorkfrontから削除されました。 Workfront Data Connect は新しい代替ソリューションであり、現在使用している Enhanced Analytics のビジュアライゼーションをレプリケートするために使用できます。 <br> 詳しくは、[Enhanced Analytics の廃止 ](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) ガイドを参照してください。


<!-- Audited: 12/2023 -->

バーンダウンビジュアライゼーションは、特定のプロジェクトのバーンダウンの推移を示し、プロジェクト状況、速度および残り時間（日数）の間の関係を理解するのに役立ちます。

![拡張分析のバーンダウンの例](assets/burndown120623.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
      <p>新規：任意</p>
      <p>または</p>
      <p>現在：Business 以上</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
      <p>新規：ライト以上</p>
      <p>または</p>
      <p>現在：レビュー以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへの表示アクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示</p> </td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 前提条件

強化機能分析を使用するための前提条件については、[強化機能分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)の「前提条件」の節を参照してください。

## バーンダウンビジュアライゼーションについて

青い実線は、開始日から予定完了日までの予定速度を示します。この線は、作業の追加、削除または更新に応じて調整され、プロジェクトが予定完了日に達すると、垂直の破線に変わります。

![予定速度](assets/burndown-planned-line.png)

実線は、プロジェクトに費やした時間数（または日数）の推移を示します。この線の色は、毎日のプロジェクトの状況を示します。

* **緑**：プロジェクトが目標どおりであることを示します。

  ![目標どおり](assets/burndown-green.png)

* **オレンジ**：プロジェクトが危険な状況にあることを示します。

  ![危険あり](assets/burndown-orange.png)

* **赤**：プロジェクトにトラブルが発生していることを示します。

  ![トラブル発生中](assets/burndown-red.png)

これらのプロジェクト状況について詳しくは、[プロジェクト状況と状況タイプの概要](../manage-work/projects/manage-projects/project-condition-and-condition-type.md)を参照してください。

作業がプロジェクトに追加されると、実線が垂直上方に移動します。プロジェクトの作業が削除されるか完了すると、実線が垂直下方に移動します。

ビジュアライゼーションの x 軸の下には、特定の日にタスクと時間数（または日数）がどのように変化したか（追加された量、完了した量およびこの 2 つの差）に関する詳細情報が表示されます。

バーンダウンビジュアライゼーションでこれらの情報をすべて表示すると、以下についての判断に役立ちます。

* 個々のプロジェクトの健全性の推移
* 発生する問題（予定外の作業）が予定作業にどのような影響を与えたか
* プロジェクトがオリジナル完了日を過ぎる原因となったイベントはどれか

このビジュアライゼーションに最適なデータを取得する方法については、[拡張分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)を参照してください。

## バーンダウンビジュアライゼーションの表示

{{step1-to-analytics}}

1. （オプション）別の日付範囲を使用するには、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![日付の選択](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用については、[拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

1. （条件付き）プロジェクトデータセットを制限する必要がある場合は、使用するフィルターを選択して適用します。

   拡張分析でのフィルターの追加について詳しくは、[拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたり Workfront からログアウトした後でもフィルターはアクティブの状態が維持されます。

1. （オプション）日付範囲にズームインするには、日付範囲の始点としてビジュアライゼーション上の点を選択し、日付範囲の終点までドラッグします。

   他のすべてのビジュアライゼーションが同じ日付範囲に更新され、期間フィルターが自動的に作成されます。

   ![期間フィルター](assets/timeframe-filter-350x220.png)

1. フライトプランまたはプロジェクトツリーマップビジュアライゼーションで、プロジェクトをクリックして詳細情報を表示します。

   フライトビジュアライゼーションのバーンダウンとタスクが表示されます。

   >[!NOTE]
   >
   >これら他のビジュアライゼーションについて詳しくは、以下を参照してください。
   >
   >   * [拡張分析での進行計画ビジュアライゼーションの表示](../enhanced-analytics/flight-plan-overview.md)
   >   * [拡張分析でプロジェクトツリーマップビジュアライゼーションを表示](../enhanced-analytics/project-treemap-overview.md)
   >   * [拡張分析の「作業中のタスク」ビジュアライゼーションの確認](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. （オプション）表示を予定時間数から&#x200B;**期間**&#x200B;に変更します。

   予定時間数はデフォルトで選択されています。

   >[!NOTE]
   >
   >**期間**&#x200B;を選択すると、すべての時間数の情報を日数に変更します。\
   >![期間バーンダウン](assets/duration-burndown-350x112.png)\
   >拡張分析エリアの期間について詳しくは、[拡張分析の概要](../enhanced-analytics/enhanced-analytics-overview.md#duration-view)の期間ビューの節を参照してください。

1. 折れ線グラフ上の任意の点をクリックします。

   正確な日付が表示され、選択した日のタスク数と時間数（または日数）に関する詳細情報がグラフの下に表示されます。

   ![バーンダウンの詳細](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >実際の速度がビジュアライゼーションの X 軸に沿った平坦な線（0 時間または 0 日間と一致）である場合は、予定時間数（または日数）はプロジェクトに追加されていなかったことを意味します。\
   >実際の速度が x 軸より上の平坦な線（ある時間数または日数と一致）であり下降しない場合は、フィルタリングされた期間に完了したタスクがなかったことを意味します。

1. （オプション）ビジュアライゼーションのデータを書き出すには、ビジュアライゼーションの右上隅にある&#x200B;**書き出し**&#x200B;アイコン ![書き出しアイコン](assets/export.png) をクリックし、書き出し形式を選択します。

   * グラフ (PNG)
   * データテーブル（XLSX）

1. （オプション）選択したプロジェクトのタスクの進捗を詳細に確認するには、バーンダウンビジュアライゼーションの下に表示される「作業中のタスク」ビジュアライゼーションを確認します。詳しくは、[拡張分析での「作業中のタスク」ビジュアライゼーションの表示](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md)を参照してください。
