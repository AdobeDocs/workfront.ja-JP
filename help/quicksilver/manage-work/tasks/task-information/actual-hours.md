---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 実際の時間数の表示
description: Adobe Workfrontで作業項目にログオンした時間は、実際の時間と見なされます。 実際の時間数は、タスク、イシューまたはプロジェクトの完了に要した実際の時間を表します。
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: 055228fd15d670a214039575dc076ab36f6e99eb
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 27%

---

# 実際の時間数の表示

<!-- Audited: 5/2025 -->

Adobe Workfront で作業項目に記録した時間は、実際の時間数とみなされます。

実際の時間数は、タスク、イシューまたはプロジェクトの完了に要した実際の時間を表します。

作業時間は、タスクと問題である作業項目に記録することをお勧めします。 ただし、Workfront管理者は、組織のワークフローに応じて、ユーザーがプロジェクトに時間をログ記録できるようにすることができます。

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
   <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスク、プロジェクト、または問題への表示以上のアクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスク、プロジェクト、イシューに対する表示またはそれ以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
 
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
   <td> <p>View or higher access to Tasks,&nbsp;Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 実際の時間数と従来の実際の時間数

実際の時間にアクセスするWorkfrontの領域に応じて、次のログ時間のいずれかを参照できます。

* プロジェクト、タスク、問題のレポートとリストでは、次の操作を行います。

   * **実際の時間数**: 2021 年 5 月以降、プロジェクト、タスクまたは問題に記録された時間。 これらの変数はWorkfront データベースに時間単位で保存され、その値フィールドは `actualWorkRequiredDouble` です。
   * **従来の実際の時間**:2021 年 5 月より前を含む、任意の時点でプロジェクト、タスク、または問題に記録された時間。 分はWorkfront データベースに分として保存され、その値フィールドは `actualWorkRequired` です。

     >[!IMPORTANT]
     >
     >プロジェクトの実際のコストは、従来の実際の時間数を使用して計算します。

* 「プロジェクト、タスク、問題の詳細」領域で、実際の時間数が次のフィールドに表示される場合があります。

   * **実際の時間**:「詳細」タブには、2021 年 5 月以降、プロジェクト、タスクまたは問題について記録された時間が表示されます。 これらの変数はWorkfront データベースに時間単位で保存され、その値フィールドは `actualWorkRequiredDouble` です。
   * **実際の時間**: プロジェクト、タスクまたは問題のカスタムフォームで、ネイティブフィールドを使用してアクセスされた場合、実際の時間ネイティブフィールドを参照するカスタムフィールドを参照します。 これらは、2021 年 5 月以降のプロジェクト、タスク、または問題についてログに記録された時間です。 これらの変数はWorkfront データベースに時間単位で保存され、その値フィールドは `actualWorkRequiredDouble` です。

>[!NOTE]
>
>可能な限り、「実際の時間数」フィールドを使用することをお勧めします。「従来の実際の時間数」フィールドは、増分の四捨五入によって不正確な時間が表示される可能性があるためです。

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

### 「詳細」セクションの実際の時間数 {#actual-hours-in-the-details-section}

「詳細」セクションの実際の時間数を検索するには、タスク、プロジェクト、イシューの場合と同じ手順を実行します。

タスクの詳細で実際の時間数を検索する手順は、次のとおりです。

1. 実際の時間数を確認するタスクに移動します。
1. 左側のパネルで、「**タスクの詳細**」をクリックします。 **概要** セクションが表示されます。
1. **作業時間** セクションで **実際の時間数** の値を見つけます。 これは、このタスクにログオンした時間の合計です。
1. （オプションおよび条件付き）「実際の時間」ネイティブフィールド参照がプロジェクト、タスクまたはイシューのカスタムフォームに追加された場合、カスタムフォームに移動して、カスタムフィールドの実際の時間を見つけます。 これは、オブジェクトに記録された時間の合計です。

### 「時間」セクションの実際の時間数 {#actual-hours-in-the-hours-section}

「時間」セクションの実際の時間数を検索するには、プロジェクト、タスク、イシューの場合と同じ手順を実行します。

タスクの「時間」セクションで実際の時間を検索するには、次の手順に従います。

1. 実際の時間数を確認するタスクに移動します。

1. 左側のパネルで、「**時間**」をクリックします。 タスクでログに記録された時間エントリのリストが表示され、「**時間**」列にはタスクの実際の時間の合計数が表示されます。

1. **標準**&#x200B;ビューと&#x200B;**プロジェクト**&#x200B;グループ化がこのリストに適用されていることを確認します。
1. タスクの実際の時間は、**実際の時間** 列のグループ化ラインに表示されます。

### レポートの実際の時間数と従来の実際の時間数

タスク、問題、またはプロジェクトの報告書を作成する際、報告書の各タスク、問題、またはプロジェクトの実際の時間数と従来の実際の時間値を表示できます。

実際の時間数と従来の実際の時間数の違いについては、この記事の [&#x200B; 実際の時間数と従来の実際の時間数 &#x200B;](#actual-hours-vs-legacy-actual-hours) の節を参照してください。

タスク・レポートに実績時間数とレガシー実績時間数を表示する手順は、次のとおりです。

{{step1-to-reports}}

1. **レポート** ページで **新規レポート** をクリックし、オブジェクトとして **タスク** を選択します。
1. ページの右下隅にある「**列を追加**」をクリックします。
1. **この列に表示** ドロップダウンフィールドに **実際の時間** と入力し始め、リストに表示されたらフィールドを選択します。
1. 上記の手順を繰り返して、「**従来の実際の時間数**」フィールドをレポートに追加します。

1. ページの左下隅の **保存して閉じる** をクリックして、レポートを保存します。

1. **このレポートに名前を付けて保存** ダイアログボックスで、新しいレポート名を入力し、「**適用**」をクリックします。
1. プロジェクトまたはイシューレポートに対して、同じ手順を繰り返します。

### リソース管理ツールの実際の時間数 {#actual-hours-in-resource-management-tools}

割り当てられたタスクやイシューに対してユーザーが実行している作業の進捗状況を確認する場合は、次のリソース管理ツールでその進捗状況を確認できます。

* 稼働率レポート。\
  詳しくは、[&#x200B; 資源稼働率レポートの概要 &#x200B;](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) を参照してください。

* リソースプランナー

  詳しくは、[&#x200B; ユーザービューの使用時にリソースプランナーで利用可能な時間、予定および実際の時間または FTE を表示 &#x200B;](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md) を参照してください。


### Workfront API の実際の時間数

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

時間を格納するほとんどのWorkfront フィールドは、数分でWorkfront データベースに保存されます。 例えば、タスクの「予定時間数」フィールドの名前はWorkfront データベースに `workRequired` まれ、分単位で保存されます。

API 呼び出し、または計算されたカスタムフィールドや列でこれらのフィールドにアクセスする場合、分から時間への変換を考慮する必要があります。

プロジェクト、タスクまたは問題に記録された実際の時間は、現在、分としてWorkfront データベースに保存されており、その値フィールドは `actualWorkRequired` です。

2025 年末にリリースされる予定の次のバージョンのWorkfront API を使用すると、実際の時間数はデータベースの次のフィールドと単位に保存されます。

* **実際の時間数**: 2021 年 5 月以降、プロジェクト、タスクまたは問題に記録された時間。 これらの変数はWorkfront データベースに時間単位で保存され、その値フィールドは `actualWorkRequiredDouble` です。
* **従来の実際の時間**:2021 年 5 月より前を含む、任意の時点でプロジェクト、タスク、または問題に記録された時間。 分はWorkfront データベースに分として保存され、その値フィールドは `actualWorkRequired` です。

  >[!IMPORTANT]
  >
  >プロジェクトの実際のコストは、従来の実際の時間数を使用して計算します。

  計算された列またはフィールドでの実際の時間数の使用について詳しくは、[&#x200B; レポートに関する FAQ](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) を参照してください。

## 時間を記録

複数の方法で、タスク、イシュー、およびプロジェクトに関する時間を記録できます。

詳しくは、[時間の記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。
