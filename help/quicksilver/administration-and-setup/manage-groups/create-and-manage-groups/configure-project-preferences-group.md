---
title: グループのプロジェクト環境設定の指定
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
description: グループ管理者で、Adobe Workfrontの管理者がシステム内のすべてのグループのプロジェクト環境設定をロック解除した場合、グループの環境設定を構成して、グループが作成する以降のすべてのプロジェクトに影響を与えることができます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: c69097fb-99e4-441b-9599-fd8af2dd7116
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '2643'
ht-degree: 2%

---

# グループのプロジェクト環境設定の指定

グループ管理者で、Adobe Workfrontの管理者がシステム内のすべてのグループのプロジェクト環境設定をロック解除した場合、グループの環境設定を構成して、グループが作成する以降のすべてのプロジェクトに影響を与えることができます。

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>* 通常、ロックが解除された環境設定は、無期限にロックが解除されたままになります。 Workfront管理者が再ロックすると、システム設定が再度有効になり、グループ管理者が行った環境設定は失われます。
>* プロジェクトに関連付けられたグループに設定された環境設定は、プロジェクトを作成するユーザーのホームグループに設定された環境設定よりも優先されます。
>* グループレベルの環境設定の中には、グループ用に作成するプロジェクトテンプレートに影響を与えるものもあります。 詳しくは、 [グループ領域で、グループのテンプレートの表示、操作、作成を行います](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) 記事内 [グループのプロジェクトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Workfrontの管理者がシステム・レベルでプリファレンスのロックを解除した後は、設定を行い、その設定をロックして、グループ内の全員とサブグループ内の全員が同じ設定を使用するようにできます。 これは、Workfront管理者がシステム内のすべてのユーザーに対して環境設定を設定およびロックする必要がある機能と同じです。 詳しくは、 [サブグループのプロジェクト、タスク、または問題の環境設定をロックまたはロック解除する](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


タスクと問題の基本設定、およびタイムシートと時間の基本設定に対して、グループレベルの構成も可能です。 詳しくは、 [グループのタスクと問題の環境設定を設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) および [グループのタイムシートと時間の基本設定を構成する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

Workfront管理者がプロジェクト環境設定のロックを解除する方法について詳しくは、 [システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除します](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## グループのロック解除されたプロジェクトの環境設定を構成する

>[!TIP]
>
>Workfrontの管理者は、設定/プロジェクトの環境設定/プロジェクトに移動して、ページ上部のボックスでグループの名前を検索することで、手順 1 ～ 4 をスキップできます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. プロジェクトの環境設定を構成するグループの名前をクリックします。
1. 左側のパネルで、 **プロジェクト環境設定**.
1. 表示されるページで、以下の 4 つのセクションのいずれかに進み、プロジェクトのステータス、タイムライン、ビジネス事例、死後の生活に関する環境設定を行います。

   >[!TIP]
   >
   >環境設定の上にマウスポインターを置くと、その設定がロックされていることを示すツールヒントが表示される場合は、Workfront管理者に問い合わせて、組織内のすべてのグループのロックを解除するように依頼できます。

* [プロジェクト状態](#project-status)
* [タイムライン](#timelines)
* [ビジネスケース](#business-cases)
* [終了後の操作](#life-after-death)

### プロジェクト状態 {#project-status}

グループに関連付けられた新しく作成されたプロジェクトに対して、次の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<tr><td>ユーザーがテンプレートを使用せずにプロジェクトを作成することを許可</td>
<td><p>この環境設定では、次の領域からプロジェクトを作成する際に、テンプレートを使用せずにプロジェクトを作成できます。</p>
<ul>
<li><p>プロジェクトのリストで「新規プロジェクト」オプションを使用します</p></li>

<li><p>イシューのページからイシューをプロジェクトに変換する</p></li>
</ul>

<p>この環境設定は、システムレベルでデフォルトで有効になっています。</p>
<p><b>メモ</b></p>
<p>ユーザーが異なる環境設定を持つ複数のグループに属する場合、1 つ以上のグループでこの環境設定が有効になっている場合、ユーザーはテンプレートを持たないプロジェクトを作成できます。</p>
</td></tr>
  <tr> 
   <td role="rowheader">新規プロジェクトのステータスを次に設定</td> 
   <td> <p>新規プロジェクトのステータスを決定します。</p> <p><b>メモ</b>   
     <ul> 
      <li>ここで選択したステータスを非表示にしたのがWorkfrontの管理者の場合、デフォルトのステータスはステータスリストの最初のステータスに変わります。</li> 
     </ul> 
     <ul> 
      <li data-mc-conditions="SnippetConditions-wf-groups.groups">グループプロジェクトのプリファレンスでは、デフォルトのステータスとして、ロック済みステータスまたは必須ステータスのみを選択できます。</li> 
      <li> <p>ロックされたシステムまたはグループのステータスがデフォルトのステータスとして設定され、後で誰かがそのステータスをロック解除した場合、システムは同じステータスタイプのロック済みステータスと置き換えようとします。</p> <p>見つからない場合は、必須のステータスを探します。</p> 
       <ul> 
        <li>ロック解除済みのデフォルトステータスと同じ必須ステータスがある場合、ロック解除されていても、必須ステータスがデフォルトステータスになります。</li> 
        <li>必須のステータスがロック解除済みのデフォルトのステータスに等しくない場合、ステータスリストの最初の必須ステータスがデフォルトのステータスになります。</li> 
       </ul> <p>必須ステータスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">システムプロジェクトステータスのリストへのアクセス</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">システムタスクステータスのリストへのアクセス</a>、および <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">システムの問題ステータスのリストへのアクセス</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">完了率の計算基準</td> 
   <td> <p>プロジェクトまたは親タスクの完了率は、タスクの全体的な進捗状況に基づきます。 この情報は、プロジェクトのタスクの期間または予定時間に基づいて計算できます。</p> <p>[ 期間 ] を選択した場合、プロジェクトの各タスクの [ 期間 ] でプロジェクトの全体の完了率が決定され、各サブタスクの [ 期間 ] で親タスクの完了率全体が決定されます。</p> <p>「期間」を選択する場合は、「タイムライン」セクションで、「通常の 1 労働時間あたり」と「通常の 1 週間あたりの稼働時間」を必ず指定してください。 Workfrontは、タスクの完了率を期間に基づいて計算する際にこの情報を使用します。 </p> <p>「計画時間」を選択する場合は、各プロジェクトのすべてのタスクに計画時間数が定義され、金額がゼロでないことを確認します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">進行状態に応じて、プロジェクトの状態を自動的に設定する</td> 
   <td> <p>この環境設定では、ユーザーは手動でプロジェクトの条件を設定できます（ターゲット時、リスク時、問題が発生した場合）。または、Workfrontで、タイムライン上のプロジェクトの進行状況に基づいて、条件（進捗状況ステータス）を自動的に設定できます。 プロジェクトの条件の詳細については、 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">プロジェクト条件と条件タイプの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>自動的にベースラインを作成する</p> </td> 
   <td> <p>このプリファレンスでは、プロジェクトのステータスが [ 現在 ] に変わると、タスクとプロジェクトの詳細の基準（スナップショット）が自動的に作成されます。 ベースラインの作成について詳しくは、 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">プロジェクトの基準を作成</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>パフォーマンス インデックス メソッド </p> </td> 
   <td> <p>プロジェクトの PIM(Performance Index Method) は、Workfrontがコスト効果指数 (CPI) や完了時の予測 (EAC) などの達成額指標の計算に使用する方法を制御します。 詳しくは、 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">コスト効果指数 (CPI) の計算</a>および <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完了時の推定 (EAC) を計算</a></p> 
    <ul> 
     <li><strong>時間ベース</strong>:Workfrontは、EAC や CPI などのパフォーマンス指標の計算に計画時間を使用します。 PIM が時間に基づいて計算されると、EAC は時間数として表示されます。 「計画時間」に 0 以外の値が設定されていることを確認します。</li> 
     <li> <p><strong>コストベース</strong>:Workfrontは、EAC や CPI などのパフォーマンス指標の計算に計画労務費を使用します。 ジョブの役割またはユーザーが時間あたりのコスト率に関連付けられていることを確認します。 PIM がコストに基づいて計算されると、EAC は通貨値として表示されます。</p> <p>プロジェクトマネージャは、プロジェクトレベルで、[ プロジェクトの詳細 ] の [ 財務 ] 領域を使用してこの設定を変更できます。詳細については、 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">プロジェクトの財務エリアで情報を管理します</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>完成時総コスト見積り </p> </td> 
   <td> <p>Workfrontが EAC(Estimate at Completion) の計算に使用するデータを決定します。EAC は、プロジェクトの概算合計コストを表します。</p> 
    <ul> 
     <li><strong>プロジェクトレベルで計算</strong>：親タスクおよびプロジェクトの EAC は、EAC 式に「実績時間」または「実績労務費」を入力することで決定されます。 この計算には、実績時間またはコストと費用が親タスクまたはプロジェクトに直接追加されます。</li> 
     <li> <p><strong>タスク/サブタスクからのロールアップ</strong>:親タスクとプロジェクトの EAC は、各子タスクの EAC を合計することで決定されます。 この計算では、親タスクまたはプロジェクトに直接追加された実績時間または実績コストと費用が除外されます。</p> <p>プロジェクトマネージャは、プロジェクトレベルで、[ プロジェクトの詳細 ] の [ 財務 ] 領域を使用してこの設定を変更できます。詳細については、 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">プロジェクトの財務エリアで情報を管理します</a>.</p> </li> 
    </ul> <p>EAC の計算方法について詳しくは、 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">完了時の推定 (EAC) を計算</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### タイムライン {#timelines}

グループに関連付けられた新しく作成されたプロジェクトに対して、次の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">スケジュールの基点</td> 
   <td> <p>新規プロジェクトが作成時に「開始日」からスケジュールされるか、「完了日」からスケジュールされるかを決定します。</p> 
    <ul> 
     <li><strong>開始日</strong>:新しいタスクのデフォルトは「As As A Possible Task」制約です。プロジェクトマネージャは、プロジェクトの計画開始日の指定を求められます。</li> 
     <li><strong>完了日</strong>:新規タスクのデフォルトは「可能な限り遅延」タスク制約です。プロジェクトマネージャは、プロジェクトの計画完了日の指定を求められます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザーの休暇</td> 
   <td> <p>タスクのプライマリ担当者が、そのタスクの予定日をプロジェクト上で調整するかどうかを指定します。</p> 
    <ul> 
     <li> <p><strong>タスク期間でのユーザーのオフ時間を考慮する</strong>:タスクのプライマリに予定されているオフタイム担当者は、タスクの期間中にオフタイムが発生した場合に、タスクの予定日を調整します。 これはデフォルト設定です。 </p> <p>例えば、「可能な限り早く」という制約を持つプライマリが 6 月 1 日に開始し、6 月 3 日に完了するようにスケジュールされていて、担当者が 6 月 2 日に「タイムオフ」とマークされている場合、タスクの計画日は 6 月 1 日から 6 月 4 日に調整されます。</p> <p><b>重要</b>:この設定を選択した場合、タスクの期間は変更されません。 タスク制約に応じて、計画日のみが変更されます。</p> </li> 
     <li><strong>タスク期間のユーザーのオフ時間を無視する</strong>:プライマリの担当者が期間中に休暇を取った場合でも、プロジェクトの各タスクの計画日は、当初の計画通りに保たれます。</li> 
    </ul> <p>この設定のオプションを選択する際は、次の点に注意してください。</p> 
    <ul> 
     <li>この設定を変更すると、変更後に作成されたプロジェクトとテンプレートのみが更新された設定を継承します。 </li> 
     <li> <p>タスクの [ タスク制約 ] の値によって、調整する予定タスクの日付が決まります。 </p> 
      <ul> 
       <li>予定開始付</li> 
       <li>予定完了日</li> 
       <li>両方の日付</li> 
       <li>どちらの日付も。 </li> 
      </ul> <p>たとえば、プライマリに固定日付の制約がある場合、タスク期間でのユーザーのタイムオフを考慮するオプションが選択されていても、タスク担当者がタイムオフになる日付は調整されません。 タスクの制約について詳しくは、 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">タスク制約の概要</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>プロジェクトタイムラインは自動的に再計算されます</strong> </p> </td> 
   <td> <p>プロジェクトのタイムラインを再計算するタイミングを指定します。 プロジェクトタイムラインの再計算について詳しくは、 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">プロジェクトタイムラインを再計算</a>.</p> <p>次のオプションは、デフォルトで有効になっています。 次の設定を 1 つ以上選択できます。</p> 
    <ul> 
     <li> <p><strong>毎晩</strong>:毎晩プロジェクトのタイムラインを再計算する場合に選択します。 タイムラインに影響を与える可能性のあるプロジェクトに対する変更は、すぐには表示されません。 Workfront​で​は、次の両方の条件を満たすプロジェクトの場合にのみ、夜間のタイムラインが再計算されます。</p> <p> 
       <ul> 
        <li>ステータスが「現在」</li> 
        <li>過去 3 か月間に更新があります</li> 
       </ul> </p> </li> 
     <li> <p><strong>プロジェクトの範囲が変更されたとき</strong>:プロジェクト範囲の変更が発生したときにプロジェクトタイムラインをすぐに再計算する場合は、これを選択します。 プロジェクト範囲の変更を構成する情報については、 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">プロジェクトタイムラインを再計算</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>複数のユーザーがタスクに割り当てられている場合は、</strong> </p> </td> 
   <td> <p>プロジェクトにスケジュールが割り当てられていない場合、またはタスクに割り当てられたユーザーにスケジュールが割り当てられていない場合、Workfrontはシステムのデフォルトスケジュールを使用してタスクのタイムラインを計算します。</p> <p>プロジェクト内の同じタスクに複数のユーザーを割り当て、スケジュールが割り当てられ、タスクに割り当てられたユーザーにもスケジュールが割り当てられている場合、Workfrontは次のスケジュールを使用します。</p> 
    <ul> 
     <li><strong>プライマリ割り当て</strong>:Workfrontは、タスク上のプライマリ割り当てのスケジュールを使用して、タイムラインを計算します。</li> 
     <li><strong>プロジェクト</strong>:Workfrontは、プロジェクトのスケジュールを使用して、各タスクのタイムラインを計算します。</li> 
    </ul> <p>スケジュールについて詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">スケジュールの作成</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>タイムラインの計算 </p> </td> 
   <td> 
    <ul> 
     <li><strong>1 日あたりの通常の時間</strong>:プロジェクトで作業するユーザーの通常の稼働日の時間数を設定します。 デフォルトは 8 時間です。</li> 
    </ul> 
    <ul> 
     <li><strong>週別の通常の稼働日数</strong>:プロジェクトで作業するユーザーに対して、標準作業週を設定します。 デフォルトは 5 日です。</li> 
    </ul> <p>これらの 2 つのオプションは、日を時間に、または週を日に変換します。</p> <p>例えば、タスクの期間が 8 時間で、期間が計画時間に基づいて計算される場合、Workfrontは期間を日数として表示するために、それらの時間を日に変換します。</p> <p>「 Typical work days per week 」フィールドから、Workfrontはシステムのフルタイム相当 (FTE) 値を計算します。 これは、Workfrontがユーザーの配分を計算する際に使用するものです。</p> <p>これらの値は、プロジェクトのタイムラインを計画したり、リソースの予算を作成したり、プロジェクトに対する時間を記録する際に使用されます。 </p> <p>これらは、システム内のユーザーのタイムシートを設定する際には使用されません。詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">タイムシートと時間の基本設定を構成する</a>.</p> <p><b>注意</b>:Workfrontの管理者は、タイムライン計算環境設定のロックを解除できません。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p><strong>カスタム四半期</strong> </p> </td> 
   <td> <p>プロジェクトで作業するユーザー向けに年別のカスタム四半期を設定します。 カスタム四半期は、通常、暦年の四半期の従来の分類と一致しない四半期です。 複数のカスタム四半期を追加できます。 詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">プロジェクトのカスタム四半期を有効にする</a>.</p> <p><b>注意</b>:Workfront管理者は、カスタム四半期の環境設定のロックを解除できません。</p> </td> 
  </tr> 
 </tbody> 
</table>

### ビジネスケース {#business-cases}

プロジェクトリクエストを送信するために、グループに関連付けられた新しく作成したプロジェクト用のビジネスケースを作成できます。 環境設定を定義して、 **ビジネス事例** フォーム。 Optimizer などの他のツールが正しく更新されるように、これらのオプションを有効にすることをお勧めします。 各フィールドに何が表示されるかについて詳しくは、 [ビジネスケースの定義](../../../manage-work/projects/define-a-business-case/define-business-case.md).

Workfront管理者がビジネスケースのセクションを有効にした後、プロジェクト所有者は、プロジェクトレベルでビジネスケースを作成できます。 ビジネス事例の作成の詳細は、 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### 終了後の操作  {#life-after-death}

グループに関連付けられた新しく作成されたプロジェクトに対して、次の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><strong>プロジェクトが完了とマークされた後も、担当者は次の操作を実行できます</strong> </p> </td> 
   <td> <p>プロジェクトのステータスが「完了」とマークされた後にタスクまたは問題を削除できるかどうかに関する、組織（またはグループのプロジェクト環境設定を構成している場合はグループ）のルールを決定します。</p> 
    <ul> 
     <li><strong>タスクを削除</strong>:プロジェクトが「完了」とマークされた後に、ユーザーがプロジェクトからタスクを削除できるようにします。<br></li> 
     <li><strong>問題を削除</strong>:プロジェクトが「完了」とマークされた後で、ユーザーがプロジェクトから問題を削除できます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><strong>プロジェクトが「完了」、「無効」、または「承認待ち」とマークされた後も、担当者は引き続き承認可能です</strong> </p> </td> 
   <td> <p>プロジェクトのステータスがマークされた後にプロジェクト内のタスク、問題、ドキュメント、その他のオブジェクトに何が起こるかに関する、組織（またはグループのプロジェクトプリファレンスを設定する場合は、グループ）の規則を決定します <strong>完了</strong>, <strong>Dead</strong>または <strong>承認待ち</strong>.</p> 
    <ul> 
     <li><strong>タスクの追加と編集</strong> ユーザーが以下を実行できるようにします。 
      <ul> 
       <li>プロジェクトが「完了」、「無効」、または「承認待ち」とマークされた後に、プロジェクト内のタスクを編集します。 これには、時間の追加やタスクの費用エントリの変更が含まれます。</li> 
       <li>プロジェクトにタスクを追加します。</li> 
      </ul></li> 
     <li><strong>イシューの追加と編集</strong>:ユーザーが以下を実行できるようにします。 
      <ul> 
       <li>プロジェクトが「完了」、「無効」または「承認待ち」とマークされた後、プロジェクト内の問題を編集します。</li> 
       <li>プロジェクトが「完了」または「無効」とマークされた後で、プロジェクトに問題を追加します。 （「承認待ち」のプロジェクトにはイシューを追加できません。）</li> 
      </ul></li> 
     <li> <p><strong>プロジェクトとそのタスクおよびタスクにドキュメントを追加</strong>:プロジェクトが「完了」または「無効」とマークされた後で、ユーザーがプロジェクトにドキュメントを追加（またはプロジェクト内のタスクや問題にドキュメントを追加）できるようにします。</p> <p>このオプションは、承認待ちのプロジェクトには適用されません。</p> </li> 
     <li> <p><strong>テンプレートの添付</strong>:プロジェクトが「完了」または「無効」とマークされた後で、ユーザーがプロジェクトにテンプレートを添付できます。</p> <p>このオプションは、承認待ちのプロジェクトには適用されません。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
