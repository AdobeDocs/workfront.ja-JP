---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクの割り当て変更の概要
description: ユーザー、チームまたはジョブの役割にタスクを割り当てたり、タスクの割り当てを解除したりできます。 複数のリソースを同時に割り当てることも、1 つのリソースのみを割り当てることもできます。 一度に 1 つのタスクを割り当てることも、複数のタスクを一括して割り当てることもできます。
author: Alina
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: f4cc5ae89c8746ec4c40ece88bfdb21dc1996575
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# タスクの割り当て変更の概要

ユーザー、チームまたはジョブの役割にタスクを割り当てたり、タスクの割り当てを解除したりできます。 複数のリソースを同時に割り当てることも、1 つのリソースのみを割り当てることもできます。 一度に 1 つのタスクを割り当てることも、複数のタスクを一括して割り当てることもできます。

>[!TIP]
>
>複数のユーザー、ジョブの役割またはチームを割り当てることができます。 アクティブなユーザー、ジョブの役割およびチームのみを割り当てることができます。
>
>非アクティブ化前にユーザー、ジョブの役割、またはチームが割り当てられた場合、そのユーザーは作業項目に割り当てられたままになります。 この場合、次の操作をお勧めします。
>
>* 作業項目をアクティブなリソースに再割り当てする。
>* 非アクティブなチームのユーザをアクティブなチームに関連付け、作業項目をアクティブなチームに再割り当てします。
>


この記事では、タスクの割り当てを変更した場合の影響に関する一般的な情報を説明します。 タスクの割り当て方法について詳しくは、次の記事を参照してください。

* タスクの割り当てについて詳しくは、 [タスクを割り当て](../../../manage-work/tasks/assign-tasks/assign-tasks.md) および [タスクリスト内の複数のユーザー割り当てを変更する](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

* 「スケジューリング」領域の複数のタスクに対する割り当ての変更の詳細は、「スケジューリング領域のタスクに対する複数のユーザー割り当ての変更」を参照してください。
* ワークロード・バランサを使用したタスクの割り当ての詳細は、 [ワークロードバランサーでの作業割り当ての概要](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

この記事の一部の情報は、問題への割り当てにも適用されます。 問題の割り当てとその他の考慮事項について詳しくは、 [問題の割り当ての変更の概要](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

## タスクのユーザー割り当てを変更するタイミング

次のような様々な理由で、タスクのユーザー割り当てを変更する場合があります。

* ユーザーがチームに参加する、またはチームから脱退する
* ユーザーがタスクの期限を超える休暇を取る

   >[!NOTE]
   >
   >ユーザーを作業に割り当てる場合、スケジュールに従って使用できるのは、タスクの予定日と予定日に影響します。 スケジュールについて詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* 特定の役割またはユーザーが複数のタスクの担当者に設定され、別のユーザーまたは役割に割り当てられるすべての項目をすばやく変更する

## 役割、チーム、ユーザーに対する複数の割り当てに関する考慮事項

作業項目に複数のリソースを割り当てる際は、次の点に注意してください。

* ユーザーのプロファイルには、複数のジョブの役割を関連付けることができます。 ユーザーとジョブの役割の関連付けについて詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 通常、タスクや問題は、1 つまたは複数のジョブの役割またはチームに最初に割り当てられます。 プロジェクトを開始する準備が整ったら、ユーザーへの割り当ても必要になる場合があります。\
   1 つ以上の役割にタスクまたはイシューが割り当てられ、ユーザーも割り当てられた場合、Adobe Workfrontは、次のルールに従って、追加のユーザーに関連付けるジョブの役割を決定します。

   * プライマリロールが 1 つだけ割り当てられ、プライマリロールと一致する場合、タスクまたはイシューは、そのジョブロールを満たすユーザーにのみ割り当てられます。
   * 複数のロールが割り当てられ、少なくとも 1 つのロールがユーザーのセカンダリロールと一致する場合、タスクまたは問題は、他のロールの 1 つ ( 複数の一致がある場合はWorkfrontがランダムに選択 ) を満たすユーザーと、追加のロールに割り当てられます。
   * 1 つ以上のジョブロールが割り当てられ、ユーザーのロールに一致するものがない場合、タスクまたはイシューはロールまたはロールの両方に割り当てられ、ユーザーにも割り当てられます。

* タスクまたはイシューがチームに割り当てられ、ユーザーも割り当てられた場合、そのタスクまたはイシューはチームとユーザーの両方に割り当てられたままになります。

## 割り当て先を削除すると、タスクの時間と割り当て率にどのような影響が及ぶか

ユーザーの削除は、タスクの時間や割り当ての割合に影響を与える可能性があります。 ユーザーを削除した場合にタスクに与える影響は、タスクに選択した期間の種類によって異なります。 期間のタイプについて詳しくは、 [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

次の期間タイプを持つタスクからユーザーを削除する場合：

* **シンプル：** そのユーザーに割り当てられた計画時間が、タスクの合計計画時間から差し引かれます。

   >[!IMPORTANT]
   >
   >タスクとプロジェクトの予定時間の合計が変更されるので、プロジェクト計画に悪影響が出る場合があります。

* **労力主導型：** 他のユーザーの配分率は変更されません。
* **計算された割り当て：** 他のユーザーの配分率は、合計が 100%になるように調整されます。
* **計算作業時間：** 他のユーザーの配分率は変更されません。

## タスクの割り当て解除に関する考慮事項

一度に 1 つのタスクから割り当てを削除することも、複数のタスクから割り当てを一括して削除することもできます。

タスクから割り当てを一括で削除する方法の詳細については、 [タスクリスト内の複数のユーザー割り当てを変更する](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md).

タスクから割り当てを削除する際は、次の点に注意してください。

* タスクからユーザーの割り当てを解除しても、そのタスクは、ユーザーがタスクで果たしたジョブの役割に割り当てられたままになります。
* タスクからジョブロールまたはチームの割り当てを解除しても、他のリソースに割り当てられていない場合、タスクは未割り当てのままになります。
