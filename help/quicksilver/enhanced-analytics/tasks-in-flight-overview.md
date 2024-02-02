---
title: 拡張分析のフライトビジュアライゼーションでのタスクの表示
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: フライトビジュアライゼーションのタスクでは、プロジェクトで進行中のタスク数（適用されたフィルター条件内）、各タスクの完了作業の割合およびタスクのスケジュールを表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: cc738450-362a-49e8-836f-611fa82057b5
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: ht
source-wordcount: '717'
ht-degree: 100%

---

# 拡張分析のフライトビジュアライゼーションでのタスクの表示

フライトビジュアライゼーションのタスクでは、プロジェクトで進行中のタスク数（適用されたフィルター条件内）、各タスクの完了作業の割合およびタスクのスケジュールを表示できます。

![](assets/tasks-in-flight-possible-replacement-350x104.png)

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront プラン</a>*</td> 
   <td> <p>ビジネス以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront ライセンスの概要</a>*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへの表示アクセス</p> <p>タスクへの表示アクセス権（タスクを更新するには、タスクへの編集アクセス権が必要です。）</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。<br>Workfront 管理者がユーザーのアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトおよびタスクの両方のオブジェクトに対する表示権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

強化機能分析を使用するための前提条件については、[強化機能分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)の「前提条件」の節を参照してください。

## フライトビジュアライゼーションのタスクについて

フライトプランビジュアライゼーションのタスクには、次のタスクの詳細が表示されます。

* **タスクの予定期間**：タスクバーの長さは、タスクの開始日と完了日に基づく予定期間を示します。

  ![](assets/tasks-in-flight-duration-350x80.png)

* **完了した作業量**：タスクバー内の濃い青色は、タスクの完了作業量を示します。この完了率は、タスクバーの右側に表示されます。

  ![](assets/tasks-in-flight-dark-blue-350x35.png)

* **未完了の作業量**：タスクバー内の薄い青色は、タスクで取り組む必要がある未完了作業量を示します。

  ![](assets/tasks-in-flight-light-blue-350x35.png)

この情報は、以下を判断する際に役立ちます。

* 仕事の作業量が焦点を当てている場所。
* どのタスクがプロジェクトをリスクにさらす可能性があるか。
* タスクがどれだけ完了に近づいているか。
* 特定のタスクについて誰と話す必要があるか。

このビジュアライゼーションに最適なデータを取得する方法について詳しくは、[拡張分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)を参照してください。

## フライトビジュアライゼーションのタスクを表示

1. メインメニューアイコン ![](assets/main-menu-icon-16x12.png) をクリックし、「**分析**」を選択します。
1. （オプション）別の日付範囲を使用するには、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用について詳しくは、[拡張分析でフィルターを適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

1. （条件付き）プロジェクトデータセットを制限する必要がある場合は、使用するフィルターを選択して適用します。

   拡張分析でのフィルターの追加について詳しくは、[拡張分析でフィルターを適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたり Workfront からログアウトした後でもフィルターはアクティブの状態が維持されます。

1. フライトプランまたはプロジェクトツリーマップビジュアライゼーションで、プロジェクトをクリックして詳細情報を表示します。

   フライトビジュアライゼーションのバーンダウンとタスクが表示されます。

   >[!NOTE]
   >
   >これら他のビジュアライゼーションについて詳しくは、以下を参照してください。
   >
   >   
   >   
   >   * [フライトプランビジュアライゼーションを拡張分析で表示](../enhanced-analytics/flight-plan-overview.md)
   >   * [プロジェクトツリーマップのビジュアライゼーションを拡張分析で表示](../enhanced-analytics/project-treemap-overview.md)
   >   * [バーンダウンのビジュアライゼーションを拡張分析で表示](../enhanced-analytics/burndown-overview.md)
   >   
   >

1. （オプション）日付範囲にズームインするには、日付範囲の開始点としてビジュアライゼーション上の点を選択し、日付範囲の終了点までドラッグします。

   他のすべてのビジュアライゼーションが同じ日付範囲に更新され、時間枠フィルターが作成されます。

   ![](assets/timeframe-filter-350x220.png)

1. （オプション）タスクの並べ替え方法を変更するには、**並べ替え**&#x200B;メニューをクリックして、新しい並べ替えオプションを選択します。

   * **完了日**
   * **アルファベット順（A～Z)**
   * **作業分割構造**（このオプションは、プロジェクト内のタスクの表示順に一致します。）

   ページ上の他のすべてのビジュアライゼーションは、並べ替えの選択に合わせて更新されます。

1. 選択したプロジェクトのタスクの進行状況を確認し、特定のタスクの上にポインタを合わせて、予定時間数、予定期限、完了率を表示します。

   ![](assets/tasks-in-flight-task-details-350x242.png)

1. タスクをクリックして画面の右側にタスクの詳細を開くと、タスクの詳細情報の確認、更新の表示または入力、タスクの変更を行うことができます。

   ![](assets/task-details-qs-350x675.png)

1. （オプション）ビジュアライゼーションデータを書き出すには、ビジュアライゼーションの右上隅にある&#x200B;**書き出しアイコン** ![](assets/export.png) をクリックして、書き出し形式を選択します。

   * **グラフ（PNG）**
   * **データテーブル（XSLX）**

