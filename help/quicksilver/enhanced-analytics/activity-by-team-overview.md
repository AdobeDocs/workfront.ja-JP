---
title: 拡張分析でチームごとのアクティビティのビジュアライゼーションを表示する
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: チーム別のアクティビティのビジュアライゼーションは、ホームチームの特定の期間に発生したアクティビティを表示し、異なるホームチームが Adobe Workfront でどのように時間を費やしたかを理解できます。このビジュアライゼーションは、Workfront でのホームチームの設定に応じて、様々なインサイトを提供し、様々な質問に答えることができます。
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 96%

---

# 拡張分析でチームごとのアクティビティのビジュアライゼーションを表示する

<!-- Audited: 12/2023 -->

チーム別のアクティビティのビジュアライゼーションは、ホームチームの特定の期間に発生したアクティビティを表示し、異なるホームチームが Adobe Workfront でどのように時間を費やしたかを理解できます。このビジュアライゼーションは、Workfront でのホームチームの設定に応じて、様々なインサイトを提供し、様々な質問に答えることができます。

>[!NOTE]
>
>プロジェクトアクティビティのビジュアライゼーションは、このビジュアライゼーションに似ていますが、ホームチームに割り当てられたユーザーではなく、プロジェクトに割り当てられたユーザーに基づくアクティビティを表示します。\
>プロジェクトアクティビティのビジュアライゼーションについて詳しくは、[強化機能分析でプロジェクトアクティビティのビジュアライゼーションを表示](../enhanced-analytics/project-activity-overview.md)を参照してください。

![](assets/activity-by-team-350x113.png){width="700"}

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
   <td>
      <p>新規：</p> 
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

## チーム別アクティビティのビジュアライゼーションについて

フィルターされた期間の特定のイベントを要約するために、様々なアクティビティが様々な色で表示されます。

* **ログインしたユーザー：**&#x200B;紫色のボックスは、ホームチームのユーザーがその日にログインしたことを示します。濃い色は、ログインしているユーザーの数が多いことを示します。

  ![](assets/project-activity-users-logged-in.png)

* **タスクステータスの変更：**&#x200B;ピンク色のボックスは、ホームチームのユーザーがその日のタスクのステータスを変更したことを示します。濃い色は、変更されたタスクステータスの数が多いことを示します。

  ![](assets/project-activity-task-status-changes.png)

* **完了したタスク：**&#x200B;青いボックスは、ホームチームのユーザーがその日にタスクを完了したことを示します。濃い色は、完了したタスクの数が多いことを示します。

  ![](assets/project-activity-tasks-completed.png)

ボックスの上にマウスを置くと、その日にアクションが完了した正確な回数が表示されます。チームを選択すると、ホームチームの各ユーザーごとのこれらのアクティビティの分類を確認できます。

この情報は、以下を判断するうえで役に立ちます。

* ホームチーム内で発生しているアクティビティとその割合。
* どのホームチームがオーバーワークになっているか、またはシステムをより多く使用しているか。
* 作業の配分がホームチームに適しているか。

このビジュアライゼーションに最適なデータを取得する方法については、[拡張分析の概要](../enhanced-analytics/enhanced-analytics-overview.md)を参照してください。

## チーム別アクティビティのビジュアライゼーションを表示する

1. メインメニューアイコン ![](assets/main-menu-icon-16x12.png) をクリックしたあと、「**分析**」を選択します。
1. 左側のパネルで、「**ユーザー**」を選択します。

   ![](assets/people-area-cropped-qs-350x276.png)

1. （オプション）別の日付範囲を使用するには、日付範囲フィルターから新しい開始日と終了日を選択します。

   ![](assets/filters-select-date-range-350x344.png)

   日付範囲フィルターの使用方法について詳しくは、[強化機能分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

1. （条件付き）チームフィルターを設定していない場合は、チームフィルターを追加し、データの表示対象となる各チームを選択します。

   強化機能分析でのフィルターの追加の詳細については、[強化機能分析でのフィルターの適用](../enhanced-analytics/use-enhanced-analytics-filters.md)を参照してください。

   フィルターを追加した後、最大 50 個のプロジェクトのデータが表示され、ページを離れたり Workfront からログアウトした後でもフィルターはアクティブの状態が維持されます。

1. （オプション）日付範囲にズームインするには、日付範囲の開始点としてビジュアライゼーション上の点を選択し、日付範囲の終了点までドラッグします。

   他のすべてのビジュアライゼーションが同じ日付範囲に更新され、時間枠フィルターが作成されます。

   ![](assets/timeframe-filter-350x220.png)

1. チーム名をクリックする

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   ホームチームが完了したアクティビティの詳細を表示します。

   リストが展開され、ホームチームに割り当てられた各ユーザーのアクティビティが表示されます。

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. 色付きのボックスの上にポインタを合わせると、ユーザーがアクションを完了した日付と、その日のアクションが完了した回数が表示されます。

   暗い色は、アクティビティが高いことを示します。

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. （オプション）ビジュアライゼーションデータを書き出すには、ビジュアライゼーションの右上隅にある書き出しアイコン ![](assets/export.png) をクリックしたあと、書き出し形式を選択します。

   * **グラフ（PNG）**
   * **データテーブル（XSLX）**

