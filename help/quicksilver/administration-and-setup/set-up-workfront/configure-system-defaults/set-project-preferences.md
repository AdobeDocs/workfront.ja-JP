---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: システム全体のプロジェクト環境設定を指定
description: ' [!DNL Adobe Workfront]  管理者は、システム全体で作成されるすべてのプロジェクトに対して、デフォルトの環境設定を指定できます。これらの環境設定は、プロジェクト、タスクおよびイシューの動作に影響を与えます。'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: cf044c8cff6b1172ec460ae232cd07c9b7c808b7
workflow-type: tm+mt
source-wordcount: '2513'
ht-degree: 90%

---

# システム全体のプロジェクト環境設定を指定

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] 管理者は、システム全体で作成されるすべてのプロジェクトに対して、デフォルトの環境設定を指定できます。これらの環境設定は、プロジェクト、タスクおよびイシューの動作に影響を与えます。

>[!NOTE]
>
>デフォルトではこれらの環境設定はロックされており、グループ管理者がグループレベルで変更することは、システム全体のすべてのグループに対して環境設定のロックを解除しない限りできません。詳しくは、[システム内のすべてのグループに対するプロジェクト環境設定のロックまたはロック解除](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] プラン</p></td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規： [!UICONTROL Standard]</p>
   または
   <p>現在： [!UICONTROL プラン ]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!UICONTROL System Administrator]</p> <p><b>メモ</b>：</p><p>それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 組織全体のプロジェクト環境設定の構成

{{step-1-to-setup}}

1. 左側のパネルで、**[!UICONTROL プロジェクト環境設定]**／**[!UICONTROL プロジェクト]**&#x200B;をクリックします。

1. 次の日： **プロジェクト環境設定** ページで、以下の 4 つのセクションのいずれかに進み、の環境設定を指定します。 [!UICONTROL プロジェクトのステータス], [!UICONTROL タイムライン], [!UICONTROL ビジネス事例]、および [!UICONTROL 死後の生活].
1. 組織全体のすべてのグループで同じプロジェクトプリファレンスを使用する場合は、各プリファレンスがロックされていることを確認します ![](assets/lock-toggle-button.png) （これはデフォルト）。

   >[!IMPORTANT]
   >
   >プロジェクト環境設定がロックされると、その環境設定に対して行った変更は、システム内のすべてのグループに継承されます。組織全体のユーザーやグループとコミュニケーションを取り、すべてのニーズがプロジェクト環境設定で指定した方法で確実に対応されるようにすることが重要です。

   環境設定をロック解除して、すべてのグループがそれぞれで環境設定を指定して管理できるようにする方法について詳しくは、[システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)を参照してください。

1. 「**[!UICONTROL 保存]**」をクリックします。

* [[!UICONTROL プロジェクトのステータス]](#project-status)
* [[!UICONTROL タイムライン]](#timelines)
* [[!UICONTROL ビジネスケース]](#business-cases)
* [[!UICONTROL 終了後の操作]](#life-after-death)

### プロジェクトのステータス {#project-status}

システム全体で新しく作成されたプロジェクトに対して、次の環境設定を指定します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Allow users to create projects without using a template]</td> 
   <td>  <p>この環境設定では、ユーザーが次の領域からプロジェクトを作成する際に、テンプレートを使用せずにプロジェクトを作成できます。 </p>
      <ul>
        <li>
        <p>プロジェクトのリストで [!UICONTROL New Project] オプションを使用する</p>
        </li>
          <li>
          <p>イシューページからイシューをプロジェクトに変換する</p>
          </li>
         </ul>
        <p>この環境設定はデフォルトで有効になっています。 </p> 
        <p><b>メモ</b></p>
        <p> グループ管理者は、グループのこの環境設定を変更できます。ユーザーが異なる環境設定を持つ複数のグループに属している場合、ホームグループでこの環境設定が有効になっていると、ユーザーはテンプレートを使用せずにプロジェクトを作成できます。</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL Set new project's status to]</td> 
   <td> <p>新規プロジェクトのステータスを決定します。</p>  <p><b>メモ</b>  
     <ul> 
      <li>あなた自身または別の [!DNL Workfront] 管理者がここで選択したステータスを非表示にすると、デフォルトのステータスは、ステータスリストの最初のステータスに変わります。</li> 
     </ul> 
     <ul> 
      <li> <p>ロックされたシステムまたはグループのステータスがデフォルトのステータスとして設定され、後で誰かがそのステータスをロック解除した場合、システムはそのステータスを、同じステータスタイプのロックされているステータスと置き換えようとします。</p> <p>見つからない場合、システムは必須ステータスを探します。</p> 
       <ul> 
        <li>ロック解除されているデフォルトのステータスと同等の必須ステータスがある場合、ロック解除されている場合でも、その必須ステータスがデフォルトのステータスになります。</li> 
        <li>必須ステータスのいずれもロック解除されているデフォルトのステータスに相当しない場合、ステータスリストの最初の必須ステータスがデフォルトのステータスになります。</li> 
       </ul> <p>必須ステータスについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">システムのプロジェクトステータスのリストへのアクセス</a>、<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">システムのタスクステータスのリストへのアクセス</a>、および<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">システムのイシューステータスのリストへのアクセス</a>の各記事を参照してください。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calculate Percent Complete based on]</td> 
   <td> <p>プロジェクトまたは親タスクの完了率は、タスクの全体的な進捗状況に基づきます。この情報は、プロジェクトのタスクの期間または予定時間数に基づいて計算できます。</p> <p>「[!UICONTROL Duration]」を選択した場合、プロジェクト内の各タスクの期間でプロジェクトの全体的な完了率が決まり、各サブタスクの期間で親タスクの全体的な完了率が決まります。</p> <p>「[!UICONTROL Duration]」を選択した場合は、「[!UICONTROL Timelines]」セクションで「[!UICONTROL Typical hours per work day]」と「[!UICONTROL Typical work days per week]」を必ず指定してください。[!DNL Workfront] では、期間に基づいてタスクの完了率を計算する際にこの情報を使用します。 </p> <p>「[!UICONTROL Planned Hours]」を選択する場合、各プロジェクトのすべてのタスクに「[!UICONTROL Planned Hours]」の数値が定義されており、その数値がゼロでないことを確認します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Automatically set the project's Condition based on the Progress Status]</td> 
   <td> <p>この環境設定を使用すると、ユーザーは、プロジェクトの [!UICONTROL 条件 ] を手動で ([!UICONTROL On Target]、[!UICONTROL At Risk]、[!UICONTROL In Troble]) に設定したり、 [!DNL Workfront] タイムライン上のプロジェクトの進行状況に基づいて、[!UICONTROL 条件 ]（進行状況ステータス）を自動的に設定します。 プロジェクト状況について詳しくは、<a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">プロジェクト状況と状況タイプの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create baselines automatically]</p> </td> 
   <td> <p>この環境設定では、プロジェクトのステータスが「[!UICONTROL Current]」に変わると、タスクおよびプロジェクト詳細のベースライン（スナップショット）が自動的に作成されます。ベースラインの作成については、<a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">プロジェクトベースラインの作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Performance Index Method] </p> </td> 
   <td> <p>プロジェクトのパフォーマンスインデックスメソッド（PIM）は、[!DNL Workfront] で[!UICONTROL Cost Performance Index]（CPI）や[!UICONTROL Estimate At Completion]（EAC）などの出来高指標の計算に使用される方法を制御します。詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Cost Performance Index]（CPI）の計算</a>と<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Calculate Estimate At Completion]（EAC）</a>を参照してください。</p> 
    <ul> 
     <li><strong>[!UICONTROL Hour-based]</strong>：[!DNL Workfront] では、「[!UICONTROL Planned Hours]」を使用して EAC や CPI などのパフォーマンス指標を計算します。PIM が時間数に基づいて計算される場合、EAC は時間数として表示されます。「[!UICONTROL Planned Hours]」に 0 以外の値が設定されていることを確認してください。</li> 
     <li> <p><strong>[!UICONTROL Cost-based]</strong>：[!DNL Workfront] では、「[!UICONTROL Planned Labor Cost]」を使用して EAC や CPI などのパフォーマンス指標を計算します。担当業務またはユーザーが 1 時間当たりのコスト率に関連付けられていることを確認します。PIM がコストに基づいて計算される場合、EAC は通貨値として表示されます。</p> <p>プロジェクトマネージャーは、[!UICONTROL Project Details]の[!UICONTROL Finance]エリアを使用して、この設定をプロジェクトレベルで変更できます。詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">プロジェクトの[!UICONTROL Finance]エリアでの情報の管理</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Estimate at Completion ]</p> </td> 
   <td> <p>プロジェクトの見込み総コストを表す[!UICONTROL Estimate at Completion]（EAC）の計算に [!DNL Workfront] で使用されるデータを決定します。</p> 
    <ul> 
     <li><strong>[!UICONTROL プロジェクトレベルで計算 ]</strong>：親タスクおよびプロジェクトの EAC は、EAC 式に [!UICONTROL 実際の時間 ] または [!UICONTROL 実際の労務費 ] を入力することで決定されます。 計算には、親タスクまたはプロジェクトに直接追加された[!UICONTROL Actual Hours]または[!UICONTROL Costs and Expenses]が含まれます。</li> 
     <li> <p><strong>[!UICONTROL Roll up from tasks/subtasks]</strong>：子タスクごとの EAC を合計することで、親タスクおよびプロジェクトの EAC が決定されます。この計算では、親タスクまたはプロジェクトに直接追加された[!UICONTROL Actual Hours]または[!UICONTROL Actual Costs and Expenses]は除外されます。</p> <p>プロジェクトマネージャーは、[!UICONTROL Project Details]の[!UICONTROL Finance]エリアを使用して、この設定をプロジェクトレベルで変更できます。詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">プロジェクトの[!UICONTROL Finance]エリアでの情報の管理</a>を参照してください。</p> </li> 
    </ul> <p>EAC の計算方法について詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Estimate At Completion]（EAC）の計算</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### タイムライン {#timelines}

システム全体で新しく作成されたプロジェクトに対して、次の環境設定を指定します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Schedule From]</td> 
   <td> <p>新規プロジェクトが作成時に開始日からスケジュールされるか、完了日からスケジュールされるかを決定します。</p> 
    <ul> 
     <li><strong>[!UICONTROL Start Date]</strong>：新しいタスクの「タスクの制約」がデフォルトで「[!UICONTROL As Soon As Possible]」になり、プロジェクトの[!UICONTROL Planned Start Date]を指定するように求めるプロンプトがプロジェクトマネージャーに表示されます。</li> 
     <li><strong>[!UICONTROL Completion Date]</strong>：新しいタスクの「タスクの制約」がデフォルトで「[!UICONTROL As Late As Possible]」になり、プロジェクトの[!UICONTROL Planned Completion Date]を指定するように求めるプロンプトがプロジェクトマネージャーに表示されます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User Time Off]</td> 
   <td> <p>プロジェクトのタスクの予定日をそのタスクのプライマリ担当者の休暇によって調整するかどうかを指定します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Consider user time off in task durations]</strong>：タスクのプライマリ担当者にスケジュールされている休暇がタスクの期間中に発生する場合、その休暇によってタスクの予定日が調整されます。これはデフォルトの設定です。 </p> <p>例えば、「[!UICONTROL As Soon As Possible]」という制約を持つタスクが 6月1日に開始し 6月3日に完了するようにスケジュールされ、6月2日がプライマリ担当者の休暇に指定されている場合、タスクの予定日は 6月1日から 6月4日までに調整されます。</p> <p><b>重要</b>：</p> <p>この設定を選択しても、タスクの期間は変わりません。タスクの制約に応じて、予定日のみが変更されます。</p> </li> 
     <li><strong>[!UICONTROL Ignore user time off in task durations]</strong>：プロジェクトの各タスクの予定日は、タスクのプライマリ担当者がその期間中に休暇を取る場合でも、元の予定日のまま変わりません。</li> 
    </ul> <p>この設定のオプションを選択する際は、次の点に注意してください。</p> 
    <ul> 
     <li>この設定を変更すると、変更後に作成されたプロジェクトとテンプレートのみが、更新された設定を継承します。 </li> 
     <li> <p>タスクの「タスクの制約」値によって、調整するタスク予定日が決まります。 </p> 
      <ul> 
       <li>予定開始日</li> 
       <li>予定完了日</li> 
       <li>両方の日付</li> 
       <li>どちらも日付でもない </li> 
      </ul> <p>例えば、タスクの制約が「[!UICONTROL Fixed Dates]」の場合、「[!UICONTROL Consider user time off in task duration]」オプションが選択されていても、プライマリ担当者が休暇を取っている場合に日付は調整されません。タスクの制約については、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">タスクの制約の概要</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL プロジェクトタイムラインは自動的に再計算されます ]</p> </td> 
   <td> <p>プロジェクトのタイムラインを再計算するタイミングを指定します。プロジェクトタイムラインの再計算については、<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">プロジェクトタイムラインの再計算</a>を参照してください。</p> <p>次のオプションが、デフォルトで有効になっています。以下の設定を 1 つ以上選択できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Every night]</strong>：毎晩プロジェクトのタイムラインを再計算する場合に選択します。タイムラインに影響を与える可能性のある変更をプロジェクトに対して行っても、それはすぐには表示されません。[!DNL Workfront​​​] では、以下の条件がすべて満たされるプロジェクトの場合にのみ、夜間にタイムラインを再計算します。</p> <p> 
       <ul> 
        <li>ステータスが「[!UICONTROL Current]」である</li> 
        <li>過去 3 か月間に更新があった</li> 
        <li>「更新の種類」が以下のいずれかである</li>
        <ul>
        <li>自動/変更時</li>
        <li>変更時のみ</li>
        <li>自動のみ</li> 
      </ul>       
    <b>ヒント：</b>
    <p>「更新の種類」が「手動のみ」のプロジェクトは、この設定の影響を受けません。</p>
    <li> <p><strong>プロジェクトのスコープが変更されたとき</strong>：プロジェクト範囲の変更に伴いプロジェクトのタイムラインを直ちに再計算する場合に選択します。プロジェクト範囲の変更の構成要素については、<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">プロジェクトタイムラインの再計算</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL When multiple users are assigned to a task use the schedule of the]</p> </td> 
   <td> <p>プロジェクトにスケジュールが割り当てられていない場合や、タスクに割り当てられたユーザーにスケジュールが割り当てられていない場合、[!DNL Workfront] では、システムのデフォルトのスケジュールを使用して、タスクのタイムラインを計算します。</p> <p>プロジェクト内の同じタスクに複数のユーザーを割り当て、プロジェクトにスケジュールが割り当てられ、タスクに割り当てられたユーザーにスケジュールも割り当てられている場合、[!UICONTROL Workfront] では次のスケジュールが使用されます。</p> 
    <ul> 
     <li><strong>[!UICONTROL Primary Assignment]</strong>：[!DNL Workfront] では、タスクに対するプライマリ割り当てのスケジュールを使用して、タイムラインを計算します。</li> 
     <li><strong>[!UICONTROL Project]</strong>：[!DNL Workfront] では、プロジェクトのスケジュールを使用して、各タスクのタイムラインを計算します。</li> 
    </ul> <p>スケジュールについて詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">スケジュールの作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Timeline Calculations] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Typical hours per work day]</strong>：プロジェクトを担当するユーザーの通常の就業日の時間数を設定します。デフォルトは 8 時間です。</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL 週別の典型的な稼動日数 ]</strong>：プロジェクトで作業するユーザーの標準作業週を設定します。 デフォルトは 5 日です。</li> 
    </ul> <p>これらの 2 つのオプションは、日数を時間数に、または週数を日数に変換します。</p> <p>例えば、予定時間数が 8 時間のタスクがあり、期間が予定時間数に基づいて計算される場合、[!DNL Workfront] では、時間数を日数に変換して、期間を日数で表示します。</p> <p>[!DNL Workfront] では、「[!UICONTROL Typical work days per week]」フィールドからシステムのフルタイム当量（FTE）値を計算します。これは、[!DNL Workfront] でユーザーへの割り当てを計算する際に使用するものです。</p> <p>これらの値は、プロジェクトのタイムラインを計画したり、リソースの予算を計上したり、プロジェクトに対する時間を記録したりする際に使用されます。 </p> <p>これらの値は、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">タイムシートと時間の環境設定の[!UICONTROL Configure]</a>で説明しているとおり、システム内のユーザーのタイムシートを設定する際には使用されません。</p> <p><b>メモ</b>：</p> <p>[!DNL Workfront] 管理者は、 [!UICONTROL タイムライン計算 ] 環境設定のロックを解除できません。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Custom Quarters]</p> </td> 
   <td> <p>プロジェクトを担当するユーザー向けに、カスタム四半期を設定します。カスタム四半期は通常、暦年の従来の四半期分類と一致しない四半期です。複数のカスタム四半期を追加できます。詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">プロジェクトのカスタム四半期の有効化</a>を参照してください。</p>  <p><b>メモ</b>： </p><p>[!DNL Workfront] 管理者は [!UICONTROL Custom Quarters] 環境設定のロックを解除できません。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ビジネスケース] {#business-cases}

新しく作成されたプロジェクトのビジネスケースをシステム全体で作成して、プロジェクトリクエストを送信できます。**[!UICONTROL ビジネスケース]**&#x200B;フォーム上でどのエリアを表示するかを指定する環境設定を定義できます。[!UICONTROL ポートフォリオオプティマイザー]などの他のツールで適切に更新されるように、これらのオプションを有効にすることをお勧めします。各フィールドに何が表示されるかについて詳しくは、 [ビジネスケースの定義：記事インデックス](../../../manage-work/projects/define-a-business-case/define-business-case.md).

[!DNL Workfront] 管理者が[!UICONTROL ビジネスケース]のセクションを有効にしてから、プロジェクト所有者がプロジェクトレベルでビジネスケースを作成できます。ビジネスケースの作成については、[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

### [!UICONTROL 終了後の操作] {#life-after-death}

システム全体で新しく作成されたプロジェクトに対して、次の環境設定を指定します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a project has been marked as Complete, people can still] </p> </td> 
   <td> <p>プロジェクトステータスが「[!UICONTROL Complete]」とマークされた後にタスクやイシューを削除できるかどうかに関して、組織（または、グループのプロジェクト環境設定を指定している場合はグループ）のルールを決定します。</p> 
    <ul> 
     <li><strong>[!UICONTROL Delete Tasks]</strong>：プロジェクトが「[!UICONTROL Complete]」とマークされた後で、ユーザーがプロジェクトからタスクを削除できます。<br></li> 
     <li><strong>[!UICONTROL Delete Issues]</strong>：プロジェクトが「[!UICONTROL Complete]」とマークされた後で、ユーザーがプロジェクトからイシューを削除できます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL After a Project is marked Complete, Dead, or it is Pending Approval, people can still]</p> </td> 
   <td> <p>プロジェクトのステータスが<strong>[!UICONTROL Complete]</strong>、<strong>[!UICONTROL Dead]</strong>または<strong>[!UICONTROL Pending Approval]</strong>とマークされた後にプロジェクト内のタスク、イシュー、ドキュメントおよびその他のオブジェクトがどうなるかに関して、組織（または、グループのプロジェクト環境設定を指定している場合はグループ）のルールを決定します。</p> 
    <ul> 
     <li><strong>[!UICONTROL Add and edit tasks]</strong>：ユーザーが以下を行えます。
      <ul>
       <li>プロジェクトが「[!UICONTROL Complete]」、「[!UICONTROL Dead]」または「[!UICONTROL Pending Approval]」とマークされた後で、プロジェクト内のタスクを編集する。これには、時間数の追加やタスクの費用エントリの変更などが含まれます。</li>
       <li>プロジェクトにタスクを追加する。</li>
      </ul></li> 
     <li><strong>[!UICONTROL Add and edit issues]</strong>：ユーザーが以下を行えます。
      <ul>
       <li>プロジェクトが「[!UICONTROL Complete]」、「[!UICONTROL Dead]」または「[!UICONTROL Pending Approval]」とマークされた後で、プロジェクト内のイシューを編集する。</li>
       <li>プロジェクトが「[!UICONTROL Complete]」または「[!UICONTROL Dead]」とマークされた後で、プロジェクトにイシューを追加する（ステータスが「[!UICONTROL Pending Approval]」のプロジェクトには、イシューを追加できません）。</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL Add documents to the project and to its tasks and issues]</strong>：プロジェクトが「[!UICONTROL Complete]」または「[!UICONTROL Dead]」とマークされた後で、ユーザーがプロジェクトにドキュメントを追加（またはプロジェクト内のタスクやイシューにドキュメントを追加）できます。</p> <p>このオプションは、承認保留中のプロジェクトには適用されません。</p> </li> 
     <li> <p><strong>[!UICONTROL Attach templates]</strong>：プロジェクトが「[!UICONTROL Complete]」または「[!UICONTROL Dead]」とマークされた後で、ユーザーがプロジェクトにテンプレートを添付できます。</p> <p>このオプションは、承認保留中のプロジェクトには適用されません。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
