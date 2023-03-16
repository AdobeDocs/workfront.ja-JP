---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: システム全体のプロジェクト環境設定の指定
description: As a [!DNL Adobe Workfront] 管理者は、システム全体で作成されるすべてのプロジェクトに対して、デフォルトの環境設定を構成できます。 これらの環境設定は、プロジェクト、タスクおよび問題の動作に影響を与えます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1a1affed-1b06-442c-98b2-9f360eee767b
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '2509'
ht-degree: 1%

---

# システム全体のプロジェクト環境設定の指定

As a [!DNL Adobe Workfront] 管理者は、システム全体で作成されるすべてのプロジェクトに対して、デフォルトの環境設定を構成できます。 これらの環境設定は、プロジェクト、タスクおよび問題の動作に影響を与えます。

>[!NOTE]
>
>デフォルトでは、これらの環境設定はロックされ、グループ管理者は、システム全体のすべてのグループのロックを解除しない限り、グループレベルで変更できません。 詳しくは、 [システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除します](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

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

## 組織全体のプロジェクト環境設定を設定

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **[!UICONTROL プロジェクト環境設定]** > **[!UICONTROL プロジェクト]**.

1. 表示されたページで、以下の 4 つのセクションのいずれかに進み、の環境設定を指定します。 [!UICONTROL プロジェクトステータス], [!UICONTROL タイムライン], [!UICONTROL ビジネス事例]、および [!UICONTROL 死後の生活].
1. 組織全体のすべてのグループで同じプロジェクト環境設定を使用する場合は、各環境設定がロックされていることを確認します ![](assets/lock-toggle-button.png) （これはデフォルト）。

   >[!IMPORTANT]
   >
   >プロジェクトプリファレンスがロックされると、そのプリファレンスに対して行った変更は、システム内のすべてのグループに継承されます。 すべてのニーズがプロジェクトの環境設定の方法で確実に考慮されるように、組織全体でユーザーやグループとコミュニケーションを取ることが重要です。

   すべてのグループが独自に設定および管理できるように環境設定をロック解除する方法については、 [システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除します](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

1. 「**[!UICONTROL 保存]**」をクリックします。

* [[!UICONTROL プロジェクト状態]](#project-status)
* [[!UICONTROL タイムライン]](#timelines)
* [[!UICONTROL ビジネスケース]](#business-cases)
* [[!UICONTROL 終了後の操作]](#life-after-death)

### プロジェクト状態 {#project-status}

システム全体で新しく作成されたプロジェクトに対して、次の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL テンプレートを使用せずにユーザーがプロジェクトを作成できるようにする ]</td> 
   <td>  <p>この環境設定では、次の領域からプロジェクトを作成する際に、テンプレートを使用せずにプロジェクトを作成できます。 </p>
      <ul>
        <li>
        <p>プロジェクトのリストでの [!UICONTROL 新規プロジェクト ] オプションの使用</p>
        </li>
          <li>
          <p>イシューのページからイシューをプロジェクトに変換する</p>
          </li>
         </ul>
        <p>この環境設定はデフォルトで有効になっています。 </p> 
        <p><b>メモ</b></p>
        <p> グループ管理者は、グループのこの環境設定を変更できます。 ユーザーが異なる環境設定を持つ複数のグループに属する場合、ホームグループでこの環境設定が有効になっていると、ユーザーはテンプレートを持たないプロジェクトを作成できます。</p> 
        </td> 
  </tr>
  <tr> 
   <td role="rowheader">[!UICONTROL 新規プロジェクトのステータスを [] に設定</td> 
   <td> <p>新規プロジェクトのステータスを決定します。</p>  <p><b>メモ</b>  
     <ul> 
      <li>もしあなたが [!DNL Workfront] 管理者は、ここで選択したステータスを非表示にします。デフォルトのステータスは、ステータス一覧の最初のステータスに変わります。</li> 
     </ul> 
     <ul> 
      <li> <p>ロックされたシステムまたはグループのステータスがデフォルトのステータスとして設定され、後で誰かがそのステータスをロック解除した場合、システムは同じステータスタイプのロック済みステータスと置き換えようとします。</p> <p>見つからない場合は、必須のステータスを探します。</p> 
       <ul> 
        <li>ロック解除済みのデフォルトステータスと同じ必須ステータスがある場合、ロック解除されていても、必須ステータスがデフォルトステータスになります。</li> 
        <li>必須のステータスがロック解除済みのデフォルトのステータスに等しくない場合、ステータスリストの最初の必須ステータスがデフォルトのステータスになります。</li> 
       </ul> <p>必須ステータスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref" data-mc-variable-override="">システムプロジェクトステータスのリストへのアクセス</a>, <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md" class="MCXref xref" data-mc-variable-override="">システムタスクステータスのリストへのアクセス</a>、および <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref" data-mc-variable-override="">システムの問題ステータスのリストへのアクセス</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 完了率の計算基準 ]</td> 
   <td> <p>プロジェクトまたは親タスクの完了率は、タスクの全体的な進捗状況に基づきます。 この情報は、プロジェクトのタスクの期間または予定時間に基づいて計算できます。</p> <p>[!UICONTROL 期間 ] を選択した場合、プロジェクト内の各タスクの「期間」でプロジェクトの全体の完了率が決定され、各サブタスクの「期間」で親タスクの完了率全体が決定されます。</p> <p>[!UICONTROL 期間 ] を選択した場合は、[!UICONTROL タイムライン ] セクションで [!UICONTROL 1 稼働日あたりの典型的な時間 ] と [!UICONTROL 1 週間あたりの典型的な稼働日数 ] を必ず指定してください。 [!DNL Workfront] この情報は、タスクの完了率を期間に基づいて計算する際に使用します。 </p> <p>[!UICONTROL 予定時間 ] を選択する場合は、各プロジェクトのすべてのタスクに [!UICONTROL 予定時間 ] の金額が定義され、金額がゼロでないことを確認します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 進行状況のステータスに基づいて、プロジェクトの条件を自動的に設定する ]</td> 
   <td> <p>この環境設定を使用すると、ユーザーは、プロジェクトの [!UICONTROL 条件 ] を手動で設定 ([!UICONTROL On Target]、[!UICONTROL At Risk]、[!UICONTROL In Trable]) したり、 [!DNL Workfront] タイムライン上のプロジェクトの進行状況に基づいて、[!UICONTROL 条件 ]（進行状況ステータス）を自動的に設定します。 プロジェクトの条件の詳細については、 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref" data-mc-variable-override="">プロジェクト条件と条件タイプの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ベースラインを自動的に作成 ]</p> </td> 
   <td> <p>この環境設定では、プロジェクトのステータスが [!UICONTROL 現在 ] に変わると、タスクとプロジェクトの詳細のベースライン（スナップショット）が自動的に作成されます。 ベースラインの作成について詳しくは、 <a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref" data-mc-variable-override="">プロジェクトの基準を作成</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL パフォーマンスインデックスメソッド ] </p> </td> 
   <td> <p>プロジェクトの Performance Index Method(PIM) は、メソッドを制御します [!DNL Workfront] は、[!UICONTROL Cost Performance Index] (CPI) や [!UICONTROL Estimate At Completion] (EAC) などの達成額指標の計算に使用します。 詳しくは、 <a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL コスト効果指数 ] (CPI) の計算</a> および <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL 完了時の推定を計算 ](EAC)</a></p> 
    <ul> 
     <li><strong>[!UICONTROL 時間ベース ]</strong>: [!DNL Workfront] は、[!UICONTROL 予定時間 ] を使用して EAC や CPI などのパフォーマンス指標を計算します。 PIM が時間に基づいて計算されると、EAC は時間数として表示されます。 [!UICONTROL Planned Hours] に 0 以外の値が設定されていることを確認してください。</li> 
     <li> <p><strong>[!UICONTROL コストベース ]</strong>: [!DNL Workfront] は、[!UICONTROL 計画労務費 ] を使用して EAC や CPI などのパフォーマンス指標を計算します。 ジョブの役割またはユーザーが時間あたりのコスト率に関連付けられていることを確認します。 PIM がコストに基づいて計算されると、EAC は通貨値として表示されます。</p> <p>プロジェクトマネージャーは、[!UICONTROL プロジェクトの詳細 ] の [!UICONTROL Finance] 領域を使用して、プロジェクトレベルでこの設定を変更できます。 詳しくは、 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">プロジェクト [!UICONTROL Finance] 領域で情報を管理</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 完了時の推定 ]</p> </td> 
   <td> <p>どのデータを特定するか [!DNL Workfront] は、を使用して [!UICONTROL 完了時の予測 ](EAC) を計算します。これは、プロジェクトの推定総コストを表します。</p> 
    <ul> 
     <li><strong>[!UICONTROL プロジェクトレベルで計算 ]</strong>：親タスクおよびプロジェクトの EAC は、EAC 式に [!UICONTROL 実績時間 ] または [!UICONTROL 実績労務費 ] を入力することで決定されます。 この計算には、[!UICONTROL 実際の時間 ] または [!UICONTROL コストと費用 ] が親タスクまたはプロジェクトに直接追加されます。</li> 
     <li> <p><strong>[!UICONTROL タスク/サブタスクからのロールアップ ]</strong>:親タスクとプロジェクトの EAC は、各子タスクの EAC を合計することで決定されます。 この計算では、親タスクまたはプロジェクトに直接追加された [!UICONTROL 実績時間 ] または [!UICONTROL 実績コストと費用 ] は除外されます。</p> <p>プロジェクトマネージャーは、[!UICONTROL プロジェクトの詳細 ] の [!UICONTROL Finance] 領域を使用して、プロジェクトレベルでこの設定を変更できます。詳しくは、 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref" data-mc-variable-override="">プロジェクト [!UICONTROL Finance] 領域で情報を管理</a>.</p> </li> 
    </ul> <p>EAC の計算方法について詳しくは、 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL 完了時の推定 ] (EAC) を計算</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### タイムライン {#timelines}

システム全体で新しく作成されたプロジェクトに対して、次の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL スケジュールの元 ]</td> 
   <td> <p>新規プロジェクトが作成時に「開始日」からスケジュールされるか、「完了日」からスケジュールされるかを決定します。</p> 
    <ul> 
     <li><strong>[!UICONTROL 開始日 ]</strong>:新しいタスクのデフォルトは [!UICONTROL 可能な限り早く ] タスク制約とプロジェクトマネージャーに対して、プロジェクトの [!UICONTROL 予定開始日 ] の指定を求めるプロンプトが表示されます。</li> 
     <li><strong>[!UICONTROL 完了日 ]</strong>:新しいタスクのデフォルトは [!UICONTROL 可能な限り遅延 ] タスク制約です。プロジェクトマネージャーは、プロジェクトの [!UICONTROL 予定完了日 ] の指定を求められます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ユーザータイムオフ ]</td> 
   <td> <p>タスクのプライマリ担当者が、そのタスクの予定日をプロジェクト上で調整するかどうかを指定します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL タスク期間でのユーザーのタイムオフを考慮する ]</strong>:タスクのプライマリに予定されているオフタイム担当者は、タスクの期間中にオフタイムが発生した場合に、タスクの予定日を調整します。 これはデフォルト設定です。 </p> <p>例えば、[!UICONTROL 可能な限り早く ] という制約を持つタスクが 6 月 1 日に開始し、6 月 3 日に完了するようにスケジュールされていて、プライマリ担当者が 6 月 2 日にタイムオフとしてマークされている場合、タスクの計画日は 6 月 1 日から 6 月 4 日に調整されます。</p> <p><b>重要</b>:この設定を選択した場合、タスクの期間は変更されません。 タスク制約に応じて、計画日のみが変更されます。</p> </li> 
     <li><strong>[!UICONTROL タスク期間のユーザータイムオフを無視する ]</strong>:プライマリの担当者が期間中に休暇を取った場合でも、プロジェクトの各タスクの計画日は、当初の計画通りに保たれます。</li> 
    </ul> <p>この設定のオプションを選択する際は、次の点に注意してください。</p> 
    <ul> 
     <li>この設定を変更すると、変更後に作成されたプロジェクトとテンプレートのみが更新された設定を継承します。 </li> 
     <li> <p>タスクの [ タスク制約 ] の値によって、調整する予定タスクの日付が決まります。 </p> 
      <ul> 
       <li>予定開始付</li> 
       <li>予定完了日</li> 
       <li>両方の日付</li> 
       <li>どちらの日付も。 </li> 
      </ul> <p>例えば、プライマリの制約が [!UICONTROL 固定日付 ] の場合、[!UICONTROL タスク期間でのユーザーのタイムオフを考慮 ] オプションが選択されていても、タスク担当者がタイムオフになる時点で日付が調整されません。 タスクの制約について詳しくは、 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref" data-mc-variable-override="">タスク制約の概要</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL プロジェクトタイムラインは自動的に再計算されます ]</p> </td> 
   <td> <p>プロジェクトのタイムラインを再計算するタイミングを指定します。 プロジェクトタイムラインの再計算について詳しくは、 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">プロジェクトタイムラインを再計算</a>.</p> <p>次のオプションは、デフォルトで有効になっています。 次の設定を 1 つ以上選択できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 毎晩 ]</strong>:毎晩プロジェクトのタイムラインを再計算する場合に選択します。 タイムラインに影響を与える可能性のあるプロジェクトに対する変更は、すぐには表示されません。 [!DNL Workfront​​​] では、次の両方の条件が満たされたプロジェクトのタイムラインが夜間に再計算されます。</p> <p> 
       <ul> 
        <li>ステータスが [!UICONTROL Current] である</li> 
        <li>過去 3 か月間に更新があります</li> 
        <li>次のいずれかの更新タイプを持っている。</li>
        <ul>
        <li>自動/変更時</li>
        <li>変更時のみ</li>
        <li>自動のみ</li> 
      </ul>       
    <b>ヒント</b>
    <p>[ 更新の種類 ] が [ 手動のみ ] のプロジェクトは、この設定の影響を受けません。</p>
    <li> <p><strong>プロジェクトの範囲が変更されたとき</strong>:プロジェクト範囲の変更が発生したときにプロジェクトタイムラインをすぐに再計算する場合は、これを選択します。 プロジェクト範囲の変更を構成する情報については、 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref" data-mc-variable-override="">プロジェクトタイムラインを再計算</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 複数のユーザーがタスクに割り当てられている場合は、[]</p> </td> 
   <td> <p>プロジェクトにスケジュールが割り当てられていない場合、またはタスクに割り当てられたユーザーにスケジュールが割り当てられていない場合は、 [!DNL Workfront] は、システムの既定のスケジュールを使用して、タスクのタイムラインを計算します。</p> <p>プロジェクト内の同じタスクに複数のユーザーを割り当てる際に、スケジュールが割り当てられ、タスクに割り当てられたユーザーにスケジュールも割り当てられる場合：[!UICONTROL Workfront] では、次のスケジュールが使用されます。</p> 
    <ul> 
     <li><strong>[!UICONTROLプライマリ割り当て ]</strong>: [!DNL Workfront] タスク上のプライマリ割り当てのスケジュールを使用して、タイムラインを計算します。</li> 
     <li><strong>[!UICONTROL プロジェクト ]</strong>: [!DNL Workfront] プロジェクトのスケジュールを使用して、各タスクのタイムラインを計算します。</li> 
    </ul> <p>スケジュールについて詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" data-mc-variable-override="">スケジュールの作成</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL タイムラインの計算 ] </p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL 1 営業日あたりの通常の時間 ]</strong>:プロジェクトで作業するユーザーの通常の稼働日の時間数を設定します。 デフォルトは 8 時間です。</li> 
    </ul> 
    <ul> 
     <li><strong>[!UICONTROL 週別の典型的な稼動日数 ]</strong>:プロジェクトで作業するユーザーに対して、標準作業週を設定します。 デフォルトは 5 日です。</li> 
    </ul> <p>これらの 2 つのオプションは、日を時間に、または週を日に変換します。</p> <p>例えば、予定時間が 8 時間のタスクがあり、期間が予定時間に基づいて計算される場合、 [!DNL Workfront] は、時間を日数に変換し、期間を日数で表示します。</p> <p>「典型的な [!UICONTROL 稼働日/週 ] 」フィールドで、次の操作をおこないます。 [!DNL Workfront] システムのフルタイム相当 (FTE) 値を計算します。 これがその通り [!DNL Workfront] は、ユーザーの割り当てを計算する際に使用します。</p> <p>これらの値は、プロジェクトのタイムラインを計画したり、リソースの予算を作成したり、プロジェクトに対する時間を記録する際に使用されます。 </p> <p>これらは、システム内のユーザーのタイムシートを設定する際には使用されません。詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL 構成 ] タイムシートと時間の基本設定</a>.</p> <p><b>注意</b>: [!DNL Workfront] 管理者は、 [!UICONTROL タイムライン計算 ] 環境設定のロックを解除できません。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL カスタム四半期 ]</p> </td> 
   <td> <p>プロジェクトで作業するユーザー向けに年別のカスタム四半期を設定します。 カスタム四半期は、通常、暦年の四半期の従来の分類と一致しない四半期です。 複数のカスタム四半期を追加できます。 詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref" data-mc-variable-override="">プロジェクトのカスタム四半期を有効にする</a>.</p>  <p><b>注意</b>: [!DNL Workfront] 管理者は [!UICONTROL Custom Quarters] 環境設定のロックを解除できません。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ビジネスケース] {#business-cases}

システム全体で新しく作成したプロジェクトのビジネスケースを作成して、プロジェクトリクエストを送信できます。 環境設定を定義して、 **[!UICONTROL ビジネス事例]** フォーム。 他のツール ( [!UICONTROL Portfolio最適化]、を適切に更新する必要があります。 各フィールドに何が表示されるかについて詳しくは、 [ビジネスケースの定義](../../../manage-work/projects/define-a-business-case/define-business-case.md).

次の期間の後 [!DNL Workfront] 管理者が [!UICONTROL ビジネス事例]を使用すると、プロジェクト所有者は、プロジェクトレベルでビジネスケースを作成できます。 ビジネス事例の作成の詳細は、 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).

### [!UICONTROL 終了後の操作] {#life-after-death}

システム全体で新しく作成されたプロジェクトに対して、次の環境設定を行います。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL プロジェクトが完了とマークされた後も、ユーザーは引き続き実行できます ] </p> </td> 
   <td> <p>タスクまたは問題をプロジェクトのステータスが [!UICONTROL 完了 ] とマークされた後に削除できるかどうかに関する、組織（またはグループのプロジェクト環境設定を設定している場合はグループ）のルールを決定します。</p> 
    <ul> 
     <li><strong>[!UICONTROL タスクを削除 ]</strong>:プロジェクトが [!UICONTROL 完了 ] とマークされた後で、ユーザーがプロジェクトからタスクを削除できるようにします。<br></li> 
     <li><strong>[!UICONTROL 削除の問題 ]</strong>:プロジェクトが [!UICONTROL 完了 ] とマークされた後で、ユーザーがプロジェクトから問題を削除できます。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL プロジェクトが完了、無効、または承認待ちとマークされた後も、担当者は引き続き可能です ]</p> </td> 
   <td> <p>プロジェクトのステータスがマークされた後にプロジェクト内のタスク、問題、ドキュメント、その他のオブジェクトに何が起こるかに関する、組織（またはグループのプロジェクトプリファレンスを設定する場合は、グループ）の規則を決定します <strong>[!UICONTROL 完了 ]</strong>, <strong>[!UICONTROL 無効 ]</strong>または <strong>[!UICONTROL 承認待ち ]</strong>.</p> 
    <ul> 
     <li><strong>[!UICONTROL タスクの追加と編集 ]</strong> ユーザーが以下を実行できるようにします。
      <ul>
       <li>プロジェクトが [!UICONTROL 完了 ]、[!UICONTROL 無効 ] とマークされた後、または [!UICONTROL 承認待ち ] になった後、プロジェクト内のタスクを編集します。 これには、時間の追加やタスクの費用エントリの変更が含まれます。</li>
       <li>プロジェクトにタスクを追加します。</li>
      </ul></li> 
     <li><strong>[!UICONTROL 問題の追加と編集 ]</strong>:ユーザーが以下を実行できるようにします。
      <ul>
       <li>プロジェクトが [!UICONTROL 完了 ]、[!UICONTROL 無効 ]、[!UICONTROL 承認待ち ] のいずれかに設定された後、プロジェクト内の問題を編集します。</li>
       <li>プロジェクトが [!UICONTROL 完了 ] または [!UICONTROL 無効 ] とマークされた後で、プロジェクトに問題を追加します。 （[!UICONTROL 承認待ち ] のプロジェクトにイシューを追加することはできません）。</li>
      </ul></li> 
     <li> <p><strong>[!UICONTROL プロジェクトおよびプロジェクトのタスクとタスクにドキュメントを追加 ]</strong>:プロジェクトが [!UICONTROL 完了 ] または [!UICONTROL 無効 ] とマークされた後で、ユーザーがプロジェクトにドキュメントを追加（またはプロジェクト内のタスクや問題にドキュメントを追加）できるようにします。</p> <p>このオプションは、承認待ちのプロジェクトには適用されません。</p> </li> 
     <li> <p><strong>[!UICONTROL テンプレートの添付 ]</strong>:プロジェクトが [!UICONTROL 完了 ] または [!UICONTROL 無効 ] とマークされた後で、ユーザーがプロジェクトにテンプレートを添付できます。</p> <p>このオプションは、承認待ちのプロジェクトには適用されません。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
