---
title: 拡張分析でのチーム容量ビジュアライゼーションの表示
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: チーム容量ビジュアライゼーションは、ホームチームが持つ総容量、過剰割り当て済みか未割り当てか、および時間の経過に伴う容量の動的さを示します。
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 4%

---

# 拡張分析でのチーム容量ビジュアライゼーションの表示

<!-- Audited: 01/2024 -->

チーム容量ビジュアライゼーションは、ホームチームが持つ総容量、過剰割り当て済みか未割り当てか、および時間の経過に伴う容量の動的さを示します。

![チームの能力](assets/team-capacity.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>
      <p>新規：任意</p>
      <p>または</p>
      <p>現在：ビジネス以上</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンスの概要</td>
   <td>
      <p>新規：明るいかそれ以上</p>
      <p>または</p>
      <p>現在：レビュー以上</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>プロジェクトへのアクセスを表示</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td>表示 </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

拡張 Analytics を使用するための前提条件については、「前提条件」の節を参照してください。 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md).

## チームの容量のビジュアライゼーションを理解する

チームの処理能力ビジュアライゼーションには、特定の日にホームチームに割り当てられた作業量が表示されます。

* **焼き切り**：濃い青色の塗りの色が点線の上にある場合、ホームチームは、チームが作業できる時間数よりも多くの作業時間を割り当てます。 これは、チームが割り当て超過で、燃え尽きに近づいている可能性があることを示しています。

  ![容量超過](assets/team-capacity-over-capacity.png)

* **未挑戦**：濃い青色の塗りの色が点線の下にある場合、ホームチームは、割り当てられている作業時間よりも多くの作業時間を使用できます。 これは、チームの割り当てが不十分で、挑戦を受けない可能性があることを示します。

  ![容量不足](assets/team-capacity-under-capacity.png)

* **残高**：明るい色やより透明な青い塗りの色がちょうど上、すぐ下、または点線にある場合、ホームチームには、使用可能な営業時間内に完了できるように、作業時間が割り当てられています。 これは、チームの作業負荷がより均衡していることを示しています。

  ![容量で](assets/team-capacity-at-capacity.png)

ビジュアライゼーションの任意のポイントにカーソルを合わせると、指定した日の次の詳細が表示されます。

* **予定時間**：チームが完了する必要がある予定作業時間数です。
* **利用可能な時間**：チームが作業できる労働時間数です。
* **処理能力**：処理能力の割合に加えて、「処理能力で」、「処理能力不足」または「処理能力超過」の指定も表示されます。

この情報を確認することで、次の項目を特定することができます。

* ホームチームが割り当て超過または割り当て超過になったとき。
* ホームチームが日々割り当て超過または割り当て超過の場合。
* ホームチームの作業量が日々どの程度安定しているか。
* 新しいワークで処理能力のイシューが発生しているかどうか。

このビジュアライゼーションに最適なデータを取得する方法については、 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md).

## チームの処理能力ビジュアライゼーションを表示

{{step1-to-analytics}}

1. 左のパネルで、「 」を選択します。 **People**.

   ![担当者を選択](assets/people-area-cropped-qs-350x276.png)

1. （オプション）別の日付範囲を使用する場合は、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![日付範囲フィルター](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （条件付き）チームフィルターを設定していない場合、チームフィルターを追加し、データを表示する各チームを選択します。

   Enhanced Analytics でのフィルターの追加について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたりWorkfrontからログアウトした後でもフィルターはアクティブなままになります。

1. リソース容量ビジュアライゼーションで、チームをクリックして詳細を表示します。

   チームの処理能力ビジュアライゼーションが表示されます。

   リソース処理能力のビジュアライゼーションについて詳しくは、 [拡張分析でのリソース容量ビジュアライゼーションの表示](../enhanced-analytics/resource-capacity-overview.md).

1. （オプション）日付範囲を拡大するには、日付範囲の開始点としてビジュアライゼーション上の点を選択し、日付範囲の終わりまでドラッグします。

   その他のビジュアライゼーションはすべて、同じ日付範囲に更新され、期間フィルターが作成されます。

   ![期間フィルター](assets/timeframe-filter-350x220.png)

1. グラフ化されたライン上のポイントの上にマウスポインターを置くと、指定した日付の予定時間と予定時間、容量の割合、およびホームチームがその時点で過ぎたか、満たされていなかったか、または能力であったかが表示されます。

   ![チーム容量のポップアップ](assets/team-capacity-capacity-pop-up-350x351.png)

1. （オプション）ビジュアライゼーションデータを書き出すには、 **書き出し** アイコン ![書き出しアイコン](assets/export.png) ビジュアライゼーションの右上隅で、エクスポート形式を選択します。

   * グラフ (PNG)
   * データテーブル (XSLX)

