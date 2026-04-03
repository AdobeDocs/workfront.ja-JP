---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 実際の時間数の表示
description: Adobe Workfrontで作業項目にログインした時間は、実際の時間と見なされます。 実際の時間数は、タスク、イシューまたはプロジェクトの完了に要した実際の時間を表します。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 27%

---

# 実際の時間数の表示

<!-- Audited: 5/2025 -->

Adobe Workfront で作業項目に記録した時間は、実際の時間数とみなされます。

実際の時間数は、タスク、イシューまたはプロジェクトの完了に要した実際の時間を表します。

タスクや問題である作業項目に時間を記録することをお勧めします。 ただし、Workfront管理者は、組織のワークフローに応じて、ユーザーにプロジェクトの作業時間を記録させることもできます。

ユーザーが時間をプロジェクトに記録できるようにシステムを設定する方法について詳しくは、[タイムシートの設定と時間環境設定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>標準<p>
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスク、プロジェクト、またはイシューへのアクセス権を表示または上位に表示する</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスク、プロジェクト、イシューに対する表示またはそれ以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
 Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks, Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## 実際の時間数と従来の実際の時間数の比較

Workfrontのどのエリアから実際の時間にアクセスするかに応じて、次のログ時間のいずれかを参照できます。

* プロジェクト、タスク、イシューのレポートとリストで次の操作を行います。

   * **実際の時間数**:2021年5月から今日までの間に、プロジェクト、タスク、または問題に対して記録された時間。 これらはWorkfront データベースに時間で保存され、値フィールドは`actualWorkRequiredDouble`です。
   * **従来の実際の時間数**: 2021年5月より前の任意の日付から今日までの間に、プロジェクト、タスク、または問題に対して記録された時間数。 これらはWorkfront データベースに分として保存され、その値フィールドは`actualWorkRequired`です。

     現在ログに記録されている時間は、実際の時間と従来の実際の時間の両方を更新します。

     >[!IMPORTANT]
     >
     >プロジェクトの実際のコストでは、従来の実際の時間数を使用して計算します。

* 「プロジェクト」、「タスク」または「イシューの詳細」エリアでは、実際の時間を次のフィールドに表示できます。

   * **実際の時間数**:「詳細」タブでは、2021年5月から今日までの間に、プロジェクト、タスク、または問題に関して記録された時間です。 これらはWorkfront データベースに時間で保存され、値フィールドは`actualWorkRequiredDouble`です。
   * **実際の時間数**: プロジェクト、タスク、またはイシューのカスタムフォームで、実際の時間数ネイティブフィールドを参照するネイティブフィールド参照カスタムフィールドを使用してアクセスされる場合。 これは、2021年5月より前の任意の日付から今日までのプロジェクト、タスク、またはイシューのログ時間です。 これらはWorkfront データベースに時間で保存され、値フィールドは`actualWorkRequiredDouble`です。

     現在ログに記録されている時間は、実際の時間と従来の実際の時間の両方を更新します。

>[!NOTE]
>
>可能な限り、「実際の時間数」フィールドを使用することをお勧めします。これは、時間を分単位で保存する場合に増分が丸められるため、「従来の実際の時間数」フィールドに不正確な時間が表示される可能性があるためです。

## タスクとイシューの実際の時間数とプロジェクトの実際の時間数

タスクとイシューの実際の時間数は、タスクとイシューに直接記録した時間数を表します。

子タスクの実際の時間数は、親タスクの実際の時間数にロールアップされます。親タスクの実際の時間数の計算には、次の式が適用されます。

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

プロジェクトの実際の時間数は、プロジェクトのすべてのタスク（親タスクに直接ログ記録された時間を含む）、プロジェクトのすべてのイシュー、およびプロジェクト自体にログ記録された実際の時間数の合計を表します。

プロジェクトの実際の時間数には、次の式が適用されます。

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## 実際の時間数の検索

項目の実際の時間数の値を検索するには、タスク、プロジェクト、イシューの場合と同じ手順を実行します。

### 「詳細」セクションの実際の時間数 {#actual-hours-in-the-details-section}

「詳細」セクションの実際の時間数を検索するには、タスク、プロジェクト、イシューの場合と同じ手順を実行します。

タスクの詳細で実際の時間数を検索する手順は、次のとおりです。

1. 実際の時間数を確認するタスクに移動します。
1. 左側のパネルで、**タスクの詳細**&#x200B;をクリックします。 **概要** セクションが表示されます。
1. 「**作業時間**」セクションで「**実際の時間**」の値を探します。 これは、このタスクにログオンした時間の合計です。
1. （オプションおよび条件付き）実際の時間数のネイティブフィールド参照がプロジェクト、タスク、またはイシューのカスタムフォームに追加された場合は、カスタムフォームに移動し、カスタムフィールドで実際の時間数を見つけます。 これは、オブジェクトに対して記録された合計時間です。

### 「時間」セクションの実際の時間数 {#actual-hours-in-the-hours-section}

「時間」セクションの実際の時間数を検索するには、プロジェクト、タスク、イシューの場合と同じ手順を実行します。

タスクの「時間」セクションで実際の時間を検索するには、次の手順を実行します。

1. 実際の時間数を確認するタスクに移動します。

1. 左側のパネルで、**時間**&#x200B;をクリックします。 タスクに記録された時間エントリのリストが表示され、**時間**&#x200B;列には、タスクの実際の時間数の合計数が表示されます。

1. **標準**&#x200B;ビューと&#x200B;**プロジェクト**&#x200B;グループ化がこのリストに適用されていることを確認します。
1. タスクの実際の時間数は、**実際の時間数**&#x200B;列のグループ化ラインに表示されます。

### レポートの実際の時間と過去の実際の時間

タスク、イシュー、またはプロジェクトのレポートを作成する際に、レポート内の各タスク、イシュー、またはプロジェクトの実際の時間と従来の実際の時間の値を表示できます。

実際の時間と従来の実際の時間の違いについて詳しくは、この記事の「[実際の時間と従来の実際の時間](#actual-hours-vs-legacy-actual-hours)」の節を参照してください。

タスクレポートで実際の時間数と以前の実際の時間数を表示するには：

{{step1-to-reports}}

1. **レポート** ページで、**新規レポート**&#x200B;をクリックし、**タスク**&#x200B;をオブジェクトとして選択します。
1. ページの右下隅にある「**列を追加**」をクリックします。
1. **この列に表示** ドロップダウンフィールドで、**実際の時間**&#x200B;と入力し始め、リストに表示されるフィールドを選択します。
1. 上記の手順を繰り返して、**従来の実際の時間** フィールドをレポートに追加します。

1. ページの左下隅にある「**保存+閉じる**」をクリックして、レポートを保存します。

1. 「**このレポートに名前を付けて保存**」ダイアログボックスで、新しいレポート名を入力し、**適用**&#x200B;をクリックします。
1. プロジェクトまたはイシューレポートに対して同じ手順を繰り返します。

### リソース管理ツールの実際の時間数 {#actual-hours-in-resource-management-tools}

割り当てられたタスクやイシューに対してユーザーが実行している作業の進捗状況を確認する場合は、次のリソース管理ツールでその進捗状況を確認できます。

* 稼働率レポート：\
  詳しくは、「[ リソース稼働率レポートの概要](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)」を参照してください。

* リソースプランナー：

  詳しくは、「[ ユーザービューの使用時にリソースプランナーで利用可能、計画、および実際の時間またはFTEを表示する](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md)」を参照してください。


### Workfront APIの実際の時間数

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

時間を格納するほとんどのWorkfront フィールドは、Workfront データベースに数分で保存されます。 例えば、タスクの「予定時間数」フィールドの名前はWorkfront データベースの`workRequired`で、分単位で保存されます。

API呼び出しまたは計算されたカスタムフィールドまたは列でこれらのフィールドにアクセスする場合、コンバージョンを分から時間まで考慮する必要があります。

プロジェクト、タスク、または問題について記録された実際の時間数は、現在、Workfront データベースに分として保存され、その値フィールドは`actualWorkRequired`です。

2025年10月から、API バージョン 21では、実際の時間は、データベースの次のフィールドと単位に保存されます。

<!--above used to be this: With the following version of the Workfront API scheduled to release later in 2025, Actual Hours are stored in the following fields and units in the database: -->

* **実際の時間数**:2021年5月以降のプロジェクト、タスク、または問題のログに記録された時間。 これらはWorkfront データベースに時間で保存され、値フィールドは`actualWorkRequiredDouble`です。
* **従来の実際の時間数**:2021年5月以前を含め、いつでもプロジェクト、タスク、または問題のログに記録される時間数。 これらはWorkfront データベースに分として保存され、その値フィールドは`actualWorkRequired`です。

API バージョンについて詳しくは、[API バージョン管理とサポートスケジュール ](/help/quicksilver/wf-api/api/api-version-support-schedule.md)を参照してください。

>[!IMPORTANT]
>
>プロジェクトの実際のコストでは、従来の実際の時間数を使用して計算します。

計算列またはフィールドで実際の時間を使用する方法について詳しくは、[FAQのレポート ](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md)を参照してください。

## 時間を記録

複数の方法で、タスク、イシュー、およびプロジェクトに関する時間を記録できます。

詳しくは、[時間の記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。
