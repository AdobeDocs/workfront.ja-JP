---
title: 特定の領域への管理者アクセス権をユーザーに付与する
description: Adobe Workfront 管理者は、アクセスレベルを使用して、プランライセンスを持つユーザーに、システムの特定の領域への管理アクセス権を付与できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
TQID: https://experienceleague.adobe.com/1nXA0NxLQW3tiIrhCKAd5EMfqBjQW68GHNN42dQmptQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9041e7a1c1bf6f7909039fe238b4564ab204752c
workflow-type: tm+mt
source-wordcount: 714
ht-degree: 87%

---

# 特定の領域に対する管理アクセス権をユーザーに付与

{{preview-fast-release-general}}

<!--Linked in several places, do not rename or change URL.-->

Adobe Workfront管理者は、アクセスレベルを使用して、StandardまたはPlan ライセンスのユーザーにシステムの特定の領域への管理アクセス権を付与できます。

>[!NOTE]
>
>これは、[ユーザーに完全な管理アクセス権を付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)で説明されている、Workfront に対する完全な管理アクセス権をユーザーに付与することとは異なります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>   <p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfrontの特定の領域への標準またはプランのユーザーの管理アクセス権を付与する

>[!IMPORTANT]
>
>ユーザーを設定した後で参照できるように、ビルトインのアクセスレベルを変更しないことを強くお勧めします。 アクセスレベルをカスタマイズするには、デフォルトのアクセスレベルをコピーし、そのコピーを変更します。 （システム管理者と外部ユーザーを除くすべてのアクセスレベルで、これを実行できます）。

{{step-1-to-setup}}

1. 左側のパネルで、「**アクセスレベル**」をクリックします。
1. Workfront の特定の領域への管理アクセス権をユーザーに付与するために使用する、アクセスレベルの名前をクリックします。
1. 「**管理アクセス権を許可**」セクションで、必要な管理アクセス権を許可するチェックボックスをオンにします。

   これらのオプションを使用すると、次の機能を付与できます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認プロセス</td> 
      <td><p>システム全体および特定のグループで使用する承認プロセスを作成および管理します。</p><p>このアクセス権がない場合、ユーザーは、管理するアクセス権を持つ項目に対して、アドホック承認プロセスのみを作成できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="preview">変更履歴</span></td> 
      <td><p><span class="preview">設定/変更履歴/変更履歴リストでWorkfrontの変更履歴ログを表示します。</span></p>
      <p><span class="preview">このアクセス権がなければ、ユーザーは設定領域にこのオプションを持ちません。</span></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">会社</td> 
      <td><p>Workfront で、新しい会社を追加および既存の会社を編集します。</p>
      <p>このアクセス権がない場合、ユーザーは既存の会社のみを表示できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムフォーム</td> 
      <td><p>グループ内でカスタムフォームを作成および編集（フィールドを追加、編集、削除）します。</p><p>このアクセス権がない場合、ユーザーは、参加や管理のアクセス権を持つオブジェクトに対してのみ、既存のフォームを添付できます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">為替レート</td> 
      <td> <p>Workfront に新しい通貨を追加します。</p> <p>このアクセス権がない場合、ユーザーは作成するプロジェクトに既存の通貨のみを追加できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">費用</td> 
      <td><p>Workfront のオブジェクトに関するすべての費用を表示します。</p><p>この場合、ユーザーは新しい費用タイプを作成できません。</p><p>このアクセス権がない場合、ユーザーは次の項目のみを表示できます。</p>
       <ul>
        <li>管理するプロジェクト、タスクまたはイシューに関する費用</li>
        <li>自身の費用</li>
        <li>部下の費用</li>
       </ul></td> 
     </tr>
     <tr> 
      <td role="rowheader">マイグループのマイルストーン</td> 
      <td>「設定」のマイルストーンパスメニューで、システム内のすべてのマイルストーンパスを表示します。 ユーザーは、自分のグループに属するマイルストーンパスを編集または削除することもできます。 ユーザーは、どのグループにも割り当てられていないマイルストーンパスを管理（編集または削除）することができません。<br><p>このアクセス権がない場合、ユーザーは既存のマイルストーンパスを表示し、管理するアクセス権を持つプロジェクトに適用することのみ可能です。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">リマインダー通知</td> 
      <td>Workfrontでリマインダー通知を作成および管理します。<br>このアクセス権を持たないユーザーは、通知の受信と表示に限定されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムシートと時間数</td> 
      <td> <p>ユーザーが Workfront ですべての時間数とタイムシートを表示できるようにします。</p> <p>このオプションを無効にすると、ユーザーは以下を数時間数しか表示できなくなります。</p> 
       <ul> 
        <li>自分が管理するプロジェクト、タスクまたはイシュー</li> 
        <li>自分のタイムシート</li> 
        <li>自分に報告するユーザーのタイムシート</li> 
        <li>自分が承認したタイムシート</li> 
       </ul> <p><b>メモ</b>:  <p>このオプションが有効か無効かに関係なく、グループ管理者は、管理するグループとサブグループのタイムシートプロファイルを作成し、ユーザープロファイルの編集アクセス権を持つグループメンバーにそれらのプロファイルを割り当てることができます。</p> <p>このオプションを有効にすると、一部のグループ管理者に過剰なアクセス権が付与される場合があります。これは、タイムシートプロファイルによって生成されたタイムシート（および時間）が、管理者が管理するグループのユーザーだけでなく、システム内のすべてのユーザーに表示されるからです。 こうしたアクセス権が必要ないグループ管理者に対しては、このオプションを無効にすることができます。</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 完了したら「**保存**」をクリックします。
1. [ユーザーの追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)で説明されているように、ユーザーに新しいアクセスレベルを割り当てます。

   >[!NOTE]
   >
   >ユーザーに対する管理アクセス権をユーザーに付与できます。 ユーザーに管理アクセス権を付与してユーザーアカウントを管理できるようにする方法について詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->

<!--
## Access of a Workfront administrator vs. access of a Standard or Plan user with administrative rights  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

The two tables below show the difference between the access rights of a user with a Workfront System Administrator access level versus those of a user with a Standard or Plan license with some administrative rights.

Workfront administrators can view all the objects in the system (regardless of who created them), create new ones, and modify or delete existing ones. They have full access to all objects in the system.

Users with a Standard or Plan license who can edit functionality in one area have full access to the functionality in that area.

>[!NOTE]
>
>Users with a Standard or Plan license who are designated as group administrators can perform some of the actions allowed for Workfront administrators. They are allowed to perform these actions only for the groups they administer, their subgroups, and the users in these groups and subgroups. For more information, see [Group administrators](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Access to the Setup area](#access-to-the-setup-area)
* [Access to objects](#access-to-objects)

### Access to the Setup area {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Standard or Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Project Preferences: Projects</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Tasks &amp; Issues</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Statuses</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Priorities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Severities</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Project Preferences: Exchange Rates</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Approvals</td> 
   <td> <p>Full access</p> </td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Processes: Milestone Paths</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Custom Forms</td> 
   <td>Full access</td> 
   <td> <p>Manage custom forms they created or custom forms shared with them.</p> <p>Attach custom forms they created or custom forms shared with them to objects they have manage or contribute permissions to.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Deleted</td> 
   <td>Full access</td> 
   <td> <p>Users who are group administrators can restore projects assigned to Groups they manage, and tasks, issues, or documents associated with those projects.</p> </td> 
  </tr> 
  <tr> 
   <td>Recycle Bin: Recently Restored</td> 
   <td>Full access</td> 
   <td>Users who are group administrators can see the items they have recently restored.</td> 
  </tr> 
  <tr> 
   <td>Job Roles</td> 
   <td>Full access</td> 
   <td> <p>Modify but not delete existing job roles.</p> <p>Add new job roles.</p> </td> 
  </tr> 
  <tr> 
   <td>Teams</td> 
   <td>Full access</td> 
   <td> <p>No access to create Teams.</p> <p>Add existing teams to users when creating or editing users.</p> </td> 
  </tr> 
  <tr> 
   <td>Groups</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groups.</p> <p>Only group administrators can manage group membership, subgroups, and group-level statuses for the groups they manage. </p> </td> 
  </tr> 
  <tr> 
   <td>Companies</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Log in As</td> 
   <td>Full access </td> 
   <td> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator, they can log in as the users in the group they administer and their subgroups. They cannot log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Schedules</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Schedules.</p> <p>Access to add existing schedules to other users, at the user level. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Timesheet Profiles</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Timesheet Profiles to users, at the user level.</p> <p>Users who are group administrators can create Timesheet Profiles for the groups they administer and their subgroups. </p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Hour Types</td> 
   <td>Full access</td> 
   <td> <p>Access to assign Hour Types to users, at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Timesheet &amp; Hours: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Event Notifications</td> 
   <td>Activate/ Deactivate all</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Reminder Notifications</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Email: Notifications: Email Templates</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Templates.</p> <p>Access to add existing Email Templates to Reminder Notifications.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Automatic Reminders</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Email: Invitations</td> 
   <td>Full access</td> 
   <td> <p>No access to edit Email Invitations.</p> <p>Access to resend email invitations to unregistered users only from the People tab.</p> </td> 
  </tr> 
  <tr> 
   <td>Email: Setup</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Scorecards</td> 
   <td>Full access</td> 
   <td> <p>Full access</p> </td> 
  </tr> 
  <tr> 
   <td>Expense Types</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Risk Types</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Access Levels</td> 
   <td> <p>Full access to modify all access levels.</p> <p>The System Administrator and External User access levels cannot be modified, by default.</p> </td> 
   <td> <p>No access to edit Access Levels.</p> <p>Assign an access level to other users which is lower or equal to theirs at the user level.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Layout Templates</td> 
   <td>Full access</td> 
   <td> <p>Access to assign existing Layout Templates to other users, at the user level. </p> <p>Users designated as group administrators can create Layout Templates for groups and subgroups they manage.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Update Feeds</td> 
   <td>Full access</td> 
   <td> <p>No access to modify Update Feeds.</p> <p>Access to add fields to be tracked in the Update Feeds when editing Custom Forms.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Filters</td> 
   <td>Full access</td> 
   <td> <p>No access to create Filters in the Setup area.</p> <p>Access to create new filters in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Views</td> 
   <td>Full access</td> 
   <td> <p>No access to create Views in the Setup area.</p> <p>Access to create new views in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: Groupings</td> 
   <td>Full access</td> 
   <td> <p>No access to create Groupings in the Setup area.</p> <p>Access to create new groupings in a list of objects.</p> </td> 
  </tr> 
  <tr> 
   <td>Interface: List Controls</td> 
   <td>Full access</td> 
   <td> <p>No access</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Cloud Providers</td> 
   <td>Full access</td> 
   <td> <p>No access to configure Cloud Providers.</p> <p>Access to link documents to and from Cloud Providers from the Documents tab, after the Cloud Providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Metadata Mapping</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>Documents: SharePoint Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a SharePoint integration.</p> <p>Access to link documents to and from SharePoint from the Documents tab, after the SharePoint integration with Workfront has been configured.</p> </td> 
  </tr> 
  <tr> 
   <td>Documents: Custom Integration</td> 
   <td>Full access</td> 
   <td> <p>No access to configure a Custom Integration.</p> <p>Access to link documents to and from third-party providers from the Documents tab, after the third-party providers have been integrated with Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>System: Branding</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Customer Info</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Single Sign-On (SSO)</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Update Users for SSO</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Kick-Starts</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Diagnostics</td> 
   <td>Full access</td> 
   <td>No access</td> 
  </tr> 
  <tr> 
   <td>System: Preferences</td> 
   <td>Full access</td> 
   <td>No access</td> 
  <tr> 
   <td>Change Tracking: Configuration</td> 
   <td>Full access</td> 
   <td>No access</td> 
  <tr> 
   <td>Change Tracking: Change History List</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
 </tbody> 
</table>

### Access to objects {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area/object</th> 
   <th>Workfront administrator </th> 
   <th>User with a Standard or Plan license and some administrative rights</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Calendars</td> 
   <td>Full access</td> 
   <td>Manage calendars they create and calendars shared with them.</td> 
  </tr> 
  <tr> 
   <td>Dashboards</td> 
   <td>Full access</td> 
   <td>Manage dashboards they create and dashboards shared with them.</td> 
  </tr> 
  <tr> 
   <td>Documents</td> 
   <td>Full access</td> 
   <td>Manage documents they upload or documents shared with them.</td> 
  </tr> 
  <tr> 
   <td>Issues</td> 
   <td>Full access</td> 
   <td>Manage issues they create or issues shared with them.</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Full access</td> 
   <td>Manage portfolios they create or portfolios shared with them. </td> 
  </tr> 
  <tr> 
   <td>Programs</td> 
   <td>Full access</td> 
   <td>Manage programs they create or programs shared with them.</td> 
  </tr> 
  <tr> 
   <td>Project</td> 
   <td>Full access</td> 
   <td>Manage projects they create or projects shared with them.</td> 
  </tr> 
  <tr> 
   <td>Reports</td> 
   <td>Full access</td> 
   <td>Manage reports they create or reports shared with them. View, copy and edit system reports.</td> 
  </tr> 
  <tr> 
   <td>Tasks</td> 
   <td>Full access</td> 
   <td>Manage tasks they create or tasks shared with the</td> 
  </tr> 
  <tr> 
   <td>Templates</td> 
   <td>Full access</td> 
   <td>Manage templates they create or templates shared with them</td> 
  </tr> 
  <tr> 
   <td>Timesheets</td> 
   <td>Full access</td> 
   <td>Full access</td> 
  </tr> 
  <tr> 
   <td>Users</td> 
   <td>Full access</td> 
   <td> <p>Limited access</p> <p>They cannot assign groups to users for which they are not a group administrator or groups that are not public.</p> <p>They cannot assign an access level to users which is higher then their own access level.</p> <p>If their group administrative access is enabled on their access level and they are designated as a group administrator on a group, they can reset the password of and log in as the users in the group they administer and their subgroups. They cannot reset the password of or log in as a System Administrator.<br>For more information about enabling group administrative access for users, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->


