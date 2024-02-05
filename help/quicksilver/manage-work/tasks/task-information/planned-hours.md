---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 予定時間数の概要
description: タスク、イシュー、またはプロジェクトに関連付けられた予定時間数は、割り当てられたユーザーがタスク、イシュー、またはプロジェクトを完了するのに必要な時間を表します。
author: Alina
feature: Work Management
exl-id: 0b86c760-691a-436e-9beb-31e9ac36440a
source-git-commit: 48efc796923079622ce4bc1c2bddb2429915c9a1
workflow-type: tm+mt
source-wordcount: '2815'
ht-degree: 90%

---

# 予定時間数の概要

<!-- Audited: 01/2024 -->

タスク、イシュー、またはプロジェクトに関連付けられた予定時間数は、割り当てられたユーザーがタスク、イシュー、またはプロジェクトを完了するのに必要な時間を表します。

## Adobe Workfront での予定時間数に関する考慮事項

* 予定時間数は、主に Adobe Workfront の作業アイテム（タスクとイシュー）と関連しています。作業アイテムからの予定時間数は、プロジェクトの予定時間数にロールアップされます。
* デフォルトでは、Workfront はタスクまたはイシューの期間内のすべての日にタスクとイシューの予定時間数を均等に配分します。
* ユーザーとロールがタスクとイシューに割り当てられると、タスクとイシューからの予定時間数が、ユーザーまたはロールの割り当てに関連付けられます。
* Workfront のリソース管理ツールを使用する場合は、タスクとイシューに対して予定時間数の値を定義する必要があります。
* 一部の期間タイプに対してのみ、タスクに対する予定時間数の値を変更できます。

  タスクの期間タイプに関するタスクの予定時間数の変更について詳しくは、この記事内の[期間タイプに基づくタスク予定時間数の更新](#update-task-planned-hours-based-on-duration-type)の節を参照してください。

* イシューに関する予定時間数の値は、いつでも変更できます。
* プロジェクトの予定時間数または親タスクの値は、すべてのタスクとサブタスクの全予定時間数の合計になるので、変更できません。
* リソース管理ツールを使用してユーザー割り当てを管理すると、タスク、タスク、問題、プロジェクトの予定時間数、および作業項目に関連付けられた割り当ての時間数が変わる場合があります。

## タスクの予定時間数とプロジェクトの予定時間数 {#planned-hours-on-tasks-vs-planned-hours-on-projects}

タスクの予定時間数から、プロジェクトの予定時間数にロールアップします。案件からの予定時間は、プロジェクトの予定時間には必ずしも含まれません。

このセクションでは、タスクとプロジェクトの予定時間数の違いについて説明します。また、プロジェクトにロールアップされるイシューの予定時間数を表示できる場所も説明します。

### タスクに関する予定時間数 {#planned-hours-on-tasks}

タスクの予定時間数は、タスクの実際の作業にかかる推定時間を示します。デフォルトでは、Workfront は予定時間数の合計をタスク期間内のすべての日に均等に配分します。1 日の予定時間数は、タスクの 1 日の割り当てになります。タスクが複数のリソースに割り当てられている場合、デフォルトでは、各リソースに 1 日の時間数が均等に割り当てられます。

ワークロードバランサーを使用して、タスクに割り当てられたユーザーの 1 日の割り当てを変更できます。これにより、タスクの期間タイプが「シンプル」の場合に、タスクの予定時間数を更新することもできます。詳しくは、[ワークロードバランサーでユーザー割り当てを管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)の記事内の「ユーザー割り当てを管理する際にタスク予定時間数を更新」の節を参照してください。

タスクにサブタスクが含まれる場合、親タスクの予定時間数は、任意のサブタスクに関するすべての予定時間数の合計になります。親タスクの予定時間数は更新できません。

>[!NOTE]
>
>予定時間数とは異なり、親タスクの実際の時間数は、親タスクに直接記録される時間です。子タスクの実際の時間数の合計を表すものではありません。\
>実際の時間数について詳しくは、[実際の時間数を表示](../../../manage-work/tasks/task-information/actual-hours.md)を参照してください。

### プロジェクトに関する予定時間数 {#planned-hours-on-projects}

プロジェクトの予定時間数は編集できません。プロジェクトの予定時間数は、プロジェクトのすべてのタスクから計算されたすべての予定時間数の合計です。

予定時間数の計算にイシューが含まれるかどうかは、予定時間数を表示するプロジェクト内の場所によって異なります。プロジェクト内の次の場所で、プロジェクトの予定時間数を表示できます。

* **「プロジェクト詳細」セクションとプロジェクトを編集ボックス**：プロジェクト上のタスクに関する予定時間数のみが考慮されます。「プロジェクト詳細」セクションまたはプロジェクトを編集ボックスでプロジェクトの予定時間数の合計を表示する場合、プロジェクトのイシューに対する予定時間数は考慮されません。

* **ワークロードバランサー**：ワークロードバランサーに表示されるタスクに関連付けられた予定時間数のみが、プロジェクトのワークロードバランサーに表示されます。ユーザーの 1 日の割り当ては、ワークロードバランサーでプロジェクトの 1 日の予定時間数を変更できます。
* **稼働率セクション**：タスクに割り当てられたユーザーとプロジェクトのイシューに関連する予定時間数は、「稼働率」セクションでプロジェクトの予定時間数の合計を表示する際に考慮されます。
* タスクリストの&#x200B;**ロール配分パネル**：担当業務に割り当てられているプロジェクト内のタスクとイシューの予定時間数、または担当業務に関連付けられているユーザーがこのエリアに表示されます。未割り当て、またはチームに割り当てられているタスクやイシューに関連する予定時間数は、このエリアには表示されません。詳しくは、[役割配分パネルでプロジェクト予定時間数を表示](../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md)を参照してください。

## タスクの期間全体での予定時間の配分

Workfront はデフォルトで、予定時間数をタスクの期間全体に均等に配分し、プロジェクトスケジュールの都合に応じて、タスクの各日に予定時間数を均等に割り当てます。

たとえば、タスクを午後 4 時に開始するように設定し、タスクの初日にスケジュールが 1 時間残っている場合、Workfront はタスク期間の初日に予定時間数を 1 時間配置し、残りの予定時間数をタスクの残りの期間で均等に割り振ります。

>[!NOTE]
>
>1 日あたりの予定時間数や 1 日あたりの配分は、タスクの期間中の 1 日の計画時間の配分です。タスクに割り当てが 1 つある場合、この数は割り当てごとの 1 日あたりの予定時間数を表します。タスクに複数の割り当てがある場合、割り当てごとの 1 日あたりの予定時間数は、タスクの 1 日あたりの予定時間数とは異なります。複数の割り当てを持つタスクの日次予定時間数は、Workfront に表示されません。

## 予定時間数の値を見つけ、理解する

予定時間数の値は、Workfront の様々なエリアで見つけることができます。

表示される計画時間数は、プロジェクト上の作業アイテムに基づくものか、表示するエリアとオブジェクトに応じて、異なる方法で計算されます。

予定時間数は、Workfront の以下のエリアで見つけることができます。

* [プロジェクト、タスクやイシューの「詳細」セクション](#the-details-section-of-a-project-task-or-issue)
* [「タスクを編集」ボックスまたは「問題を編集」ボックス](#the-edit-task-or-edit-issue-box)
* [レポート](#reports)
* [ワークロードバランサー](#the-workload-balancer)
* [リソースプランナー](#the-resource-planner)
* [稼動率レポート](#the-utilization-report)
* [役割割り当てパネル](#the-role-allocation-panel)

### プロジェクト、タスクやイシューの「詳細」セクション {#the-details-section-of-a-project-task-or-issue}

![「詳細に関する予定時間」セクション](assets/planned-hours-on-details-for-project.png)

タスク、問題、またはプロジェクトの [ 詳細 ] セクションの [ 予定時間 ] は、アイテムに関連付けられた合計予定時間です。

プロジェクトの予定時間数について詳しくは、この記事にある[タスクの予定時間数とプロジェクトの予定時間数](#planned-hours-on-tasks-vs-planned-hours-on-projects)の節を参照してください。

### 「タスクを編集」ボックスまたは「イシューを編集」ボックス {#the-edit-task-or-edit-issue-box}

![タスクを編集ボックス](assets/planned-hours-on-edit-task-box-nwe.png)

タスクまたはイシューの「編集」ボックスの予定時間数は、それぞれの項目の予定時間数の合計です。

プロジェクトの予定時間数について詳しくは、この記事にある[タスクの予定時間数とプロジェクトの予定時間数](#planned-hours-on-tasks-vs-planned-hours-on-projects)の節を参照してください。

タスクの場合は、特定の期間タイプに対してのみ計画時間数を編集できます。 詳しくは、 [期間タイプに基づくタスク予定時間の更新](#update-task-planned-hours-based-on-duration-type) 」の節を参照してください。

割り当てエリアで、タスクやイシューに割り当てられた、それぞれのユーザーまたは担当業務に対する計画時間数の個々の配分を表示することができます。

### レポート {#reports}

![レポートの予定時間](assets/planned-hours-on-task-report.png)

プロジェクトレポート、タスクレポート、イシューレポートに、予定時間数フィールドを追加できます。

予定時間数の列は、デフォルトでタスクリストの標準ビューに含まれています。

タスク、イシューやプロジェクトレポートの予定時間数は、それぞれの項目の「詳細」セクションまたは「編集」ボックスに表示されるそれぞれの項目の予定時間数の合計です。

レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

>[!NOTE]
>
>プロジェクト（財務データ）レポートを作成して、日付別にグループ化する場合、予定時間数には、プロジェクトのタスクのタイムラインに応じて、プロジェクトの予定時間数の一部分が表示される場合があります。デフォルトでは、Workfront はタスクの予定時間数をタスク期間内のすべての日に均等に配分します。特定の時間枠の計画時間数は、プロジェクト（財務データ）レポートのその時間枠に対して Workfront によって設定された均等配分と一致します。

<!--
### The Scheduling areas  {#the-scheduling-areas}

![](assets/task-detail-expanded-in-scheduler-with-planned-hours-and-adjusted-daily-allocations-nwe-350x323.png)

The Planned Hours for tasks and issues display in the Scheduling areas in the Planned Hours field.

You can view the daily allocation of Planned Hours for each user assigned to a task or an issue in the Scheduling areas.

The daily hour amount represents one of the following:

* the default amount equally distributed by Workfront for each day of the Duration of the tasks or issues
* the adjusted daily allocation managed by resource managers.

  For information about adjusting daily allocations in the Scheduling tools, see [Manage user allocations in the Scheduling areas](../../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).
-->

### ワークロードバランサー {#the-workload-balancer}

![ワークロードバランサーの予定時間](assets/planned-hours-on-wb-expanded-with-pti-info.png)

タスク、イシュー、プロジェクトの以下の計画時間数は、ワークロードバランサーのタスク名、イシュー名やプロジェクト名の右側に表示されます。

* タスクおよびイシューの場合は、それらに関連する予定時間数が表示されます。
* プロジェクトの場合は、画面に表示されるタスクとイシューの予定時間数の合計が表示されます。

  >[!TIP]
  >
  >ワークロードバランサーでは、プロジェクトの詳細エリアでの表示とは異なり、プロジェクトのすべての予定時間数が表示されるわけではありません。

ワークロードバランサーで、タスクやイシューに割り当てられたそれぞれのユーザーの予定時間数の 1 日の割り当てを表示できます。

予定時間数の 1 日の時間数は、以下のいずれかを表します。

* タスク、イシューやプロジェクトの期間の毎日に Workfront が均等に配分するデフォルトの時間数
* リソースマネージャが管理する調整済みの日次配分

  ワークロードバランサーでの毎日の配分の調整について詳しくは、[ワークロードバランサーでユーザー割り当てを管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

### リソースプランナー {#the-resource-planner}

![リソース・プランナの計画時間](assets/planned-hours-on-all-objects-in-resource-planned-expanded.png)

リソース・プランナは、プロジェクト、タスクおよびタスクの計画時間を表示します。

リソースプランナーの PLN 列で、作業アイテムに関連付けられたユーザーおよび担当業務に対する計画時間数の毎週の割り当てを表示することができます。

>[!TIP]
>
>ワークロードバランサーでの毎日の配分の調整は、リソースプランナーでのタスクとイシューに対する毎週の配分に影響を与えます。

それぞれのオブジェクトの計画時間数の値は、リソースプランナーに適用するビューに応じて異なります。詳しくは、[リソースプランナーのプロジェクトビューと役割ビューでの時間数、FTE、コスト情報の概要](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)を参照してください。

タスクやイシューの予定時間数の週次の時間数は、次のいずれかを表します。

* Workfront によってタスクやイシューの期間の各日付に均等に配分された、デフォルトの週次の数
* ワークロード・バランサのリソース・マネージャが管理する調整済の週次配分

  ワークロードバランサーでの毎日の配分の調整について詳しくは、[ワークロードバランサーでユーザー割り当てを管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

プロジェクト、ユーザー、役割の週次の数は、関連付けられたタスクやイシューの予定時間数の週次の時間数による影響を受けます。

### 稼働率レポート {#the-utilization-report}

プロジェクトの予定時間数は、各タスクや各イシューの割り当てに関連付けられた時間です。

>[!IMPORTANT]
>
>稼働率レポートの予定時間数は、割り当てに関連付けられており、タスクやイシュー自体には関連付けられていないことに注意してください。稼働率レポートの予定時間数は、プロジェクトのタスクやイシューの予定時間数と必ずしも一致しません。ただし、予定時間数は、タスクやイシューの割り当てに関連付けられた時間と一致します。

稼働率レポートでは、次のタイプの予定時間数を確認できます。

* 含まれるプロジェクトの全期間にわたる、プロジェクトのすべての割り当ての予定時間数の合計
* 指定した日付範囲のみにおける、すべての割り当ての予定時間数の合計（個別の週または月を指定可能）。

  ワークロードバランサーを使用してユーザーの日次の配分を調整している場合、稼働率レポートで選択した日付にタスクの期間またはイシューの期間が一部しか含まれていないと、特定の日付範囲の予定時間数に影響することがあります。ユーザーの日次の配分の調整について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

詳しくは、[リソース稼働率情報の表示](../../../resource-mgmt/resource-utilization/view-utilization-information.md)を参照してください。

### 役割割り当てパネル

役割の配分パネルの予定時間数は、プロジェクトの全期間における、プロジェクトのタスクやイシューの各担当業務に割り当てられた予定時間数を表します。この数は、リソースプランナーの役割の予定時間数と一致します。

>[!TIP]
>
ユーザーに関連付けられた予定時間数は、役割の配分パネルには表示されないことに注意してください。

詳しくは、[ワークロードバランサーのプロジェクトとイニシアチブの役割の配分を表示](../../../scenario-planner/show-role-allocation-workload-balancer.md)を参照してください。

## 期間タイプに基づいてタスクの予定時間数を更新 {#update-task-planned-hours-based-on-duration-type}

タスクの特定の期間タイプである場合に限り、タスクの編集時にタスクの予定時間数の合計を更新できます。

次のシナリオが存在します。

* タスクの予定時間数は、タスクの編集時に期間タイプで「予定割り当て時間」または「シンプル」を使用した場合にのみ変更できます。

  予定割り当て時間期間タイプについて詳しくは、[期間タイプの概要：予定割り当て時間](../../../manage-work/tasks/taskdurtn/calculated-assignment.md)を参照してください。

  シンプル期間タイプについて詳しくは、[期間タイプの概要：シンプル](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)を参照してください。

* タスクへのユーザーの配分を管理する際に、ワークロードバランサーでタスクの予定時間数を更新できるのは、シンプル期間タイプのタスクに対してのみとなります。ワークロードバランサーでのユーザーの配分の管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。
* 期間タイプが「残存作業時間の優先」または「予定作業」のタスクに対しては、予定時間数を変更できません。この場合、Workfrontはタスクの期間に基づいて計画時間を決定します。ただし、この場合、計画時間は常に期間（時間）と等しく、割り当てられたリソースの割合配分の影響を受けません。

  残存作業時間の優先期間タイプの詳細は、[期間タイプの概要：残存作業時間の優先](../../../manage-work/tasks/taskdurtn/effort-driven.md)を参照してください。

  予定作業期間タイプについて詳しくは、[期間タイプの概要：予定作業](../../../manage-work/tasks/taskdurtn/calculated-work.md)を参照してください。

## ユーザーの配分の管理時にタスクの予定時間数を更新

タスクへのユーザーまたは担当業務の配分を手動で更新する際に、タスクの予定時間数を更新できます。これは、タスクの期間タイプがシンプルの場合にのみ可能です。

詳しくは、[期間タイプの概要：シンプル](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)を参照してください。

ワークロードバランサーを使用する際に、タスクに割り当てられたユーザーや担当業務の配分全体、またはユーザーの日次の配分のいずれかを更新できます。

タスクの全体的なユーザーおよび担当業務の配分の管理について詳しくは、[タスクに対するユーザーと役割の時間配分を管理](../../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md)を参照してください。

タスクの日次の配分の管理について詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

タスクのユーザーまたは担当業務の配分を手動で更新する際は、次のシナリオが存在します。

* タスクの予定時間数に対する変更をトリガーするために個々のユーザーまたは役割の配分を手動で更新していない場合、タスクの割り当てを追加、削除、置換する際に、予定時間数は変更されません。タスクに新しい割り当てを追加すると、個々の配分がすべての担当者間で再配分されます。
* タスクの予定時間数に対する変更をトリガーするために配分を手動で更新している場合、タスクから割り当てを削除すると、予定時間数は減少します。割り当てを置き換える場合、予定時間数は変更されません。
* タスクの予定時間数に対する変更をトリガーするために配分を手動で更新しており、タスクに割り当てを追加する場合、新しい割り当てにはデフォルトで 0 時間が配分されます。タスクに対する配分を手動で更新する必要があります。これは、予定時間に影響を与える可能性があります。
* タスクの予定時間数に対する変更をトリガーするために配分を手動で更新しておらず、タスクに対するすべての割り当てを削除した場合、予定時間数は変更されません。
* タスクの予定時間数に対する変更をトリガーするために配分を手動で更新しておらず、タスクに対するすべての割り当てを削除した場合、予定時間数も削除され、タスクの予定時間数は 0 になります。

>[!NOTE]
>
例えば、タスクに 10 時間の計画時間があり、2 人の担当者がある場合、デフォルトでは各割り当て時間は 5 時間になります。
>
* ワークロードバランサーを使用して個々のユーザーへの配分や毎日の配分をアップデートせず、タスクから担当者の一部または全部を削除した場合、タスクの予定時間数は 10 時間のままです。
* 割り当ての分配をそれぞれ 4 時間から 6 時間に手動で変更し、6 時間が割り当てられたユーザーとその担当業務を削除すると、タスクの予定時間数は 4 時間にアップデートされます。4 時間が割り当てられているユーザーも削除し、しかし削除したユーザーに関連付けられた担当業務は維持する場合、タスクの予定時間数は 4 時間のままです。4 時間に割り当てられた最後のユーザーと、そのジョブの役割が未割り当てのままの場合、タスク「計画時間」は 0 になります。

## 作業量を使用してタスクの予定時間数を自動的に更新

作業量を使用してタスクの完了に必要な作業量を見積もると、タスクの予定時間数が自動的にアップデートされます。これは、単純期間タイプのタスクに対してのみ可能です。

作業量を使用してタスク量を見積もる方法について詳しくは、[作業量の概要](../../../manage-work/tasks/task-information/work-effort.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this issue has the explanation of how Planned Hours should work - from Vazgen and Anna: https://hub.workfront.com/issue/6217dced00730b7034c4b808339a35ce/</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Details of their comments: </p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Anna Asatryan</p>
<p>3/22/2022 At 3:16 PM</p>
<p>&nbsp;</p>
<p>to Mark Paul, Corrie Butler, Arman Simonyan, Gagik Khalatyan, Alina Wilson, Artur Sargsyan, Vazgen Babayan, Anna Asatryan</p>
<p>I have done some rough calculations on what the planned hours/revenues should look like Book.xlsx . And if we look, for example at the 2 users highlighted in one of the screenshots their planned hours look way off from what the calculation looks like in the spreadsheet (i.e. equally distributed allocation). When looking at the Workload balancer (the second screenshot), as an example for the user Yashas Mitta, I can see that the allocation has been modified. Obviously the utilization report calculates the allocations based on the modified contouring using the new work per day calculation. The project financial report uses the old, equal distribution of allocation along the full duration of the task. Hence. there is a difference when grouping per periods.</p>
<p>Vazgen Babayan</p>
<p>I believe we will need to prioritise syncing the project financial data report with the new work per day.</p>
<p>Alina Wilson</p>
<p>@Anna Asatryan , do you have a definition of what we should say in documentation (glossary, for example) for how the Planned Hours (or Planned Revenue) is calculated, keeping in mind that we don't document the concept of "workPerDay". We call them "daily allocations", for example, but let me know if that's accurate, too.</p>
<p>Vazgen Babayan</p>
<p>Last Thursday at 3:13 PM</p>
<p>I think an important note here is that regardless the calculation, even if the both views used the same formula, they will not display the same data, because the underlying data sources are different. The Financial Data report does not respect user-entered allocations in Workload Balancer at this moment. So there will be a clear discrepancy, as Anna showed in her message. My recommendation for communication will be to explain that the data sources are different so there can be a mismatch in data and that we will look into addressing that on our roadmap.</p>
<p>Alina Wilson</p>
<p>So far, I hear you guys say this (with my questions for confirmation/ comments in bold):</p>
<p>- the utilization report calculates the allocations based on the modified contouring using the new work per day calculation (so this is what we see in the Workload Balancer, right?)</p>
<p>- the project financial report uses the old, equal distribution of allocation along the full duration of the task (this is before the daily allocations for example were modified in the WB, right?)</p>
<p>I have these additional questions:</p>
<p>- what does the Project Details show? Which Planned Hours, for instance - because earlier, we had a question about this also. - which numbers?</p>
<p>- what does any Planned Hours/ Planned Revenue field that can be pulled in any other report (outside of Financial Data and Utilization reports) show? - which numbers?</p>
<p>- are there any other areas I am not thinking of that we need to document, @Corrie Butler</p>
<p>I will try to document all the possible areas where these display but please help. Thanks!</p>
<p>Vazgen Babayan</p>
<p>Last Saturday at 3:41 PM</p>
<ul>
<li> <p>Confirming the first two points </p> </li>
</ul>
<p>For the following questions</p>
<ul>
<li> <p>Project details show an aggregated sum of task planned hours. It doesn't have anything to do with the work per day because it always deals with total numbers for the whole duration of the Project/Task.</p> </li>
<li> <p>Same thing applies to the Planned Hours and Planned Revenue fields in reports - they show totals for the whole Project/Task duration and thus have no use of work per day.</p> </li>
<li> <p>Can't think of any other fields related to this right now.</p> </li>
<li> <p>In general, if I were to summarize the system behavior, it's as follows:</p> </li>
<li> <p>Every area that only deals with total numbers of Planned Hours / Planned Revenue, uses the numbers entered on the tasks. Those are Task / Project Details, reports exposing those fields.</p> </li>
<li> <p>Areas that deal with time-sensitive portions of Planned Hours / Planned Revenue, use work per day. Those are all Resource Management tools - Workload Balancer, Resource Planner, Utilization Report, importing projects via Scenario Planner.</p> </li>
<li> <p>All the areas in the second point support user-edited allocations made in Workload Balancer.</p> </li>
<li> <p>Scheduling area and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from Workload Balancer.</p> </li>
<li> <p>Scheduling will be removed this year, and we need to do work to move the Project Financial Data reports to the new work per day sometime after Q3.</p> </li>
</ul>
<p>Alina Wilson</p>
<p>@Vazgen Babayan , one clarifying question: when you say "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" - you mean that those use the system default which spreads the allocations evenly, correct? Because you can edit (daily) allocations in Scheduling tools, but it doesn't use that, correct? It uses the default of the daily allocation that the system figures out when dividing the Planned Hours by the number of days in the Duration. Please let me know. And thanks!</p>
<p>Anna Asatryan</p>
<p>Yesterday at 11:42 AM</p>
<p>@Alina Wilson , that's correct, when saying "Scheduling and Project Financial Data reports use the old version of the work per day, which doesn't respect user-edited allocations from WB" Vazgen meant that it spreads the allocation evenly.</p>
<p>As for the scheduling, the allocation modification that's being done there isn't reflected anywhere else in the application other than in the Scheduling itself. That's probably one of the reasons it's being deprecated.</p>
</div>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <br> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: everything below is drafted because I replaced it with the table above)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can find the Planned Hours information on tasks, issues, or projects in the following locations:</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours in the Details  section  of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours in the Details  section  is identical for tasks, issues, and projects. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the Planned Hours value on the Details  section  of a task: </p>
<ol>
<li value="1">Go to a task for which you want to review the Planned Hours.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Overview</strong> area and notice the Planned Hours value.</p> <p>This value represents the time it would take the user assigned to the task to complete it. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3> </h3>
<p>The Planned Hours in the Edit box of a task, issue, or project are the total Planned Hours of the respective item. </p>
<p>Finding the Planned Hours while editing a task or an issue is identical. </p> <note type="tip">
You cannot edit the Planned Hours of projects manually, as they are a calculation of all Planned Hours of all the tasks on the project.
</note>
<p>To locate the value of Planned Hours while editing a task:</p>
<ol>
<li value="1">Go to the task or issue you want to view Planned Hours for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png"> next to the task name, then click <strong>Edit</strong>.</p> <p>The Planned Hours are located in the <strong>Overview</strong> section. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The Planned Hours column is included in the Standard view of a task list, by default. For issues and projects, you can add it to the view, when you are editing the view or when you build a report. </p>
<p>The Planned Hours in a task, issue, or project report are the total Planned Hours of the respective item as they display in the Details  section  or the Edit box of the items. </p>
<p>Adding the Planned Hours column to a project view is similar to building a view in a project report. </p>
<p>To show Planned Hours in a project report:</p>
<ol>
<li value="1"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Workfront, then click <strong>Reports</strong>. </p> </li>
<li value="2">Click <strong>New Report</strong>, then choose <strong>Project</strong> as your object.</li>
<li value="3">Click <strong>Add Column</strong>, and start typing <strong>Planned Hours</strong> when the <strong>Show in this column</strong> drop-down field is displayed. Select the field when it appears in the list.</li>
<li value="4"> <p>Click <strong>Save + Close</strong> to save the report. </p> <p>The Planned Hours column shows the total number of Planned Hours on each project. </p> </li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Planned Hours in Resource Management tools</p> <note type="important">
When viewing Planned Hours in the Resource Management tools by a specific time frame, the daily allocations for each work item and the daily allocations for the resources assigned to the work items during that time frame can influence the daily Planned Hours of projects or work items.
</note>
<p>You can see the value of Planned Hours for your tasks, issues, or projects when using the following Resource Management tools:</p>
<ul>
<li> <p>Resource Planner</p> <p>For information about using the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p> </li>
<li> <p>Utilization Report.</p> <p>For information about the utilization report, see <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">Overview of the Resource Utilization report</a>.</p> </li>
<li>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Workload Balancer or Scheduling areas in the following sections:</p>
<ul>
<li>Scheduling or Workload Balancer sections in the Resourcing area</li>
<li>Scheduling or Workload Balancer section at the project level</li>
<li>Schedule or Workload Balancer section at the team level</li>
</ul>
</div> <p>For information about scheduling resources, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p> <p>For information about the Workload Balancer, see <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Workload Balancer overview</a>. </p> </li>
<li> <p><b>Role Allocation panel</b> in the project  task list or  Workload Balancer: The Planned Hours for the tasks and the issues on the project that are assigned to a job role or a user associated with a job role are taken into account in this area. For more information, see <a href="../../../manage-work/projects/planning-a-project/view-planed-hours-in-role-allocation-panel.md" class="MCXref xref">View project Planned Hours in the Role Allocation panel</a>. </p> </li>
</ul>
</div>
-->
