---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクリスト内の複数のユーザー割り当てを変更する
description: タスクの割り当てを管理する場合、タスクのリストの一括編集機能を使用して、複数のタスクに対して同時に変更を加えることができます。
author: Alina
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# タスクリスト内の複数のユーザー割り当てを変更する

<!--
<p>There is a similar article in Resource Scheduling and a similar one for Issues; when things change, you might need to update all 3</p>
-->

タスクの割り当てを管理する場合、タスクのリストの一括編集機能を使用して、複数のタスクに対して同時に変更を加えることができます。

この記事では、タスクリスト内の複数のタスクに対する複数のユーザー割り当てを変更する方法について説明します。 他の領域の複数のタスクに対する割り当てを変更する場合は、次の記事も参照してください。

* ワークロード・バランサを使用したタスクの割り当ての詳細は、 [ワークロードバランサーでの作業割り当ての概要](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

リスト内の 1 つのリソースにタスクを割り当てる方法については、 [タスクを割り当て](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

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
   <td> <p>プロジェクトとタスクへのアクセスを編集</p> <p>ユーザーへのアクセス権を表示するか、それ以上に設定する</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに権限を付与するか、それ以上の権限を付与する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on tasks</h2>
<p>(NOTE: moved to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>You might want to modify the user assignments for multiple tasks for a variety of reasons, including the following:</p>
<ul>
<li>Users join or leave your team</li>
<li> <p>A user takes a vacation that extends beyond task due dates</p> <note type="note">
When assigning users to work, their availability according to their schedules affects the Planned and Projected Dates of tasks. For information about schedules, see
<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.
</note> </li>
<li>A specific role or user is set as the assignee for multiple tasks and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
<p><strong>How removing assignees affects task hours and allocation percentages</strong></p>
<p>(NOTE: move to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm) </p>
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration&nbsp;Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration&nbsp;Types:</p>
<ul>
<li> <p><strong>Simple:</strong> The planned hours assigned to that user are subtracted from the task's total planned hours.</p> <note type="important">
<span class="s1">This could negatively affect your project plan because it changes the total planned hours for the task and the project.</span>
</note> </li>
<li><span class="s1"><strong>Effort Driven:</strong> The allocation percentage does not change for other users.</span> </li>
<li><span class="s1"><strong>Calculated Assignment:</strong> The allocation percentages of other users are adjusted so that the total equals 100%.</span> </li>
<li><span class="s1"><strong>Calculated Work:</strong> The allocation percentage does not change for other users.</span> </li>
</ul>
</div>
-->

## 複数のタスクの割り当てを変更する

1. 割り当てを変更するタスクの一覧に移動します。
1. （オプション）変更する担当者に割り当てられたタスクのみを表示するフィルターを作成します。

   例えば、複数のタスクのデフォルトの担当者として特定の役割がプロジェクトに含まれている場合は、その役割を担当者として持つタスクのみを表示するフィルタを作成できます。 次に、役割を特定のユーザーに置き換えます。

   フィルターの作成について詳しくは、 [フィルターを作成または編集](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).


1. ロールに対してフィルターを設定するには、「 」を選択します。 **割り当ての役割**&#x200B;を選択し、「 **ID**.

   >[!TIP]
   >
   >次を使用しない **割り当て先** フィールドに入力します。 タスクに割り当て可能なプライマリの代わりに、タスクのロール所有者のみが検索されます。

   または

   ユーザーをフィルターするには、「 」を選択します。 **割り当てユーザー、** 次に、 **ID。**

   >[!TIP]
   >
   >次を使用しない **割り当て先** フィールドに入力します。 これにより、プライマリに割り当て可能なユーザーの代わりに、タスクのユーザー所有者のみが検索されます。

1. 割り当てを変更するタスクを選択し、 **編集** アイコン ![](assets/edit-icon.png).

   タスクを編集ページが表示されます。 編集した項目は、ページの左上隅に表示されます。

1. 次に移動： **割り当て** 」セクションに入力します。
1. 担当者を追加または削除するには、次のいずれかの操作を行います。

   >[!IMPORTANT]
   >
   >担当者を削除すると、タスクの時間と割り当ての割合に影響を与える場合があります。 詳しくは、 [割り当て先を削除すると、タスクの時間と割り当て率にどのような影響が及ぶか](#how-removing-assignees-affects-task-hours-and-allocation-percentages) 」を参照してください。

   * 新しい担当者を追加するには：

      1. 内 **割り当て** セクション、選択 **担当者**.

         選択したすべてのタスクで共通する情報が表示されます。 例えば、同じユーザーがすべてのタスクに割り当てられている場合、そのユーザーは **担当者** 列。 選択したタスク間で情報が共通でない場合は、情報は表示されません。

      1. ユーザー、ロール、またはチームの名前を入力し、リストに表示されたら選択します。 割り当てが追加され、選択したタスクの現在の割り当ては置き換えられません。


     >[!TIP]
     >
     > * 複数のユーザー、ジョブの役割またはチームを割り当てることができます。 アクティブなユーザー、ジョブの役割およびチームのみを割り当てることができます。
     >   
     > * ユーザー割り当てを追加する際には、アバター、ユーザーのプライマリの役割、または電子メールアドレスに注意して、同じ名前のユーザーを区別します。 ユーザーを追加したときに表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。 ユーザーがユーザーの電子メールを表示するには、アクセスレベルで [ 連絡先情報の表示 ] 設定を有効にしておく必要があります。 詳しくは、 [ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
     > 
     >   非アクティブ化前にユーザー、ジョブの役割、またはチームが割り当てられた場合、そのユーザーは作業項目に割り当てられたままになります。 この場合、次の操作をお勧めします。
     >   
     >     * 作業項目をアクティブなリソースに再割り当てする。
     >     * 非アクティブなチームのユーザをアクティブなチームに関連付け、作業項目をアクティブなチームに再割り当てします。


   * 個々の担当者を削除するには：

      1. 次をクリック： **X アイコン** 担当者が「割り当て」リストに表示される場合に削除する担当者の名前の横に表示されます。

         または

         （条件付き）削除する担当者が、選択したタスクの一部にのみ担当者が割り当てられているので、[ 割り当て ] セクションに表示されない場合は、[ **担当者を削除** 削除する担当者の名前を入力し、ドロップダウンリストに表示されたら、名前をクリックします。

   * 既存のすべての担当者を削除するには：

      1. クリック **既存の担当者をすべて削除**&#x200B;を選択し、「 **はい、すべての担当者を削除します**.

         これにより、共通の担当者（編集ダイアログボックスに表示される担当者）だけでなく、選択したすべてのタスクのすべての担当者も削除されます。

     タスクからユーザーを削除すると、タスクの時間や割り当ての割合に影響を与える場合があります。

     詳しくは、 [タスクの割り当て変更の概要](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

1. （オプション）担当者に対して、次のいずれかのオプションを変更します。

   * （条件付き） **割り当て%または時間**:新しい配分率または時間を指定します。

     >[!NOTE]
     >
     >このオプションは、編集中のすべてのタスクで期間のタイプが同じである場合にのみ変更できます。 「期間タイプ」が「計算作業」または「労力主導」の場合、配分率を更新できます。 期間タイプが「シンプル」の場合は、時間を更新できます。 期間のタイプについて詳しくは、 [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).
     >
     >
     フィールドが空白の場合は、タスク間で値が異なります。ただし、変更は可能です。

   * **タスク所有者**:担当者が編集中のすべてのタスクのタスクの所有者にするには、このオプションを選択します。
   * **担当者の役割**:ドロップダウンリストから役割を選択します。 選択しない場合、Adobe Workfrontはユーザーのプライマリロールを自動的に選択します。

1. クリック **変更を保存します。**
