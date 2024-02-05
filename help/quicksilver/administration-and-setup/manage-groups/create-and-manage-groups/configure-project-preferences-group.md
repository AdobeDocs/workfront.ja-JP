---
title: グループのプロジェクト環境設定の指定
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: Adobe Workfront 管理者がシステム内のすべてのグループのプロジェクト環境設定のロックを解除している場合は、グループ管理者は、グループが作成する後続のすべてのプロジェクトに影響を与えるように、グループのその環境設定を指定することができます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '2658'
ht-degree: 99%

---

# グループのプロジェクト環境設定の指定

Adobe Workfront 管理者がシステム内のすべてのグループのプロジェクト環境設定のロックを解除している場合は、グループ管理者は、グループが作成する後続のすべてのプロジェクトに影響を与えるように、グループのその環境設定を指定することができます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>* 通常、ロック解除された環境設定は、無期限にロック解除されたままになります。Workfront 管理者が再ロックすると、システム設定が再度有効になり、グループ管理者が行った環境設定は失われます。
>* プロジェクトに関連付けられたグループ向けの環境設定のセットは、プロジェクトを作成するユーザーのホームグループ向けの環境設定のセットよりも優先されます。
>* グループレベルの環境設定の中には、グループ用に作成するプロジェクトテンプレートに影響を与えるものがあります。詳しくは、[グループのプロジェクトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md)の記事内の、[グループエリアから、グループのテンプレートの表示、操作、作成を実施](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view)の節を参照してください。
>
>* Workfront 管理者がシステムレベルで環境設定をロック解除した後は、これを設定してからロックすると、グループおよびそのサブグループ内の全員が、同じ設定を使用できるようになります。これは、Workfront 管理者がシステム内のすべてのユーザーに対して環境設定を指定およびロックするための機能と同じです。詳しくは、[サブグループのプロジェクト、タスク、イシューの環境設定のロックまたはロック解除](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)を参照してください。
>

タスクとイシューの環境設定、およびタイムシートと時間の環境設定を、グループレベルで指定することもできます。詳しくは、[グループのタスクとイシューの環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)および[グループのタイムシートと時間の環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)を参照してください。

Workfront 管理者が環境設定をロック解除する方法について詳しくは、[システム内のすべてのグループのプロジェクト環境設定のロックまたはロック解除](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)を参照してください。

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

&#42;ご利用のプランまたはライセンスタイプを確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## グループのロック解除されたプロジェクトの環境設定の指定

>[!TIP]
>
>Workfront 管理者は、設定／プロジェクトの環境設定／プロジェクトに移動して、ページの上部にあるボックスでグループの名前を検索することにより、手順 1 から 4 をスキップできます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、**設定**&#x200B;アイコン ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、**グループ** ![](assets/groups-icon.png)をクリックします。

1. プロジェクトの環境設定を指定するグループの名前をクリックします。
1. 左側のパネルで、**プロジェクトの環境設定**&#x200B;をクリックします。
1. 表示されるページで、以下の 4 つのセクションのいずれかに進み、プロジェクトのステータス、タイムライン、ビジネスケース、終了後の操作に関する環境設定を行います。

   >[!TIP]
   >
   >環境設定にポインタを合わせると、その設定がロックされていることを示すツールヒントが表示される場合は、Workfront 管理者に問い合わせて、組織内のすべてのグループについてロックを解除するように依頼します。

* [プロジェクトのステータス](#project-status)
* [タイムライン](#timelines)
* [ビジネスケース](#business-cases)
* [終了後の操作](#life-after-death)

### プロジェクトのステータス {#project-status}

グループに関連付けられた新しく作成されたプロジェクトに対して、以下の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>ユーザーがテンプレートを使用せずにプロジェクトを作成することを許可</td>
<td><p>この環境設定では、ユーザーが次の領域からプロジェクトを作成する際に、テンプレートを使用せずにプロジェクトを作成できます。</p>
<ul>
<li><p>プロジェクトのリストで「新規プロジェクト」オプションを使用</p></li>

<li><p>イシューページからイシューをプロジェクトに変換する</p></li>
</ul>

<p>この環境設定は、システムレベルでデフォルトで有効になっています。</p>
<p><b>メモ</b></p>
<p>ユーザーが異なる環境設定を持つ複数のグループに属していて、1 つ以上のグループでこの環境設定が有効になっている場合、ユーザーはテンプレートを使用せずにプロジェクトを作成できます。</p>
</td></tr>
  <tr> 
   <td role="rowheader">新規プロジェクトのステータスを次のように設定</td> 
   <td> <p>新規プロジェクトのステータスを決定します。</p> <p><b>メモ</b>   
     <ul> 
      <li>ご自身または別の Workfront 管理者がここで選択したステータスを非表示にすると、デフォルトのステータスは、ステータスリストの最初のステータスに変わります。</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">グループプロジェクトの環境設定では、ロック済みステータスまたは必須ステータスのみを、デフォルトのステータスとして選択できます。</li> 
      <li> <p>ロックされたシステムまたはグループのステータスがデフォルトのステータスとして設定され、後で誰かがそのステータスをロック解除した場合、システムはそのステータスを、同じステータスタイプのロックされているステータスと置き換えようとします。</p> <p>見つからない場合、システムは必須ステータスを探します。</p> 
       <ul> 
        <li>ロック解除されているデフォルトのステータスと同等の必須ステータスがある場合、ロック解除されている場合でも、その必須ステータスがデフォルトのステータスになります。</li> 
        <li>必須ステータスのいずれもロック解除されているデフォルトのステータスに相当しない場合、ステータスリストの最初の必須ステータスがデフォルトのステータスになります。</li> 
       </ul> <p>必須ステータスについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">システムのプロジェクトステータスのリストへのアクセス</a>、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">システムのタスクステータスのリストへのアクセス</a>および<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">システムのイシューステータスのリストへのアクセス</a>の各記事を参照してください。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">以下に基づいて完了率を計算</td> 
   <td> <p>プロジェクトまたは親タスクの完了率は、タスクの全体的な進捗状況に基づきます。この情報は、プロジェクトのタスクの期間または予定時間数に基づいて計算できます。</p> <p>期間を選択した場合、プロジェクト内のそれぞれのタスクの期間でプロジェクトの全体的な完了率が決まり、それぞれのサブタスクの期間で親タスクの全体的な完了率が決まります。</p> <p>期間を選択する場合は、「タイムライン」セクションで、作業日あたりの標準的な時間数と 1 週間あたりの標準的な作業日数を必ず指定してください。Workfront では、期間に基づいてタスクの完了率を計算する際にこの情報を使用します。 </p> <p>予定時間数を選択する場合は、それぞれのプロジェクトのすべてのタスクに予定時間数の数値が定義され、その数値がゼロでないことを確認します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">進捗ステータスに応じて、プロジェクトの状況を自動的に設定</td> 
   <td> <p>この環境設定を使用すると、ユーザーはプロジェクトの状況（目標どおり、リスクあり、問題あり）を手動で設定できます。あるいはタイムライン上のプロジェクトの進行状況に基づいて、Workfront に状況（進捗ステータス）を自動的に設定させることができます。プロジェクト状況について詳しくは、<a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">プロジェクト状況と状況タイプの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>自動的にベースラインを作成</p> </td> 
   <td> <p>この環境設定では、プロジェクトのステータスが現在に変わると、タスクおよびプロジェクト詳細のベースライン（スナップショット）が自動的に作成されます。ベースラインの作成について詳しくは、<a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">プロジェクトのベースラインの作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>パフォーマンスインデックスメソッド </p> </td> 
   <td> <p>プロジェクトのパフォーマンスインデックスメソッド（PIM）は、Workfront がコスト効率指数（CPI）や完了時の見積り（EAC）などの出来高指標を計算するために使用する方法を制御します。詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">コスト効率指数（CPI）の計算</a>および<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完了時の見積り（EAC）の計算</a>を参照してください。</p> 
    <ul> 
     <li><strong>時間ベース</strong>：Workfront は予定時間数を使用して、EAC や CPI などのパフォーマンス指標を計算します。PIM が時間数に基づいて計算される場合、EAC は時間数として表示されます。予定時間数に 0 以外の値が設定されていることを確認します。</li> 
     <li> <p><strong>コストベース</strong>：Workfront は、予定労力コストを使用して、EAC や CPI などのパフォーマンス指標を計算します。担当業務またはユーザーが 1 時間当たりのコスト率に関連付けられていることを確認します。PIM がコストに基づいて計算される場合、EAC は通貨値として表示されます。</p> <p>プロジェクトマネージャーは、プロジェクト詳細にある財務エリアを使用して、プロジェクトレベルでこの設定を変更できます。詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">プロジェクトの財務エリアでの情報の管理</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>完成時総コスト見積り </p> </td> 
   <td> <p>プロジェクトの見込み総コストを表す完成時総コスト見積り（EAC）を計算するために Workfront がどのデータを使用するかを決定します。</p> 
    <ul> 
     <li><strong>プロジェクトレベルで計算</strong>：親タスクとプロジェクトの EAC は、EAC 式の実際の時間数または実際の労力コストを入力すると決定されます。この計算には、親タスクやプロジェクトに直接追加された実際の時間数またはコストと費用が含まれます。</li> 
     <li> <p><strong>タスクやサブタスクからロールアップ</strong>：親タスクとプロジェクトの EAC は、それぞれの子タスクの EAC を合計することによって決定されます。この計算からは、親タスクやプロジェクトに直接追加された実際の時間数および実際のコストと費用が除外されます。</p> <p>プロジェクトマネージャーは、プロジェクト詳細にある財務エリアを使用して、プロジェクトレベルでこの設定を変更できます。詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">プロジェクトの財務エリアでの情報の管理</a>を参照してください。</p> </li> 
    </ul> <p>EAC の計算方法について詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完成時総コスト見積り（EAC）の計算</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### タイムライン {#timelines}

グループに関連付けられた新しく作成されたプロジェクトに対して、以下の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">スケジュールの基点</td> 
   <td> <p>新規プロジェクトが作成時に開始日からスケジュールされるか、完了日からスケジュールされるかを決定します。</p> 
    <ul> 
     <li><strong>開始日</strong>：新規タスクのデフォルトは「できるだけ早く」というタスク制約事項で、プロジェクトマネージャーにはプロジェクトの予定開始日の指定を求められます。</li> 
     <li><strong>完了日</strong>：新しいタスクのデフォルトは「可能な限り遅延する」タスク制約で、プロジェクトマネージャーはプロジェクトの完了予定日の指定を求められます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザーの休暇</td> 
   <td> <p>プロジェクトのタスクの予定日をそのタスクのプライマリ担当者の休暇によって調整するかどうかを指定します。</p> 
    <ul> 
     <li> <p><strong>タスク期間でのユーザーの休暇を考慮する</strong>：タスクのプライマリ担当者にスケジュールされている休暇がタスクの期間中に発生する場合、その休暇によってタスクの予定日が調整されます。これはデフォルトの設定です。 </p> <p>例えば、「可能な限り早く」という制約を持つタスクが 6月1日に開始し 6月3日に完了するようにスケジュールされ、6月2日がプライマリ担当者の休暇に指定されている場合、タスクの予定日は 6月1日から 6月4日までに調整されます。</p> <p><b>重要</b>：この設定を選択しても、タスクの期間は変わりません。タスクの制約に応じて、予定日のみが変更されます。</p> </li> 
     <li><strong>タスク期間のユーザーの休暇を無視する</strong>：プロジェクトの各タスクの予定日は、タスクのプライマリ担当者がその期間中に休暇を取る場合でも、元の予定日のまま変わりません。</li> 
    </ul> <p>この設定のオプションを選択する際は、次の点に注意してください。</p> 
    <ul> 
     <li>この設定を変更すると、変更後に作成されたプロジェクトとテンプレートのみが、更新された設定を継承します。 </li> 
     <li> <p>タスクの「タスクの制約」値によって、調整するタスク予定日が決まります。 </p> 
      <ul> 
       <li>予定開始日</li> 
       <li>予定完了日</li> 
       <li>両方の日付</li> 
       <li>どちらも日付でもない </li> 
      </ul> <p>例えば、タスクに固定日付の制約があると、タスク継続期間中のユーザーの休暇を考慮するが選択されていても、プライマリ担当者が休暇をとった場合に日付が調整されません。タスクの制約については、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">タスクの制約の概要</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>プロジェクトタイムラインを自動的に再計算するタイミング</strong> </p> </td> 
   <td> <p>プロジェクトのタイムラインを再計算するタイミングを指定します。プロジェクトタイムラインの再計算については、<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">プロジェクトタイムラインの再計算</a>を参照してください。</p> <p>次のオプションが、デフォルトで有効になっています。以下の設定を 1 つ以上選択できます。</p> 
    <ul> 
     <li> <p><strong>毎晩</strong>：毎晩プロジェクトのタイムラインを再計算する場合に選択します。タイムラインに影響を与える可能性のある変更をプロジェクトに対して行っても、それはすぐには表示されません。Workfront では、以下の条件がすべて満たされるプロジェクトの場合にのみ、夜間にタイムラインを再計算します。</p> <p> 
       <ul> 
        <li>ステータスが「現在」であること</li> 
        <li>過去 3 か月間に更新があった</li> 
       </ul> </p> </li> 
     <li> <p><strong>プロジェクトのスコープが変更されたとき</strong>：プロジェクト範囲の変更に伴いプロジェクトのタイムラインを直ちに再計算する場合に選択します。プロジェクト範囲の変更の構成要素については、<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">プロジェクトタイムラインの再計算</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>複数のユーザーがタスクに割り当てられた時は、以下のスケジュールを使用する</strong> </p> </td> 
   <td> <p>プロジェクトにスケジュールが割り当てられていない場合や、タスクに割り当てられたユーザーにスケジュールが割り当てられていない場合、Workfront では、システムのデフォルトのスケジュールを使用して、タスクのタイムラインを計算します。</p> <p>プロジェクトの同じタスクに複数のユーザーを割り当て、そのタスクに割り当てられているユーザーにもスケジュールが割り当てられている場合、Workfront では以下のスケジュールを使用します。</p> 
    <ul> 
     <li><strong>プライマリ割り当て</strong>：Workfront では、タスクに対するプライマリ割り当てのスケジュールを使用して、タイムラインを計算します。</li> 
     <li><strong>プロジェクト</strong>：Workfront では、プロジェクトのスケジュールを使用して、各タスクのタイムラインを計算します。</li> 
    </ul> <p>スケジュールについて詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">スケジュールの作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>タイムラインの計算 </p> </td> 
   <td> 
    <ul> 
     <li><strong>1 日あたりの通常の時間</strong>：プロジェクトを担当するユーザーの通常の就業日の時間数を設定します。デフォルトは 8 時間です。</li> 
    </ul> 
    <ul> 
     <li><strong>週別の通常の稼働日数</strong>：プロジェクトを担当するユーザーの標準の週労働時間を設定します。デフォルトは 5 日です。</li> 
    </ul> <p>これらの 2 つのオプションは、日数を時間数に、または週数を日数に変換します。</p> <p>例えば、予定時間数が 8 時間のタスクがあり、期間が予定時間数に基づいて計算される場合、Workfront では、時間数を日数に変換して、期間を日数で表示します。</p> <p>Workfront では、「1 週間あたりの標準的な作業日数」フィールドからシステムのフルタイム当量（FTE）値を計算します。これは、Workfront でユーザーへの割り当てを計算する際に使用するものです。</p> <p>これらの値は、プロジェクトのタイムラインを計画したり、リソースの予算を計上したり、プロジェクトに対する時間を記録したりする際に使用されます。 </p> <p>これらの値は、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">タイムシートと時間の環境設定の指定</a>で説明しているとおり、システム内のユーザーのタイムシートを設定する際には使用されません。</p> <p><b>メモ</b>：Workfront 管理者はタイムライン計算環境設定のロックを解除できません。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>カスタム四半期</strong> </p> </td> 
   <td> <p>プロジェクトを担当するユーザー向けに、カスタム四半期を設定します。カスタム四半期は通常、暦年の従来の四半期分類と一致しない四半期です。複数のカスタム四半期を追加できます。詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">プロジェクトのカスタム四半期の有効化</a>を参照してください。</p> <p><b>メモ</b>：Workfront 管理者はカスタム四半期の環境設定をロック解除できません。</p> </td> 
  </tr> 
 </tbody> 
</table>

### ビジネスケース {#business-cases}

グループに関連付けられた新しく作成されたプロジェクトのビジネスケースを作成して、プロジェクトリクエストを送信できます。**ビジネスケース**&#x200B;フォーム上でどのエリアを表示するかを指定する環境設定を定義できます。ポートフォリオオプティマイザーなどの他のツールで適切に更新されるように、これらのオプションを有効にすることをお勧めします。各フィールドに何が表示されるかについて詳しくは、 [ビジネスケースの定義：記事インデックス](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Workfront 管理者がビジネスケースのセクションを有効にしてから、プロジェクト所有者がプロジェクトレベルでビジネスケースを作成できます。ビジネスケースの作成については、[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

### 終了後の操作  {#life-after-death}

グループに関連付けられた新しく作成されたプロジェクトに対して、以下の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>プロジェクトの状態が完了となった後も許可する操作</strong> </p> </td> 
   <td> <p>プロジェクトステータスが「完了」とマークされた後にタスクやイシューを削除できるかどうかに関して、組織（または、グループのプロジェクト環境設定を指定している場合はグループ）のルールを決定します。</p> 
    <ul> 
     <li><strong>タスクを削除</strong>：プロジェクトが「完了」とマークされた後で、ユーザーがプロジェクトからタスクを削除できます。<br></li> 
     <li><strong>イシューを削除</strong>：プロジェクトが「完了」とマークされた後で、ユーザーがプロジェクトからイシューを削除できます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>プロジェクトのステータスが「完了」、「無効」、または「承認待ち」となった後も許可する操作</strong> </p> </td> 
   <td> <p>プロジェクトのステータスが「<strong>完了</strong>」、「<strong>無効</strong>」、または「<strong>承認待ち</strong>」とマークされた後にプロジェクト内のタスク、イシュー、ドキュメントおよびその他のオブジェクトがどうなるかに関して、組織（または、グループのプロジェクト環境設定を指定している場合はグループ）のルールを決定します。</p> 
    <ul> 
     <li><strong>タスクの追加と編集</strong>：ユーザーが以下を行えます。 
      <ul> 
       <li>プロジェクトが「完了」、「無効」、または「承認待ち」とマークされた後で、プロジェクト内のタスクを編集します。これには、時間数の追加やタスクの費用エントリの変更などが含まれます。</li> 
       <li>プロジェクトにタスクを追加する。</li> 
      </ul></li> 
     <li><strong>イシューの追加と編集</strong>：ユーザーが以下を行えます。 
      <ul> 
       <li>プロジェクトが「完了」、「停止」、または「承認待ち」とマークされた後で、プロジェクト内のイシューを編集します。</li> 
       <li>プロジェクトが「完了」または「無効」とマークされた後で、プロジェクトにイシューを追加します。（「承認待ち」のプロジェクトにはイシューを追加できません。）</li> 
      </ul></li> 
     <li> <p><strong>プロジェクトとそのタスクおよびイシューにドキュメントを追加</strong>：プロジェクトが「完了」または「無効」とマークされた後で、ユーザーがプロジェクトにドキュメントを追加（またはプロジェクト内のタスクやイシューにドキュメントを追加）できます。</p> <p>このオプションは、承認保留中のプロジェクトには適用されません。</p> </li> 
     <li> <p><strong>テンプレートの添付</strong>：プロジェクトが「完了」または「無効」とマークされた後で、ユーザーがプロジェクトにテンプレートを添付できます。</p> <p>このオプションは、承認保留中のプロジェクトには適用されません。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
