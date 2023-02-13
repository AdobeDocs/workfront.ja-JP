---
title: 拡張分析でのプロジェクトアクティビティのビジュアライゼーションの表示
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: プロジェクトアクティビティビジュアライゼーションは、特定の期間に発生した、プロジェクトレベルのアクティビティ（プロジェクトに割り当てられた各人のアクティビティ）の集計ビューを表示します。 フォーカスを絞り込んでプロジェクト内のアクティビティを理解したり、プロジェクトアクティビティをAdobe Workfrontの他のプロジェクトと比較したりできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 1%

---

# 拡張分析でのプロジェクトアクティビティのビジュアライゼーションの表示

プロジェクトアクティビティビジュアライゼーションは、特定の期間に発生した、プロジェクトレベルのアクティビティ（プロジェクトに割り当てられた各人のアクティビティ）の集計ビューを表示します。 フォーカスを絞り込んでプロジェクト内のアクティビティを理解したり、プロジェクトアクティビティをAdobe Workfrontの他のプロジェクトと比較したりできます。

>[!NOTE]
>
>チーム別のアクティビティビジュアライゼーションは、このビジュアライゼーションと同じように動作しますが、チーム別のアクティビティビジュアライゼーションには、すべてのプロジェクトのホームチームアクティビティが表示されます。\
>チーム別アクティビティのビジュアライゼーションについて詳しくは、 [Enhanced Analytics でのチーム別アクティビティのビジュアライゼーションの表示](../enhanced-analytics/activity-by-team-overview.md).

<!--WRITER bad link; there is no Activity by Team.png
[![](assets/project-activity-350x114.png)](../Resources/Images/Analytics/Activity by Team.png)
-->

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfrontプラン</a>*</td> 
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

## プロジェクトアクティビティのビジュアライゼーションについて

プロジェクトアクティビティは様々な色で表示され、一定期間にプロジェクト内の特定のイベントを要約します。

* **ログインしたユーザー**:紫色のボックスは、その日にログインしたプロジェクトに割り当てられたユーザーを示します。 濃い色は、ログインする人の数が多いことを示します。

   ![](assets/project-activity-users-logged-in.png)

* **タスクステータスの変更**:ピンク色のボックスは、その日のプロジェクトのタスクのステータスを変更したことを示します。 濃い色は、タスクステータスの数が多く変化することを示します。

   ![](assets/project-activity-task-status-changes.png)

* **完了したタスク**:青いボックスは、担当者がプロジェクトのタスクを完了したことを示します。 濃い色は、完了するタスクの数が多いことを示します。

   ![](assets/project-activity-tasks-completed.png)

ボックスの上にマウスポインターを置くと、特定の日にアクションが完了した正確な回数が表示されます。 プロジェクトを選択して、プロジェクトの個々の投稿者によるこれらのアクティビティの分類を表示できます。

この情報を表示すると、次の項目を特定するのに役立ちます。

* 特定のプロジェクトに対する「 」アクティビティ。
* 他のプロジェクトと比較した、1 つのプロジェクトのアクティビティ。
* プロジェクトで作業しているユーザーと頻度。

このビジュアライゼーションに最適なデータを取得する方法については、 [分析の強化の概要](../enhanced-analytics/enhanced-analytics-overview.md).

## プロジェクトアクティビティのビジュアライゼーションを表示

1. メインメニューアイコンをクリックします。 ![](assets/main-menu-icon-16x12.png)を選択し、「 **Analytics**.
1. （オプション）別の日付範囲を使用する場合は、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >3 ヶ月を超える期間に対して日付範囲を選択した場合、プロジェクトアクティビティのビジュアライゼーションにはデータが表示されません。

1. （条件付き）プロジェクトデータセットを制限する必要がある場合は、使用するフィルタを選択して適用します。

   Enhanced Analytics でのフィルターの追加について詳しくは、 [拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md).

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたりWorkfrontからログアウトした後でもフィルターはアクティブなままになります。

1. （オプション）日付範囲を拡大するには、日付範囲の開始点としてビジュアライゼーション上の点を選択し、日付範囲の終わりまでドラッグします。

   その他のビジュアライゼーションはすべて、同じ日付範囲に更新され、期間フィルターが作成されます。

   ![](assets/timeframe-filter-350x220.png)

1. （オプション）プロジェクトの並べ替え方法を変更するには、 **並べ替え基準** メニューで、新しい並べ替えオプションを選択します。

   * **A - Z**
   * **Z - A**
   * **完了予定日**
   * **予定開始日**

   ページ上のその他すべてのビジュアライゼーションは、並べ替えの選択に合わせて更新されます。

1. （条件付き）データセットに 50 個を超えるプロジェクトがある場合、ビジュアライゼーションの左下隅にある矢印を使用して、50 個のプロジェクトの 1 つのグループから次のグループに移動します。

   ページ上のその他すべてのビジュアライゼーションは、ページの選択に合わせて更新されます。

   ![](assets/pagination-350x118.png)

1. ビジュアライゼーションのプロジェクトをクリックして、プロジェクトの詳細を表示します。

   リストが展開し、プロジェクトの個々の投稿者のアクティビティが表示されます。

1. ボックスにマウスポインターを置くと、ユーザーがアクションを完了した日付と、その日のアクションが完了した回数が表示されます。

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. （オプション）ビジュアライゼーションデータを書き出すには、 **書き出しアイコン** ![](assets/export.png) ビジュアライゼーションの右上隅で、エクスポート形式を選択します。

   * **グラフ (PNG)**
   * **データテーブル (XSLX)**

