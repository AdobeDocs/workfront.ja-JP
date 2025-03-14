---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクのユーザーと役割の割り当て時間の管理
description: タスクにユーザーまたはロールを割り当てると、タスクを完了するために一定時間作業するように割り当てられます。タスク期間のタイプが「シンプル」の場合、各ユーザーまたは担当業務がタスクに割り当てられた際に割り当てられる時間数を、手動で変更できます。
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 1211a441b542df49480d933d4c25b0c31ef0883d
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 81%

---

# タスクに関するユーザーと役割の割り当て時間の管理

割り当て時間は、割り当てられたリソースがタスクの作業に費やす予定時間の合計を表します。 時間は、タスクの期間全体を通して、ユーザーが割り当てられた時間を、特定の 1 日、1 週間、1 か月に表します。

>[!NOTE]
>
>ユーザーを作業に割り当てる場合、ユーザーのスケジュールに応じた空き時間は、タスクやイシューの予定日と見込日に影響します。スケジュールについて詳しくは、[スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

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
   <td> <p>新規：標準 </p>
   <p>現在：ワーク以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する参加以上の権限</p> <p>権限を編集し、タスクの編集ボックスで時間配分を更新</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タスクの時間配分を変更する際の考慮事項

>[!IMPORTANT]
>
>タスクの各割り当てに対する配分を手動で変更すると、それに応じてタスクの予定時間数が更新される場合があります。詳しくは、[計画時間の概要](../../../manage-work/tasks/task-information/planned-hours.md)記事内の[ユーザー割り当て管理時のタスクの予定時間数の更新](../../../manage-work/tasks/task-information/planned-hours.md#update)の節を参照してください。

* タスクに割り当てられた個々のリソースに配分された時間の合計は、タスクの予定時間数を表します。
* 1 つのタスクに 1 人のユーザーまたは役割が割り当てられている場合、そのユーザーまたは役割に割り当てられた時間数は、タスクの予定時間数と一致します。
* 複数の割り当てを行う場合、タスクの期間タイプが「シンプル」であれば、デフォルトで、各ユーザーまたは担当業務に対して、タスクでの作業に割り当てられる時間は均等になります。詳しくは、次の記事を参照してください。

   * [タスクの期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [期間タイプの概要：シンプル](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* タスクに [ シンプル期間 ] タイプが設定されている場合、各ユーザーまたは担当業務に割り当てられた時間数を手動で変更して、一部のタスクの担当者が他のタスクよりも作業に時間がかかる可能性があることを示すことができます。
* タスクに割り当てられたチームに配分された時間数を変更することはできません。
* イシューのユーザーまたは担当業務の割り当てを手動で変更することはできません。
* また、ワークロードバランサーを使用して、タスクやイシューに対するユーザーの日別、週別、月別の割り当てを管理することもできます。詳しくは、[ワークロードバランサーでのユーザー割り当ての管理](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)を参照してください。

## タスクのユーザーまたは役割の時間配分を変更

1. 時間配分を変更する割り当てのタスクに移動します。
1. タスク名の横にある&#x200B;**その他**&#x200B;メニュー ![](assets/qs-more-icon-on-an-object.png)、「**編集**」、「**割り当て**」の順にクリックします。

   または

   タスクヘッダーにある&#x200B;**割り当て**&#x200B;エリアを選択し、「**詳細**」をクリックします。

1. タスクの&#x200B;**期間タイプ**&#x200B;が&#x200B;**シンプル**&#x200B;であることを確認します。
1. タスクの担当者ごとに&#x200B;**配分**&#x200B;を変更します。これは、タスクの期間全体に対する、このタスクへの各割り当ての全体的な配分です。これにより、タスクの全体的な予定時間数が更新される場合もあります。

   ![ 割り当ての変更 ](assets/advanced-assignments-duration-type-allocations.png)

1. **保存**&#x200B;をクリックします。
