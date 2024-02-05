---
title: 拡張分析でプロジェクトアクティビティビジュアライゼーションを表示
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: プロジェクトアクティビティのビジュアライゼーションには、特定の時間枠に発生したプロジェクトレベルのアクティビティ（プロジェクトに割り当てられた各人のアクティビティ）の集計ビューが表示されます。フォーカスを絞り込んでプロジェクト内のアクティビティを理解したり、プロジェクトのアクティビティを Adobe Workfront の他のプロジェクトと比較したりできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 96%

---

# 拡張分析でプロジェクトアクティビティビジュアライゼーションを表示

<!-- Audited: 12/2023 -->

プロジェクトアクティビティのビジュアライゼーションには、特定の時間枠に発生したプロジェクトレベルのアクティビティ（プロジェクトに割り当てられた各人のアクティビティ）の集計ビューが表示されます。フォーカスを絞り込んでプロジェクト内のアクティビティを理解したり、プロジェクトのアクティビティを Adobe Workfront の他のプロジェクトと比較したりできます。

>[!NOTE]
>
>チーム別のアクティビティビジュアライゼーションはこのビジュアライゼーションと同様に動作しますが、チーム別のアクティビティのビジュアライゼーションでは、すべてのプロジェクトのホームチームのアクティビティが表示されます。\
>チーム別のアクティビティのビジュアライゼーションの詳細については、[拡張分析でチームごとのアクティビティのビジュアライゼーションを表示](../enhanced-analytics/activity-by-team-overview.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront プラン</a></td> 
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
   <td> <p>プロジェクトへの表示アクセス</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

拡張分析を使用するための前提条件については、[拡張分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)の前提条件の節を参照してください。

## プロジェクトアクティビティのビジュアライゼーションを理解する

プロジェクトアクティビティは、プロジェクト内の特定のイベントを一定期間にわたって要約するためにさまざまなカラーで表示されます。

* **ログインしたユーザー**：紫色のボックスは、プロジェクトに割り当てられたユーザーがその日にログインしたことを示します。濃い色は、ログインしているユーザーの数が多いことを示します。

  ![](assets/project-activity-users-logged-in.png)

* **タスクステータスの変更**：ピンク色のボックスは、その日にユーザーがプロジェクトのタスクのステータスを変更したことを示します。濃い色は、変更されたタスクステータスの数が多いことを示します。

  ![](assets/project-activity-task-status-changes.png)

* **完了したタスク**：青いボックスは、ユーザーがプロジェクトのタスクを完了したことを示します。濃い色は、完了したタスクの数が多いことを示します。

  ![](assets/project-activity-tasks-completed.png)

ボックスの上にマウスを置くと、その日にアクションが完了した正確な回数が表示されます。プロジェクトを選択すると、プロジェクトの個々の投稿者ごとのアクティビティの内訳を確認できます。

この情報を確認することで、次の項目を特定するのに役立ちます。

* 特定のプロジェクトのアクティビティ。
* 他のプロジェクトと比較した、あるプロジェクトのアクティビティ。
* プロジェクトで作業しているユーザーと作業頻度。

このビジュアライゼーションに最適なデータを取得する方法については、[拡張分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)を参照してください。

## プロジェクトアクティビティのビジュアライゼーションを表示

1. メインメニューアイコン ![](assets/main-menu-icon-16x12.png) をクリックしたあと、「**分析**」を選択します。
1. （オプション）別の日付範囲を使用するには、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用については、[拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

   >[!NOTE]
   >
   >3 か月を超える期間の日付範囲を選択した場合、プロジェクトアクティビティビジュアライゼーションにはデータが表示されません。

1. （条件付き）プロジェクトデータセットを制限する必要がある場合は、使用するフィルターを選択して適用します。

   拡張分析でのフィルターの追加について詳しくは、[拡張分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたり Workfront からログアウトした後でもフィルターはアクティブの状態が維持されます。

1. （オプション）日付範囲にズームインするには、日付範囲の開始点としてビジュアライゼーション上の点を選択し、日付範囲の終了点までドラッグします。

   他のすべてのビジュアライゼーションが同じ日付範囲に更新され、時間枠フィルターが作成されます。

   ![](assets/timeframe-filter-350x220.png)

1. （オプション）プロジェクトの並べ替え方法を変更するには、**並べ替え** メニューをクリックして、新しい並べ替えオプションを選択します。

   * **A - Z**
   * **Z - A**
   * **完了予定日**
   * **予定開始日**

   ページ上の他のすべてのビジュアライゼーションは、並べ替えの選択に合わせて更新されます。

1. （条件付き）データセット内に 50 を超えるプロジェクトがある場合は、ビジュアリゼーションの左下隅にある矢印を使用すると、50 プロジェクトから成る 1 つのグループから次のグループに移動できます。

   ページ上の他のすべてのビジュアライゼーションは、ページの選択に合わせて更新されます。

   ![](assets/pagination-350x118.png)

1. ビジュアライゼーションのプロジェクトをクリックすると、プロジェクトの詳細が表示されます。

   リストが展開されて、プロジェクトにおける個々の投稿者のアクティビティが表示されます。

1. ボックスの上にマウスを置くと、ユーザーがアクションを完了した日付と、その日にアクションが完了した回数が表示されます。

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. （オプション）ビジュアライゼーションデータを書き出すには、ビジュアライゼーションの右上隅にある&#x200B;**書き出しアイコン** ![](assets/export.png) をクリックし、次に書き出し形式を選択します。

   * **グラフ（PNG）**
   * **データテーブル（XSLX）**

