---
title: 拡張分析でのバーンダウンビジュアライゼーションの表示
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: バーンダウンビジュアライゼーションは、特定のプロジェクトの時間の経過に伴うバーンダウンを示し、プロジェクトの状態、速度、残り時間（日数）間の関係を理解するのに役立ちます。
author: Nolan
feature: Reports and Dashboards
exl-id: e67c92d5-b309-406b-b6f0-4d414d0e7dcc
source-git-commit: 6d2494f1ccb2f9b222a953ed8bae922bd0f26389
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# 拡張分析でのバーンダウンビジュアライゼーションの表示

バーンダウンビジュアライゼーションは、特定のプロジェクトの時間の経過に伴うバーンダウンを示し、プロジェクトの状態、速度、残り時間（日数）間の関係を理解するのに役立ちます。

![分析の強化バーンダウンの例](assets/burndown120623.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>
      <p>新規：任意</p>
      <p>または</p>
      <p>現在：ビジネス以上</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>
      <p>新規：明るいかそれ以上</p>
      <p>または</p>
      <p>現在：レビュー以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。<br>Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

拡張 Analytics を使用するための前提条件については、「前提条件」の節を参照してください。 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites).

## バーンダウンビジュアライゼーションの理解

青い実線は、開始日から計画完了日までの計画速度を示します。 作業の追加、削除、更新に応じてこの線が調整され、プロジェクトが計画完了日に達すると、縦破線に変わります。

![計画速度](assets/burndown-planned-line.png)

実際の行には、時間の経過に伴うプロジェクトでの滞在時間（日数）が表示されます。 この線の色は、毎日のプロジェクトの状態を示します。

* **緑**：プロジェクトはターゲットになっています。

  ![ターゲット時](assets/burndown-green.png)

* **オレンジ**：プロジェクトがリスクにさらされています。

  ![危険な状態](assets/burndown-orange.png)

* **赤**：プロジェクトに問題が発生しています。

  ![問題が発生](assets/burndown-red.png)

これらのプロジェクト条件の詳細については、 [プロジェクト条件と条件タイプの概要](../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

実際の線が垂直に上に移動すると、作業がプロジェクトに追加されます。 線が垂直に下に移動すると、プロジェクトの作業が削除または完了します。

ビジュアライゼーションの x 軸の下に、指定した日にタスクや時間（または日）がどのように変化したか（追加された金額、完了した金額、および 2 つの差）に関する詳細を表示できます。

バーンダウンビジュアライゼーションでこれらの情報をすべて表示すると、次の項目を判断できます。

* 時間の経過に伴う個々のプロジェクトの健全性
* 発生する問題（または計画外の作業）が計画作業に与える影響
* 元の完了日を過ぎてプロジェクトを延長したイベント

このビジュアライゼーションに最適なデータを取得する方法については、 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md).

## バーンダウンビジュアライゼーションの表示

{{step1-to-analytics}}

1. （オプション）別の日付範囲を使用する場合は、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![日付を選択](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （条件付き）プロジェクトデータセットを制限する必要がある場合は、使用するフィルタを選択して適用します。

   Enhanced Analytics でのフィルターの追加について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたりWorkfrontからログアウトした後でもフィルターはアクティブなままになります。

1. （オプション）日付範囲を拡大するには、日付範囲の開始点となるビジュアライゼーション上のポイントを選択し、日付範囲の終わりまでドラッグします。

   その他のビジュアライゼーションはすべて同じ日付範囲に更新され、時間枠フィルターが自動的に作成されます。

   ![期間フィルター](assets/timeframe-filter-350x220.png)

1. フライトプランまたはプロジェクトツリーマップビジュアライゼーションで、プロジェクトをクリックして詳細を表示します。

   フライトビジュアライゼーションのバーンダウンとタスクが表示されます。

   >[!NOTE]
   >
   >これらの他のビジュアライゼーションについて詳しくは、次を参照してください。
   >
   >   * [Enhanced Analytics でのフライトプランビジュアライゼーションの表示](../enhanced-analytics/flight-plan-overview.md)
   >   * [拡張分析でのプロジェクトツリーマップビジュアライゼーションの表示](../enhanced-analytics/project-treemap-overview.md)
   >   * [Enhanced Analytics でのフライトビジュアライゼーションでのタスクの表示](../enhanced-analytics/tasks-in-flight-overview.md)
   >

1. （オプション）予定時間からにビューを変更します。 **duration**.

   デフォルトでは、予定時間が選択されています。

   >[!NOTE]
   >
   >選択 **duration** すべての時間の情報を日に変更します。\
   >![持続時間のバーンダウン](assets/duration-burndown-350x112.png)\
   >Enhanced 分析領域の期間について詳しくは、 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md#duration-view).

1. 折れ線グラフ上の任意の点をクリックします。

   選択した日の正確な日付と、タスクおよび時間（または日）に関する詳細情報がグラフの下に表示されます。

   ![バーンダウンの詳細](assets/burndown-task-and-hour-changes-350x121.png)

   >[!NOTE]
   >
   >実際の速度がビジュアライゼーションの X 軸（0 時間または 0 日間のインライン）に沿った平らな線である場合は、計画された時間（または日）はプロジェクトに追加されていませんでした。\
   >実際の速度が x 軸の上のフラットな線（時間数または日数を含むインライン）で下降しない場合、フィルタリングされた期間内にタスクが完了しなかったことを意味します。

1. （オプション）ビジュアライゼーションデータを書き出すには、 **書き出し** アイコン ![書き出しアイコン](assets/export.png)ビジュアライゼーションの右上隅で、エクスポート形式を選択します。

   * グラフ (PNG)
   * データテーブル (XSLX)

1. （オプション）選択したプロジェクトのタスクの進行状況に関する詳細を確認するには、バーンダウンビジュアライゼーションの下に表示されるフライト中のタスクビジュアライゼーションを確認します。 詳しくは、 [Enhanced Analytics でのフライトビジュアライゼーションでのタスクの表示](/help/quicksilver/enhanced-analytics/tasks-in-flight-overview.md).
