---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: システム全体のタスクおよびイシューの環境設定を行う
description: タスクとイシューに関するシステム全体の環境設定を指定できます。これらの環境設定は、Workfront でのユーザーによるタスクおよびイシューの作成方法に影響します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '2228'
ht-degree: 85%

---

# システム全体のタスクとイシューの環境設定を指定

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


[!DNL Adobe Workfront] 管理者は、タスクとイシューに関するシステム全体の環境設定を指定できます。これらの環境設定は、[!DNL Workfront] でのユーザーによるタスクおよびイシューの作成方法に影響します。

デフォルトではタスクとイシューの環境設定はロックされているので、システム全体のすべてのグループに対してロックを解除しない限り、グループ管理者はグループレベルでそれらを変更することできません。詳しくは、この記事の[グループのタスクとイシューの環境設定をロック](#lock-task-and-issue-preferences-for-groups)の節を参照してください。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront] 内の全員のタスクとイシューの環境設定を行う

{{step-1-to-setup}}

1. 左側のパネルで、**[!UICONTROL プロジェクト環境設定]**／**[!UICONTROL タスクとイシュー]をクリックします。**

1. 表示されたページで、以下の 6 つのセクションのいずれかに進み、[!UICONTROL 新規タスクの初期設定]、[!UICONTROL イシュー]、[!UICONTROL 削除]、[!UICONTROL 実際の日付]、[!UICONTROL アクセス]の設定を行います。

   * [[!UICONTROL 新規タスクの初期設定]](#new-task-defaults)
   * [[!UICONTROL イシュー]](#issues)
   * [[!UICONTROL 削除]](#deletion)
   * [移動](#move)
   * [[!UICONTROL 実際の日付]](#actual-dates)
   * [[!UICONTROL 委任]](#delegation)
   * [[!UICONTROL アクセス]](#access)


### [!UICONTROL 新規タスクの初期設定] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Start Date]</td> 
    <td> <p>プロジェクトマネージャーについて、新規タスクのデフォルトの開始日を決定します。新規タスクの開始日は、プロジェクトの予定開始日か、タスクの作成日のどちらかです。</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Duration Type] </p> </td> 
    <td> <p>リソースの数（およびその割り当て率）とタスクの期間または合計作業量との関係を決定します。詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">タスクの期間と期間のタイプ</a>を参照してください</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Revenue Type]</td> 
    <td> <p>タスクの計画収益見積もりと実績収益見積もりを計算します。<strong>[!UICONTROL Revenue Type]</strong> が <strong>[!UICONTROL Not Billable]</strong> に設定されている場合、予定時間数と記録された実際の時間数ではタスクの収益見積もりは生成されず、タスクの作業はプロジェクトレベルの収益には寄与しません。</p>
         <p>様々な収益タイプについて詳しくは、<a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md"> 請求と収益の概要 </a> を参照してください。</p></td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Cost Type]</td> 
    <td> <p>タスクの計画コスト見積もりと実績コスト見積もりを計算します。<strong>[!UICONTROL No Cost]</strong> に設定する場合、計画時間と記録された実績時間では、タスクの計画コスト見積もりや実績コストの見積もりは生成されず、タスクの作業はプロジェクトレベルのコストには寄与しません。</p> </td> 
    </tr> 
  </tbody> 
</table>

### イシュー {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Automatically update Resolvable Issue status when the status of the Resolving Object changes]</td> 
    <td> <p>誰かがあるイシューをプロジェクトまたはタスクに変換すると、元のイシューと変換後のプロジェクトまたはタスクの両方が解決オブジェクトになります。この設定を使用すると、元のイシューの解決策を解決可能なオブジェクトの解決策に関連付けることができます。オブジェクトの解決に関して詳しくは、<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解決および解決可能なオブジェクトの概要</a>を参照してください。</p> <p>この設定を効果的にするには、「<strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong>」オプションを選択する必要があります。</p> 
      <ul> 
      <li>この設定を有効にすると、イシューと、プロジェクトまたはタスクの両方で、同じキーを使用してカスタムのステータスを作成できます。プロジェクトまたはタスク（解決可能なオブジェクト）がカスタムのステータスに変わると、その変更はイシューのステータスにも反映されます。ステータスキーは、イシューとプロジェクトまたはタスクのステータスで同じにする必要があります。</li> 
      <li>この設定を無効にすると、解決するオブジェクトのステータスは、カスタムのステータスではなく、自動的にデフォルトのステータスに設定されます。デフォルトのステータスについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">システムイシューステータスのリストへのアクセス</a>を参照してください。</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL 問題をタスクに変換する際に が発生する &#x200B;]</td> 
    <td> <p>このセクションの設定で、イシューからタスクへ変換するプロセスで起こることを定めます。</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the task]</strong>：イシューを変換する場合、タスクが完了するまで、イシューはイシューとして表示され続けます。タスクが完了すると、イシューのステータスは自動的に [!UICONTROL Closed] に変わります。選択を解除すると、イシューは削除されます。</p> <p><b>メモ</b>：  <p>この設定のステータスに関係なく、イシューを削除するアクセス権や権限を持たないユーザーは、イシューを変換する際にイシューを削除できません。イシューに対するアクセス権および権限について詳しくは、次を参照してください。</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">イシューへのアクセスの許可</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the task]</strong>：タスクを確認したり、その進捗を常に把握したり、タスクの「更新」セクションにコメントを付けたりできるように、プライマリ連絡先（イシュー作成者）にタスクに対する表示アクセス権を付与します。</li> 
      <li> <p><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong>：イシューを変換するユーザーが、イシューをタスクに変換する際に、これらのオプションを変更できます。</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When converting an issue to a project]</td> 
    <td> <p>このセクションの設定で、イシューからプロジェクトへ変換するプロセスで起こることを定めます。</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Keep the original issue and tie its resolution to the project]</strong>：イシューを変換する場合、プロジェクトが完了するまで、イシューはイシューとして表示され続けます。プロジェクトが完了すると、イシューのステータスは自動的に [!UICONTROL Closed] に変わります。選択を解除すると、イシューは削除されます。 </p> <p><b>メモ</b>：  <p>この設定のステータスに関係なく、イシューを削除するアクセス権や権限を持たないユーザーは、イシューを変換する際にイシューを削除できません。イシューに対するアクセス権および権限について詳しくは、次を参照してください。</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">イシューへのアクセスの許可</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Allow Primary Contact to have access to the project]</strong>：プロジェクトを確認したり、進捗を常に把握したり、プロジェクトの「更新」セクションにコメントを付けたりできるように、プライマリ連絡先（イシュー作成者）にプロジェクトに対する表示アクセス権を付与します。</li> 
      <li><strong>[!UICONTROL Allow these settings to be changed during conversion]</strong>：イシューをプロジェクトに変換する際に、変換するユーザーがリストに表示されているオプションを変更できるようにします。</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL 削除] {#deletion}

**[!UICONTROL ユーザーがログ時間のあるタスクおよび問題を削除することを許可]**：時間が記録されるタスクまたは問題を削除することを許可するかどうかを決定できます。 このオプションはデフォルトで選択されています。

>[!TIP]
>
>この設定は、時間が記録されるタスクやイシューを持つプロジェクトの削除にも適用されます。この設定は、時間がプロジェクトに直接記録されるようなプロジェクトの削除には適用されません。

* このオプションを選択すると、タスクまたはイシューを削除する際に、警告メッセージが表示されます。この警告は、タスクまたはイシューが時間を記録していた場合、その時間はプロジェクトに移動されるか、削除されることを知らせるものです。時間を削除するか、プロジェクトに移動するかは、「[!UICONTROL 設定]」の「[!UICONTROL タイムシートおよび時間設定]」エリアで設定できます。警告が表示されたことを確認すると、タスクまたはイシューは削除されます。「タイムシートおよび時間設定」の指定について詳しくは、[タイムシートおよび時間設定の指定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

  >[!TIP]
  >
  >時間を記録していたタスクとイシューを削除すると、記録されていた時間は削除されるか、「[!UICONTROL 設定]」の「[!UICONTROL タイムシートおよび時間設定]」エリアの設定に基づいて保持されます。プロジェクトの削除時に警告メッセージは表示されません。

* このオプションの選択を解除すると、時間が記録されたタスクやイシューを削除したり、タスクやイシューの時間が記録されたプロジェクトを削除したりした際に、禁止の警告が表示されます。この警告は、時間が記録されたタスクやイシューの削除を管理者が禁止していることを示しています。タスク、イシュー、およびタスクやイシューの時間が記録されたプロジェクトは削除できません。

### 移動

**[!UICONTROL ユーザーがログ時間のあるタスクおよび問題を移動することを許可]**：時間が記録されるタスクまたは問題を移動することを許可するかどうかを決定できます。 このオプションはデフォルトで選択されています。

* 選択すると、時間がログに記録されたタスクと問題を移動できます。 時間は、タスクや問題とも移動します。

* このオプションの選択を解除すると、ログ時間のあるタスクや問題を別のプロジェクトに移動する際に禁止を示す警告が表示されます。 警告は、管理者がタスクまたはログ時間に関する問題の移動を許可しないことを指定します。 時間が記録されたタスクまたは問題は移動できません。 このオプションの選択を解除した場合でも、同じプロジェクト内でタスクを移動できます。

### [!UICONTROL 実際の日付] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue goes from "New" to "In Progress," set the Actual Start Date to]</td> 
    <td> <p>タスクまたはイシューが <strong>[!UICONTROL New]</strong> から <strong>[!UICONTROL In Progress]</strong> に変わったとき、[!DNL Workfront] で実際の開始日が記録されるタイミングとして、次のオプションのいずれかを選択します。</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]：</strong>実際の開始日は、現在の日付に設定されます。</li> 
      <li><strong>[!UICONTROL The Planned Start Date]：</strong>実際の開始日は、タスクまたはイシューの予定開始日に設定されます。</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When a task or issue is completed, set the Actual Completion Date to]</td> 
    <td> <p>タスクまたはイシューが完了したとき、[!DNL Workfront] で実際の完了日が記録されるタイミングとして、次のオプションのいずれかを選択します。</p> 
      <ul> 
      <li><strong>[!UICONTROL Now]：</strong>実際の完了日は、現在の日付に設定されます。</li> 
      <li> <p><strong>[!UICONTROL The Planned Completion Date]：</strong>実際の完了日は、タスクまたはイシューの予定完了日に設定されます。</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### 委任

「**[!UICONTROL ユーザーがタスクおよびイシューを委任することを許可]**」設定を有効にすると、システム内のすべてのユーザーが一時的に他のユーザーに作業を委任できます。

この設定を有効にすると、次の情報が表示されます。

* [!UICONTROL **ホーム**] エリアにある [!UICONTROL &#x200B; マイ作業 &#x200B;]、[!UICONTROL &#x200B; マイタスク &#x200B;] または [!UICONTROL &#x200B; マイイシュー &#x200B;] ウィジェットの [!UICONTROL &#x200B; 委任 &#x200B;] リンク。 ここからタスクとイシューの割り当てを委任できます。

  >[!NOTE]
  >
  >  「[!UICONTROL **承認を委任**]」リンクは、「[!UICONTROL &#x200B; ホーム &#x200B;] 領域で常に有効になっています。

* タスクまたはイシューのヘッダー内の「[!UICONTROL 割り当てと委任]」エリアで、タスクまたはイシューが別のユーザーに委任されたことを示すメッセージ。
* タスクまたはイシューが [!UICONTROL &#x200B; ホーム &#x200B;] の [!UICONTROL &#x200B; 担当作業 &#x200B;] ウィジェットで別のユーザーに委任されていることを示します。

  「[!UICONTROL &#x200B; ユーザーがタスクおよび問題を委任することを許可 &#x200B;]」設定を無効にすると、現在スケジュールされている委任が停止され、委任されたユーザーには、委任が停止したことを通知するメールが届きます。

他のユーザーへの作業の委任について詳しくは、次の記事を参照してください。

* [作業の委任の概要](../../../manage-work/delegate-work/delegate-work-overview.md)
* [タスクおよびイシューのデリゲート](../../../manage-work/delegate-work/how-to-delegate-work.md)


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
    <td role="rowheader">[!UICONTROL When someone is assigned to a task]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task]</strong>：ユーザーが割り当て先のタスクに対して持つデフォルトの権限を定義します。タスクの権限について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセスを許可</a>を参照してください。</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project]</strong>：ユーザーが割り当て先のタスクを含んだプロジェクトに対して持つデフォルトの権限を定義します。プロジェクトの権限について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境を設定</a>を参照してください。</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone is assigned to an issue]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to a task]</strong>：ユーザーが割り当て先のタスクに対して持つデフォルトの権限を定義します。タスクの権限について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセスを許可</a>を参照してください。</li> 
      <li> <p><strong>[!UICONTROL Also grant them ... access to the project]</strong>：ユーザーが割り当て先のタスクを含んだプロジェクトに対して持つデフォルトの権限を定義します。プロジェクトの権限について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境を設定</a>を参照してください。</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL When someone submits a request]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Give them ... access to the issue]</strong>：ユーザーが送信したリクエストに対して持つデフォルトの権限を定義します。詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a>を参照してください。</li> 
      <li> <p><strong>[!UICONTROL People from the same company will inherit the same permissions for all requests]</strong>：ユーザーは、同じ会社の他のユーザーによって送信されたリクエストを表示できます。これらのリクエストに対する権限は、独自に送信されたリクエストに対する権限と同じです。</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. 「**[!UICONTROL 保存]**」をクリックします。

## グループのタスクとイシューの環境設定をロック {#lock-task-and-issue-preferences-for-groups}

組織内のグループで、一意のワークフロー用に別々に設定されたタスクまたはイシューの環境設定が必要な場合は、組織全体のすべてのグループの環境設定のロックを解除して、グループごとに設定できます。環境設定のロックが解除され、グループ管理者が変更を加えると、グループに関連するタスクやイシューは、システムレベルの設定ではなく、環境設定のグループレベルの設定に影響されます。

グループ管理者がグループに対してタスクとイシューの環境設定を行う方法について詳しくは、[グループのタスクとイシューの環境設定を行う](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)を参照してください。

>[!NOTE]
>
>[!DNL Workfront] 管理者がシステムレベルで環境設定のロックを解除すると、グループ管理者は環境設定を指定でき、そのグループとその下に属するサブグループの全員が同じ設定を使用するようにロックできます。これは、[!DNL Workfront] 管理者がシステム内のすべてのユーザーに対して環境設定を指定およびロックする操作と同じです。詳しくは、[グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)および[サブグループのプロジェクト、タスクまたはイシューの環境設定をロックまたはロック解除](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)を参照してください。

タスクやイシューの設定をロックまたはロック解除して、グループが設定できるようにするには、次の手順に従います。

{{step-1-to-setup}}

1. **[!UICONTROL プロジェクト環境設定]**／**[!UICONTROL タスクとイシュー]**&#x200B;をクリックします。

1. 次のいずれかの操作を行います。

   * グループの下のグループの管理者がグループの環境設定を設定できるようにするには、そのロックを解除します ![&#x200B; ロック解除切替スイッチ &#x200B;](assets/unlock-toggle-button.png)。
   * グループとその下のすべてのグループで環境設定の設定を使用する場合は、ロックされている（デフォルト）ことを確認します。

     >[!IMPORTANT]
     >
     >ロックされた環境設定を指定する際にすべてのニーズが考慮されるように、システム全体の管理者やグループ内のユーザーとコミュニケーションを取ることをお勧めします。ロックすると、その設定がシステム内のすべてのグループに継承されます。また、環境設定のロックが一定期間解除されている場合、設定はグループ管理者が指定した設定と置き換えられます。

1. 「**[!UICONTROL 保存]**」をクリックします。
