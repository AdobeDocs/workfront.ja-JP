---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクの割り当て
description: タスクをユーザー、役割やチームに割り当てて、タスクの完了担当者を指定できます。一度に複数のリソースに対して 1 つのタスクを割り当てることができます。
author: Lisa
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 21c98e443a6d6ca79045e2f4aba5f792340833cd
workflow-type: tm+mt
source-wordcount: '1617'
ht-degree: 82%

---

# タスクを割り当て

<!--Audited: 10/2025-->

<!--remove production/ preview and old/ new experience references at prod-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Second Quarter 2026 release overview](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md). 

</div>-->

ユーザー、担当業務やチームにタスクを割り当てて、タスクの完了担当者を指定できます。一度に複数のリソースに対して 1 つのタスクを割り当てることができます。

>[!TIP]
>
>複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
>
>非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
>
>* 作業アイテムをアクティブなリソースに再割り当てする。
>* 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。
>

タスクに割り当てられたユーザー数と、タスク所有者のスケジュールによって、タスクの予定日が変更され、その結果、プロジェクトのタイムラインが変更されることがあります。複数のユーザーをタスクに割り当てることの影響について詳しくは、[タスクの割り当て変更の概要](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)を参照してください。

タスクの割り当てに関して詳しくは、この記事に加え、以下の記事を読むことをお勧めします。

* [タスクの割り当て変更の概要](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)
* [スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [スマート割り当ての実行](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [詳細な割り当てを作成](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [タスクリスト内の複数のユーザー割り当てを変更](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)
* [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)
* [プロジェクトの概要を計画](../../../manage-work/projects/planning-a-project/plan-project.md)
* [タスクの予定完了日の概要](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [プロジェクトの予定完了日を設定](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [システム全体のプロジェクト環境を設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)
* [ワークロードバランサーでの作業割り当ての概要](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

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
   <p>Work またはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>プロジェクトとタスクへのアクセス権を編集</p> <p>ユーザーに対する表示以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td>
   <td>タスクに対する参加以上の権限</td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 担当業務、チーム、ユーザーに対する複数の割り当てに関する考慮事項

作業アイテムに複数のリソースを割り当てる際は、次の点を考慮してください。

* ユーザーのプロファイルには、複数の担当業務を関連付けることができます。ユーザーと担当業務の関連付けについて詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

* 1 つのタスクやイシューに複数のユーザーを割り当てた場合、最初に選択した 1 人のユーザーが自動的にタスクやイシューの所有者に指定されます。
これを変更する手順については、[詳細な割り当てを作成](create-advanced-assignments.md)の記事にある、「プライマリオプションを作成」オプションに関する情報を参照してください。

* チームは、タスクやイシューのプライマリの担当者にすることはできません。ユーザーや担当業務のみが、タスクやイシューのプライマリとして指定できます。

<!-- If a task is assigned to multiple teams, the primary team sees the Work On It button. waiting on team to verify if this is true. (Courtney)
You cannot make a team be a Primary on a task/ issue. (Alina) -->

* プロジェクトのタスクやイシューは、最初に 1 つ以上のチームまたは担当業務に割り当てられる場合があります。プロジェクトを開始する準備が整ったら、ユーザーに割り当てる必要が生じる場合もあります。

  <table>
  <col> 
  <col> 
  <tbody>
  <tr>
   <td>チーム</td>
   <td>タスクをチームに割り当て、さらにユーザーを割り当てた場合、そのユーザーがチームのメンバーでない場合でも、タスクはチームとユーザーに割り当てられたままになります。</td>
  </tr>
  <tr>
   <td>担当業務</td>
   <td><p>1 つまたは複数の役割にタスクやイシューを割り当て、続いてユーザーも割り当てた場合は、以下のルールに従って、追加のユーザー（が存在する場合）に関連付ける担当業務を決定します。</p>
     <ul>
      <li>割り当てられた担当業務が 1 つだけで、これが（ユーザーのプロファイルで設定される）ユーザーの主要な役割に一致する場合、タスクやイシューはそのユーザーのみに割り当てられます。</li>
      <li>複数の役割が割り当てられ、そのうち 1 つ以上がユーザーの他の役割のいずれかと一致する場合、タスクやイシューが、追加されたすべての役割と併せて、そのユーザーに割り当てられます（複数の役割が一致する場合はランダムに選択されます）。</li>
      <li>1 つ以上の担当業務が割り当てられ、ユーザーの担当業務に一致するものがない場合、タスクやイシューは、1 つまたは複数の役割、およびユーザーの両方に割り当てられます。</li>
     </ul>
   <p>ユーザーの主な役割とその他の役割について詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">ユーザーのプロファイルの編集</a>を参照してください。</p>
   </td> 
     </tr>
  </tbody>
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations for multiple user assignments and using schedules</h2>
<p>(NOTE: moved to the Modify task assignments overview standalone article)</p>
<p>You can assign multiple resources to a task. When you assign a user to a task, Workfront uses the user's schedule to calculate the planned dates for the task which ultimately determine the timeline of the project. Using the schedule of the user takes into account their time off, holidays, and weekend days which are considered non-working days when task activity cannot occur. </p>
<p>When you assign multiple users to a task, your Workfront administrator <span>or a group administrator</span> determines which one of the following schedules Workfront uses to determine the planned dates of the tasks, based on schedules: </p>
<ul>
<li> <p><strong>The Primary Assignee's schedule</strong>: this is the schedule associated with the user designated as the task Owner.</p> <p>For information about associating users with schedules, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li>
<li><strong>The Project's schedule</strong>: this is the schedule associated with the project. For adding a schedule to a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
</ul>
<p>For information about setting up which schedule a project uses in the case of multiple assignments, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p>
</div>
-->

## 単一のタスクを割り当て

1. 割り当てるタスクに移動します。
1. タスクのヘッダーにある **割り当て** フィールドの **割り当て先** をクリックします

   または

   タスクが既に割り当てられている場合は、割り当ての名前をクリックします。

   ![割り当て](assets/assignments-from-task-header-0825.png)

1. 次のいずれかの操作を行います。

   * 割り当てるユーザー、担当業務、またはチームの名前の入力を開始し、リストに表示されたらクリックします。

     >[!TIP]
     >
     >ユーザー割り当てを追加する際には、アバター、ユーザーの主要な役割やメールアドレスに注意して、同じ名前のユーザーを区別してください。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。
     >
     >ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

   * （条件付き） **ユーザーとチーム** または **担当業務** リストに表示されている名前の 1 つをクリックします。 詳しくは、[スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

     タスクに割り当てるユーザー、チーム、担当業務の名前の入力を開始し、リストに表示されたら選択できます。

   * 「**詳細**」をクリックします。

     詳細な割り当てを行う方法について詳しくは、[詳細な割り当てを作成](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)を参照してください。

1. 「**保存**」をクリックします。
1. （オプションおよび条件付き）「**詳細**」をクリックした場合、タスクの右側のパネルにある&#x200B;**「X」アイコン**&#x200B;をクリックして、割り当てを削除します。

## リストをインライン編集時にタスクを割り当て

いずれかの割り当てフィールドがリストの表示に示されている場合、リストまたはレポート内のタスクを割り当てることができます。これは、タスクをより迅速に割り当てる方法です。この記事では、リスト内の 1 つのタスクの割り当てを変更する方法について説明します。リスト内の複数のタスクに対する複数の割り当てを変更する方法について詳しくは、[タスクリスト内の複数のユーザー割り当ての変更](../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md)を参照してください。

表示に示されるフィールドに応じて、タスクに以下のエンティティを割り当てることができます。

| フィールド | 割り当てられたエンティティ |
|---|---|
| **割り当て先** | 1 人のユーザーの割り当て |
| **割り当て** | 1 人のユーザーの割り当て |
| **割り当て** | ユーザー、担当業務やチームの割り当て |

リスト内のタスクを割り当てる手順は、以下のように行います。

1. 表示内の、割り当て先フィールド、割り当て済みフィールドや、割り当フィールドを持つタスクのリストに移動します。
1. （オプション）**自動保存**&#x200B;ドロップダウンメニューをクリックし、以下のオプションから選択します。

   | オプション | オプションの説明 |
   |---|---|
   | 自動保存 | タスクに加えた変更は自動的に保存され、元に戻すことはできません |
   | 手動保存 | 変更を手動で保存する必要があります。保存する前であれば変更内容を元に戻すことができます。 |
   | タイムラインの計画 | 変更を手動で保存する必要があります。保存する前であれば変更内容を元に戻すことができます。手動保存を選択する場合よりも、変更およびすべてのプロジェクトの依存関係を保存する方がより迅速です。 |

   リストで編集する際にタスクを保存する方法に関して詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

1. タスクを割り当てるには、以下のいずれかを実行します。

   * **割り当て先**&#x200B;または&#x200B;**割り当て**&#x200B;フィールドの内側をクリックし、タスクに割り当てるアクティブなユーザーの名前を入力し、リストに表示されたらクリックします。
   * **割当て**&#x200B;フィールドの内側をクリックし、タスクに割り当てるアクティブなユーザー、担当業務やチームの名前を入力し、リストに表示されたらクリックします。

     >[!TIP]
     >
     >ユーザー割り当てを追加する際には、アバター、ユーザーの主要な役割やメールアドレスに注意して、同じ名前のユーザーを区別してください。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。
     >
     >ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

     <!--<span class="preview">When adding a job role assignment, you can search for the job role or location. Select a Job role to use the default billing rate for the assignment, or select a Rate Card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. （条件付き）「割り当て」フィールドで、リストの下部にある **詳細** をクリックするか、割り当てボックスの右上隅にある **人物アイコン**![ 人物アイコン ](assets/teams.png) をクリックして、**詳細な割り当て** ボックスを開き、詳細な割り当てを作成します。

   詳しくは、[詳細な割り当てを作成](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)を参照してください。

   >[!TIP]
   >
   >割り当て先フィールドまたは割り当て済みフィールドからは、詳細な割り当てを行うことはできません。

1. タスクに担当者を追加した後、Enter キーを押すか、ページ上の任意の場所をクリックして、「自動保存」を選択した場合に変更を保存します。それ以外の場合は、「**保存**」をクリックします。

## リストから複数のタスクを一括で割り当て

1. 一括で割り当てるタスクのリストに移動します。
1. （条件付き）「**自動保存**」オプションは、プロジェクトのタスクのリストにある場合に選択します。

   >[!IMPORTANT]
   >
   >プロジェクトにタスクを手動で保存する場合は、タスクを一括で編集できません。

1. タスクリストで複数のタスクを選択します。
1. 「**編集**」をクリックします。

   **タスクを編集** ボックスが開きます。

1. **割り当て** エリアで、表示された **ユーザー、役割、チームを検索** フィールドにユーザー、チーム、または役割の名前を入力し始め、リストに表示されたらクリックします

   >[!IMPORTANT]
   >
   >タスクが既に割り当てられている場合、ここに指定したリソースは、タスク上の既存のリソースを置き換える代わりに、タスクに追加されます。

1. 選択したタスクに対して、次のフィールドを指定します。

   * 割り当て名にポインタを合わせて、「**タスクを作成**」をクリックし、どの担当者がプライマリのオーナーであるかを示します。
   * **期間タイプ**

     タスクの期間のタイプについて詳しくは、[タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

   * **期間**
   * **予定時間数**

     （詳しくは、[タスクの編集](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください）

1. （任意）既存の担当者をすべてのタスクから削除する場合は、「**ユーザー、役割またはチームを検索**」フィールドで、名前の横にある **x** をクリックします。

1. 「**保存**」をクリックします。
1. （オプションおよび条件付き）タスクのリストに **割り当て先** または **割り当て** フィールドが表示されたら、タスクのこれらの列の 1 つ内をクリックして、担当者の名前の横にある **X アイコン** をクリックすると、タスクから削除できます。


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations about unassigning tasks</h2>
<p>(NOTE: moved this to the new article: /Content/Manage work/Tasks/Assign tasks/modify-task-assignments-overview.htm)</p>
<p>You can remove assignments from one task at a time, or you can remove assignments from multiple tasks in bulk.</p>
<p>For more information about removing assignments from tasks in bulk, see <a href="../../../manage-work/tasks/assign-tasks/modify-multiple-assignments-in-task-list.md" class="MCXref xref">Modify multiple user assignments in a task list</a>. </p>
<p>Consider the following when removing assignments from tasks: </p>
<ul>
<li>When you unassign a user from a task, the task remains assigned to the job role that the user fulfilled on the task.</li>
<li>When you unassign a job role or a team from a task, the task remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->


<!--Assigning multiple tasks in bulk from a list differs depending on which environment you choose. 

### Assign multiple tasks in bulk from a list in the Production environment

1. Go to a list of tasks that you want to assign in bulk. 
1. (Conditional) Ensure that the **Autosave** option is selected if you are on a list of tasks under a project.

   >[!IMPORTANT]
   >
   >You cannot edit tasks in bulk when saving tasks manually on a project.

1. Select several tasks in the tasks list. 
1. Click **Edit**.

   The **Edit Tasks** dialog box opens in the new experience.

1. Continue assigning the tasks using the new experience.

   For more information, see the section [Assign multiple tasks in bulk from a list in the new experience](#assign-multiple-tasks-in-bulk-from-a-list-in-the-new-experience) in this article.

1. (Optional) Click **Switch back to old experience** at the bottom of the **Edit Tasks** box to open the old experience.

1. (Conditional) Using the old experience, in the **Assignments** area, select the **Assignee** box, then start typing the name of a user, job role, or team that you want to assign to all the tasks.

   >[!IMPORTANT]
   >
   >If any of the tasks is already assigned, the resources you indicate here are added to the tasks instead of replacing the existing resources on the tasks. 

1. (Optional) Select the radio button in the **Task Owner** column to indicate which resource is the primary assignee or the Owner of the task, when you assign more than one resource to the task. This is not available for teams. 
1. (Conditional) Specify the **Allocation %** for each resource assigned to the task if all the tasks you selected have a Duration Type of Effort Driven or Calculated Assignment. This indicates how much of their time these resources should spend on completing the task. This is only available for users and job roles.

   Or

   Specify the amount of **Hours** for each resource assigned to the task if all the tasks you selected have a Duration Type of Simple. The total of all hours for all resources should equal the number of Planned Hours for the task.

   >[!IMPORTANT]
   >
   >You cannot specify the allocation percentage or the number of hours per resource if the tasks you selected have different Duration Types or of the tasks you selected have different Duration Types.

   For information about Duration Type on tasks, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Optional) Select a role that the user should fulfill on the task from the **Pick a role** drop-down menu in the **Assignee's Role** column when you assign users to tasks. If you do not select a role, Workfront automatically selects the user's Primary Role. 

1. (Optional) If you want to remove existing assignees from all tasks do one of the following:

   1. Start typing the name of a user, role, or team you want to remove from the task, then select it when it appears on the list and click **Remove Assignee** to remove more assignees.
   1. Click **Remove All Existing Assignees** to remove all assignees from all selected tasks.

1. Click **Save Changes**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of tasks, click inside one of these columns for a task, then click the **X icon** next to the name of an assignee to remove it from the task.


#### Assign multiple tasks in bulk from a list in the new experience

1. Go to a list of tasks that you want to assign in bulk.
1. (Conditional) Ensure that the **Autosave** option is selected if you are on a list of tasks under a project.

   >[!IMPORTANT]
   >
   >You cannot edit tasks in bulk when saving tasks manually on a project.

1. Select several tasks in the tasks list. 
1. Click **Edit**.

   The **Edit Tasks** dialog box opens.

1. In the **Assignments** area, start typing the name of users, teams, or roles in the **Search people, roles, or teams** field provided, then click them when they display in the list

   Or 

   Click **Assign to me** to assign it to yourself.

   >[!IMPORTANT]
   >
   >If any of the tasks is already assigned, the resources you indicate here are added to the tasks instead of replacing the existing resources on the tasks.

1. Click inside the **Duration Type** field and choose a Duration Type. 

   For information about Duration Type on tasks, see [Overview of Task Duration and Duration Type](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Conditional) Depending on what **Duration Type** you selected, update the following fields: 

   * Duration
   * Planned Hours

      For more information, see [Edit tasks](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md). 

1. (Optional) If you want to remove existing assignees from all tasks, click the **x** next to their name in the **Search people, roles, or teams** field.

1. Click **Save**.
1. (Optional and conditional) When the **Assigned to** or the **Assignments** fields display in your list of tasks, click inside one of these columns for a task, then click the **X icon** next to the name of an assignee to remove it from the task.

<div class="preview">
### Assign multiple tasks in bulk from a list in the Preview environment
-->