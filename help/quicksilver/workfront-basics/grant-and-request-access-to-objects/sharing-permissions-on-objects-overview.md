---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: オブジェクトに対する共有権限の概要
description: 自分が作成したオブジェクトや自分が共有していたオブジェクトに対する権限を共有または削除できます。
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 0%

---

# オブジェクトに対する共有権限の概要

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->

アクセス権のあるオブジェクトに対する権限を共有するのはAdobe Workfront管理者である必要はありませんが、オブジェクトに対する権限はWorkfront管理者が設定したアクセスレベルで機能します。

アクセスレベルと権限の詳細については、 [アクセスレベルと権限の連携](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

自分が作成したオブジェクトや自分が共有していたオブジェクトに対する権限を共有または削除できます。 オブジェクトの作成者でない場合は、オブジェクトに対する共有権限に加えて、アクセスレベルで共有するオブジェクトに対する共有アクセス権が必要です。 アクセス・レベルの詳細は、 [アクセスレベルの概要](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Workfront管理者は、システム内のすべてのユーザーに対して、それらの項目の所有者にならずに、システム内の項目に対する権限を追加または削除できます。

## Workfrontで共有できるオブジェクト

Workfrontで以下のオブジェクトを他のユーザーと共有できます。

* **プロジェクト**:詳しくは、 [Adobe Workfrontでプロジェクトを共有する](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **テンプレート**:詳しくは、 [プロジェクトテンプレートの共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolio**:詳しくは、 [ポートフォリオの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* **プログラム**:詳しくは、 [プログラムの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **タスク**:詳しくは、 [タスクの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **問題**:詳しくは、 [イシューの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **ドキュメント**:詳しくは、 [ドキュメントの共有](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **ドキュメントフォルダ**:詳しくは、 [ドキュメントフォルダーの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **配達確認**:詳しくは、 [Workfrontの配達確認での配達確認の共有](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

* **レポート、ダッシュボード、カレンダー**:詳しくは、 [レポート、ダッシュボード、カレンダーの共有](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). さらに、次の記事も参照してください。

   * [Adobe Workfrontでのレポートの共有](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [ダッシュボードの共有](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [カレンダーレポートの共有](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **フィルター、ビュー、グループ化**:詳しくは、 [フィルター、表示またはグループ化の共有](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **プラン**:詳しくは、 [シナリオプランナーでのプランの共有](../../scenario-planner/share-a-plan.md).

   追加のライセンスが必要です。

* **目標**:詳しくは、 [Workfront目標での目標の共有](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

   追加のライセンスが必要です。

## オブジェクトの共有に関する考慮事項

* オブジェクトに対して持っているのと同じレベルまたは低レベルの権限のみを共有できます。

   例えば、オブジェクトに対する Contribute の権限を持っている場合、そのオブジェクトに対する別のユーザに管理権限を付与することはできません。

* ユーザーのアクセスレベルより高いアクセスレベルのオブジェクトを共有することはできません。 例えば、ユーザーのアクセスレベルでプロジェクトへの表示アクセス権を持っている場合、プロジェクトに対する管理権限を付与することはできません。
* 少なくとも 1 つのオブジェクトを表示する権限を持つユーザーは、そのオブジェクトを他のユーザーと共有できます。
* オブジェクトは、アクティブなユーザー、ジョブの役割、チーム、グループ、会社と共有できます。

   >[!NOTE]
   >
   >プランや目標は、他のアクティブなユーザーとのみ共有できます。 追加のライセンスが必要です。
   >
   >
   >詳しくは、以下を参照してください。
   >
   >* [シナリオプランナーでのプランの共有](../../scenario-planner/share-a-plan.md)
   >* [Workfront目標での目標の共有](../../workfront-goals/workfront-goals-settings/share-a-goal.md)


## 制限の共有

オブジェクトは、最大 100 個のエンティティ（ユーザー、チーム、グループ、ジョブの役割、会社）と共有できます。 この制限を回避するため、個々のユーザーとではなく、グループ、チームまたは会社とオブジェクトを共有することをお勧めします。

## オブジェクトの権限の共有

次の表に、オブジェクトの共有時に選択できる権限のレベルを示します。 すべてのオブジェクトで、使用可能なすべての設定があるわけではありません。 別のエンティティに、オブジェクトの表示または管理の権限を付与することができます。 プロジェクト、タスク、またはイシューを共有している場合は、Contribute に権限を付与することもできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ビュー</td> 
   <td> <p>オブジェクトに対して、次の操作を実行できます。</p> 
    <ul> 
     <li>オブジェクトの表示</li> 
     <li>オブジェクトにドキュメントを追加する</li> 
     <li>オブジェクトに関する財務情報の表示</li> 
     <li> <p>オブジェクトの共有<br></p> <p>オブジェクトを共有する場合、他のユーザーには、上位レベルではなく、オブジェクトに対してのみ持っているのと同じ権限レベルを付与できます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">参加</td> 
   <td> <p>オブジェクトに対して、次の操作を実行できます。</p> 
    <ul> 
     <li>それを表示</li> 
     <li>表示権限に含まれるすべてのアクション。</li> 
     <li>費用を追加します</li> 
     <li>タスクまたはプロジェクトのタスクを追加する</li> 
     <li>タスクを追加します（プロジェクトの場合）</li> 
     <li>カスタムFormsの編集</li> 
     <li>オブジェクトに対するログ時間</li> 
     <li>割り当てを行う</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">管理</td> 
   <td> <p>オブジェクトに対して、次の操作を実行できます。</p> 
    <ul> 
     <li>それを表示</li> 
     <li>表示および投稿権限に含まれるすべてのアクション</li> 
     <li>削除</li> 
     <li>財務情報の管理</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">これを外部ユーザーに公開する</td> 
   <td> <p>Workfrontアカウントを持っていないユーザーは、リンクをクリックしてオブジェクトを表示できます。 これは、すべてのオブジェクトに対して使用できるわけではありません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">システム全体で表示できるようにします。</td> 
   <td> <p>このオブジェクトは、Workfrontアカウントを持つすべてのユーザーが検索で見つけ、表示することができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 継承された権限とオブジェクトの階層について

* [親オブジェクトから継承された権限](#permissions-inherited-from-parent-objects)
* [組織のメンバーシップによって取得された権限](#permissions-acquired-through-organizational-memberships) 

### 親オブジェクトから継承された権限 {#permissions-inherited-from-parent-objects}

Workfrontの権限は、階層的に継承されます。 つまり、親オブジェクトのユーザーに対して権限を付与する場合、デフォルトでは、親オブジェクトに関連付けられている子オブジェクトに対しても同じ権限が付与されます。

たとえば、あるユーザに Contribute の権限を与えると、そのユーザは、そのプロジェクトに関連するすべてのタスクと問題（子オブジェクト）に対する Contribute の権限を持ちます。

上記の例では、権限を子オブジェクトに制限することはできません。 プロジェクトに関連付けられた子オブジェクトに対して Contribute 権限を持たせたくない場合は、継承された権限をオブジェクトから手動で削除し、その後、詳細設定を含め、個々のユーザの権限を調整する必要があります。 

Workfrontのオブジェクトの階層と相互依存関係について詳しくは、 [オブジェクトの相互依存性と階層](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 記事内 [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Workfront管理者は、アクセスレベルでドキュメントの継承された権限を無効にできます。 アクセスレベルでドキュメントの継承された権限を無効にする方法については、 [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### 組織のメンバーシップによって取得された権限  {#permissions-acquired-through-organizational-memberships}

オブジェクト上のユーザーのグループに対して「管理」権限を付与し、同じオブジェクト上のそのグループ内の個々のユーザーに対して「表示」権限を付与すると、そのユーザーは最高レベルの権限（「管理」）を付与されます。 

権限レベルが高い組織単位（グループ、チーム、ジョブロール、または会社）に既に属するユーザーに低い権限を付与する場合は、組織単位から権限を削除し、低い権限を持つユーザーを個別に追加する必要があります。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## オブジェクトの共有

オブジェクトの共有方法については、 [オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## オブジェクトから権限を削除

オブジェクトから権限を削除する方法については、 [オブジェクトから権限を削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## オブジェクトに対する権限のリクエスト

ユーザーが、表示する権限を持たないオブジェクトへのリンクを送信した場合、またはオブジェクトに対する権限を低く設定し、より高いレベルの権限を要求する場合は、そのオブジェクトに対する権限を要求できます。 

オブジェクトに対する共有権限を持つすべてのユーザーから、オブジェクトへのアクセス権をリクエストできます。 

オブジェクトに対する権限のリクエストの詳細については、 [オブジェクトへのアクセスのリクエスト](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
