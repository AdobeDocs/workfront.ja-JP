---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: オブジェクトに対する権限の共有の概要
description: 自分が作成したオブジェクトや自分と共有されたオブジェクトに対する権限を共有または削除できます。
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 88%

---

# オブジェクトに対する権限の共有の概要

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
システム内のユーザーとオブジェクトを共有する場合、受信者に表示、投稿、管理の権限を付与できます。

アクセス権のあるオブジェクトに対する権限を共有するのはAdobe Workfront管理者である必要はありませんが、オブジェクトに対する権限はWorkfront管理者が設定したアクセスレベル内で機能します。

自分が作成したオブジェクトや自分と共有されたオブジェクトに対する権限を共有または削除できます。オブジェクトの作成者でない場合は、オブジェクトに対する共有権限に加えて、アクセスレベルで共有するオブジェクトに対する共有アクセス権が必要です。アクセスレベルについて詳しくは、[新しいアクセスレベルの概要](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)または[アクセスレベルの概要](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)を参照してください。

>[!NOTE]
>
>Workfront 管理者は、システム内のすべてのユーザーに対して、システム内のアイテムに対する権限の追加や削除を、それらのアイテムの所有者にならなくても行うことができます。

## Workfront で共有できるオブジェクト

Workfront で以下のオブジェクトを他のユーザーと共有できます。

* **プロジェクト**：詳しくは、[Adobe Workfront でプロジェクトを共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。

* **テンプレート**：詳しくは、[プロジェクトテンプレートを共有](../../manage-work/projects/create-and-manage-templates/share-project-template.md)を参照してください。

* **ポートフォリオ**：詳しくは、[ポートフォリオの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md)を参照してください。

* **プログラム**：詳しくは、[プログラムの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md)を参照してください。

* **タスク**：詳しくは、[タスクの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)を参照してください。

* **イシュー**：詳しくは、[イシューの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)を参照してください。

* **ドキュメント**：詳しくは、[ドキュメントの共有](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md)を参照してください。

* **ドキュメントフォルダー**：詳しくは、[ドキュメントフォルダーの共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)を参照してください。

* **配達確認**：詳しくは、 [Workfront内での配達確認の共有](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **レポート、ダッシュボード、カレンダー**：詳しくは、[レポート、ダッシュボード、カレンダーの共有](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)を参照してください。さらに、次の記事も参照してください。

   * [Adobe Workfront でのレポートの共有](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [ダッシュボードの共有](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [カレンダーレポートの共有](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **フィルター、ビュー、グループ化**：詳しくは、[フィルター、ビューまたはグループ化の共有](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)を参照してください。

* **計画**：詳しくは、[シナリオプランナーでの計画の共有](../../scenario-planner/share-a-plan.md)を参照してください。

  追加のライセンスが必要です。

* **目標**：詳しくは、[Workfront Goals での目標の共有](../../workfront-goals/workfront-goals-settings/share-a-goal.md)を参照してください。

  追加のライセンスが必要です。

## オブジェクトの共有に関する考慮事項

* オブジェクトに対する自身の権限と同等以下の権限のみを共有できます。

  例えば、オブジェクトに対する参加権限を持っている場合、別のユーザーに対して、そのオブジェクトの管理権限を付与することはできません。

* ユーザーのアクセスレベルより高いアクセスレベルのオブジェクトを共有することはできません。

  例えば、ユーザーのアクセスレベルでプロジェクトへの表示アクセス権を持っている場合、プロジェクトに対する管理権限を付与することはできません。
* あるオブジェクトに対して表示以上の権限を持つユーザーは、そのオブジェクトを他のユーザーと共有できます。
* オブジェクトは、アクティブなユーザー、担当業務、チーム、グループまたは会社と共有できます。

  >[!NOTE]
  >
  >プランや目標は、他のアクティブなユーザーとのみ共有できます。追加のライセンスが必要です。
  >
  >
  >詳しくは、以下を参照してください。
  >
  >* [シナリオプランナーで計画を共有](../../scenario-planner/share-a-plan.md)
  >* [Workfront Goals での目標の共有](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

## 制限を共有

オブジェクトは、最大 100 個のエンティティ（ユーザー、チーム、グループ、担当業務、会社）と共有できます。この制限を回避するため、個々のユーザーとではなく、グループ、チームまたは会社とオブジェクトを共有することをお勧めします。

## オブジェクトの権限を共有

次の表に、オブジェクトの共有時に選択できる権限のレベルを示します。すべてのオブジェクトで、すべての設定が使用できるわけではありません。別のエンティティに、オブジェクトを表示または管理する権限を付与することができます。プロジェクト、タスク、またはイシューを共有している場合は、それらへの参加権限も付与することができます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>表示</strong></td> 
   <td> <p>オブジェクトに対して、次のアクションを実行できます。</p> 
    <ul> 
     <li><p>オブジェクトを表示</p></li> 
     <li><p>オブジェクトにドキュメントを追加</p></li> 
     <li><p>オブジェクトに関する財務情報を表示</p></li> 
     <li> <p>オブジェクトを共有<br></p> <p>オブジェクトを共有する際、他のユーザーに付与できるのは、オブジェクトに対する自身の権限と同程度の権限のみです（自身の権限以上ではない）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>参加</strong></td> 
   <td> <p>オブジェクトに対して、次のアクションを実行できます。</p> 
    <ul> 
     <li>表示権限に含まれるすべてのアクション。</li> 
     <li>費用を追加</li> 
     <li>イシューを追加（タスクまたはプロジェクトの場合）</li> 
     <li>タスクを追加（プロジェクトの場合）</li> 
     <li>カスタムフォームを編集</li> 
     <li>オブジェクトに対する時間を記録</li> 
     <li>割り当ての作成</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>管理</strong></td> 
   <td> <p>オブジェクトに対して、次のアクションを実行できます。</p> 
    <ul> 
     <li>表示および参加権限に含まれるすべてのアクション</li> 
     <li>削除</li> 
     <li>財務情報の管理</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>外部ユーザーに公開する</strong></td> 
   <td> <p>Workfront アカウントを持っていないユーザーは、リンクをクリックしてオブジェクトを表示できます。これは、すべてのオブジェクトに対して使用できるわけではありません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>システム全体で表示できるようにします。</strong></td> 
   <td> <p>Workfront アカウントを持つすべてのユーザーが検索でこのオブジェクトを見つけ、表示することができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 継承された権限とオブジェクトの階層について

### 親オブジェクトから継承された権限 {#permissions-inherited-from-parent-objects}

Workfront の権限は、階層的に継承されます。つまり、親オブジェクトのユーザーに対して権限を付与する場合、デフォルトでは、親オブジェクトに関連付けられている子オブジェクトに対しても同じ権限が付与されます。

たとえば、あるユーザーにプロジェクトへの参加権限を与えると、ユーザーはそのプロジェクトに関連するすべてのタスクとイシュー（子オブジェクト）に対する参加権限を持ちます。

上記の例では、子オブジェクトの権限を制限することはできません。プロジェクトに関連付けられた子オブジェクトに対して参加権限を持たせたくない場合は、継承された権限をオブジェクトから手動で削除し、その後、詳細設定を含め、個々のユーザーの権限を調整する必要があります。 

Workfrontのオブジェクトの階層と相互依存関係について詳しくは、 [オブジェクトの相互依存性と階層](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) 記事内 [Adobe Workfrontオブジェクトの概要](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Workfront 管理者は、アクセスレベルでドキュメントの継承された権限を無効にできます。アクセスレベルでドキュメントの継承された権限を無効にする方法について詳しくは、[カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

### 組織のメンバーシップによって取得された権限 {#permissions-acquired-through-organizational-memberships}

オブジェクト上のユーザーのグループに対して管理権限を付与し、同じオブジェクト上でそのグループ内の個々のユーザーに対して表示権限を付与すると、そのユーザーはオブジェクト上のグループメンバーシップを通して最高レベルの権限（管理）を付与されます。 

権限レベルが高い組織単位（グループ、チーム、担当業務、または会社）に既に属するユーザーに低い権限を付与する場合は、組織単位から権限を削除し、低い権限を持つユーザーを個別に追加する必要があります。

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

オブジェクトの共有方法について詳しくは、[オブジェクトを共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。

## オブジェクトから権限を削除

オブジェクトから権限を削除する方法について詳しくは、[オブジェクトから権限を削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)を参照してください。

## オブジェクトに対する権限のリクエスト

表示する権限を持たないオブジェクトへのリンクを受信した場合、またはオブジェクトに対して低い権限を持っており、より高いレベルの権限へのリクエストが必要な場合は、そのオブジェクトに対する権限をリクエストできます。 

オブジェクトに対する共有権限を持つすべてのユーザーが、オブジェクトへのアクセス権をリクエストできます。 

オブジェクトに対する権限のリクエストについて詳しくは、[オブジェクトへのアクセスのリクエスト](../../workfront-basics/grant-and-request-access-to-objects/request-access.md)を参照してください。
