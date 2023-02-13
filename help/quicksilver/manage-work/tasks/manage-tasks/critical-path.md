---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: プロジェクトの概要の重要なパス
description: プロジェクトのクリティカルパスの決定は、Adobe Workfrontが、プロジェクトのタイムラインに影響を与える可能性のある、プロジェクト内の一連のタスクにフラグを設定する自動的な方法です。 プロジェクトのタイムラインに影響を与える可能性のあるタスクは、クリティカルパスタスクとしてフラグ付けされます。
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# プロジェクトの概要の重要なパス

プロジェクトのクリティカルパスの決定は、Adobe Workfrontが、プロジェクトのタイムラインに影響を与える可能性のある、プロジェクト内の一連のタスクにフラグを設定する自動的な方法です。 プロジェクトのタイムラインに影響を与える可能性のあるタスクは、クリティカルパスタスクとしてフラグ付けされます。

次の機能は、プロジェクトの重要なパスに影響を与える可能性があります。

* プロジェクトの作業分類構造。

   作業分類構造の詳細については、 [プロジェクト内の作業分類構造の決定](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* 各タスクが完了するまでに要する時間（期間）です。
* タスク間の依存関係。

   次の点に注意してください。

   * [ クリティカルパス ] のタスクに先行タスク関係がある場合、先行タスクや後続タスクの日付の変更が従属タスクに直接影響する場合は、先行タスクや後続タスクも [ クリティカルパス ] に表示されます。

      >[!TIP]
      >
      >タスクの後続タスクの日付が、依存タスクの日付に直接影響を与えず、プロジェクトの日付にも影響を与えない場合、後続タスクは [ クリティカルパス ] には影響を与えません。
      >
      >
      >![](assets/successor-not-on-critical-path-350x150.png)     >

   * サブタスクをクリティカルパスタスクとして指定した場合、親タスクの予測開始日時がサブタスクと同じであれば、親タスクもクリティカルパスタスクとして識別されます。

これらの機能を考慮し、最も早いタスクとプロジェクトの終了を決定するタスクの間の最長パスを使用して、クリティカルパスが計算されます。 クリティカルパスの計算では、各タスクを開始および終了できる最も早い時間と最新の時間が考慮されます。この時間は、プロジェクトの時間を長くする必要はありません。 このプロセスは、どのタスクが「重要」（かつ最も長いパスに属する）か、どのタスクが「総浮動小数」（プロジェクトを長くすることなく遅延できます）かを決定します。

クリティカルパスでのタスクのアクティビティの遅延は、プロジェクトの完了予定日に直接影響します（クリティカルパスに浮動小数点はありません）。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクへのアクセス権を表示または上限に設定</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する表示権限以上の権限 </p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## クリティカルパスの表示

Workfrontアプリケーションの次の領域で、クリティカルパスに属するタスクを表示できます。

* [ガントチャートにクリティカルパスを表示](#view-the-critical-path-in-the-gantt-chart)
* [タスクリストまたはレポートにクリティカルパスを表示](#view-the-critical-path-in-a-task-list-or-report)

### ガントチャートにクリティカルパスを表示 {#view-the-critical-path-in-the-gantt-chart}

ガント・チャートのクリティカル・パスにタスクを表示する手順は、次のとおりです。

1. クリティカルパスを表示するプロジェクトに移動します。
1. クリック **タスク** をクリックします。
1. 次をクリック： **ガントチャート** アイコンが表示されます。

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. を展開します。 **オプション** メニューを開き、 **クリティカルパス** オプション。

   クリティカルパス上のタスクは、ガントチャートでタイムラインの上に赤い線が引かれています。

   ![crtitical_path_on_gant__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### タスクリストまたはレポートにクリティカルパスを表示 {#view-the-critical-path-in-a-task-list-or-report}

タスクのリストのクリティカルパスにあるタスクを表示するには、次の手順に従います。

1. クリティカルパスを表示するプロジェクトに移動します。
1. クリック **タスク** をクリックします。
1. 次の **表示** ドロップダウンメニューで、「 **ステータス**.

   クリティカルパス上のタスクには、 **クリティカルパス** 旗 **フラグ** 」列に表示されます。

   同じビューをタスクレポートに適用できます。

   レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   または

   次の **フィルター** ドロップダウンメニューで、「 **新しいフィルター**.

1. クリック **フィルタールールを追加** 入力を開始 **重要** 内 **次の場合にのみタスクを表示：** フィールドに入力します。

1. リストに表示される場合に選択します。
1. クリック **フィルターを保存**.

   リストには、クリティカルパス上のタスクのみが表示されます。
