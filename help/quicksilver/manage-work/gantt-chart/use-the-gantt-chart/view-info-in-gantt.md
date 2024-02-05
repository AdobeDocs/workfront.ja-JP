---
navigation-topic: use-the-gantt-chart
title: '[!UICONTROL ガントチャート]での情報の表示'
description: タスクリストガントチャートとプロジェクトリストガントチャートには、プロジェクトとタスクに関する情報が表示されます。
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 99%

---

# [!UICONTROL ガントチャート]での情報を表示

タスクリスト[!UICONTROL ガントチャート]とプロジェクトリスト[!UICONTROL ガントチャート]には、プロジェクトとタスクに関する情報が表示されます。

## アクセス要件

この記事の手順に従うには、以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンスの概要*</td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトとタスクに対する[!UICONTROL View]以上のアクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する[!UICONTROL View]以上のアクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!UICONTROL ガントチャート]を見つける

Workfront 内の複数の領域から、タスクリストガントチャートとプロジェクトリスト[!UICONTROL ガントチャート]の両方を見つけることができます。詳しくは、[[!UICONTROL ガントチャートの概要]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)を参照してください。

## [!UICONTROL クリティカルパス]上のタスクを表示

プロジェクトリスト[!UICONTROL ガントチャート]では、[!UICONTROL クリティカルパス]上にないタスクは水色の水平線で表示されます。プロジェクトの[!UICONTROL クリティカルパス]上にあるタスクは、赤い水平線で表示されます。

[!UICONTROL クリティカルパス]のタスクについて詳しくは、[プロジェクトの[!UICONTROL クリティカルパスの概要]](../../../manage-work/tasks/manage-tasks/critical-path.md)を参照してください。

## プロジェクトリスト[!UICONTROL ガントチャート]でタスク情報を表示

プロジェクトのタスク情報は、プロジェクトリストから直接表示できます。タスクは、各プロジェクト名の下に表示されます。

>[!NOTE]
>
>プロジェクトリスト[!UICONTROL ガントチャート]からタスクを編集することはできません。

次の領域のプロジェクトのリストからプロジェクトのタスク情報を直接表示できます。

* [!UICONTROL プロジェクト]領域
* ポートフォリオ内
* プログラム内

プロジェクトのリストからプロジェクト内のタスクを表示するには、次の手順に従います。

1. 上記のいずれかの領域に移動します。

   例えば、[!UICONTROL メインメニュー]から、**[!UICONTROL プロジェクト]**&#x200B;をクリックします。

   プロジェクトのリストが表示されます。

1. 画面の右上隅にある **[!UICONTROL ガントチャート]** アイコン ![](assets/gantt-icon-nwe.png) をクリックします。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. **[!UICONTROL タスクリストを表示]**&#x200B;アイコンをクリックします。

1. 左側のプロジェクトリストで、プロジェクト名の横にあるドロップダウン矢印をクリックして、そのプロジェクトの下にあるタスクを表示します。\
   これにより、タスク情報が[!UICONTROL ガントチャート]に表示されます。\
   ![Show_task_list_enabled_project_expanded.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. （オプション）右上隅にある&#x200B;**[!UICONTROL 印刷]**&#x200B;アイコンをクリックして、[!UICONTROL ガントチャート]を書き出します。

   >[!NOTE]
   >
   >プロジェクトリスト[!UICONTROL ガントチャート]はプロジェクトのみを書き出します。タスク情報は含まれていません。

## [!UICONTROL ガントチャート]に情報が表示される期間を変更

[!UICONTROL ガントチャート]に表示される期間を調整してより詳細に情報を表示したり、日、週、月、四半期、または年のビューにすばやく移動できます。

* [期間の詳細レベルを変更](#change-the-time-period-on-a-granular-level)
* [日、週、月、四半期、または年ごとに情報を表示](#view-information-by-day-week-month-quarter-or-year)

### 期間の詳細レベルを変更 {#change-the-time-period-on-a-granular-level}

1. [!UICONTROL ガントチャート] のタイムラインにマウスポインターを置き、ズームインジケーターを左から右にドラッグしてタイムラインを拡大または縮小します。\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### 日、週、月、四半期、または年ごとに情報を表示 {#view-information-by-day-week-month-quarter-or-year}

1. [!UICONTROL ガントチャート]で、時間枠ドロップダウンメニューをクリックします。

   ![](assets/timeline-options.png)

1. 次の利用可能なオプションから時間枠を選択します。

   * **[!UICONTROL 全体を表示]**：このオプションはプロジェクト全体のタイムラインを表示します。
   * **[!UICONTROL すべてのプロジェクト]**：このオプションは、プロジェクトリストガントチャートでのみ使用できます。
   * **[!UICONTROL 年]**
   * **[!UICONTROL 四半期]**
   * **[!UICONTROL 月]**
   * **[!UICONTROL 週]**
   * **[!UICONTROL 日]**

1. （オプション）[!UICONTROL 週]や[!UICONTROL 日]など、より詳細な時間枠を選択し、[!UICONTROL ガントチャート]の下部にある水平スクロールバーをクリックしてドラッグし、プロジェクトのタイムラインを左から右に移動します。\
   [!UICONTROL ガント]のタイムラインスナップショットでプロジェクト全体が表示されます。

   >[!TIP]
   >
   >タイムラインのスナップショットは、水平スクロールバーをクリックした後にのみ表示されます。

   ![stretchy_gantt_minimap_with_outline__1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. （オプション）タイムラインのスナップショット内の任意の場所をクリックすると、プロジェクトの期間内の特定のポイントに移動します。\
   または\
   スナップショットビューアーのハンドルをドラッグして、特定のタイムライン範囲を選択し、メインの[!UICONTROL ガント]に表示します。

## フィルター、ビュー、グループ化の使用

[!UICONTROL ガントチャート]は、タスクリストに現在表示されている情報を視覚的に表現したものです。フィルター、ビュー、グループ化は、両方の[!UICONTROL ガントチャート]のリストにあるオブジェクトを適用できます。

>[!CAUTION]
>
>[!UICONTROL 手動]保存／[!UICONTROL タイムライン計画]を選択してタスクリストへの変更を保存する場合、フィルター、ビュー、グループ化を適用することはできません。リスト内のタスクに対する変更の保存について詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

リストに適用したフィルターとグループ化は、プロジェクトリストとタスクリストの両方の[!UICONTROL ガントチャート]に反映され、ガントチャートが書き出されたときにも含まれます。

* フィルター\
   リストにフィルターを適用すると、[!UICONTROL ガントチャート]に表示される情報を制御できます。\
   フィルターの適用について詳しくは、  [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* グループ化\
   リストに適用したグループ化は、[!UICONTROL ガントチャート]に反映されます。\
   グループ化の適用について詳しくは、[Adobe Workfront のグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

ビューは、[!UICONTROL ガントチャート]に反映されません。ただし、[!UICONTROL ガントチャート]を書き出すと（詳しくは、[[!UICONTROL ガントチャート]を PDF に書き出し](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)を参照してください）、[!UICONTROL ガントチャート]に加えてタスクリストが書き出され、現在のビューがリストに適用されます。

## 表示オプションを設定

両方の[!UICONTROL ガントチャート]に表示する情報の種類を選択できます。詳しくは、[[!UICONTROL ガントチャート]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)に表示する情報の設定を参照してください。
