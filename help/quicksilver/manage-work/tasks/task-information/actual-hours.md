---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 実際の時間の表示
description: Adobe Workfrontで作業項目にログオンする時間は、「実際の時間」と見なされます。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 実際の時間の表示

Adobe Workfrontで作業項目にログオンする時間は、「実際の時間」と見なされます。

[ 実績時間 ] は、タスク、懸案事項、またはプロジェクトの完了に要した実績時間を表します。

時間は、タスクと問題を含む作業項目にログオンすることをお勧めします。

ただし、Workfront管理者は、組織内のワークフローに応じて、ユーザーがプロジェクトに時間をログオンできるようにすることができます。

ユーザーがプロジェクトに時間を記録できるようにシステムを設定する方法について詳しくは、 [タイムシートと時間の基本設定を構成する](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td> <p>タスク、プロジェクト、または問題へのアクセス権を表示または高くする</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスク、プロジェクトまたはイシューに対する権限を表示または上限に設定する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトの実際の時間に対するタスクと問題の実際の時間

タスクと問題に関する実際の時間数は、タスクと問題に直接記録される時間数を表します。

>[!NOTE]
>
>[ 子タスクからの実績時間 ] は、親タスクの実績時間にまで積み上げられます。 次の式は、親タスクの実績時間に適用されます。

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

[ プロジェクトの実績時間 ] は、プロジェクト上のすべてのタスク（親タスクに直接ログオンした時間を含む）、プロジェクト上のすべての問題、およびプロジェクト自体にログオンした実績時間の合計を表します。

次の式は、プロジェクトの実績時間に適用されます。

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 実際の時間を検索

ある品目の実績時間の値の検索は、タスク、プロジェクトおよび問題で同じです。

タスクに関する実際の時間情報は、次の場所にあります。

* [「詳細」セクションの実際の時間](#actual-hours-in-the-details-section)
* [「時間」セクションの実際の時間](#actual-hours-in-the-hours-section)
* [レポートの実際の時間](#actual-hours-in-reports)
* [リソース管理ツールの実績時間](#actual-hours-in-resource-management-tools)

### 「詳細」セクションの実際の時間 {#actual-hours-in-the-details-section}

「詳細」セクションの実際の時間の検索は、プロジェクト、タスクおよび問題の場合と同じです。

「タスク詳細」で実績時間を検索する手順は、次のとおりです。

1. 実績時間を確認するタスクに移動します。
1. クリック **タスクの詳細** をクリックします。
1. クリック **概要** そして気がつきましょう **実際の時間** の値です。

   このタスクにログオンした合計時間です。

### 「時間」セクションの実際の時間 {#actual-hours-in-the-hours-section}

「時間」セクションの実際の時間の検索は、プロジェクト、タスクおよび問題の場合と同じです。

「 Actual Hours in Hours 」セクションを検索するには：

1. 実績時間を確認するタスクに移動します。
1. クリック **時間** をクリックします。

   設定に応じて、「時間」セクションが「 **さらに表示**.

   タスクに記録された時間エントリのリストが表示されます。

1. 次を確認します。 **標準** 表示と **プロジェクト** グループ化がこのリストに適用されます。

   グループ化行に表示される **時間** 列は、タスクの実績時間の合計数です。

### レポートの実際の時間 {#actual-hours-in-reports}

タスク、タスク、またはプロジェクトのレポートを作成する際に、レポート内の各タスク、タスク、またはプロジェクトの [ 実績時間 ] の値を表示できます。

[ 実績時間 ] 列をタスクビューに追加する操作は、レポートのビューの作成と似ています。

タスク・レポートに実績時間を表示する手順は、次のとおりです。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Workfrontの右上隅で、 **レポート**.
1. クリック **新しいレポート**&#x200B;を選択して、 **タスク** を選択します。

1. クリック **列を追加**&#x200B;入力を開始 **実際の時間** ( **この列に表示** ドロップダウンフィールドが表示されます。 リストに表示されるフィールドを選択します。

1. クリック **保存して閉じる** をクリックしてレポートを保存します。

   「Actual Hours」列には、各タスクで記録された時間数が表示されます。

### リソース管理ツールの実績時間 {#actual-hours-in-resource-management-tools}

割り当てられたタスクやタスクに対してユーザーが実行している作業の進捗状況を確認する場合は、次のリソース管理ツールでその進捗状況を確認できます。

* 使用率レポート。\
   使用率レポートについて詳しくは、 [リソース使用率レポートの概要](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* リソースプランナ.

   リソース・プランナでの実績時間の表示の詳細は、次を参照してください： [ユーザー・ビューを使用する場合は、リソース・プランナで「使用可能」、「計画済」、「実績時間」または「工数」を表示します](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## ログ時間

タスク、問題、プロジェクトに関する時間は、複数の方法で記録できます。

Workfrontでのログ時間について詳しくは、 [ログ時間](../../../timesheets/create-and-manage-timesheets/log-time.md).
