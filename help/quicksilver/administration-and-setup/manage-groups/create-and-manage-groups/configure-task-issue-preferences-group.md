---
title: グループのタスクとイシューの環境設定を行う
user-type: administrator
product-area: system-administration;user-management;setup
keywords: グループ、環境設定、タスク、イシュー、ロック解除
navigation-topic: create-and-manage-groups
description: 組織内のグループが、システムレベルでの設定方法とは別に、タスクまたはイシューの環境設定を行う必要がある場合、Adobe Workfront の管理者が環境設定をロック解除できます。その後、グループ管理者はグループの環境設定を実施することができ、これはグループに関連するすべてのタスクやイシューに影響を与えます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 4a9936b6bc034f2176167fc3939d647ee679a888
workflow-type: tm+mt
source-wordcount: '1895'
ht-degree: 99%

---

# グループのタスクとイシューの環境設定を行う

組織内のグループが、システムレベルでの設定方法とは別に、タスクまたはイシューの環境設定を行う必要がある場合、Adobe Workfront の管理者が環境設定をロック解除できます。その後、グループ管理者はグループの環境設定を実施することができ、これはグループに関連するすべてのタスクやイシューに影響を与えます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

Workfront 管理者が環境設定をロック解除する方法について詳しくは、[システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)を参照してください。

>[!TIP]
>
>プロジェクトの環境設定では、グループレベルの設定も可能です。詳しくは、[グループのプロジェクト環境設定の実施](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)を参照してください。

>[!NOTE]
>
>* 通常、ロック解除された環境設定は、無期限にロック解除されたままになります。Workfront 管理者が再ロックすると、システム設定が再度有効になり、グループ管理者が行った環境設定は失われます。
>* プロジェクトに関連付けられたグループ向けの環境設定のセットは、プロジェクトを作成するユーザーのホームグループ向けの環境設定のセットよりも優先されます。
>* グループレベルの環境設定の中には、グループ用に作成するプロジェクトテンプレートに影響を与えるものがあります。詳しくは、[グループのプロジェクトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)の記事内の、[グループエリアから、グループのテンプレートの表示、操作、作成を実施](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view)の節を参照してください。
>
>* Workfront 管理者がシステムレベルで環境設定をロック解除した後は、これを設定してからロックすると、グループおよびそのサブグループ内の全員が、同じ設定を使用できるようになります。これは、Workfront 管理者がシステム内のすべてのユーザーに対して環境設定を指定およびロックするための機能と同じです。詳しくは、[サブグループのプロジェクト、タスク、イシューの環境設定をロックまたはロック解除](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)を参照してください。
>

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスタイプを確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## トップレベルグループのロックが解除されたタスクとイシューの環境設定を指定

>[!TIP]
>
>Workfront の管理者は、設定／プロジェクトの環境設定／タスクとイシューに移動して、ページの上部にあるボックスでグループの名前を検索することにより、手順 1 から 4 をスキップできます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、**設定**&#x200B;アイコン ![](assets/gear-icon-settings.png) をクリックします。

1. 左パネルで、**グループ**&#x200B;アイコン ![](assets/groups-icon.png) をクリックします。

1. ロックが解除されたタスクとイシューの環境設定を実施するグループの名前をクリックします。
1. グループに対して表示されるページの左側のパネルで、**タスクとイシューの環境設定**&#x200B;をクリックします。
1. 表示されるページで、これらの手順の下にリストされている 5 つのセクションのいずれかに進み、新規タスクのデフォルト、イシュー、削除、実際の日付、アクセスの各エリアの設定を行い、「**保存**」をクリックします。

   実施する環境設定のためにロックアイコン ![](assets/lock-toggle-button-dimmed.png) の上にポインタを合わせると、ロックされていることを知らせるツールヒントが表示される場合は、Workfront 管理者に問い合わせて、組織内のすべてのグループをロック解除するように依頼できます。

   ロックが解除されると、ユーザーと他のグループ管理者は、自分のグループに対してこれを別々に設定できます。また、自分のグループと自分のグループの下の任意のサブグループに対してロックすることもできます。

   * [新規タスクの初期設定](#new-task-defaults)
   * [イシュー](#issues)
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
      <td> <p>プロジェクトマネージャーについて、新規タスクのデフォルトの開始日を決定します。新規タスクの開始日は、プロジェクトの予定開始日か、タスクの作成日のどちらかです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>期間タイプ </p> </td> 
      <td> <p>リソースの数（およびその割り当て率）とタスクの期間または合計作業量との関係を決定します。詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">タスクの期間と期間の種類：記事のインデックス</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">収益タイプ</td> 
      <td> <p>タスクの計画収益見積もりと実績収益見積もりを計算します。<strong>収益タイプ</strong>が<strong>請求不可</strong>の場合、計画時間と記録された実際の時間では、タスクの収益見積もりは生成されず、タスクの作業はプロジェクトレベルの収益には寄与しません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">コストタイプ</td> 
      <td> <p>タスクの計画コスト見積もりと実績コスト見積もりを計算します。「<strong>コストなし</strong>」に設定した場合、計画時間と記録された実績時間では、タスクの計画コスト見積もりや実績コストの見積もりは生成されず、タスクの作業はプロジェクトレベルのコストには寄与しません。</p> </td> 
     </tr> 
    </tbody> 
   </table>

### イシュー {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">解決オブジェクトの状態が変わると、解決可能なイシューの状態を自動的に更新する</td> 
      <td> <p>誰かがあるイシューをプロジェクトまたはタスクに変換すると、元のイシューと変換後のプロジェクトまたはタスクの両方が解決オブジェクトになります。この設定を使用すると、元のイシューの解決策を解決可能なオブジェクトの解決策に関連付けることができます。オブジェクトの解決に関して詳しくは、<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解決オブジェクトと解決可能なオブジェクトの概要</a>を参照してください。</p> <p>この設定を効果的にするには、「<strong>元のイシューを保持して、その解決策をタスクに結び付け</strong>」オプションを選択する必要があります。</p> 
       <ul> 
        <li>この設定を有効にすると、イシューと、プロジェクトまたはタスクの両方で、同じキーを使用してカスタムのステータスを作成できます。プロジェクトまたはタスク（解決可能なオブジェクト）がカスタムのステータスに変わると、その変更はイシューのステータスにも反映されます。ステータスキーは、イシューとプロジェクトまたはタスクのステータスで同じにする必要があります。</li> 
        <li>この設定を無効にすると、解決するオブジェクトのステータスは、カスタムのステータスではなく、自動的にデフォルトのステータスに設定されます。デフォルトのステータスについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">システムイシューステータスのリストへのアクセス</a>を参照してください。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">イシューをタスクに変換するとき</td> 
      <td> <p>このセクションの設定で、イシューからタスクへ変換するプロセスで起こることを定めます。</p> 
       <ul> 
        <li><strong>元のイシューを保持し、その解決策をタスクに関連付ける</strong>：イシューを変換する際、タスクが完了するまで、イシューはイシューとして表示され続けます。タスクが完了すると、イシューのステータスは自動的にクローズに変わります。</li> 
        <li><strong>プライマリ連絡先にタスクへのアクセスを許す</strong>：タスクのレビュー、更新、進捗の確認ができるように、プライマリ連絡先（イシュー作成者）がタスクにアクセスできるようにします。</li> 
        <li> <p><strong>変換中にこれらの設定を変更できるようにする</strong>：イシューをタスクに変換する際に、変換するユーザーがこれらのオプションを変更できるようにします。</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">イシューをプロジェクトに変換するとき</td> 
      <td> <p>このセクションの設定で、イシューからプロジェクトへ変換するプロセスで起こることを定めます。</p> 
       <ul> 
        <li><strong>元のイシューを保持し、その解決策をプロジェクトに関連付ける</strong>：イシューを変換する際、プロジェクトが完了するまで、イシューはイシューとして表示され続けます。プロジェクトが完了すると、イシューのステータスは自動的にクローズに変わります。</li> 
        <li><strong>プライマリ連絡先にプロジェクトへのアクセスを許す</strong>：プロジェクトのレビュー、更新、進捗の確認ができるように、プライマリ連絡先（イシュー作成者）がプロジェクトにアクセスできるようにします。</li> 
        <li><strong>変換中にこれらの設定を変更できるようにする</strong>：イシューをプロジェクトに変換する際に、変換するユーザーがリストに表示されているオプションを変更できるようにします。</li> 
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
      <td role="rowheader">ユーザーに対して、時間が記録されたタスクとイシューの削除を許可する</td> 
      <td> <p> 時間が記録されるタスクやイシューの削除を許可するかどうかを指定します。このオプションはデフォルトで選択されています。</p> 
       <div> 
        <p><b>ヒント</b>：この設定は、時間が記録されるタスクやイシューを持つプロジェクトの削除にも適用されます。この設定は、時間がプロジェクトに直接記録されるようなプロジェクトの削除には適用されません。 </p> 
        <p>次の点に注意してください。</p> 
        <ul> 
         <li> <p>このオプションを選択すると、タスクまたはイシューを削除する際に、警告メッセージが表示されます。この警告は、タスクまたはイシューが時間を記録していた場合、その時間はプロジェクトに移動されるか、削除されることを知らせるものです。時間を削除するか、プロジェクトに移動するかは、「設定」のタイムシートと時間の環境設定エリアで設定できます。警告が表示されたことを確認すると、タスクまたはイシューは削除されます。タイムシートと時間の環境設定について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">タイムシートと時間の環境設定</a>を参照してください。 </p> <p>ヒント：<span>時間を記録していたタスクとイシューを削除すると、「設定」のタイムシートと時間の環境設定エリアの設定に基づいて、記録されていた時間は削除されるか、保持されます。</span> </p> </li> 
         <li><span>このオプションの選択を解除すると、時間が記録されたタスクやイシューを削除したり、タスクやイシューの時間が記録されたプロジェクトを削除したりした際に、禁止の警告が表示されます。</span> <span></span>この警告は、時間が記録されたタスクやイシューを削除することを管理者が禁止していることを示しています。タスク、イシュー<span>、およびタスクやイシュー</span>の時間が記録されたプロジェクトは削除できません。 </li> 
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
      <td role="rowheader">タスクまたはイシューが新規から処理中に変わったときの、実際の開始日の設定</td> 
      <td> <p>タスクまたはイシューが<strong>新規</strong>から<strong>処理中</strong>に変わったとき、Workfront で実際の開始日が記録されるタイミングとして、次のオプションのいずれかを選択します。</p> 
       <ul> 
        <li><strong>今：</strong>実際の開始日は現在の日付に設定されます。</li> 
        <li><strong>予定開始日：</strong>実際の開始日は、タスクまたはイシューの予定開始日に設定されます。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タスクまたはイシューが完了したときの、実際の完了日の設定</td> 
      <td> <p>タスクまたはイシューが完了したとき、Workfront で実際の完了日が記録されるタイミングとして、次のオプションのいずれかを選択します。</p> 
       <ul> 
        <li><strong>今：</strong>実際の完了日は現在の日付に設定されます。</li> 
        <li> <p><strong>予定完了日：</strong>実際の完了日は、タスクまたはイシューの予定完了日に設定されます。</p> </li> 
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
        <li><strong>タスクへのアクセス権を付与する</strong>：ユーザーが割り当て先のタスクに対して持つデフォルトの権限を定義します。タスクの権限について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</li> 
        <li> <p><strong>プロジェクトへのアクセス権も付与する</strong>：ユーザーが割り当て先のタスクを含んだプロジェクトに対して持つデフォルトの権限を定義します。プロジェクトの権限について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境の設定</a>を参照してください。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">誰かがイシューに割り当てられたとき</td> 
      <td> 
       <ul> 
        <li><strong>タスクへのアクセス権を付与</strong>：ユーザーが割り当て先のタスクに対して持つデフォルトの権限を定義します。タスクの権限について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセスを許可</a>を参照してください。</li> 
        <li> <p><strong>プロジェクトへのアクセス権も付与</strong>：ユーザーが割り当て先のタスクを含んだプロジェクトに対して持つデフォルトの権限を定義します。プロジェクトの権限について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境を設定</a>を参照してください。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">誰かがリクエストを送信したとき</td> 
      <td> 
       <ul> 
        <li><strong>イシューに対する ... アクセス権をユーザーに付与</strong>：ユーザーが送信したリクエストに対して持つデフォルトの権限を定義します。詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a>を参照してください。</li> 
        <li> <p><strong>同じ会社のユーザーはすべてのリクエストに対して同じ権限を継承</strong>：ユーザーは、同じ会社の他のユーザーによって送信されたリクエストを表示できます。これらのリクエストに対する権限は、独自に送信されたリクエストに対する権限と同じです。</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
