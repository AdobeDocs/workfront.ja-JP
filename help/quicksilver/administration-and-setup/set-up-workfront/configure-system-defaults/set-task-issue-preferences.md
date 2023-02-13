---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: システム全体のタスクと問題の環境設定を構成
description: タスクと問題に関するシステム全体の環境設定を構成できます。 これらの環境設定は、Workfrontでのユーザーによるタスクおよびイシューの作成方法に影響します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 1%

---

# システム全体のタスクと問題の環境設定を構成

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

As a [!DNL Adobe Workfront] 管理者は、タスクと問題に関するシステム全体の環境設定を構成できます。 これらの環境設定は、ユーザーが [!DNL Workfront].

デフォルトでは、タスクと問題の環境設定はロックされ、システム全体ですべてのグループのロックを解除しない限り、グループ管理者はグループレベルで変更できません。 詳しくは、 [グループのタスクと問題の環境設定をロックする](#lock-task-and-issue-preferences-for-groups) 」を参照してください。

<!--SPLIT OUT BOTTOM SECTION TO NEW ARTICLE?-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## の全員にタスクとタスクの環境設定を指定 [!DNL Workfront]

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **[!UICONTROL プロジェクト環境設定]** >**[!UICONTROL タスクと問題].**

1. 表示されたページで、次の 5 つのセクションのいずれかに進み、 [!UICONTROL 新規タスクのデフォルト], [!UICONTROL 問題], [!UICONTROL 削除], [!UICONTROL 実際の日付]、および [!UICONTROL アクセス].
1. 「**[!UICONTROL 保存]**」をクリックします。

* [[!UICONTROL 新規タスクの初期設定]](#new-task-defaults)
* [[!UICONTROL 問題]](#issues)
* [[!UICONTROL 削除]](#deletion)
* [[!UICONTROL 実際の日付]](#actual-dates)
* [[!UICONTROL 委任]](#delegation)

   <!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
  -->

* [[!UICONTROL アクセス]](#access)

### [!UICONTROL 新規タスクの初期設定] {#new-task-defaults}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 新規タスクの開始日 ]</td> 
   <td> <p>プロジェクトマネージャの新しいタスクの既定の開始日を指定します。 新規タスクの開始日は、プロジェクトの計画開始日か、タスクの作成日のどちらかです。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 期間の種類 ] </p> </td> 
   <td> <p>リソースの数（およびその割り当て率）とタスクの期間または総労力との関係を決定します。 詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプ</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 売上高タイプ ]</td> 
   <td> <p>タスクの計画収益見積もりと実績収益見積もりを計算します。 次の場合に <strong>[!UICONTROL 売上高タイプ ]</strong> が<strong>[!UICONTROL 請求不可 ]</strong>計画時間と記録された実際の時間では、タスクの収益見積もりは生成されず、タスクの作業はプロジェクトレベルの売上高には影響しません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コストタイプ ]</td> 
   <td> <p>タスクの予定コスト見積もりと実績コスト見積もりを計算します。 に設定する場合 <strong>[!UICONTROL コストなし ]</strong>計画時間と記録された実績時間では、タスクの計画済みコストまたは実績コストの見積もりは生成されず、タスクの作業はプロジェクトレベルのコストには影響しません。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 問題 {#issues}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 解決可能な問題のステータスを、解決オブジェクトのステータスが変更されたときに自動的に更新 ]</td> 
   <td> <p>誰かがイシューをプロジェクトまたはタスクに変換すると、元のイシューと変換後のプロジェクトまたはタスクの両方がオブジェクトの解決になります。 この設定では、元の問題の解決と、解決可能なオブジェクトの解決とを関連付けることができます。 オブジェクトの解決の詳細については、 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">オブジェクトの解決と解決の概要 </a>.</p> <p>この設定を有効にするには、 <strong>[!UICONTROL 元の問題を保持し、解決をタスクに結び付けます ]</strong> を選択する必要があります。</p> 
    <ul> 
     <li>この設定を有効にすると、イシュー、プロジェクト、タスクの両方で同じキーを使用してカスタムステータスを作成できます。 プロジェクトまたはタスク（解決可能なオブジェクト）がカスタムステータスに変わると、変更は問題のステータスにも反映されます。 イシュー、プロジェクトまたはタスクのステータスについて、ステータスキーは同じにする必要があります。</li> 
     <li>この設定を無効にした場合、解決するオブジェクトのステータスは、カスタムのステータスではなく、自動的にデフォルトのステータスに設定されます。 デフォルトのステータスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">システムの問題ステータスのリストへのアクセス</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader" [!UICONTROL>イシューをタスクに変換する場合 ]</td> 
   <td> <p>このセクションの設定は、問題からタスクへの変換プロセス中に何が起こるかを決定します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 元の問題を保持し、解決をタスクに結び付けます ]</strong>:イシューを変換する場合、タスクが完了するまで、イシューはイシューとして表示され続けます。 タスクが完了すると、問題のステータスが自動的に [!UICONTROL クローズ済み ] に変わります。 選択を解除すると、問題は削除されます。</p> <p><b>メモ</b>:  <p>この設定の状態に関係なく、アクセス権やイシューを削除する権限を持たないユーザーは、イシューを変換する際にイシューを削除できません。 アクセスおよび問題に対する権限について詳しくは、次を参照してください。</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">問題へのアクセス権の付与</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有 </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROLプライマリ連絡先にタスクへのアクセスを許可 ]</strong>:タスクをレビューし、更新を行い、進捗状況を常に知らせるために、主要連絡先（イシュー作成者）がタスクにアクセスできるようにします</li> 
     <li> <p><strong>[!UICONTROL 変換時にこれらの設定を変更できるようにする ]</strong>:イシューをタスクに変換する際に、イシューを変換するユーザーがこれらのオプションを変更できるようにします。</p> <!--
       Screenshot when possible</p>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 問題をプロジェクトに変換する場合 ]</td> 
   <td> <p>この節の設定は、問題からプロジェクトへの変換プロセス中に何が起こるかを決定します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 元の問題を維持し、その解決をプロジェクトに結び付ける ]</strong>:イシューを変換する場合、プロジェクトが完了するまで、イシューはイシューとして表示され続けます。 問題のステータスは、プロジェクトが完了すると、自動的に [!UICONTROL クローズ済み ] に変わります。 選択を解除すると、問題は削除されます。 </p> <p><b>メモ</b>:  <p>この設定の状態に関係なく、アクセス権やイシューを削除する権限を持たないユーザーは、イシューを変換する際にイシューを削除できません。 アクセスおよび問題に対する権限について詳しくは、次を参照してください。</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">問題へのアクセス権の付与</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有 </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROLプライマリ連絡先がプロジェクトにアクセスできるようにする ]</strong>:主要連絡先（イシュー作成者）がプロジェクトにアクセスし、プロジェクトのレビュー、更新をおこない、進行状況を常に知らせます。</li> 
     <li><strong>[!UICONTROL 変換時にこれらの設定を変更できるようにする ]</strong>:イシューを変換するユーザーが、イシューをプロジェクトに変換する際に、リストに表示されるオプションを変更できるようにします。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 削除] {#deletion}

**[!UICONTROL ログに記録された時間のタスクと問題の削除をユーザーに許可]**:タスクの削除を許可するか、時間が記録される問題を許可するかを指定できます。 このオプションはデフォルトで選択されています。

>[!TIP]
>
>この設定は、タスクを持つプロジェクトや、ログオン時間に関する問題が発生したプロジェクトの削除にも適用されます。 この設定は、プロジェクトの時刻が直接記録されるプロジェクトの削除には適用されません。

* このオプションを選択すると、タスクまたはイシューを削除する際に、情報の警告が表示されます。 この警告は、タスクまたは問題がログに記録された時間が過ぎると、プロジェクトに移動されるか、削除されることを示します。 時間を削除するか、または [!UICONTROL タイムシートと時間の基本設定] 領域 [!UICONTROL 設定]. 警告が表示されたことを確認すると、タスクまたはイシューは削除されます。 タイムシートと時間の基本設定の構成の詳細については、「 [タイムシートと時間の基本設定を構成する](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   >[!TIP]
   >
   >ログに記録された時間を持つタスクと問題を含むプロジェクトを削除すると、記録された時間は削除されるか、 [!UICONTROL タイムシートと時間の基本設定] ～の面積 [!UICONTROL 設定]. プロジェクトの削除時に警告メッセージが表示されない。

* このオプションを選択解除すると、タスクやログに記録された時間の問題を削除した場合、またはタスクや問題のログに記録された時間のあるプロジェクトを削除した場合に、非常に多くの警告が表示されます。 警告は、管理者がログに記録された時間に関するタスクや問題を削除できないことを示します。 タスクと問題に関してログに記録された時間のあるタスク、問題、またはプロジェクトは削除できません。

### [!UICONTROL 実際の日付] {#actual-dates}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL タスクまたはイシューが「新規」から「処理中」に変わったら、「実際の開始日」を [] に設定します</td> 
   <td> <p>実際の開始日が次の場所に記録される場合に、次のオプションの 1 つを選択します。 [!DNL Workfront] タスクまたは問題が <strong>[!UICONTROL 新規 ]</strong> から <strong>[!UICONTROL 処理中 ]</strong>:</p> 
    <ul> 
     <li><strong>[!UICONTROL 今すぐ ]:</strong> 実際の開始日は現在の日付に設定されます。</li> 
     <li><strong>[!UICONTROL 予定開始日 ]:</strong> [ 実績開始日 ] は、タスクまたはタスクの [ 計画開始日 ] に設定されます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タスクまたはイシューが完了したら、「実際の完了日」を [] に設定します</td> 
   <td> <p>実際の完了日が次の場所に記録される場合に、次のオプションの 1 つを選択します。 [!DNL Workfront] タスクまたはイシューが完了したとき：</p> 
    <ul> 
     <li><strong>[!UICONTROL 今すぐ ]:</strong> 実際の完了日は現在の日付に設定されます。</li> 
     <li> <p><strong>[!UICONTROL 計画完了日 ]:</strong> 実績完了日は、タスクまたは発行の計画完了日に設定されます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 委任

の有効化 [!UICONTROL ユーザーがタスクと問題を委任することを許可] を設定すると、のすべてのユーザーが作業を一時的に他のユーザーに委任できます。

この設定を有効にすると、次の情報が表示されます。

* この [!UICONTROL 委任] リンク [!UICONTROL ホーム] 領域 ここから承認、タスクおよび問題の割り当てを委任できます。
* タスクまたはイシューが [!UICONTROL 割り当てと委任] タスクまたはイシューのヘッダー内の領域

この [!UICONTROL ユーザーがタスクと問題を委任することを許可] 設定すると、現在スケジュールされている委任は停止され、委任されたユーザーは、委任が停止されたことを示す電子メール通知を受け取ります。

他のユーザーへの作業の委任について詳しくは、次の記事を参照してください。

* [作業の委任の概要](../../../manage-work/delegate-work/delegate-work-overview.md)
* [タスクと問題の委任を管理](../../../manage-work/delegate-work/how-to-delegate-work.md)

<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL アクセス] {#access}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 任意のユーザーがタスクに割り当てられたとき ]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL タスクへのアクセス権を付与 ]</strong>:割り当て先のタスクに対してユーザーが持つデフォルトの権限を定義します。 タスク権限の詳細については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</li> 
     <li> <p><strong>[!UICONTROL プロジェクトへのアクセス権も付与 ]</strong>:タスクが割り当てられているプロジェクトに対してユーザーが持つデフォルトの権限を定義します。 プロジェクト権限の詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 任意のユーザーがイシューに割り当てられたとき ]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL タスクへのアクセス権を付与 ]</strong>:割り当て先のタスクに対してユーザーが持つデフォルトの権限を定義します。 タスク権限の詳細については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</li> 
     <li> <p><strong>[!UICONTROL プロジェクトへのアクセス権も付与 ]</strong>:タスクが割り当てられているプロジェクトに対してユーザーが持つデフォルトの権限を定義します。 プロジェクト権限の詳細については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 任意のユーザーがリクエストを送信したとき ]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL 問題へのアクセス権を付与 ]</strong>:ユーザーが送信したリクエストに対して持つデフォルトの権限を定義します。 詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有 </a>.</li> 
     <li> <p><strong>[!UICONTROL 同じ会社の担当者は、すべてのリクエストに対して同じ権限を継承します ]</strong>:ユーザーが同じ会社の他のユーザーから送信された要求を表示することを許可します。 これらのリクエストに対する権限は、独自に送信されたリクエストに対する権限と同じです。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## グループのタスクと問題の環境設定をロックする {#lock-task-and-issue-preferences-for-groups}

組織内のグループで、一意のワークフロー用に別々に設定されたタスクまたは問題の環境設定が必要な場合は、組織全体のすべてのグループの環境設定のロックを解除して、グループごとに設定できます。 プリファレンスのロックが解除され、グループ管理者が変更すると、グループに関連するタスクや問題は、システムレベルの設定ではなく、プリファレンスのグループレベルの設定の影響を受けます。

グループ管理者がグループに対してタスクと問題の環境設定を行う方法については、 [グループのタスクと問題の環境設定を設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>次の後： [!DNL Workfront] 管理者は、システムレベルでプリファレンスのロックを解除し、任意のグループ管理者が設定を行い、そのグループと以下のサブグループの全員が同じ設定を使用するようにロックできます。 これは、 [!DNL Workfront] 管理者は、システム内のすべてのユーザーに対して環境設定を設定およびロックする必要があります。 詳しくは、 [グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) および [サブグループのプロジェクト、タスク、または問題の環境設定をロックまたはロック解除する](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

タスクまたはイシューの環境設定をロックまたはロック解除して、グループが設定できるようにするには

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL プロジェクト環境設定]** > **[!UICONTROL タスクと問題]**.

1. 次のいずれかの操作を行います。

   * グループの下のグループの管理者がグループの環境設定を構成できるようにするには、グループのロックを解除します ![](assets/unlock-toggle-button.png).
   * グループとその下のすべてのグループで設定を使用して環境設定を行う場合は、そのグループがロックされている（デフォルト）ことを確認します。

      >[!IMPORTANT]
      >
      >ロックされた環境設定を構成する際にすべてのニーズが考慮されるように、システム全体の管理者やグループ内のユーザーとコミュニケーションを取ることをお勧めします。 ロックすると、その設定がシステム内のすべてのグループに継承されます。 また、環境設定のロックが一定期間解除されている場合は、グループ管理者が行った設定がその設定に置き換えられます。

1. 「**[!UICONTROL 保存]**」をクリックします。
