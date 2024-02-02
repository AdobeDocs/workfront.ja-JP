---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 実際の時間数の表示
description: Adobe Workfront で作業項目に記録した時間は、実際の時間数とみなされます。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '796'
ht-degree: 100%

---

# 実際の時間数の表示

Adobe Workfront で作業項目に記録した時間は、実際の時間数とみなされます。

実際の時間数は、タスク、イシューまたはプロジェクトの完了に要した実際の時間を表します。

タスクとイシューを含む作業項目に時間を記録しておくことをお勧めします。

ただし、Workfront 管理者は、組織内のワークフローに応じて、ユーザーがプロジェクトに時間を記録できるようにすることもできます。

ユーザーが時間をプロジェクトに記録できるようにシステムを設定する方法について詳しくは、[タイムシートの設定と時間環境設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスク、プロジェクト、イシューに対する表示またはそれ以上のアクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスク、プロジェクト、イシューに対する表示またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## タスクとイシューの実際の時間数とプロジェクトの実際の時間数

タスクとイシューの実際の時間数は、タスクとイシューに直接記録した時間数を表します。

>[!NOTE]
>
>子タスクの実際の時間数は、親タスクの実際の時間数にロールアップされます。親タスクの実際の時間数の計算には、次の式が適用されます。

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

プロジェクトの実際の時間数は、プロジェクトのすべてのタスクの時間数（親タスクに直接記録した時間を含む）とプロジェクトのすべてのイシューの時間数、およびプロジェクト自体に記録した実際の時間数の合計です。

プロジェクトの実際の時間数には、次の式が適用されます。

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 実際の時間数の検索

項目の実際の時間数の値を検索するには、タスク、プロジェクト、イシューの場合と同じ手順を実行します。

タスクの実際の時間数に関する情報は、次の場所で確認できます。

* [「詳細」セクションの実際の時間数](#actual-hours-in-the-details-section)
* [「時間」セクションの実際の時間数](#actual-hours-in-the-hours-section)
* [レポートの実際の時間数](#actual-hours-in-reports)
* [リソース管理ツールの実際の時間数](#actual-hours-in-resource-management-tools)

### 「詳細」セクションの実際の時間数 {#actual-hours-in-the-details-section}

「詳細」セクションの実際の時間数を検索するには、タスク、プロジェクト、イシューの場合と同じ手順を実行します。

タスクの詳細で実際の時間数を検索する手順は、次のとおりです。

1. 実際の時間数を確認したいタスクに移動します。
1. 左パネルの&#x200B;**タスクの詳細**&#x200B;をクリックします。
1. 「**概要**」をクリックし、**実際の時間数**&#x200B;の値を確認します。

   これは、このタスクにログオンした時間の合計です。

### 「時間」セクションの実際の時間数 {#actual-hours-in-the-hours-section}

「時間」セクションの実際の時間数を検索するには、プロジェクト、タスク、イシューの場合と同じ手順を実行します。

「時間」セクションで実際の時間数を検索する手順は、次のとおりです。

1. 実際の時間数を確認したいタスクに移動します。
1. 左パネルの「**時間**」をクリックします。

   設定によっては、「時間」セクションが&#x200B;**表示を増やす**&#x200B;の下に表示される場合があります。

   これにより、タスクに記録した時間エントリのリストが表示されます。

1. **標準**&#x200B;ビューと&#x200B;**プロジェクト**&#x200B;グループ化がこのリストに適用されていることを確認します。

   **時間**&#x200B;列のグループ化行に表示される数は、タスクの実際の時間数の合計数です。

### レポートの実際の時間数 {#actual-hours-in-reports}

タスク、イシュー、またはプロジェクトのレポートを作成する際に、レポート内の各タスク、イシュー、またはプロジェクトの実際の時間数を表示できます。

実際の時間数の列をタスクビューに追加する操作は、レポートのビューの作成の操作に類似しています。

タスクレポートに実際の時間数を表示する手順は、次のとおりです。

1. Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) を選択し、「**レポート**」をクリックします。
1. 「**新しいレポート**」をクリックし、オブジェクトとして「**タスク**」を選択します。

1. 「**列を追加**」をクリックし、**この列に表示**&#x200B;ドロップダウンフィールドが表示されたら&#x200B;**実際の時間数**&#x200B;の入力を開始します。フィールドがリストに表示されたら選択します。

1. 「**保存して閉じる**」をクリックして、レポートを保存します。

   実際の時間数の列には、各タスクで記録された時間数が表示されます。

### リソース管理ツールの実際の時間数 {#actual-hours-in-resource-management-tools}

割り当てられたタスクやイシューに対してユーザーが実行している作業の進捗状況を確認する場合は、次のリソース管理ツールでその進捗状況を確認できます。

* 稼働率レポート。\
  稼働率レポートについて詳しくは、[リソース稼働率レポートの概要](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

* リソースプランナー。

  リソースプランナーでの実際の時間数の表示について詳しくは、[ユーザービューを使用する場合に、リソースプランナーで利用可能、予定、実際の時間数、または FTE を表示](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)を参照してください。

## 時間を記録

複数の方法で、タスク、イシュー、およびプロジェクトに関する時間を記録できます。

Workfront での時間の記録について詳しくは、[時間の記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。
