---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: タイムシートプロファイルの作成、編集および割り当て
description: 追加の介入なしに、ユーザーに対して定期タイムシートを生成するタイムシートプロファイルを作成および編集し割り当てることができます。これにより、時間を節約し、ユーザー間の一貫性を確保できます。
author: Lisa
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: b0b9b80b4eb718e3e131ee0cd022f54cb906f187
workflow-type: tm+mt
source-wordcount: '1584'
ht-degree: 68%

---

# タイムシートプロファイルの作成、編集および割り当て

<!--Audited: 06/2025-->

追加の介入なしに、ユーザーに対して定期タイムシートを生成するタイムシートプロファイルを作成および編集し割り当てることができます。これにより、時間を節約し、次の情報についてユーザー間で一貫性を保つことができます。

* タイムシートの時間枠
* 承認者
* 一般的な時間タイプ

タイムシートを手動で作成する方法について詳しくは、[1 回限りのタイムシートの作成](../../timesheets/create-and-manage-timesheets/create-tmshts.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><p>タイムシートへの管理アクセス</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タイムシートプロファイルを作成または編集

<!--Old info: 
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>現在のタイムシートでタイムシート プロファイルの変更を有効にするには、タイムシート プロファイルを変更する前に既存のタイムシートを削除し、新しいタイムシートを生成する必要があります。 手順については、[Adobe Workfront のタイムシートの削除](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)および[タイムシートを手動で生成](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)を参照してください。

{{step-1-to-setup}}

1. システム全体で使用するタイムシート プロファイルを作成または編集する場合は、[**タイムシートおよび時間**] をクリックします。

   または

   グループのタイムシート プロファイルを作成または編集する場合は、[**グループ**] をクリックし、グループ名をクリックします。

1. 「**定期タイムシート**」をクリックします。
1. 定期タイムシートを作成するには、[**新規プロファイル**] をクリックします。

   または

   既存のタイムシートプロファイルを編集するには、編集するタイムシートプロファイルを選択し、「**編集**」をクリックします。

   新規または既存の定期タイムシート ページが表示されます。

1. 次の情報を更新します。

   * **名前**：タイムシートプロファイルの名前を追加します。 タイムシートと同じ期間を共有するユーザーがいるチームまたはグループの名前を指定できます。 必須フィールドです。
   * **説明**：定期タイムシートの詳細情報を追加します。
   * **管理アクセス権限を持つグループ**：システムレベルのタイムシートプロファイルを作成する場合は、このフィールドを空白のままにします。

     ユーザーアカウントを編集できるユーザーは、システムレベルのタイムシートを他のユーザーに添付できます。

     システムレベルのタイムシートプロファイルを編集できるのは、Workfront 管理者だけです。

     管理しているグループのタイムシートプロファイルを作成する場合は、ここでグループを指定します。

     この操作を実行しても、グループ内のユーザーにタイムシートプロファイルは割り当てられません。グループの管理者がタイムシートプロファイルを変更できるだけです。手順 6 で、プロファイルをユーザーに割り当てます。

     >[!NOTE]
     >
     >グループ外のユーザーがタイムシート プロファイルを他のユーザーに添付する場合、このタイムシート プロファイルを表示または添付することはできません。

   * **タイムシートを作成**：タイムシートプロファイルがタイムシートを生成するタイミングを指定します。 タイムシートは、週ごと、2 週間ごと、半月ごと、月ごとに自動生成するよう設定できます。タイムシートを生成する曜日を選択します。

     週ごとのタイムシートは、タイムシートの生成日に開始します。例えば、毎週木曜日に週次のタイムシートを作成する場合、タイムシートの週の最初の曜日は木曜日になります。

     >[!NOTE]
     >
     >Workfront は常に 2 つのタイムシートを一度に作成します。最初のタイムシートには常に現在の日付が含まれ、2 番目のタイムシートは最初のタイムシートの期間が終わった時点で開始されます。

   * **承認者**：承認者は、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。 タイムシートでは、最大 7 人のユーザーを承認者として指定できます。複数のユーザーを指定しておくと、承認者の不在時に別の承認者を確実に利用することができます。ユーザーがタイムシートを承認のために送信すると、すべての承認者に通知が届きます。タイムシートの承認に必要なのは、1 人のユーザーの承認のみです。

     承認者として設定できるのは、タイムシートの管理権限を持つユーザーのみです。タイムシートの管理権限について詳しくは、[ユーザーに対する特定のエリアへの管理アクセス権の付与](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

     ドロップダウンメニューを使用して、タイムシートの承認者を選択します（承認者が必要な場合）。 以下のオプションから選択できます。

      * **なし**：タイムシートを承認する必要はありません。
      * **マネージャー**：これは、システムによって設定されるデフォルトの承認者です。マネージャーとして指定されたユーザーが、承認を受けるために送信されたタイムシートを承認します。
      * **特定のユーザー**：特定のユーザーを名前で、タイムシート承認者として指定できます。 1 つのタイムシートに複数の承認者を設定できます。この場合、承認者のうちの 1 人がタイムシートを承認すると、タイムシートは&#x200B;**クローズ**&#x200B;とマークされ、残りのすべての承認者のタイムシート承認リストに表示されなくなります。

   * **時間を編集可能**：承認者がタイムシートの時間を編集できるようにするには、このオプションを選択します。

     これは、設定／タイムシートと時間／環境設定領域の「**タイムシートの編集を所有者と管理者に制限**」とともに機能します。詳しくは、[タイムシートと時間の環境設定の構成](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

     次のシナリオが存在します。

     「**タイムシートの編集を所有者と管理者に制限**」オプションが有効な場合は、以下のようになります。

      * 承認者は、[ 時間の編集が可能 ] が有効になっているかどうかに関係なく、タイムシートの承認と拒否のみ行うことができます。
      * タイムシート所有者のマネージャーは、自分のダイレクトレポートのタイムシートのみを表示できます。

     「**タイムシートの編集を所有者と管理者に制限**」オプションが無効である場合は、以下のようになります。

      * **時間を編集可能** が有効になっている場合、承認者はタイムシートを送信、再オープンまたはクローズし、時間を編集できます。
      * **時間を編集可能** が無効になっている場合、承認者はタイムシートを送信、再オープンまたはクローズできず、時間を編集できません。 承認者が行えるのは、タイムシートの承認または却下のみです。
      * タイムシート所有者のマネージャーは、ダイレクトレポートのタイムシートの提出、取り消し、リオープン、編集を行うことができます。

     >[!NOTE]
     >
     >承認を受けるためにタイムシートを送信すると、時間を編集できなくなります。提出されたタイムシートを編集可能な状態に戻すには、タイムシートを取り消すか、承認者にタイムシートを却下させます。詳しくは、[承認を受けるためのタイムシートの送信](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)と[タイムシートの承認](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md)を参照してください。

   * **超過作業時間**: タイムシートで「超過作業時間」ボックスを非表示にするよう選択できます。 このオプションはデフォルトでは無効になっています。
   * **利用可能な時間タイプ**：この設定は、一般的な時間タイプのみを対象としており、プロジェクト固有の時間タイプは対象としていません。

     デフォルトでは、タイムシートのすべての一般的な時間がユーザーに表示されます。ただし、特定のユーザーセットに対して特定の一般的な時間のみを表示する場合は、このフィールドのタイムシートプロファイルで選択することにより、タイムシートに表示する必要のある一般的な時間を選択できます。すべての一般的な時間を無効にする場合は、すべての時間タイプの選択を解除して、一般的な時間のセクションを含まないタイムシートを生成します。

   * **リマインダー通知**：リマインダー通知を追加します。 Workfrontからユーザーにリマインダーを送信し、タイムシートの入力や承認を求めます。 リマインダ通知を作成してから、タイムシートプロファイルに関連付けてください。

1. タイムシートプロファイルを特定のユーザー、グループまたは（Workfront管理者の場合）チームに関連付けるには、ページの下部までスクロールして、「ユーザーを割り当て **セクションを見つけ** す。

   ユーザー、グループ、またはチームの名前の入力を開始し、ドロップダウンリストに表示されたらクリックします。

   <!--To associate the timesheet profile with specific users, groups, or (if you are a Workfront administrator) teams, scroll towards the bottom of the page and find the **Assign People** section.-->

   グループ管理者は、自分が管理するグループにタイムシートプロファイルを割り当てることができますが、チームに割り当てることはできません。詳しくは、この記事内の[タイムシートプロファイルを割り当てるグループ管理者の制限](#limitations-for-a-group-administrator-assigning-a-timesheet-profile)を参照してください。

   >[!NOTE]
   >
   >* また、ユーザープロファイルを編集することで、ユーザーをタイムシートプロファイルに関連付けることもできます。詳しくは、[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。
   >* グループを追加すると、「ユーザーを割り当て」タブにはグループ名のみが表示され、グループメンバーのリストは表示されません。ここにリスト表示されるグループメンバーを確認するには、「変更を保存」をクリックし、作成したばかりのタイムシートプロファイルの名前をクリックします。
   >* この手順を完了すると、タイムシートプロファイルは、現在の期間の既存のタイムシートを持たない、割り当てられたユーザーやグループメンバーに対してのみタイムシートを生成します。

1. 「**保存**」をクリックします。

1. タイムシートプロファイルリストの上部で、「**その他**」アイコン ![ その他アイコン ](assets/more-icon.png) をクリックし、「**タイムシートを生成**」をクリックします。

   タイムシートが正常に生成されたことを示す確認が画面の下部に表示されます。 作成した新規プロファイルに基づいて、新しいタイムシートが生成されます。

   詳しくは、「[ タイムシートを手動で生成する ](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)」を参照してください。

   タイムシートプロファイルで初めてタイムシートが生成されると、現在の時間を含む期間と次の期間の両方について、ユーザーごとに 2 つのタイムシートが作成されます。

   その後、新しいタイムシートを生成するたびに、ユーザーごとに 1 つのタイムシートが作成されます。

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## タイムシートプロファイルを割り当てるグループ管理者の制限事項 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

グループ管理者で、管理アクセスオプションの「タイムシートと時間」がアクセスレベルで無効になっている場合は、タイムシートプロファイルは作成できますが、割り当ては以下に対してのみ行うことができます。

* 自分が管理するグループ
* 自分が管理するグループ内の個々ユーザー（ユーザーに対する編集のためのアクセス権がある）

これらのグループとユーザーに関しては、タイムシートプロファイルが生成するタイムシートに対するアクセス権がありません。

さらに、アクセスレベルで「ユーザー管理者（グループユーザー）」オプションも無効になっている場合は、自分が管理するグループにタイムシートプロファイルを割り当てることができますが、影響を受けるのは、自分が編集アクセス権を持つグループ内のユーザーのみです。ユーザーに対して編集アクセス権のないユーザーがグループに含まれている場合、そのユーザーには、グループの他のメンバーとともにはタイムシートプロファイルが割り当てられません。

アクセスレベルの「タイムシートと時間」オプションについて詳しくは、[特定のエリアに対する管理者アクセス権のユーザーへの付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

アクセスレベルの「ユーザー管理者（グループユーザー）」オプションについて詳しくは、[ユーザーへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

## 複数の繰り返しタイムシートプロファイル

以下が該当する場合、組織向けに複数のタイムシートプロファイルを持つことができます。

* 異なるユーザーのセットに対する一意の支払期間
* 異なるユーザーのセットに対する一意の承認者
* 異なるユーザーのセットに対する一意の一般的な時間数の要件

1 人のユーザーを一度に複数のタイムシートプロファイルに関連付けることはできません。

<!--
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p> Add a name for the timesheet profile. It could be the name of a team or a group whose people share the same timeframe for their timesheets. </p> <p>This ia a required field.</p> </td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td> <p> Add more information about the timesheet profile.     
      </p> </td> 
     </tr>

   <tr> 
   <td role="rowheader"><strong>Group with Administration Access</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>If you are creating a system-level timesheet profile, leave this field blank.</p> <p>Any user who can edit user accounts can attach a system-level timesheet to other users.</p> <p>Only a Workfront administrator can edit a system-level timesheet profile.</p> </li> 
      </ul> 
     <ul> 
      <li> <p>If you are creating a timesheet profile for a group you administer, identify the group here.</p> <p>This does not assign the timesheet profile to the users in the group; it only allows the group's administrators to modify the timesheet profile. You will assign the profile to users in Step 6.</p>

   <p><b>NOTE</b>: When users outside the group are attaching timesheet profiles to other users, they won't be able to see or attach this timesheet profile.</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Create timesheets</strong> </td> 
      <td> <p> <p>Specify when the timesheet profile should generate the timesheets. A timesheet can be set to automatically generate on a weekly, bi-weekly, semi-monthly, or monthly basis. Select the day of the week when you want the timesheet to be produced.</p>
      <p>A weekly timesheet begins on the date it is generated. For example, if you create weekly timesheets every Thursday, the first day of the week on the timesheet is Thursday.</p>
    
      
   <p><b>NOTE</b>: Workfront always creates two timesheets at a time: the first timesheet always includes the current date, and the second timesheet starts when the time frame of the first one ends.</p> </p> </td> 
   </tr> 
     <tr> 
      <td role="rowheader"><p><strong>Approvers</strong></p> </td> 
      <td> <p> <p>Approvers are users who approve the timesheet for the users associated with the timesheet. You can identify up to 7 users as approvers on a timesheet. Identifying multiple users is useful to ensure an approver is available when someone is out of the office. All approvers are notified when a user submits the timesheet for approval. Only one user is required to approve the timesheet in order for it to be approved.</p> <p>Only users with timesheet administrative rights can be set as approvers. For more information about timesheet administrative rights, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Use the drop-down menu&nbsp;to select&nbsp;the approver&nbsp;for the timesheet (if an approver is required). You can select from the following options:</p> 
      <ul> 
      <li><strong>None</strong>: The timesheet does not need to&nbsp;be approved.</li> 
      <li><strong>Their Manager</strong>: This is the default approver, set by the system. In this case, the user designated as their manager approves the timesheet when it is submitted for approval.</li> 
      <li><strong>Specific People:</strong>&nbsp;You can designate specific users, by name, as timesheet approvers. You can have multiple approvers on a timesheet. In this case, after&nbsp;one of the approvers approves the timesheet, the timesheet is marked as <strong>Closed</strong> and it disappears from the timesheet approvals list of all the remaining approvers.</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Can edit time </strong> </td> 
      <td> <p> <p>Select this option to allow the approvers to edit hours on the timesheet. 

   <p>This option works together with the **Restrict timesheet editing to owners and admins** setting in the Setup > Timesheet & Hours > Preferences area. For more information, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">Configure timesheet and hour preferences</a>.</p>

   <p>The following scenarios exist: </p>

   <ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is enabled:</li>
      <ul><li>Approvers can only approve and reject timesheet, regardless of whether the <b>Can edit time</b> is enabled or not. </li>
      <li>Timesheet owners' managers can only view their direct reports' timesheets.</li></ul>
      <li>When the <b>Restrict timesheet editing to owners and admins</b> option is disabled:</li>
    <ul><li>When the <b>Can edit time</b> is enabled, approvers can submit, reopen, or close the timesheet and can edit the time.</li>
      <li>When the <b>Can edit time</b> is disabled, approvers cannot submit, reopen, or close the timesheet and cannot edit the time. Approvers can only approve or reject the timesheet. </li>
      <li>Timesheet owners' managers can submit, recall, reopen, and edit their direct reports' timesheets.</li></ul>
      </ul>

   <p>

   <b>NOTE</b>: Once you submit a timesheet for approval, you can no longer edit the hours. To return a submitted timesheet to an editable state, recall the timesheet or have the approver reject the timesheet. For more information, see <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">Submit a timesheet for approval</a> and <a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">Approve a timesheet</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Overtime</strong> </td> 
      <td>You can choose to hide the Overtime box in timesheets. This option is disabled by default.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Available Hour Types</strong> </td> 
      <td><p>This setting refers only to General Hour Types, and not to project-specific hour types. </p>
      <p>By default, users see all general hours on a timesheet. However, if your organization wants only specific general hours to be shown for a particular set of users, you can select the general hours that they need to see in their timesheets by selecting them in their timesheet profile in this field. If you want to disable all general hours, deselect all hour types to generate the timesheet without a section for general hours.</p></td> 
     </tr> 

   <tr> 
      <td role="rowheader"><strong>Reminder notifications</strong> </td> 
      <td> <p> Add a reminder notification. Workfront will send reminders to users to ask them to complete or approve their timesheets. You must create reminder notifications before you can associate them with a timesheet profile.  </p> </td> 
     </tr>
    </tbody> 
   </table>
-->