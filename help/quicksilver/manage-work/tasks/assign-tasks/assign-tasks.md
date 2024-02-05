---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクを割り当て
description: タスクをユーザー、役割やチームに割り当てて、タスクの完了担当者を指定できます。一度に複数のリソースに対して 1 つのタスクを割り当てることができます。
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 611b136e-2c3f-4eac-9d75-e8c12e06148d
source-git-commit: 13a1d9ebee75c468ce55794db130f01ba658f125
workflow-type: tm+mt
source-wordcount: '1953'
ht-degree: 100%

---

# タスクを割り当て

{{highlighted-preview}}

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

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View or higher access to Users</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>プロジェクトとタスクへのアクセス権を編集</p> <p>ユーザーに対する表示以上のアクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクへの参加以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

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
1. タスクまたはイシューのヘッダーの&#x200B;**割当て**&#x200B;フィールドにある&#x200B;**割り当て先**&#x200B;をクリックします。

   または

   タスクまたはイシューが既に割り当てられている場合は、割り当ての名前をクリックします。

   ![](../assign-tasks/assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. 次のいずれかの操作を行います。

   * 割り当てるユーザー、役割、またはチームの名前を入力し、リストに表示されたらクリックします。


     >[!TIP]
     >
     >ユーザー割り当てを追加する際には、アバター、ユーザーの主要な役割やメールアドレスに注意して、同じ名前のユーザーを区別してください。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。
     >
     >ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。
     >
     ><span class="preview">担当業務の割り当てを追加する際に、担当業務や場所を検索することができます。割り当てにデフォルトの請求レートを使用する場合は、システム／デフォルトの担当業務を選択し、料金カードから請求レートを使用する場合は、料金カードの担当業務を選択します。料金カードに関して詳しくは、[料金カードの管理](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)を参照してください。</span>


   * （条件付き）**提案された割り当て**&#x200B;リストが表示される場合は、このリスト中の名前のいずれかをクリックします。詳しくは、[スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

   * 「**詳細**」をクリックします。

     詳細な割り当てを行う方法について詳しくは、[詳細な割り当てを作成](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)を参照してください。

1. 「**保存**」をクリックします。
1. （オプションおよび条件付き）「**詳細**」をクリックした場合、タスクの右側のパネルにある&#x200B;**「X」アイコン**&#x200B;をクリックして、割り当てを削除します。

## リスト内のタスクの割り当て

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
     >
     ><span class="preview">担当業務の割り当てを追加する際に、担当業務または場所を検索できます。割り当てにデフォルトの請求レートを使用する場合は、システム／デフォルトの担当業務を選択し、料金カードから請求レートを使用する場合は、料金カードの担当業務を選択します。評価カードについて詳しくは、[評価カードの管理](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)を参照してください。</span>


1. （条件付き）**割り当て**&#x200B;フィールドで、割り当てボックスの右上隅にある&#x200B;**人物**&#x200B;アイコンをクリックして、**詳細な割り当て**&#x200B;ボックスを開き、詳細な割り当てを作成します。

   <!--
   there is a People icon in NWE but it's hard to see - you need to assign the task to at least 2 users, not roles, or teams, before it shows up</p>
   -->

   詳しくは、[詳細な割り当てを作成](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)を参照してください。

   >[!TIP]
   >
   >割り当て先フィールドまたは割り当て済みフィールドからは、詳細な割り当てを行うことはできません。

1. タスクに担当者を追加した後、Enter キーを押すか、ページ上の任意の場所をクリックして、「自動保存」を選択した場合に変更を保存します。それ以外の場合は、「**保存**」をクリックします。

## ユーザーに複数のタスクを割り当てる

1. 一括で割り当てるタスクのリストに移動します。
1. （条件付き）「**自動保存**」オプションは、プロジェクトのタスクのリストにある場合に選択します。

   >[!IMPORTANT]
   >
   >プロジェクトにタスクを手動で保存する場合は、タスクを一括で編集できません。

1. タスクリストで複数のタスクを選択します。
1. 「**編集**」をクリックします。

   **タスクを編集**&#x200B;ダイアログボックスが開きます。

1. **割り当て**&#x200B;エリアで、**担当者**&#x200B;ボックスを選択し、すべてのタスクに割り当てるユーザー名、担当業務、またはチームを入力します。

   >[!IMPORTANT]
   >
   >タスクが既に割り当てられている場合、ここに指定したリソースは、タスク上の既存のリソースを置き換える代わりに、タスクに追加されます。

1. （オプション）複数のリソースをタスクに割り当てる場合は、**タスク責任者**&#x200B;列にあるラジオボタンを選択して、タスクの主担当者または所有者であるリソースを示します。これは、チームには使用できません。
1. （条件付き）選択したすべてのタスクに残存作業時間の優先または予定割り当て時間の期間タイプがある場合、タスクに割り当てられた各リソースに対して&#x200B;**割り当て％**&#x200B;を指定します。これは、これらのリソースがタスクの完了に費やす時間を示します。これは、ユーザーと担当業務でのみ使用できます。

   または

   選択したすべてのタスクの期間の種類がシンプルの場合は、タスクに割り当てられた各リソースの&#x200B;**時間**&#x200B;量を指定します。すべてのリソースの全時間の合計は、タスクの予定時間数と等しくする必要があります。

   >[!IMPORTANT]
   >
   >選択したタスクの期間の種類や選択したタスクの期間の種類が異なる場合は、割り当ての割合またはリソースごとの時間数を指定できません。

   タスクの期間のタイプについて詳しくは、[タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

1. （オプション）ユーザーをタスクに割り当てる場合、**担当者の役割**&#x200B;列の&#x200B;**役割を選択**&#x200B;ドロップダウンメニューから、ユーザーがタスクで果たすべき役割を選択します。役割を選択しない場合、Workfront はユーザーの主要役割を自動的選択します。

1. （オプション）すべてのタスクから既存の担当者を削除する場合は、以下の操作のいずれかを行います。

   1. タスクから削除するユーザー、役割、チームの名前を入力し、リストに表示されたらそれを選択し、**担当者を削除**&#x200B;をクリックしてさらに担当者を削除します。
   1. **既存の担当者をすべて削除**&#x200B;をクリックし、選択したすべてのタスクからすべての担当者を削除します。

1. 「**変更を保存**」をクリックします。
1. （オプションおよび条件付き）タスクのリストに「割り当て先」フィールドまたは「割り当て」フィールドが表示されたら、タスクのこれらの列のいずれかの内側をクリックし、担当者の名前の横にある **X アイコン**&#x200B;をクリックして、タスクから削除します。

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


