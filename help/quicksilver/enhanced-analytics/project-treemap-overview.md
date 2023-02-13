---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: 拡張分析でのプロジェクトツリーマップビジュアライゼーションの表示
description: プロジェクトツリーマップビジュアライゼーションは、サイズの他の作業作業と比較して、特定の時間枠（日）で作業した時間や日を表示します。 これは、ユーザーがプロジェクトに費やした時間を把握するのに役立ちます。
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# 拡張分析でのプロジェクトツリーマップビジュアライゼーションの表示

プロジェクトツリーマップビジュアライゼーションは、サイズの他の作業作業と比較して、特定の時間枠（日）で作業した時間や日を表示します。 これは、ユーザーがプロジェクトに費やした時間を把握するのに役立ちます。

![](assets/project-treemap-350x126.png)

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfrontプラン</a>*</td> 
   <td> <p>ビジネス以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfrontライセンスの概要</a>*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。<br>Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ビュー</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

拡張 Analytics を使用するための前提条件については、 [分析の強化の概要](../enhanced-analytics/enhanced-analytics-overview.md).

## プロジェクトツリーマップビジュアライゼーションについて

プロジェクトツリーマップビジュアライゼーションのボックスはプロジェクトを表し、ボックスのサイズは、様々なプロジェクトに費やした時間の比較を示します。 ボックスが大きいほど、プロジェクトに費やす時間が長くなります。

プロジェクトツリーマップビジュアライゼーションは、次の要素で構成されます。

* **小さく、薄い青いボックス**:時間や日数が少ないプロジェクトは、明るい青色の小さなボックスとして表示されます。

   ![](assets/project-treemap-smaller-box.png)

* **大きい濃い青のボックス**:時間や日数が長いプロジェクトは、大きなボックスに濃い青で表示されます。

   ![](assets/project-treemap-larger-box-350x205.png)

* **中サイズの青いボックス**:2 つのカテゴリの間にあるプロジェクトは、濃い青と薄い青の色の間に青のシェードが付いた中サイズのボックスとして表示されます。 中サイズのボックスには、青の 3 つの色合いが可能です。

右側の凡例は、青の各シェードの完了時間の内訳を示しています。 この凡例は動的で、データに応じて更新されます。

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>予定時間ではなく期間別のプロジェクトツリーマップビジュアライゼーションを表示している場合、この凡例には、青のシェードごとの作業日数の分類が表示されます。\
>![](assets/project-treemap-days-worked.png)>

この情報を表示すると、次の項目を特定するのに役立ちます。

* 選択した日付範囲で作業中の項目の優先度。
* どのチームが時間を費やしているか。
* チームが正しいことに注力している場合。
* 特定のプロジェクトをクリックしたとき、その期間にプロジェクトの範囲がどの程度変化したか。

このビジュアライゼーションに最適なデータを取得する方法については、 [分析の強化の概要](../enhanced-analytics/enhanced-analytics-overview.md).

## プロジェクトツリーマップビジュアライゼーションの表示

1. メインメニューアイコンをクリックします。 ![](assets/main-menu-icon-16x12.png)を選択し、「 **Analytics**.
1. （オプション）別の日付範囲を使用する場合は、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （条件付き）プロジェクトデータセットを制限する必要がある場合は、使用するフィルタを選択して適用します。

   Enhanced Analytics でのフィルターの追加について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたりWorkfrontからログアウトした後でもフィルターはアクティブなままになります。

1. （オプション）プロジェクトの並べ替え方法を変更するには、 **並べ替え基準** プロジェクトツリーマップビジュアライゼーションの右上隅にあるメニューで、新しい並べ替えオプションを選択します。

   * **A - Z**
   * **Z - A**
   * **完了予定日**
   * **予定開始日**

   ページ上のその他すべてのビジュアライゼーションは、並べ替えの選択に合わせて更新されます。

1. （条件付き）データセットに 50 個を超えるプロジェクトがある場合、ビジュアライゼーションの左下隅にある矢印を使用して、50 個のプロジェクトの 1 つのグループから次のグループに移動します。

   ページ上のその他すべてのビジュアライゼーションは、ページの選択に合わせて更新されます。

   ![](assets/pagination-350x118.png)

1. （オプション）次の場所からビューを変更します。 **予定時間** から **duration**.

   デフォルトでは、予定時間が選択されています。

1. プロジェクトの上にマウスポインターを置くと、プロジェクトの状態と、合計計画時間数、合計完了時間数、および 1 日あたりのプロジェクトの平均滞在時間数が表示されます。

   ![](assets/project-treemap-project-details-350x404.png)

   >[!NOTE]
   >
   >選択した **duration** 表示すると、次の期間の詳細が表示されます。
   >
   >* **計画期間**:プロジェクトを完了する予定の日数。
   >* **勤務日数**:上部で選択した日付範囲内に完了した各タスクの予定期間を、1 日の時間数で割った値です。

   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >期間について詳しくは、 [分析の強化の概要](../enhanced-analytics/enhanced-analytics-overview.md).

1. （オプション）ビジュアライゼーションデータを書き出すには、 **書き出しアイコン** ![](assets/export.png) ビジュアライゼーションの右上隅で、エクスポート形式を選択します。

   * **グラフ (PNG)**
   * **データテーブル (XSLX)**

1. プロジェクトをクリックして、 Burndown と Tasks をフライトビジュアライゼーションで開き、タスクと時間（または日）がプロジェクトのサイズに与えた影響をより深く把握します。

バーンダウンビジュアライゼーションについて詳しくは、 [拡張分析でのバーンダウンビジュアライゼーションの表示](../enhanced-analytics/burndown-overview.md). フライトビジュアライゼーションのタスクについて詳しくは、 [Enhanced Analytics でのフライトビジュアライゼーションでのタスクの表示](../enhanced-analytics/tasks-in-flight-overview.md).

