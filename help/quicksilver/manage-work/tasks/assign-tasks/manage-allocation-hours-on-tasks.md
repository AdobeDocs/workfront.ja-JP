---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクに関するユーザーと役割の割り当て時間の管理
description: タスクにユーザーまたはロールを割り当てると、タスクを完了するために一定時間作業するように割り当てられます。タスク期間のタイプが「シンプル」の場合、各ユーザーまたは担当業務がタスクに割り当てられた際に割り当てられる時間数を、手動で変更できます。
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '580'
ht-degree: 100%

---

# タスクに関するユーザーと役割の割り当て時間の管理

タスクにユーザーまたはロールを割り当てると、タスクを完了するために一定時間作業するように割り当てられます。タスク期間のタイプが「シンプル」の場合、各ユーザーまたは担当業務がタスクに割り当てられた際に割り当てられる時間数を、手動で変更できます。

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
   <td> <p>タスクへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する参加以上の権限</p> <p>権限を編集し、タスクの編集ボックスで時間配分を更新</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## タスクの時間配分を変更する際の考慮事項

>[!IMPORTANT]
>
>タスクの各割り当てに対する配分を手動で変更すると、それに応じてタスクの予定時間数が更新される場合があります。詳しくは、[計画時間の概要](../../../manage-work/tasks/task-information/planned-hours.md)記事内の[ユーザー割り当て管理時のタスクの予定時間数の更新](../../../manage-work/tasks/task-information/planned-hours.md#update)の節を参照してください。

* タスクに割り当てられた個々のリソースに配分された時間の合計は、タスクの予定時間数を表します。
* 1 つのタスクに 1 人のユーザーまたは役割が割り当てられている場合、そのユーザーまたは役割に割り当てられた時間数は、タスクの予定時間数と一致します。
* 複数の割り当てを行う場合、タスクの期間タイプが「シンプル」であれば、デフォルトで、各ユーザーまたは担当業務に対して、タスクでの作業に割り当てられる時間は均等になります。詳しくは、次の記事を参照してください。

   * [タスクの期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [期間タイプの概要：シンプル](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* タスクの期間タイプが「シンプル」の場合、各ユーザーまたは担当業務に割り当てられた時間数を手動で変更して、タスクの割り当て先の一部が、他の割り当て先よりも作業時間が長くなる可能性があることを示すことができます。
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

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 「**保存**」をクリックします。
