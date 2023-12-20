---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: タイムシートプロファイルの作成、編集、割り当て
description: ユーザーからの追加の介入なしに、ユーザーに対して定期的なタイムシートを生成するタイムシートプロファイルを作成、編集、割り当てることができます。 これにより、時間を節約し、ユーザー間の一貫性を確保できます。
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 3983f82dfa668c3fcb0948a759ba47a76ec52f86
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 0%

---

# タイムシートプロファイルの作成、編集、割り当て

ユーザーからの追加の介入なしに、ユーザーに対して定期的なタイムシートを生成するタイムシートプロファイルを作成、編集、割り当てることができます。 これにより、時間を節約し、次の情報をユーザー間で一貫性を保つことができます。

* タイムシートの期間
* 承認者
* 一般的な時間タイプ

タイムシートを手動で作成する方法の詳細については、「 [単一使用のタイムシートを作成する](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>新規：標準 </p>
 <p>または</p> 
<p>現在：プラン </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タイムシートに対する管理者アクセス権が必要です。 </p> <p>詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## タイムシートプロファイルを作成または編集する

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>現在のタイムシートのタイムシートプロファイルの変更を有効にするには、既存のタイムシートを削除してから、新しいタイムシートを生成する必要があります。 手順については、 [Adobe Workfrontのタイムシートを削除](../../timesheets/create-and-manage-timesheets/delete-timesheets.md) および [タイムシートを手動で生成する](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

{{step-1-to-setup}}

1. システム全体で使用するタイムシートプロファイルを作成または編集する場合は、[ ] をクリックします。 **タイムシートと時間**.

   または

   グループのタイムシートプロファイルを作成または編集する場合は、 **グループ**&#x200B;をクリックし、グループの名前をクリックします。

1. クリック **タイムシートプロファイル**.
1. 新しいタイムシートプロファイルを作成するには、次をクリックします。 **新しいプロファイル**.

   または

   既存のタイムシートプロファイルを編集するには、編集するタイムシートプロファイルを選択し、[ ] をクリックします **編集**.

   新規または既存のタイムシートプロファイルが表示されます。


1. 次の日： **詳細を設定** タブ、入力 **名前** および **説明** タイムシートプロファイルに次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>管理アクセス権を持つグループ</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>システムレベルのタイムシートプロファイルを作成する場合は、このフィールドを空白のままにします。</p> <p>ユーザーアカウントを編集できるユーザーは、システムレベルのタイムシートを他のユーザーに添付できます。</p> <p>システムレベルのタイムシートプロファイルを編集できるのは、Workfront管理者だけです。</p> </li> 
      </ul> 
     <ul> 
      <li> <p>管理しているグループのタイムシートプロファイルを作成する場合は、ここでグループを指定します。</p> <p>この操作を実行しても、グループ内のユーザーにタイムシートプロファイルが割り当てられるわけではありません。グループの管理者がタイムシートプロファイルを変更できるのは、グループの管理者だけです。 手順 6 で、プロファイルをユーザーに割り当てます。</p>

   <p><b>注意</b>：グループ外のユーザーがタイムシートプロファイルを他のユーザーに添付すると、このタイムシートプロファイルを表示または添付できなくなります。</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>タイムシートを作成</strong> </td> 
      <td> <p> <p>タイムシートプロファイルがタイムシートを生成するタイミングを指定します。 タイムシートは、週単位、週単位、月単位、月単位で自動的に生成するように設定できます。 タイムシートを作成する曜日を選択します。</p>
      <p>週別タイムシートは、生成された日に開始されます。 たとえば、毎週木曜日に週別タイムシートを作成する場合、タイムシートの週の最初の曜日は木曜日になります。</p>


   <p><b>注意</b>:Workfrontは常に 2 つのタイムシートを一度に作成します。最初のタイムシートには常に現在の日付が含まれ、2 番目のタイムシートは最初のタイムシートの期間が終わるときに開始します。</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>承認者</strong></p> </td> 
      <td> <p> <p>承認者は、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。 タイムシートでは、最大 7 人のユーザーを承認者として識別できます。 複数のユーザーを識別すると、不在時に承認者を確実に使用できます。 ユーザーがタイムシートを承認用に送信すると、すべての承認者に通知が送信されます。 タイムシートを承認するには、1 人のユーザーのみがタイムシートを承認する必要があります。</p> <p>タイムシート管理権限を持つユーザーのみが承認者として設定できます。 タイムシート管理権限の詳細については、「 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> <p>ドロップダウンメニューを使用して、タイムシートの承認者を選択します（承認者が必要な場合）。 次のオプションから選択できます。</p> 
      <ul> 
      <li><strong>なし</strong>：タイムシートを承認する必要はありません。</li> 
      <li><strong>彼らの支配人</strong>：これは、システムによって設定されるデフォルトの承認者です。 この場合、管理者として指定されたユーザーが、承認用にタイムシートを送信する際にタイムシートを承認します。</li> 
      <li><strong>特定の担当者：</strong> 特定のユーザーを名前でタイムシートの承認者として指定できます。 1 つのタイムシートに複数の承認者を設定できます。 この場合、承認者の 1 人がタイムシートを承認すると、タイムシートは次のようにマークされます。 <strong>閉じる</strong> 残りのすべての承認者のタイムシート承認リストに表示されなくなります。</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>時間を編集可能 </strong> </td> 
      <td> <p> <p>承認者がタイムシートの時間を編集できるようにするには、このオプションを選択します。

   このオプションは、 **タイムシートの編集を所有者と管理者に制限する** [ 設定 ] > [ タイムシートと時間 ] > [ 基本設定 ] 領域で設定します。 詳しくは、 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">タイムシートと時間の基本設定を構成する</a>.

   次のシナリオが存在します。

   <ul>
      <li>次の場合に <b>タイムシートの編集を所有者と管理者に制限する</b> オプションは有効です。</li>
      <ul><li>承認者は、タイムシートの承認と拒否を実行できます。タイムシートの承認と拒否は、 <b>時間を編集可能</b> が有効かどうか。 </li>
      <li>タイムシート所有者のマネージャは、自分の直属のレポートのタイムシートのみを表示できます。</li></ul>
      <li>次の場合に <b>タイムシートの編集を所有者と管理者に制限する</b> オプションは無効です。</li>
    <ul><li>次の場合に <b>時間を編集可能</b> が有効になっている場合、承認者はタイムシートを送信、再度開く、または閉じて、時間を編集できます。</li>
      <li>次の場合に <b>時間を編集可能</b> が無効になっている場合、承認者はタイムシートを送信、再度開く、または閉じることができず、時間を編集できません。 承認者は、タイムシートの承認または拒否のみを行うことができます。 </li>
      <li>タイムシート所有者のマネージャは、自分の直属の部下のタイムシートを提出、取り消し、再度開き、編集することができます。</li></ul>
      </ul>

   <p>

   <b>注意</b>：タイムシートを承認用に送信すると、時間を編集できなくなります。 提出されたタイムシートを編集可能な状態に戻すには、タイムシートを取り消すか、承認者にタイムシートを拒否させます。 詳しくは、 <a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">承認用のタイムシートを送信</a> および<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">タイムシートを承認</a>.</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>利用可能な時間タイプ</strong> </td> 
      <td><p>この設定は、一般的な時間の種類のみを参照し、プロジェクト固有の時間の種類は参照しません。 </p>
      <p>既定では、ユーザーはタイムシートの全一般時間を表示します。 ただし、特定のユーザーセットに対して特定の一般時間のみを表示する場合は、このフィールドのタイムシートプロファイルで、タイムシートに表示する必要のある一般時間を選択できます。 すべての一般時間を無効にする場合は、すべての時間タイプの選択を解除して、一般時間のセクションを含まないタイムシートを生成します。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">残業</span> </td> 
      <td>タイムシートの [ 超過時間 ] ボックスを非表示にすることもできます。 このオプションはデフォルトでは無効になっています。</td> 
     </tr> 
    </tbody> 
    </table>

1. 次をクリック： **担当者の割り当て** タブを使用して、タイムシートプロファイルを特定のユーザー、グループ、または (Workfront管理者の場合は ) チームに関連付けます。 ユーザー、グループ、またはチームの名前を入力し始め、ドロップダウンリストに表示されたらクリックします。

   グループ管理者は、タイムシートプロファイルを管理グループに割り当てることができますが、チームに割り当てることはできません。 詳しくは、 [タイムシートプロファイルを割り当てるグループ管理者の制限](#limitations-for-a-group-administrator-assigning-a-timesheet-profile) 」を参照してください。

   >[!NOTE]
   >
   >* また、ユーザープロファイルを編集することで、ユーザーをタイムシートプロファイルに関連付けることもできます。 詳しくは、 [ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
   >* グループを追加すると、グループ名のみが「担当者を割り当て」タブに表示され、グループメンバーのリストには表示されません。 ここに表示されるグループメンバを確認するには、[ 変更の保存 ] をクリックし、作成したタイムシートプロファイルの名前をクリックします。
   >* これらの手順を完了すると、タイムシートプロファイルは、現在の期間の既存のタイムシートを持たない割り当て済みのユーザーまたはグループメンバーに対してのみタイムシートを生成します。

1. 「**変更を保存**」をクリックします。

   タイムシートプロファイルがタイムシートを初めて生成する場合、各ユーザーに対して 2 つのタイムシートが作成されます。 その後、新しいタイムシートが生成されるたびに、タイムシートがユーザーごとに作成されます。

   <!--the content in the table above will need to match the content in the Create timesheets article-->

## タイムシートプロファイルを割り当てるグループ管理者の制限 {#limitations-for-a-group-administrator-assigning-a-timesheet-profile}

グループ管理者で、[ タイムシートと時間 ] がアクセスレベルで無効になっている場合は、タイムシートプロファイルを作成できますが、割り当てるのは次の場所だけです。

* 管理するグループ
* 管理するグループ内のユーザーを編集するためのアクセス権を持つ個々のユーザー

これらのグループとユーザーに対しては、タイムシートプロファイルが生成するタイムシートにアクセスできません。

また、アクセスレベルで [ ユーザー管理者（グループユーザー）] オプションも無効になっている場合は、管理するグループにタイムシートプロファイルを割り当てることができますが、編集するアクセス権を持つグループ内のユーザーのみに影響します。 編集するアクセス権のないユーザーがグループに含まれている場合、残りのグループと共にタイムシートプロファイルが割り当てられません。

アクセスレベルの [ タイムシートと時間 ] オプションの詳細については、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

アクセスレベルの「ユーザー管理者（グループユーザー） 」オプションについて詳しくは、 [ユーザーへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## 複数の反復タイムシートプロファイル

次の場合、組織に複数のタイムシートプロファイルを持つことができます。

* 異なるユーザーのセットに対する一意の支払期間
* 異なるユーザーのセットの一意の承認者
* 異なるユーザーセットに対する一意の一般時間要件

1 人のユーザーを一度に複数のタイムシートプロファイルに関連付けることはできません。 
