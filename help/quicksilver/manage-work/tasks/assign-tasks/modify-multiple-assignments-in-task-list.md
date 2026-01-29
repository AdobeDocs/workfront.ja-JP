---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクリスト内の複数のユーザー割り当ての変更
description: タスクの割り当てを管理する場合、タスクのリストの一括編集機能を使用して、複数のタスクに対して同時に変更を加えることができます。
author: Lisa
feature: Work Management, Tasks, Resource Management
role: User
exl-id: 04f7761f-da94-4858-85c5-8dc97bd78bee
source-git-commit: 4167910f36921e04351190f722ea1e7fac9641c7
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 75%

---

# タスクリスト内の複数のユーザー割り当ての変更

<!--Audited: 11/2025-->

<!--remove the old/new experience references when the toggles are removed-->

<!--
this article is similar and updates on this one might need to be repeated here: help/quicksilver/manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

タスクの割り当てを管理する場合、タスクのリストの一括編集機能を使用して、複数のタスクに対して同時に変更を加えることができます。

この記事では、タスクリスト内の複数のタスクに対する複数のユーザー割り当てを変更する方法について説明します。他の領域の複数のタスクに対する割り当てを変更する場合は、次の記事も参照してください。

* ワークロードバランサーを使用したタスクの割り当てについて詳しくは、[ワークロードバランサーでの作業割り当ての概要](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)を参照してください。

リスト内の 1 つのリソースにタスクを割り当てる方法については、[タスクの割り当て](../../../manage-work/tasks/assign-tasks/assign-tasks.md)を参照してください。

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
   <td>タスクへの投稿以上の権限</td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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
<p>Removing users can affect task hours and allocation percentages. The effect that removing a user has on the task depends on the Duration Type that was selected for the task. For information about Duration Type, see <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">Overview of Task Duration and Duration Type</a>.</p>
<p>When you delete a user from a task with the following Duration Types:</p>
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

## 複数のタスクの割り当てを変更

1. 割り当てを変更するタスクの一覧に移動します。
1. （オプション）変更する担当者に割り当てられたタスクのみを表示するフィルターを作成します。

   例えば、複数のタスクのデフォルトの担当者として特定の役割がプロジェクトに含まれている場合は、その役割を担当者として持つタスクのみを表示するフィルターを作成できます。次に、役割を特定のユーザーに置き換えます。

   フィルターの作成について詳しくは、[フィルターを作成または編集](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。


1. 役割に対してフィルターを設定するには、「**割り当てられた役割**」を選択し、次に「**ID**」をクリックします。

   >[!TIP]
   >
   >「**割り当て先**」フィールドは使用しないでください。これにより、タスクのプライマリ所有者のみが検索され、プライマリ所有者に割り当てられる役割は検索されません。

   または

   ユーザーに対してフィルターを設定するには、「**割り当てられたユーザー**」を選択し、次に「**ID**」をクリックします。

   >[!TIP]
   >
   >「**割り当て先**」フィールドは使用しないでください。これにより、タスクのプライマリ所有者のみが検索され、プライマリ所有者に割り当てられるユーザーは検索されません。

1. 割り当てを変更するタスクを選択し、**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。

   タスクの割り当ての編集は、選択した環境によって異なります。

1. （条件付き）実稼動環境を使用してタスクを割り当てると、新しいエクスペリエンスに **タスクを編集** ボックスが開きます。 実稼動環境で次の操作を行います。

   1. 担当者を追加または削除するには、次のいずれかの操作を行います。

      * 担当者を追加するには、「**ユーザー、役割、チームを検索**」フィールドに担当者の名前を入力し始め、リストに表示されたら選択します。
      * 担当者を削除するには、名前の右側にある **x** アイコンをクリックします。 すべてのタスクに共通の担当者のみがリストに表示されます。
      * 「自分に割り当て」をクリックして、選択したタスクを自分に割り当てます。

   1. （条件付き）新しいエクスペリエンスを使用する場合は、「**保存**」をクリックします。

   1. （任意） **タスクを編集** ボックスの下部にある **古いエクスペリエンスに切り替える** をクリックします。

      古いエクスペリエンスで **タスクを編集** ボックスが開きます。

   1. （条件付き）古いエクスペリエンスで、次の手順を実行して担当者を変更します。

      1. **割り当て**&#x200B;セクションに移動します。

         >[!IMPORTANT]
         >
         >担当者を削除すると、タスクの時間と割り当ての割合に影響を与える場合があります。詳しくは、[割り当て先を削除すると、タスクの時間と割り当て率にどのような影響が及ぶか](#how-removing-assignees-affects-task-hours-and-allocation-percentages)を参照してください。

      1. 担当者を追加または削除するには、次のいずれかの操作を行います。

         * 新しい割り当て先を追加するには：

            1. **割り当て** セクションで、「**担当者**」を選択します。

               選択したすべてのタスクで共通する情報が表示されます。例えば、同じユーザーがすべてのタスクに割り当てられている場合、そのユーザーは&#x200B;**担当者**&#x200B;列に表示されます。選択したタスク間で情報が共通でない場合は、情報は表示されません。

            1. ユーザー、役割またはチームの名前を入力していき、名前がリストに表示されたら選択します。割り当てが追加され、選択したタスクの現在の割り当ては置き換えられません。

           >[!TIP]
           >
           > * 複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
           >   
           > * ユーザー割り当てを追加する際には、アバター、ユーザーの主要な役割やメールアドレスに注意して、同じ名前のユーザーを区別してください。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。
           > 
           >   非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
           >   
           >     * 作業アイテムをアクティブなリソースに再割り当てする。
           >     * 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。


         * 個々の割り当て先を削除するには：

            1. 割り当てリストに割り当て先が表示されている場合は、削除する割り当て先の名前の横にある **X アイコン**&#x200B;をクリックします。

               または

               （条件付き）削除したい割り当て先が、選択したイシューの一部にのみ割り当てられているために「割り当て」セクションに表示されない場合は、「**担当者を削除**」をクリックして削除したい割り当て先の名前を入力し始め、名前がドロップダウンリストに表示されたらクリックします。

         * 既存の割り当て先をすべて削除するには：

            1. 「**既存の担当者をすべて削除**」をクリックし、「**はい、担当者をすべて削除します**」をクリックします。

               これにより、共通の担当者（編集ダイアログボックスに表示される担当者）だけでなく、選択したすべてのタスクのすべての担当者も削除されます。

           ユーザーをタスクから削除すると、タスクの時間や配分率に影響を与える可能性があります。

           詳しくは、[タスクの割り当て変更の概要](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)を参照してください。

      1. （オプション）担当者に対して、次のいずれかのオプションを変更します。

         * （条件付き） **割り当て率または時間**：新しい配分率または時間を指定します。

         >[!NOTE]
         >
         >このオプションは、編集中のすべてのタスクで期間タイプが同じである場合にのみ変更できます。「期間タイプ」が「予定作業」または「残存作業時間の優先」の場合、配分率を更新できます。期間タイプが「単純」の場合は、時間を更新できます。 期間タイプについて詳しくは、[&#x200B; タスク期間と期間タイプの概要 &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) を参照してください。
         >
         >
         >このフィールドが空白の場合、値はタスク間で異なりますが、変更は可能です。

         * **タスク責任者**：このオプションを選択すると、担当者が編集中のすべてのタスクの、タスクの所有者になります。
         * **割り当て先の役割**：ドロップダウンリストから役割を選択します。選択しない場合、Adobe Workfront はユーザーのプライマリ役割を自動的に選択します。

      1. 「**変更を保存**」をクリックします。



   1. <span class="preview"> （条件付き） プレビュー環境を使用してタスクを割り当てると、「**タスクを編集** ボックスが開きます。 プレビュー環境で </span> を実行します。

      <div class="preview">

      1. 担当者を追加または削除するには、次のいずれかの操作を行います。

         * 担当者を追加するには、「**ユーザー、役割、チームを検索**」フィールドに担当者の名前を入力し始め、リストに表示されたら選択します。

           新しい担当者が、選択したタスクの既存の担当者に追加されます。
         * 担当者を削除するには、「担当者を削除 **ボックスで担当者の名前をクリックし** す

           または

           **既存の担当者をすべて削除** をクリックします。

           担当者が選択したすべてのタスクから削除されます。

           ユーザーをタスクから削除すると、タスクの時間や配分率に影響を与える可能性があります。

           詳しくは、[タスクの割り当て変更の概要](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md)を参照してください。


           >[!TIP]
           >
           >* 複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
           >   
           >* ユーザー割り当てを追加する際には、アバター、ユーザーの主要な役割やメールアドレスに注意して、同じ名前のユーザーを区別してください。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。
           > 
           >   非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
           >   
           >* 作業アイテムをアクティブなリソースに再割り当てする。
           >* 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。


      1. （オプション）担当者に対して、次のいずれかのオプションを変更します。

         * （条件付き） **割り当て率または時間**：新しい配分率または時間を指定します。

         >[!NOTE]
         >
         >このオプションは、編集中のすべてのタスクで期間タイプが同じである場合にのみ変更できます。「期間タイプ」が「予定作業」または「残存作業時間の優先」の場合、配分率を更新できます。期間タイプが「単純」の場合は、時間を更新できます。 期間タイプについて詳しくは、[&#x200B; タスク期間と期間タイプの概要 &#x200B;](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) を参照してください。
         >
         >
         >このフィールドが空白の場合、値はタスク間で異なりますが、変更は可能です。

         * **プライマリを作成**：選択したタスクにポインタを合わせて、このオプションを選択すると、担当者は編集中のすべてのタスクのタスクの所有者になります。
         * **割り当て先の役割**：ドロップダウンリストから役割を選択します。選択しない場合、Adobe Workfront はユーザーのプライマリ役割を自動的に選択します。
         * **期間タイプ**
         * **期間**
         * **予定時間数**

      1. 「**保存**」をクリックします。

         </div>





