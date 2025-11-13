---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクのユーザーと役割の割り当て時間の管理
description: タスクにユーザーまたはロールを割り当てると、タスクを完了するために一定時間作業するように割り当てられます。タスク期間のタイプが「シンプル」の場合、各ユーザーまたは担当業務がタスクに割り当てられた際に割り当てられる時間数を、手動で変更できます。
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 66%

---

# タスクに関するユーザーと役割の割り当て時間の管理

<!--Audited: 10/2025-->

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->


<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

割り当て時間は、割り当てられたリソースがタスクの作業に費やす予定時間の合計を表します。 時間は、タスクの期間全体を通して、ユーザーが割り当てられた時間を、特定の 1 日、1 週間、1 か月に表します。

タスクに対して高度な割り当てを行う際に、割り当て時間を変更できます。

>[!NOTE]
>
>ユーザーを作業に割り当てる場合、ユーザーのスケジュールに応じた空き時間は、タスクやイシューの予定日と見込日に影響します。スケジュールについて詳しくは、[スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>ワークまたはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>タスクへのアクセスを編集</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td>
   <td><p>タスクに対する参加以上の権限</p>
   <p>古いエクスペリエンスを使用してタスクを編集する際に、「タスクを編集」ボックスで割り当て時間を更新する権限を編集します。 新しいエクスペリエンスでタスクを編集する際に、「タスクを編集」ボックスで割り当て時間を管理できなくなりました。</p> <p>詳しくは、<a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">タスクを編集</a>を参照してください。</p></td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation hours in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation hours in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.-->


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
1. タスクヘッダーの **割り当て** エリアをクリックし、**詳細** をクリックします。
1. タスクの&#x200B;**期間タイプ**&#x200B;が&#x200B;**シンプル**&#x200B;であることを確認します。
1. 各タスク担当者の **割り当て** フィールドを変更します。 これは、タスクの期間全体に対する、このタスクへの各割り当ての全体的な配分です。これにより、タスクの全体 **予定時間数** も更新される可能性があります。

   ![&#x200B; 割り当ての変更 &#x200B;](assets/advanced-assignments-duration-type-allocations.png)

1. 「**保存**」をクリックします。
