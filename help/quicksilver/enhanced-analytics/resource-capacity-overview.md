---
title: 拡張分析でのリソース容量ビジュアライゼーションの表示
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Adobe Workfrontの拡張分析リソース容量ビジュアライゼーショングラフを表示して、チームが終了したか、中にいたか、または容量にいたかを評価できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 1%

---

# 拡張分析でのリソース容量ビジュアライゼーションの表示

<!--Audited: 01/2024-->

Adobe Workfrontの拡張分析リソース容量ビジュアライゼーショングラフを表示して、チームが終了したか、中にいたか、または容量にいたかを評価できます。

リソースのビジュアライゼーションで示したチームは、指定した期間に作業に割り当てられたユーザーのホームチームを指します。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfrontプラン</a>*</td> 
   <td> <p>現在：ビジネス以上</p>
   または
   <p>新規：任意</p>
    </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license*</td> 
   <td> <p>現在：レビュー以上</p>
   または
   <p>新規：標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベルの設定</td> 
   <td> <p>プロジェクトへのアクセスを表示</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>プロジェクトに対する表示権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

拡張 Analytics を使用するための前提条件については、「前提条件」の節を参照してください。 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md).

## リソース容量のビジュアライゼーションについて

「生産資源生産能力」ビジュアライゼーションでは、チームの生産能力が超過したか、不足していたか、または生産能力であるかが表示されます。 この計算は次の項目に基づいておこなわれます。

* **使用可能な容量**：フィルタリングされた期間にホームチームが作業できる時間の合計

  >[!NOTE]
  >
  >将来の期間を調べると、使用可能な容量は過去 7 日間のチームの能力に基づいて計算されます。 このため、スケジュールされた PTO は考慮されません。

* **計画能力**：フィルターを適用した期間にホームチームから予想される予定作業時間の合計

ホームチームの予定時間と実際の予定時間をこの比較で比較すると、十分な作業をホームチームに割り当てていないか、または大量の作業負荷からの燃え尽きを経験しているかを判断するのに役立ちます。

![](assets/resource-capacity-350x110.png)

「生産資源生産能力」ビジュアライゼーションには、次の詳細が表示されます。

* **計画能力**：ホームチーム名をインラインで指定し、青い円はホームチームに割り当てられている予定時間数を表します。

  ![](assets/resource-capacity-blue-circle.png)

* **実際の容量**：ホームチーム名をインラインで指定します。縦線は、ホームチームが使用できる時間数を表します。

  ![](assets/resource-capacity-vertical-line.png)

* **容量超過**：垂直線の右側に水平線と青い円が表示されると、ホームチームに割り当てられた作業量は、使用可能な時間数を超えていました。 つまり、フィルターを適用した期間でチームが容量を超えている可能性があります。 チームが完了する必要がある残り時間数が青い円の右側に表示されます。

  ![](assets/resource-capacity-over-capacity.png)

* **容量不足**：ホームチームは、縦線の左側に横線と青い円が表示されている場合、割り当てられた予定作業時間よりも時間が長くなります。 つまり、フィルターを適用した期間でチームの処理能力が低下している可能性があります。 ホームチームが作業を完了するのに使用できる時間の追加数が、青い円の左側に表示されます。

  ![](assets/resource-capacity-under-capacity.png)

チームの行にカーソルを合わせると、計画済み容量と使用可能容量の正確な時間数、およびホームチームが処理能力を超えた時間数、または不足している時間数が表示されます。

この情報を確認することで、次の項目を特定することができます。

* チームが割り当て超過または未割り当ての場合。
* 最も大きなプロジェクトは、ホームチームが注力しているプロジェクトです。
* どのチームが作業に使用できるか。

このビジュアライゼーションに最適なデータを取得する方法については、 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md).

## リソース処理能力ビジュアライゼーションの表示

{{step1-to-analytics}}

1. 左のパネルで、「 」を選択します。 **People**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. （オプション）別の日付範囲を使用する場合は、グラフの右上隅にある日付範囲フィルターから新しい開始日と終了日を選択します。

   ![](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （条件付き）チームフィルターを設定していない場合、チームフィルターを追加し、データを表示する各チームを選択します。

   Enhanced Analytics でのフィルターの追加について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたりWorkfrontからログアウトした後でもフィルターはアクティブなままになります。

1. （オプション）日付範囲を拡大するには、日付範囲の開始点としてビジュアライゼーション上の点を選択し、日付範囲の終わりまでドラッグします。

   その他のビジュアライゼーションはすべて、同じ日付範囲に更新され、期間フィルターが作成されます。

   ![](assets/timeframe-filter-350x220.png)

1. ホームチームの行の上にマウスポインターを置くと、次の情報が表示されます。

   * スケジュール可能な残り時間数
   * ホームチームが完了するまでに計画した時間数
   * 作業時間の合計数。 作業時間の合計数には、次のラベルが含まれる場合があります。

      * 超過
      * の下
      * 容量で。

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. （オプション）ビジュアライゼーションデータを書き出すには、 **書き出しアイコン** ![](assets/export.png) ビジュアライゼーションの右上隅で、エクスポート形式を選択します。

   * **グラフ (PNG)**
   * **データテーブル (XSLX)**

1. ホームチーム名をクリックすると、チームの能力ビジュアライゼーションの詳細が表示されます。

   チームの容量のビジュアライゼーションの詳細については、 [拡張分析でのチーム容量ビジュアライゼーションの表示](../enhanced-analytics/team-capacity-overview.md).


