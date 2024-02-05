---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: タイムシートプロファイルの作成、編集および割り当て
description: 追加の介入なしに、ユーザーに対して定期タイムシートを生成するタイムシートプロファイルを作成および編集し割り当てることができます。これにより、時間を節約し、ユーザー間の一貫性を確保できます。
author: Alina
feature: Timesheets
exl-id: 8f4826bd-82b4-4157-a7d4-a7c94b8fc879
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 93%

---

# タイムシートプロファイルの作成、編集および割り当て

追加の介入なしに、ユーザーに対して定期タイムシートを生成するタイムシートプロファイルを作成および編集し割り当てることができます。これにより、時間を節約し、次の情報についてユーザー間で一貫性を保つことができます。

* タイムシートの時間枠
* 承認者
* 一般的な時間タイプ

タイムシートを手動で作成する方法について詳しくは、[1 回限りのタイムシートの作成](../../timesheets/create-and-manage-timesheets/create-tmshts.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>新規：標準 </p>
 <p>または</p> 
<p>現在：プラン </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タイムシートに対する管理アクセス権が必要です。 </p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## タイムシートプロファイルを作成または編集

<!--
<div style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p style="color: #ff1493;">Alina drafted an Important note under this heading because Tracy/WorkEx said this is not working as designed - the changes WILL take effect the minute to make them for existing timesheets - see this issue - https://hub.workfront.com/issue/5dba59f600c401cca536567c368aa299/overview</p>
<p style="color: #ff1493;">Important: The changes you make to an existing timesheet profile are not automatically applied to timesheets that have already been generated. The changes you make to a timesheet prile are applied only to the timesheets that are&nbsp;generated after the timesheet profiles changes are made. To&nbsp;apply your&nbsp;changes to the timesheet profile for the timesheets that are already generated, you must delete the existing timesheets and manually generate&nbsp;them.For more information about deleting and manually generating timesheets, see&nbsp;Delete and manually generating Timesheets.</p>
</div>
-->

>[!IMPORTANT]
>
>現在のタイムシートのタイムシートプロファイルの変更を有効にするには、既存のタイムシートを削除してから、新しいタイムシートを生成する必要があります。手順については、[Adobe Workfront のタイムシートの削除](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)および[タイムシートを手動で生成](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)を参照してください。

{{step-1-to-setup}}

1. システム全体で使用するタイムシートプロファイルを作成または編集する場合は、「**タイムシートと時間**」をクリックします。

   または

   グループのタイムシートプロファイルを作成または編集する場合は、「**グループ**」をクリックし、グループの名前をクリックします。

1. 「**タイムシートプロファイル**」をクリックします。
1. 新しいタイムシートプロファイルを作成するには、「**新規プロファイル**」をクリックします。

   または

   既存のタイムシートプロファイルを編集するには、編集するタイムシートプロファイルを選択し、「**編集**」をクリックします。

   新規または既存のタイムシートプロファイルが表示されます。


1. 「**詳細の設定**」タブで、タイムシートプロファイルの&#x200B;**名前**&#x200B;および&#x200B;**説明**&#x200B;と、次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>管理アクセス権限を持ったグループ</strong> </td> 
      <td> <p> 
      <ul> 
      <li> <p>システムレベルのタイムシートプロファイルを作成する場合は、このフィールドを空白のままにします。</p> <p>ユーザーアカウントを編集できるユーザーは、システムレベルのタイムシートを他のユーザーに添付できます。</p> <p>システムレベルのタイムシートプロファイルを編集できるのは、Workfront 管理者だけです。</p> </li> 
      </ul> 
     <ul> 
      <li> <p>管理しているグループのタイムシートプロファイルを作成する場合は、ここでグループを指定します。</p> <p>この操作を実行しても、グループ内のユーザーにタイムシートプロファイルは割り当てられません。グループの管理者がタイムシートプロファイルを変更できるだけです。手順 6 で、プロファイルをユーザーに割り当てます。</p>

   <p><b>注意</b>：グループ外のユーザーがタイムシートプロファイルを他のユーザーに添付すると、このタイムシートプロファイルを表示または添付できなくなります。</p> </li> 
      </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>タイムシートを作成</strong> </td> 
      <td> <p> <p>タイムシートプロファイルがタイムシートを生成するタイミングを指定します。タイムシートは、週ごと、2 週間ごと、半月ごと、月ごとに自動生成するよう設定できます。タイムシートを生成する曜日を選択します。</p>
      <p>週ごとのタイムシートは、タイムシートの生成日に開始します。例えば、毎週木曜日に週次のタイムシートを作成する場合、タイムシートの週の最初の曜日は木曜日になります。</p>


   <p><b>注意</b>:Workfrontは常に 2 つのタイムシートを一度に作成します。最初のタイムシートには常に現在の日付が含まれ、2 番目のタイムシートは最初のタイムシートの期間が終わるときに開始します。</p> </p> </td> 
    </tr> 
     <tr> 
      <td role="rowheader"><p><strong>承認者</strong></p> </td> 
      <td> <p> <p>承認者とは、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。タイムシートでは、最大 7 人のユーザーを承認者として指定できます。複数のユーザーを指定しておくと、承認者の不在時に別の承認者を確実に利用することができます。ユーザーがタイムシートを承認のために送信すると、すべての承認者に通知が届きます。タイムシートの承認に必要なのは、1 人のユーザーの承認のみです。</p> <p>承認者として設定できるのは、タイムシートの管理権限を持つユーザーのみです。タイムシートの管理権限について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">ユーザーに対する特定のエリアへの管理アクセス権の付与</a>を参照してください。</p> <p>ドロップダウンメニューを使用して、タイムシートの承認者を選択します（承認者が必要な場合）。以下のオプションから選択できます。</p> 
      <ul> 
      <li><strong>なし</strong>：タイムシートを承認する必要はありません。</li> 
      <li><strong>マネージャー</strong>：これは、システムによって設定されるデフォルトの承認者です。マネージャーとして指定されたユーザーが、承認を受けるために送信されたタイムシートを承認します。</li> 
      <li><strong>特定のユーザー：</strong>特定のユーザーをタイムシートの承認者として名前で指定できます。1 つのタイムシートに複数の承認者を設定できます。ここでは、1 人の承認者がタイムシートを承認すると、タイムシートが<strong>クローズ</strong>としてマークされ、残りの承認者の承認リストにそのタイムシートが表示されなくなります。</li> 
       </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>時間を編集可能</strong> </td> 
      <td> <p> <p>承認者がタイムシートの時間を編集できるようにするには、このオプションを選択します。

   これは、設定／タイムシートと時間／環境設定領域の「**タイムシートの編集を所有者と管理者に制限**」とともに機能します。詳しくは、<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md">タイムシートと時間の環境設定の構成</a>を参照してください。

   次のシナリオが存在します。

   <ul>
      <li>「<b>タイムシートの編集を所有者と管理者に制限</b>」オプションが有効な場合は、以下のようになります。</li>
      <ul><li>「<b>時間を編集可能</b>」が有効かどうかに関わらず、承認者はタイムシートの承認および拒否できます。 </li>
      <li>タイムシート所有者のマネージャーは、自分のダイレクトレポートのタイムシートのみを表示できます。</li></ul>
      <li>「<b>タイムシートの編集を所有者と管理者に制限</b>」オプションが無効である場合は、以下のようになります。</li>
    <ul><li>「<b>時間を編集可能</b>」が有効になっている場合、承認者はタイムシートの送信、リオープン、またはクローズを行うことが可能で、時間を編集できます。</li>
      <li>「<b>時間を編集可能</b>」が無効になっている場合、承認者はタイムシートの送信、リオープン、またはクローズを行うことが不可能で、時間を編集できません。承認者が行えるのは、タイムシートの承認または却下のみです。 </li>
      <li>タイムシート所有者のマネージャーは、ダイレクトレポートのタイムシートの提出、取り消し、リオープン、編集を行うことができます。</li></ul>
      </ul>

   <p>

   <b>注意</b>：タイムシートを承認用に送信すると、時間を編集できなくなります。 提出されたタイムシートを編集可能な状態に戻すには、タイムシートを取り消すか、承認者にタイムシートを却下させます。詳しくは、<a href="../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md">承認に向けたタイムシートの送信</a>および<a href="../../timesheets/create-and-manage-timesheets/timesheet-approvals.md">タイムシートの承認</a>を参照してください。</p> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>使用できる時間タイプ</strong> </td> 
      <td><p>この設定は一般的な時間タイプのみを参照し、プロジェクト固有の時間タイプは参照しません。 </p>
      <p>デフォルトでは、タイムシートのすべての一般的な時間がユーザーに表示されます。ただし、特定のユーザーセットに対して特定の一般的な時間のみを表示する場合は、このフィールドのタイムシートプロファイルで選択することにより、タイムシートに表示する必要のある一般的な時間を選択できます。すべての一般的な時間を無効にする場合は、すべての時間タイプの選択を解除して、一般的な時間のセクションを含まないタイムシートを生成します。</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">超過作業時間</span> </td> 
      <td>タイムシートの「超過作業時間」ボックスは非表示にすることができます。このオプションはデフォルトでは無効になっています。</td> 
     </tr> 
    </tbody> 
    </table>

1. 「**ユーザーの割り当て**」タブをクリックし、タイムシートプロファイルを特定のユーザー、グループ、または（Workfront 管理者の場合は）チームに関連付けます。ユーザー、グループ、またはチームの名前の入力を開始し、ドロップダウンリストに表示されたらクリックします。

   グループ管理者は、自分が管理するグループにタイムシートプロファイルを割り当てることができますが、チームに割り当てることはできません。詳しくは、この記事内の[タイムシートプロファイルを割り当てるグループ管理者の制限](#limitations-for-a-group-administrator-assigning-a-timesheet-profile)を参照してください。

   >[!NOTE]
   >
   >* また、ユーザープロファイルを編集することで、ユーザーをタイムシートプロファイルに関連付けることもできます。詳しくは、[ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。
   >* グループを追加すると、「ユーザーを割り当て」タブにはグループ名のみが表示され、グループメンバーのリストは表示されません。ここにリスト表示されるグループメンバーを確認するには、「変更を保存」をクリックし、作成したばかりのタイムシートプロファイルの名前をクリックします。
   >* この手順を完了すると、タイムシートプロファイルは、現在の期間の既存のタイムシートを持たない、割り当てられたユーザーやグループメンバーに対してのみタイムシートを生成します。

1. 「**変更を保存**」をクリックします。

   タイムシートプロファイルがタイムシートを初めて生成する場合、各ユーザーに対して 2 つのタイムシートが作成されます。その後、新しいタイムシートが生成されるたびに、各ユーザーに対して 1 つのタイムシートが作成されます。

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
