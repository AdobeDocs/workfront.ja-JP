---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスク割当て変更の概要
description: ユーザー、チームまたは担当業務にタスクを割り当てたり、タスクの割り当てを解除したりできます。複数のリソースを同時に割り当てることも、1 つのリソースのみを割り当てることもできます。一度に 1 つのタスクを割り当てることも、複数のタスクを一括して割り当てることもできます。
author: Lisa
feature: Work Management
exl-id: e774f2db-494d-4f93-8727-3c073e5f930b
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 99%

---

# タスクの割り当て変更の概要

ユーザー、チームまたは担当業務にタスクを割り当てたり、タスクの割り当てを解除したりできます。複数のリソースを同時に割り当てることも、1 つのリソースのみを割り当てることもできます。一度に 1 つのタスクを割り当てることも、複数のタスクを一括して割り当てることもできます。

>[!TIP]
>
>複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
>
>非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
>
>* 作業アイテムをアクティブなリソースに再割り当てする。
>* 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。
>

この記事では、タスクの割り当てを変更した場合の影響に関する一般的な情報を説明します。タスクの割り当て方法について詳しくは、次の記事を参照してください。

* タスクの割り当てについて詳しくは、[タスクの割り当て](../../../manage-work/tasks/assign-tasks/assign-tasks.md)および[タスクリスト内の複数のユーザー割り当てを変更](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)を参照してください。

* スケジュールエリアの複数のタスクに対する割り当ての変更について詳しくは、「スケジュール用エリアのタスクに対する複数のユーザー割り当ての変更」を参照してください。
* ワークロードバランサーを使用したタスクの割り当てについて詳しくは、[ワークロードバランサーでの作業割り当ての概要](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)を参照してください。

この記事の一部の情報は、イシューへの割り当てにも当てはまります。イシューの割り当てとその他の考慮事項について詳しくは、[イシューの割り当ての変更の概要](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)を参照してください。

## タスクのユーザー割り当てを変更するタイミング

次のような様々な理由で、タスクのユーザー割り当てを変更する場合があります。

* ユーザーがチームに参加する、またはチームから脱退する
* ユーザーの休暇が、タスクの期限を過ぎても続いている

  >[!NOTE]
  >
  >ユーザーを作業に割り当てる場合、スケジュールに応じたユーザーの空き時間がタスクの予定日と見込日に影響します。スケジュールについて詳しくは、[スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

* 特定の役割またはユーザーが複数のタスクの担当者に設定されているので、別のユーザーまたは役割に割り当てられるすべての項目をすばやく変更する必要がある

## 担当業務、チーム、ユーザーに対する複数の割り当てに関する考慮事項

作業アイテムに複数のリソースを割り当てる際は、次の点を考慮してください。

* ユーザーのプロファイルには、複数の担当業務を関連付けることができます。ユーザーと担当業務の関連付けについて詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

* 通常、タスクやイシューはまず、1 つまたは複数の担当業務またはチームに割り当てられます。プロジェクトを開始する準備が整ったら、ユーザーに割り当てる必要が生じる場合もあります。\
  1 つまたは複数の役割にタスクまたはイシューが割り当てられ、続いてユーザーも割り当てられた場合、Adobe Workfront は次のルールに従って、ユーザー（が存在する場合）に関連付ける担当業務を決定します。

   * 割り当てられた担当業務が 1 つだけで、これがユーザーの主要役割に一致する場合、タスクやイシューは主要役割を果たすユーザーのみに割り当てられます。
   * 複数の役割が割り当てられ、そのうち少なくとも 1 つがユーザーのセカンダリの役割と一致する場合、タスクまたはイシューは、その他の役割の 1 つ（複数の一致がある場合は Workfront がランダムに選択したもの）を果たすユーザー、および追加されたすべての役割に割り当てられます。
   * 1 つ以上の担当業務が割り当てられ、ユーザーの役割に一致するものがない場合、タスクまたはイシューは 1 つまたは複数の役割、およびユーザーの両方に割り当てられます。

* タスクまたはイシューがチームに割り当てられ、ユーザーも割り当てられた場合、そのタスクまたはイシューはチームとユーザーの両方に割り当てられたままになります。

## 担当者の削除がタスクの時間と配分率に与える影響

ユーザーを削除すると、タスクの時間や配分率に影響を与える可能性があります。ユーザーを削除した場合にタスクに与える影響は、タスクに対して選択された期間タイプによって異なります。期間タイプについて詳しくは、[タスクの期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

次の期間タイプを持つタスクからユーザーを削除する場合：

* **シンプル：**&#x200B;そのユーザーに割り当てられた予定時間数が、タスクの予定時間数の合計から差し引かれます。

  >[!IMPORTANT]
  >
  >タスクとプロジェクトの予定時間数の合計が変更されるので、プロジェクトの計画に悪影響が出る場合があります。

* **残存作業時間の優先：**&#x200B;他のユーザーの配分率は変更されません。
* **予定割り当て時間：**&#x200B;他のユーザーの配分率は、合計が 100％になるように調整されます。
* **予定作業：**&#x200B;他のユーザーの配分率は変更されません。

## タスクの割り当て解除に関する考慮事項

一度に 1 つのタスクから割り当てを削除することも、複数のタスクから割り当てを一括で削除することもできます。

タスクから割り当てを一括で削除する方法の詳細については、[タスクリスト内の複数のユーザー割り当てを変更する](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)を参照してください。

タスクから割り当てを削除する際は、次の点に注意してください。

* タスクからユーザーの割り当てを解除しても、タスクは、ユーザーがタスクで処理した担当業務に割り当てられたままになります。
* 担当業務またはチームをタスクから割り当て解除しても、そのタスクが他のリソースに割り当てられていない場合、タスクは未割り当てのままになります。
