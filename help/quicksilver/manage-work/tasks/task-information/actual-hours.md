---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 実際の時間数の表示
description: Adobe Workfront で作業項目に記録した時間は、実際の時間数とみなされます。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 63%

---

# 実際の時間数の表示

<!-- Audited: 5/2025 -->

Adobe Workfront で作業項目に記録した時間は、実際の時間数とみなされます。

実際の時間数は、タスク、イシューまたはプロジェクトの完了に要した実際の時間を表します。

作業時間は、タスクと問題である作業項目に記録することをお勧めします。 ただし、Workfront管理者は、組織のワークフローに応じて、ユーザーがプロジェクトに時間をログ記録できるようにすることができます。

ユーザーが時間をプロジェクトに記録できるようにシステムを設定する方法について詳しくは、[タイムシートの設定と時間環境設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>新規：標準<p>
   <p>または</p>
   <p>現在：ワーク以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスク、プロジェクト、イシューに対する表示またはそれ以上のアクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスク、プロジェクト、イシューに対する表示またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タスクとイシューの実際の時間数とプロジェクトの実際の時間数

タスクとイシューの実際の時間数は、タスクとイシューに直接記録した時間数を表します。

子タスクの実際の時間数は、親タスクの実際の時間数にロールアップされます。親タスクの実際の時間数の計算には、次の式が適用されます。

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

プロジェクトの実際の時間数は、すべてのプロジェクトのタスク （親タスクに直接ログ記録された時間を含む）、すべてのプロジェクトの問題、およびプロジェクト自体にログ記録された実際の時間の合計を表します。

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

1. 実際の時間数を確認するタスクに移動します。
1. 左側のパネルで、「**タスクの詳細**」をクリックします。 **概要** セクションが表示されます。
1. **作業時間** セクションで **実際の時間数** の値を見つけます。 これは、このタスクにログオンした時間の合計です。

### 「時間」セクションの実際の時間数 {#actual-hours-in-the-hours-section}

「時間」セクションの実際の時間数を検索するには、プロジェクト、タスク、イシューの場合と同じ手順を実行します。

「実際の時間数（時間）」セクションを検索する手順は、次のとおりです。

1. 実際の時間数を確認するタスクに移動します。

1. 左側のパネルで、「**時間**」をクリックします。 タスクでログに記録された時間エントリのリストが表示され、「**時間**」列にはタスクの実際の時間の合計数が表示されます。

1. **標準**&#x200B;ビューと&#x200B;**プロジェクト**&#x200B;グループ化がこのリストに適用されていることを確認します。

### レポートの実際の時間数 {#actual-hours-in-reports}

タスク、イシュー、またはプロジェクトのレポートを作成する際に、レポート内の各タスク、イシュー、またはプロジェクトの実際の時間数を表示できます。

タスクレポートに実際の時間数を表示する手順は、次のとおりです。

{{step1-to-reports}}

1. **レポート** ページで **新規レポート** をクリックし、オブジェクトとして **タスク** を選択します。
1. ページの右下隅にある「**列を追加**」をクリックします。
1. 表示される **この列に表示** ドロップダウンフィールドで「**実際の時間数** を入力し始め、リストに表示されたらフィールドを選択します。

1. ページの左下隅の **保存して閉じる** をクリックして、レポートを保存します。

1. **このレポートに名前を付けて保存** ダイアログボックスで、新しいレポート名を入力し、「**適用**」をクリックします。

### リソース管理ツールの実際の時間数 {#actual-hours-in-resource-management-tools}

割り当てられたタスクやイシューに対してユーザーが実行している作業の進捗状況を確認する場合は、次のリソース管理ツールでその進捗状況を確認できます。

* 稼働率レポート。\
  詳しくは、[ 資源稼働率レポートの概要 ](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) を参照してください。

* リソースプランナー

  詳しくは、[ ユーザービューの使用時にリソースプランナーで利用可能な時間、予定および実際の時間または FTE を表示 ](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md) を参照してください。

## 時間を記録

複数の方法で、タスク、イシュー、およびプロジェクトに関する時間を記録できます。

詳しくは、[時間の記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。
