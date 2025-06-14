---
title: 拡張分析での進行計画ビジュアライゼーションの表示
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 進行計画ビジュアライゼーションは、（適用されたフィルター条件内で）実行されたプロジェクトの数、これらのプロジェクトの期間中に発生した条件の変化、およびこれらのプロジェクトが計画完了期限にどの程度近づいているかを示します。
author: Nolan
feature: Reports and Dashboards
exl-id: c64ed752-151a-40f7-ab18-684e2cd032bc
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 93%

---

# 拡張分析での進行計画ビジュアライゼーションの表示

>[!IMPORTANT]
>
>Enhanced Analytics は、5 月 27 日（PT）にWorkfrontから削除されました。 Workfront Data Connect は新しい代替ソリューションであり、現在使用している Enhanced Analytics のビジュアライゼーションをレプリケートするために使用できます。 <br> 詳しくは、[Enhanced Analytics の廃止 ](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md) ガイドを参照してください。


進行計画ビジュアライゼーションは、（適用されたフィルター条件内で）実行されたプロジェクトの数、これらのプロジェクトの期間中に発生した条件の変化、およびこれらのプロジェクトが計画完了期限にどの程度近づいているかを示します。

![ 運航計画 ](assets/flight-plan-350x132.png)

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Adobe Workfront プラン</a>*</td> 
   <td> <p>ビジネス以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront ライセンスの概要</a>*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへの表示アクセス</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。<br>Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対するアクセス権の表示</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

強化機能分析を使用するための前提条件については、[強化機能分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)の「前提条件」の節を参照してください。

## 進行計画ビジュアライゼーションについて

プロジェクトの実際の期間には、次のプロジェクト状況のみが表示されます。

* 目標どおり
* リスクあり
* トラブル発生中

プロジェクト状況について詳しくは、[プロジェクト状況と状況タイプの概要](../manage-work/projects/manage-projects/project-condition-and-condition-type.md)を参照してください。

進行計画ビジュアライゼーションには、次のプロジェクトの詳細が表示されます。

* **予定期間**：青い水平線はプロジェクトの計画長を表し、線の両端に三角形が表示され、開始日と終了日が示されます。

  ![ 予定期間 ](assets/planned-duration-line-350x37.png)

* **実際の期間**：予定期間の下の色付きの太い線は、プロジェクトの実際の長さを表します。線の色は、プロジェクトの生活中の特定の時間におけるプロジェクトの条件に応じて変わります。

  ![ 実際の期間 ](assets/actual-duration-line.png)

* **実際の状況**：太い色付きの線は、時間の異なる時点でのプロジェクトの状態も表示します。線の色は、プロジェクトの条件に応じて変化します。

   * **緑**：目標通り
   * **オレンジ**：危険あり
   * **赤**：トラブル発生中

  ![ 実際の状況 ](assets/actual-condition-color.png)

進行計画ビジュアライゼーションのプロジェクト行にポインタを合わせると、プロジェクトの予定期間、現在のプロジェクト状況、および該当する場合はカスタム条件に関する情報を確認できます。期間や状況に影響を与えた可能性のある内容について詳しくは、拡張分析領域の他のビジュアライゼーションを参照してください。

この情報は、以下を判断するうえで役に立ちます。

* 予定完了日を過ぎてプロジェクトを延長したイベント。
* プロジェクトでイシューが発生し始めたタイミング。
* 同じ期間にわたってオープンになっているプロジェクトの数。
* アクティブなプロジェクトの数。
* 特別な注意やサポートを必要とするプロジェクト。

このビジュアライゼーションに最適なデータを取得する方法について詳しくは、[拡張分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)を参照してください。

## 進行計画ビジュアライゼーションの表示

1. **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon-16x12.png) をクリックし、「**Analytics**」を選択します。
1. （オプション）別の日付範囲を使用するには、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![日付範囲を選択](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用については、[拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

1. （条件付き）プロジェクトデータセットを制限する必要がある場合は、使用するフィルターを選択して適用します。

   拡張分析でのフィルターの追加について詳しくは、[拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたり Workfront からログアウトした後でもフィルターはアクティブの状態が維持されます。

1. （オプション）日付範囲にズームインするには、日付範囲の開始点としてビジュアライゼーション上の点を選択し、日付範囲の終了点までドラッグします。

   他のすべてのビジュアライゼーションが同じ日付範囲に更新され、時間枠フィルターが作成されます。

   ![期間フィルター](assets/timeframe-filter-350x220.png)

1. （オプション）プロジェクトの並べ替え方法を変更するには、進行計画ビジュアライゼーションの右上隅にある&#x200B;**並べ替え**&#x200B;メニューをクリックし、新しい並べ替えオプションを選択します。

   * **A - Z**
   * **Z - A**
   * **完了予定日**
   * **予定開始日**

   ページ上の他のすべてのビジュアライゼーションは、並べ替えの選択に合わせて更新されます。

1. （条件付き）データセット内に 50 を超えるプロジェクトがある場合は、ビジュアリゼーションの左下隅にある矢印を使用すると、50 プロジェクトから成る 1 つのグループから次のグループに移動できます。

   ページ上の他のすべてのビジュアライゼーションは、ページの選択に合わせて更新されます。

   ![ ページネーション ](assets/pagination-350x118.png)

1. プロジェクトバーグラフにポインタを合わせると、青い日付線と、次の詳細が表示されます。

   * 予定タイムライン
   * 現在の状況
   * カスタム条件（該当する場合）

   ![ プロジェクト棒グラフ ](assets/project-bar-graph-350x143.png)

1. （オプション）ビジュアライゼーションデータを書き出すには、ビジュアライゼーションの右上隅にある&#x200B;**書き出し**&#x200B;アイコン ![書き出しアイコン](assets/export.png) をクリックし、書き出し形式を選択します。

   * **グラフ（PNG）**
   * **データテーブル（XSLX）**

1. その他のプロジェクト情報を表示するには、ビジュアライゼーション上のプロジェクトをクリックして、フライトビジュアライゼーションのバーンダウンとタスクを開きます。

   これらのビジュアライゼーションは、プロジェクトがトラックから外れた原因についてより深い洞察を得るのに役立ちます。また、進行中のプロジェクトを簡単にチェックインできます。\
   バーンダウンのビジュアライゼーションについて詳しくは、[強化機能分析でバーンダウンビジュアライゼーションを表示](../enhanced-analytics/burndown-overview.md)を参照してください。フライトビジュアライゼーションのタスクについて詳しくは、[拡張分析におけるフライトビジュアライゼーションのタスクの表示](../enhanced-analytics/tasks-in-flight-overview.md)を参照してください。

