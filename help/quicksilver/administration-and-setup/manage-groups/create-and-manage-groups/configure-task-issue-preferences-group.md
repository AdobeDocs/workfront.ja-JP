---
title: グループのタスクと問題の環境設定を設定する
user-type: administrator
product-area: system-administration;user-management;setup
keywords: グループ，環境設定，タスク，問題，ロック解除
navigation-topic: create-and-manage-groups
description: 組織内のグループが、システムレベルでの設定方法とは別に、タスクまたはイシューの環境設定をおこなう必要がある場合、Adobe Workfrontの管理者が環境設定のロックを解除できます。 その後、グループ管理者として、グループの環境設定を構成し、グループに関連するすべてのタスクや問題に影響を与えます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 2%

---

# グループのタスクと問題の環境設定を設定する

組織内のグループが、システムレベルでの設定方法とは別に、タスクまたはイシューの環境設定をおこなう必要がある場合、Adobe Workfrontの管理者が環境設定のロックを解除できます。 その後、グループ管理者として、グループの環境設定を構成し、グループに関連するすべてのタスクや問題に影響を与えます。

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

Workfront管理者が環境設定をロック解除する方法について詳しくは、 [システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除します](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>プロジェクトの環境設定では、グループレベルの設定も可能です。 詳しくは、 [グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* 通常、ロックが解除された環境設定は、無期限にロックが解除されたままになります。 Workfront管理者が再ロックすると、システム設定が再度有効になり、グループ管理者が行った環境設定は失われます。
>* プロジェクトに関連付けられたグループに設定された環境設定は、プロジェクトを作成するユーザーのホームグループに設定された環境設定よりも優先されます。
>* グループレベルの環境設定の中には、グループ用に作成するプロジェクトテンプレートに影響を与えるものもあります。 詳しくは、 [グループ領域で、グループのテンプレートの表示、操作、作成を行います](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 記事内 [グループのプロジェクトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Workfrontの管理者がシステム・レベルでプリファレンスのロックを解除した後は、設定を行い、その設定をロックして、グループ内の全員とサブグループ内の全員が同じ設定を使用するようにできます。 これは、Workfront管理者がシステム内のすべてのユーザーに対して環境設定を設定およびロックする必要がある機能と同じです。 詳しくは、 [サブグループのプロジェクト、タスク、または問題の環境設定をロックまたはロック解除する](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## トップレベルグループのロックが解除されたタスクと問題の環境設定を構成する

>[!TIP]
>
>Workfrontの管理者は、セットアップ/プロジェクトの環境設定/タスクと問題に移動して、ページの上部にあるボックスでグループの名前を検索することで、手順 1 ～ 4 をスキップできます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. ロックが解除されたタスクと問題の環境設定を設定するグループの名前をクリックします。
1. グループに対して表示されるページの左パネルで、 **タスクと問題の環境設定**.
1. 表示されるページで、次の 5 つのセクションのいずれかを続行して、[ 新しいタスクの既定 ]、[ タスクの既定値 ]、[ タスクの削除 ]、[ 実績日 ]、[ アクセス ] の各領域の設定を行い、[ ] **保存**.

   ロックアイコンの上にマウスポインターを置くと、 ![](assets/lock-toggle-button-dimmed.png) 設定が必要で、ロックされていることを知らせるツールヒントが表示される環境設定の場合は、Workfront管理者に問い合わせて、組織内のすべてのグループのロックを解除してもらうことができます。

   ロックが解除されると、ユーザーと他のグループ管理者は、自分のグループに対して別々に設定できます。 また、自分のグループと自分のグループの下のサブグループに対してロックすることもできます。

   * [新規タスクの初期設定](#new-task-defaults)
   * [問題](#issues)
   * [削除](#deletion)
   * [実際の日付](#actual-dates)

      <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [アクセス](#access)

### 新規タスクの初期設定 {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新規タスクの開始日</td> 
      <td> <p>プロジェクトマネージャの新しいタスクの既定の開始日を指定します。 新規タスクの開始日は、プロジェクトの計画開始日か、タスクの作成日のどちらかです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>期間タイプ </p> </td> 
      <td> <p>リソースの数（およびその割り当て率）とタスクの期間または総労力との関係を決定します。 詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプ</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">収益タイプ</td> 
      <td> <p>タスクの計画収益見積もりと実績収益見積もりを計算します。 次の場合に <strong>売上高タイプ</strong> が<strong>請求不可</strong>計画時間と記録された実際の時間では、タスクの収益見積もりは生成されず、タスクの作業はプロジェクトレベルの売上高には影響しません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">コストの種類</td> 
      <td> <p>タスクの予定コスト見積もりと実績コスト見積もりを計算します。 に設定する場合 <strong>コストなし</strong>計画時間と記録された実績時間では、タスクの計画済みコストまたは実績コストの見積もりは生成されず、タスクの作業はプロジェクトレベルのコストには影響しません。</p> </td> 
     </tr> 
    </tbody> 
   </table>

### 問題 {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">解決オブジェクトの状態が変わると、解決可能問題の状態を自動的に更新します</td> 
      <td> <p>誰かがイシューをプロジェクトまたはタスクに変換すると、元のイシューと変換後のプロジェクトまたはタスクの両方がオブジェクトの解決になります。 この設定では、元の問題の解決と、解決可能なオブジェクトの解決とを関連付けることができます。 オブジェクトの解決の詳細については、 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">オブジェクトの解決と解決の概要 </a>.</p> <p>この設定を有効にするには、 <strong>元の問題を保持し、その解決をタスクに結び付けます</strong> を選択する必要があります。</p> 
       <ul> 
        <li>この設定を有効にすると、イシュー、プロジェクト、タスクの両方で同じキーを使用してカスタムステータスを作成できます。 プロジェクトまたはタスク（解決可能なオブジェクト）がカスタムステータスに変わると、変更は問題のステータスにも反映されます。 イシュー、プロジェクトまたはタスクのステータスについて、ステータスキーは同じにする必要があります。</li> 
        <li>この設定を無効にした場合、解決するオブジェクトのステータスは、カスタムのステータスではなく、自動的にデフォルトのステータスに設定されます。 デフォルトのステータスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">システムの問題ステータスのリストへのアクセス</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">イシューをタスクに変換する場合</td> 
      <td> <p>このセクションの設定は、問題からタスクへの変換プロセス中に何が起こるかを決定します。</p> 
       <ul> 
        <li><strong>元の問題を保持し、その解決をタスクに結び付けます</strong>:イシューを変換する場合、タスクが完了するまで、イシューはイシューとして表示され続けます。 タスクが完了すると、イシューのステータスは自動的に「クローズ」に変わります。</li> 
        <li><strong>プライマリの連絡先にタスクへのアクセスを許可</strong>:タスクをレビューし、更新を行い、進捗状況を常に知らせるために、主要連絡先（イシュー作成者）がタスクにアクセスできるようにします</li> 
        <li> <p><strong>変換時にこれらの設定を変更できるようにする</strong>:イシューをタスクに変換する際に、イシューを変換するユーザーがこれらのオプションを変更できるようにします。</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">イシューをプロジェクトに変換する場合</td> 
      <td> <p>この節の設定は、問題からプロジェクトへの変換プロセス中に何が起こるかを決定します。</p> 
       <ul> 
        <li><strong>元の問題を保持し、その解決をプロジェクトに結び付けます</strong>:イシューを変換する場合、プロジェクトが完了するまで、イシューはイシューとして表示され続けます。 プロジェクトが完了すると、問題のステータスが自動的に「クローズ」に変わります。</li> 
        <li><strong>プライマリの連絡先がプロジェクトにアクセスできるようにする</strong>:主要連絡先（イシュー作成者）がプロジェクトにアクセスし、プロジェクトのレビュー、更新をおこない、進行状況を常に知らせます。</li> 
        <li><strong>変換時にこれらの設定を変更できるようにする</strong>:イシューを変換するユーザーが、イシューをプロジェクトに変換する際に、リストに表示されるオプションを変更できるようにします。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### 削除 {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ユーザーにログ時間のあるタスクと問題の削除を許可する</td> 
      <td> <p> タスクの削除を許可するか、時間が記録される問題を許可するかを指定できます。 このオプションはデフォルトで選択されています。</p> 
       <div> 
        <p><b>ヒント</b>:この設定は、タスクを持つプロジェクトや、ログオン時間に関する問題が発生したプロジェクトの削除にも適用されます。 この設定は、プロジェクトの時刻が直接記録されるプロジェクトの削除には適用されません。 </p> 
        <p>次の点に注意してください。</p> 
        <ul> 
         <li> <p>このオプションを選択すると、タスクまたはイシューを削除する際に、情報の警告が表示されます。 この警告は、タスクまたは問題がログに記録された時間が過ぎると、プロジェクトに移動されるか、削除されることを示します。 時間を削除するか、プロジェクトに移動するかは、セットアップの [ タイムシートと時間の基本設定 ] 領域で設定できます。 警告が表示されたことを確認すると、タスクまたはイシューは削除されます。 タイムシートと時間の基本設定の構成の詳細については、「 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">タイムシートと時間の基本設定を構成する</a>. </p> <p>ヒント： <span>タスクと問題が記録されたプロジェクトを削除すると、記録された時間は削除されるか、[ セットアップ ] の [ タイムシートと時間の基本設定 ] 領域の設定に従って保持されます</span>. </p> </li> 
         <li><span>このオプションを選択解除すると、タスクやログに記録された時間の問題を削除したり、タスクや問題のログに記録された時間のあるプロジェクトを削除したりした場合に、非常に多くの警告が表示されます</span> <span>.</span> 警告は、管理者がログに記録された時間に関するタスクや問題を削除できないことを示します。 タスク、問題<span>、タスクや問題に関して数時間のログが記録されたプロジェクト</span> は削除できません。 </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### 実際の日付 {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">タスクまたはタスクが「新規」から「処理中」に変わったら、「実績開始日」を「次の日付に設定します：</td> 
      <td> <p>タスクまたは問題の発生時にWorkfrontで実際の開始日が記録される場合に、次のオプションのいずれかを選択します <strong>新規</strong> から <strong>処理中</strong>:</p> 
       <ul> 
        <li><strong>今：</strong> 実際の開始日は現在の日付に設定されます。</li> 
        <li><strong>計画開始日：</strong> [ 実績開始日 ] は、タスクまたはタスクの [ 計画開始日 ] に設定されます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクまたはイシューが完了したら、「実際の完了日」を「</td> 
      <td> <p>タスクまたはイシューが完了したときにWorkfrontで実際の完了日が記録される場合は、次のオプションのいずれかを選択します。</p> 
       <ul> 
        <li><strong>今：</strong> 実際の完了日は現在の日付に設定されます。</li> 
        <li> <p><strong>計画完了日：</strong> 実績完了日は、タスクまたは発行の計画完了日に設定されます。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### アクセス {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">誰かがタスクに割り当てられたとき</td> 
      <td> 
       <ul> 
        <li><strong>タスクへのアクセス権をユーザーに与える</strong>:割り当て先のタスクに対してユーザーが持つデフォルトの権限を定義します。 タスク権限の詳細については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> ユーザーへのアクセス権の付与</a>.</li> 
        <li> <p><strong>また、ユーザーにプロジェクトへのアクセス権を付与します。</strong>:タスクが割り当てられているプロジェクトに対してユーザーが持つデフォルトの権限を定義します。 プロジェクト権限の詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">誰かが問題に割り当てられたとき</td> 
      <td> 
       <ul> 
        <li><strong>タスクへのアクセス権をユーザーに与える</strong>:割り当て先のタスクに対してユーザーが持つデフォルトの権限を定義します。 タスク権限の詳細については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</li> 
        <li> <p><strong>また、ユーザーにプロジェクトへのアクセス権を付与します。</strong>:タスクが割り当てられているプロジェクトに対してユーザーが持つデフォルトの権限を定義します。 プロジェクト権限の詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">誰かがリクエストを送信したとき</td> 
      <td> 
       <ul> 
        <li><strong>問題に対するアクセス権をユーザーに与えます。</strong>:ユーザーが送信したリクエストに対して持つデフォルトの権限を定義します。 詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a>.</li> 
        <li> <p><strong>同じ会社の担当者は、すべてのリクエストに対して同じ権限を継承します</strong>:ユーザーが同じ会社の他のユーザーから送信された要求を表示することを許可します。 これらのリクエストに対する権限は、独自に送信されたリクエストに対する権限と同じです。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
