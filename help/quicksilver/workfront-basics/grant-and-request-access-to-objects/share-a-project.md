---
title: Adobe Workfront でプロジェクトを共有
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーにプロジェクトの表示や編集のアクセス権を付与できます。詳細については、プロジェクトへのアクセス権の付与を参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 96%

---

# Adobe Workfront でプロジェクトを共有

<!-- Audited: 1/2024 -->

Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーにプロジェクトの表示や編集のアクセス権を付与できます。詳しくは、[プロジェクトへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)を参照してください。

ユーザーに付与されるアクセスレベルに加えて、自分が共有のアクセス権を持つ特定のプロジェクトを表示、投稿、管理する権限をユーザーに付与することもできます。

権限は、Workfrontの 1 つの項目に固有で、その項目に対して実行できるアクションを定義します。

## プロジェクトの共有に関する考慮事項

以下の考慮事項に加えて、[オブジェクトに対する権限の共有の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

* デフォルトでは、プロジェクトの作成者にはプロジェクトを管理する権限があり、プロジェクト所有者としても指定されます。プロジェクトが別の所有者に割り当てられている場合、そのユーザーはプロジェクトを管理する権限も持ちます。プロジェクト作成者（または所有者）がプロジェクトを他のユーザーと共有する場合、そのユーザーに特定の権限を付与し、プロジェクトでの作業中に実行できる操作を制御します。

  ただし、プロジェクト所有者がプランナーライセンスを持っていない場合、プロジェクトを管理するためのフルアクセス権は持ちません。プロジェクトを管理する権限を持つのは、プランライセンスを持つユーザーのみです。詳しくは、[アクセスレベルと権限の連携方法](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)を参照してください。

* プロジェクトは個別に共有することも、一度に複数共有することもできます。プロジェクトの共有は、他のオブジェクトを共有する場合と同じです。Workfront でのアイテムの共有について詳しくは、[オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。
* プロジェクトに次の権限を付与できます。

   * 表示
   * 管理
   * 参加

     ![](assets/view-on-projects-190x207.png) ![](assets/contribute-on-projects-159x243.png) ![](assets/manage-on-projects-178x230.png)

* プロジェクトを共有する場合、特に指定のない限り、すべてのタスク、イシューおよびドキュメントは同じ権限を継承します。

  プロジェクトに対するユーザーの権限に基づいてプロジェクトでのタスクやイシューへのアクセス権を管理する方法について詳しくは、[プロジェクトの編集](../../manage-work/projects/manage-projects/edit-projects.md)の記事で[](../../manage-work/projects/manage-projects/edit-projects.md#access)の節を参照してください。

  Workfront 管理者は、ドキュメントがユーザーのアクセスレベルの上位のオブジェクトから権限を継承するかどうかを指定できます。ドキュメントに対する継承された権限の制限について詳しくは、[カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

* 子オブジェクトが継承しないように、継承された権限をプロジェクトから削除できます。 継承された権限をオブジェクトから削除する方法について詳しくは、[オブジェクトからの権限の削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)を参照してください。

## プロジェクトを共有する方法 {#ways-to-share-a-project}

プロジェクトは次の方法で共有できます。

* 次のいずれかの操作を行って手動で操作：

   * プロジェクトチームにユーザーを追加。プロジェクトチームにユーザーを追加すると、プロジェクトに対する表示権限が自動的に取得されます。\
     プロジェクトチームにユーザーを追加する方法について詳しくは、[プロジェクトチームの概要](../../manage-work/projects/planning-a-project/project-team-overview.md)の「プロジェクトチームにユーザーを追加」の節を参照してください。
   * プロジェクトを個別に、または一括で共有（「**共有**」オプションを使用する場合）。

     プロジェクトの共有は、Adobe Workfront で他のすべてのオブジェクトを共有する方法と同様です。

     Workfront でのオブジェクトの共有について詳しくは、[オブジェクトを共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。

* 自動的。次のいずれかの操作を行って設定します。

   * 既に他のユーザーと共有されている&#x200B;**ポートフォリオ**&#x200B;または&#x200B;**プログラム**&#x200B;にプロジェクトを配置。ポートフォリオやプログラムに対してユーザーが持っている権限と同じ権限を、プロジェクトに対しても取得します。\
     プロジェクトを&#x200B;**ポートフォリオ**&#x200B;に追加する方法について詳しくは、[ポートフォリオへのプロジェクトの追加](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md)を参照してください。\
     プロジェクトを&#x200B;**プログラム**&#x200B;に追加する方法について詳しくは、[プログラムにプロジェクトを追加](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md)を参照してください。

     オブジェクトに対する継承された権限の表示について詳しくは、[オブジェクトで継承された権限の表示](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)を参照してください。

   * プロジェクトの作成に使用したテンプレートで、プロジェクト共有にエンティティを追加します。テンプレートからプロジェクトを共有する方法については、[テンプレートを共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)を参照してください。
   * プロジェクトアクセステンプレートを定義します。

     プロジェクトアクセステンプレートを定義するには、[オブジェクトを共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。

     >[!TIP]
     >
     >テンプレートを添付または保存する際に、テンプレートプロジェクト共有ルールをクリアできます。

   * プロジェクトを編集し、**このプロジェクトへのアクセス権が付与されたユーザーに**&#x200B;の設定を定義。詳しくは、[プロジェクトの編集](../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)&nbsp;</li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## 各種ライセンスタイプの制限事項

* Worker ライセンスを持つユーザーには、プロジェクトを管理する権限がありません。 作業者の場合、最も高い共有権限は参加です。
* リクエストライセンスを持つユーザーはプロジェクト情報を表示できますが、プロジェクトへのアクセスは制限されています。
* プロジェクトのステータス変更の例外は、表示または参加の権限を持つユーザーが承認プロセスにも含まれている場合に発生します。 プロジェクトを承認すると、プロジェクトのステータスを変更できますが、ステータスは承認または却下の事前定義済みのステータスです。
* プロジェクトをコピーできるようにするには、ユーザーがアクセスレベルでプロジェクトを作成するアクセス権も持っている必要があります。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see&nbsp;<a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can&nbsp;delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.&nbsp;
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## プロジェクト権限オプション

次の表に、ユーザーがプロジェクトを共有する際に付与できる権限を示します。 ユーザーがライセンスに基づいて取得するアクセスについて詳しくは、[プロジェクトへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)を参照してください。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>アクション</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>参加</strong> </p> </th> 
   <th> <p><strong>ビュー</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>カスタムフォームを追加</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>カスタムフィールドを更新</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>承認プロセスを追加</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクトを承認</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>時間を承認</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクトを作成</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>ドキュメントを追加</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>イシューを追加</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスクを追加</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクトのコピー</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクトの削除</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>予定日の変更</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクトを共有</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>システム全体で共有</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクトの表示</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>アップデート／コメント</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>ステータスの変更</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>時間の記録</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>割り当ての編集</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>ベースラインを管理</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>リスクを管理*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>財務の管理*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>費用を追加／編集*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>財務情報を表示*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>テンプレートを添付</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>テンプレートとして保存</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>ビジネスケースを追加／編集</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクト詳細を編集</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>スタッフを編集</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>MS Project にエクスポートする</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>財務／タイムラインを再計算*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>キューのプロパティを設定</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>リストでプロジェクトを一括編集</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;財務データにアクセスできないユーザーは、プロジェクトに対する編集アクセス権を持っていても、プロジェクトのリスクや財務を管理できません。 財務データへのアクセスについて詳しくは、[財務データへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。
