---
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
title: 拡張分析でのプロジェクトツリーマップビジュアライゼーションの表示
description: プロジェクトツリーマップビジュアライゼーションは、サイズの他の作業作業と比較して、特定の時間枠（日）で作業した時間や日を表示します。 これは、ユーザーがプロジェクトに費やした時間を把握するのに役立ちます。
author: Nolan
feature: Reports and Dashboards
exl-id: 6216465e-c3bb-4f2f-b71c-766ad0c2ed40
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 2%

---

# 拡張分析でのプロジェクトツリーマップビジュアライゼーションの表示

<!-- Audited: 12/2023 -->

プロジェクトツリーマップビジュアライゼーションは、サイズの他の作業作業と比較して、特定の時間枠（日）で作業した時間や日を表示します。 これは、ユーザーがプロジェクトに費やした時間を把握するのに役立ちます。

![](assets/project-treemap-350x126.png){width="700"}

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfrontプラン</a></td> 
   <td> <p>ビジネス以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfrontライセンスの概要</a></td> 
   <td>   <p>新規：</p> 
   <ul><li>明るいか高い</li></ul>
   <p>現在：</p>
   <ul><li>レビュー以上</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを表示</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>表示</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

拡張 Analytics を使用するための前提条件については、「前提条件」の節を参照してください。 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md).

## プロジェクトツリーマップビジュアライゼーションについて

プロジェクトツリーマップビジュアライゼーションのボックスはプロジェクトを表し、ボックスのサイズは、様々なプロジェクトに費やした時間の比較を示します。 ボックスが大きいほど、プロジェクトに費やす時間が長くなります。

プロジェクトツリーマップビジュアライゼーションは、次の要素で構成されます。

* **小さく、薄い青いボックス**：時間や日数が少ないプロジェクトは、明るい青の小さなボックスとして表示されます。

  ![](assets/project-treemap-smaller-box.png)

* **大きい濃い青のボックス**：より長い時間（または日）を持つプロジェクトは、濃い青の大きなボックスとして表示されます。

  ![](assets/project-treemap-larger-box-350x205.png)

* **中サイズの青いボックス**:2 つのカテゴリの間にあるプロジェクトは、濃い青と薄い青の間に青のシェードが付いた中サイズのボックスとして表示されます。 中サイズのボックスには、青の 3 つの色合いが可能です。

右側の凡例は、青の各シェードの完了時間の内訳を示しています。 この凡例は動的で、データに応じて更新されます。

![](assets/project-treemap-hours-completed.png)

>[!NOTE]
>
>予定時間ではなく期間別のプロジェクトツリーマップビジュアライゼーションを表示している場合、この凡例には、青のシェードごとの作業日数の分類が表示されます。\
>![](assets/project-treemap-days-worked.png)>

この情報を確認することで、次の項目を特定することができます。

* 選択した日付範囲内で作業中の項目の優先度。
* どのチームが時間を費やしているか。
* チームが正しいことに注力している場合。
* 特定のプロジェクトをクリックしたとき、その期間にプロジェクトの範囲がどの程度変化したか。

このビジュアライゼーションに最適なデータを取得する方法については、 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md).

## プロジェクトツリーマップビジュアライゼーションの表示

1. メインメニューアイコンをクリックします。 ![](assets/main-menu-icon-16x12.png)を選択し、「 **Analytics**.
1. （オプション）別の日付範囲を使用する場合は、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （条件付き）プロジェクトデータセットを制限する必要がある場合は、使用するフィルタを選択して適用します。

   Enhanced Analytics でのフィルターの追加について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたりWorkfrontからログアウトした後でもフィルターはアクティブなままになります。

1. （オプション）プロジェクトの並べ替え方法を変更するには、 **並べ替え基準** プロジェクトツリーマップビジュアライゼーションの右上隅にあるメニューで、新しい並べ替えオプションを選択します。

   * **A ～ Z**
   * **Z - A**
   * **計画完了日**
   * **計画開始日**

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
   >次を選択した場合、 **duration** 表示すると、次の期間の詳細が表示されます。
   >
   >* **計画期間**：プロジェクトの完了を予定している日数です。
   >* **稼働日数**：上部で選択した日付範囲内で完了した各タスクの予定期間を、1 日の時間数で割った値です。
   >   
   >![](assets/duration-treemap-350x159.png)
   >
   >期間について詳しくは、 [分析の概要の強化](../enhanced-analytics/enhanced-analytics-overview.md).

1. （オプション）ビジュアライゼーションデータを書き出すには、 **書き出しアイコン** ![](assets/export.png) ビジュアライゼーションの右上隅で、エクスポート形式を選択します。

   * **グラフ (PNG)**
   * **データテーブル (XSLX)**

1. プロジェクトをクリックして、 Burndown と Tasks をフライトビジュアライゼーションで開き、タスクと時間（または日）がプロジェクトのサイズに与えた影響をより深く把握します。

バーンダウンビジュアライゼーションについて詳しくは、 [拡張分析でのバーンダウンビジュアライゼーションの表示](../enhanced-analytics/burndown-overview.md). フライトビジュアライゼーションのタスクについて詳しくは、 [Enhanced Analytics でのフライトビジュアライゼーションでのタスクの表示](../enhanced-analytics/tasks-in-flight-overview.md).

