---
content-type: reference
navigation-topic: workfront-navigation
title: 用語集 [!DNL Adobe Workfront] 用語
description: The [!DNL Adobe Workfront] 用語集には、Adobe Workfrontでよく使用される用語が記載されています。
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: bc7039bc4b8b257fc55e71e73f72327fdb417837
workflow-type: tm+mt
source-wordcount: '19729'
ht-degree: 0%

---

# 用語集 [!DNL Adobe Workfront] 用語

>[!IMPORTANT]
>
>この記事は、 [!DNL Adobe Workfront] アプリケーション、 [!DNL Workfront] ドキュメントを参照するか、作業の計画と管理に関する一般的な話をする場合に使用します。 現在この情報を更新中です。そのため、このテーブルは完了していない可能性があります。 この情報を網羅的に検討する際は、この免責事項を削除します。

次の表は、Adobe Workfrontでよく使用される用語の一覧です。

## A ～ C

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>オブジェクト名</strong></th> 
   <th><strong>説明</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL アクセスレベル ]</td> 
   <td>ユーザーがWorkfront内の様々なオブジェクトやツールを操作する方法を決定するユーザープロファイル。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アクティブタスク ]</td> 
   <td>現在のプロジェクト内の不完全なタスクで、先行タスクによる作業を妨げず、将来の予定開始日を持つタスク制約を持たないもの。 つまり、今日の作業も可能です。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL アクティビティ ]</td> 
   <td>In [!DNL Workfront Goals]の場合、アクティビティは目標の進捗状況インジケーターです。 手動で更新するプログレスバー、または目標に関連付けられたプロジェクトを指定できます。 アクティビティをレポートに表示することはできません。また、 [!DNL Workfront] API. アクティビティについて詳しくは、 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront目標の結果とアクティビティの概要</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 実際のコスト ]</td> 
   <td> <p>タスクおよびタスクの場合、タスクまたはタスクに割り当てられたリソースの 1 時間あたりのコスト率に関して、実際にログインした時間に関連するコストです。 プロジェクトの場合、これは、プロジェクトのタスクと問題に関するすべての [!UICONTROL 実績コスト ] の合計です。 詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 実費コスト ]</td> 
   <td> <p>プロジェクトまたはタスクでログに記録されたすべての費用の [!UICONTROL 実際の金額 ] の合計です。</p> <b>例 </b>
   <p>Task 1 の費用を作成し、[!UICONTROL Actual Amount] フィールドに$600.00 と入力した場合、このタスクの [!UICONTROL Actual Expense Cost] は$600.00 になります。 </p> 
   <p>プロジェクトの場合、 [!DNL Workfront] では、次の式を使用して [!UICONTROL 実費 ] を計算します。</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 実際の時間 ]</td> 
   <td> <p>プロジェクト、タスク、または問題報告では、[!UICONTROL 実際の時間 ] は、プロジェクト、タスク、または問題に関して記録されたすべての時間の合計です。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span> タスク 1 の [!UICONTROL 更新 ] タブから「ログ時間」をクリックし、25 時間と入力した場合、タスク 1 の実際の時間は 25 時間になります。 </p> <p>[!DNL Workfront] 次の式を使用して、親タスクまたはプロジェクトの [!UICONTROL 実際の時間 ] を計算します。</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 実際の労務費 ]</td> 
   <td> <p>タスクまたはプロジェクトに投資された労務に関連する [!UICONTROL 実績コスト ]。 </p> <p>タスクの場合、 [!DNL Workfront] 次の式を使用して [!UICONTROL 実際の労務費 ] を計算します。</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>タスクのコストタイプが [!UICONTROL ユーザー（1 時間ごと）] の場合、 [!DNL Workfront] はユーザー率を使用します。 タスクのコストタイプが [!UICONTROL 1 時間ごとの役割 ] の場合、 [!DNL Workfront] は、役職率を使用して [!UICONTROL 実際の労務費 ] を計算します。 </p> <p>プロジェクトの場合、 [!DNL Workfront] では、次の式を使用して [!UICONTROL 実際の労務費 ] を計算します。</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span>例えば、ユーザーが [!UICONTROL User Hourly] [!UICONTROL Cost Type] でタスクに対して 5 時間ログに記録し、その時間単価が$100 の場合、[!UICONTROL Actual Labor Cost] は$500 になります。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 実際の売上高 ] </td> 
   <td> <p>プロジェクトまたはタスクの [!UICONTROL 実際の売上高 ] は、プロジェクトまたはタスクの [!UICONTROL 実際の時間 ] に関連する金額です。 </p> <p>での売上高の追跡について詳しくは、 [!DNL Workfront]を参照してください。 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と売上高の概要</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 実際の開始 ]</td> 
   <td>ユーザーが割り当てられた作業で進行中のオブジェクトを変更したときのタイムスタンプ。</td> 
  </tr> 
  <!--<tr> 
 <td>A type of work process that is unplanned.</td> 
 -->
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Additional Schedules</td> 
    <td>An additional preset to be used for a new user group.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Agile] 手法</td> 
   <td>複数の機能を持つチームとのニーズとソリューションの共同進化に基づく手法の一種。 固定されたタイムラインに基づく柔軟性と変化を促進します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>従来のチームとは異なります。見込みの作業をバックログから取り出し、[!UICONTROL 反復 ] と呼ばれる一定の期間内に作業を行うからです。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL すべてのマイチーム ]</td> 
   <td> <p>この情報が [!UICONTROL フィルター ] で参照される場合、このフィールドには、ログインユーザーが属するチームのいずれかに属するユーザー、またはログインユーザーが属するチームに割り当てられた作業項目が表示されます。 </p> <p>他のユーザーとレポートを共有する際に、より一般的なレポートにするには、このフィールドをフィルターで使用することをお勧めします。 この方法では、1 つのレポートのみを作成できます。このレポートには、ログインしたユーザーに応じて常にカスタマイズされるので、ログインしたユーザーに応じて異なる情報が表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配分日 ]</td> 
   <td> <p>このフィールドは、次のタイプのレポートで確認できます。</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project] （金融データ）</li> 
     <li>[!UICONTROL 予算時間 ]</li> 
    </ul> <p>の<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL プロジェクト（金融データ）] レポート： </p> 
    <ul> 
     <li>理解を試みる際にこのレポートを作成する <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      --> リソースに割り当てられる [!UICONTROL 予定時間 ] の量。</li> 
     <li> <p>[!UICONTROL 配分日 ] は、タスクへの [!UICONTROL ジョブロール ] の配分が開始される週の最初の日（日曜日）です。 リソース（[!UICONTROL ジョブロール ]）には、割り当て先のタスクの [!UICONTROL 期間 ] の間の [!UICONTROL 割り当て日 ] の数と同じ数の日付を設定できます。 タスクが複数ヶ月にわたる場合、タスクの期間内であれば、月の最初の日を [!UICONTROL 割り当て日 ] にすることもできます。</p> <p>例えば、3 週間以上にわたるタスクに [!UICONTROL ジョブロール ] を割り当て、[!UICONTROL 予定時間 ] を 90 時間に設定することができます。 これらの時間はタスクの期間中に均等に配分され、毎日 6 つの [!UICONTROL 予定時間 ] がジョブの役割に割り当てられます。</p> <p><em> [!UICONTROL 日別予定時間 ] = [!UICONTROL 合計予定時間 ]/タスク期間中の [!UICONTROL 稼働日数 ] </em> </p> <p>その結果、3 つの [!UICONTROL 配分日 ] がタスクの [!UICONTROL 期間 ] の間、毎週日曜日に 1 つずつ、それぞれに一定数の [!UICONTROL 予定時間 ] が関連付けられています。<br>タスクが 1 ヶ月の最終週の真ん中に開始し、新しい月の初めから 2 週間が終了した場合、タスクには 4 つの [!UICONTROL 配分日 ] が割り当てられます。1 つはタスクの期間中の毎週日曜日に対して 1 つで、もう 1 つは新しい月の初日です。</p> <p>この情報を最大限に活用するために、 <!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> プロジェクト（金融データ）レポートを作成し、[!UICONTROL Allocation Date] のマトリックスグループを追加した後、最も正確なデータを得るために、週別、月別、四半期別または年別の結果をグループ化します。<br>マトリックスのグループ化の作成について詳しくは、「 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">マトリックスレポートの作成</a>.</p> </li> 
    </ul> <p>[!UICONTROL Project (Financial Data)] レポートに財務情報が入力されるのは、関連付けられているデータが 5 歳未満の場合のみです。 例えば、2015 年 1 月にジョブの役割がタスクに割り当てられ、今日が 2021 年 9 月の場合、ジョブの役割の [!UICONTROL Allocation Date] などの財務フィールドは [!UICONTROL Project (Financial Data)] レポートに入力されません。 </p> 
    <div> 
     <p>[!UICONTROL Budgeted Hour] レポートの場合：</p> 
     <ul> 
      <li>リソースに割り当てられる [!UICONTROL 予算時間 ] の量を把握する場合や、リソースプランナーのプロジェクトに割り当てられる場合は、このレポートを作成します。</li> 
      <li> <p>[!UICONTROL 割り当て日 ] は、[!UICONTROL Resource Planner] で時間を予算化した週の最初の日（日曜日）です。 </p> <p>ヒント：   <p>ある週が 2 か月にわたる場合、レポートに 2 つの行 (1 つは週の最初の日（最初の月の最初の週の日曜日）に対応し、2 つ目の行には 2 か月の最初の日が表示されます。 </p> <p>例えば、ユーザーに対して 6 月 30 日（日曜日）～7 月 6 日（土曜日）の週に 8 時間を予算を割り当てた場合、2 つの行には 6 月 30 日と 7 月 1 日の [!UICONTROL Allocation Date] が表示されます。 </p> </p> <p>でのリソース予算の作成に関する情報 [!DNL Resource Planner]（記事を参照）。 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">予算リソース ( [!DNL Resource Planner] [!UICONTROL Project] ビューと [!UICONTROL Role] ビューの使用</a>.</p> <p>[!UICONTROL Budgeted Hour] レポートの作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">レポート：予算時間</a>. </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL のお知らせ ]</td> 
   <td> <p>システム内のユーザー情報に通信する方法。 この情報は、多くの場合、 [!DNL Workfront] を管理者または管理者からユーザーに追加します。 </p> <p>詳しくは、 <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">お知らせの送信</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アプリ統合 ]</td> 
   <td>最も一般的に、アプリはソフトウェアアプリケーションへのコネクタを表しますが、データを操作する特別な関数を表すこともできます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 承認者の決定 ]</td> 
   <td> <p>[!UICONTROL 配達確認の承認 ] レポートで、このフィールドには、アクティブでなくなった配達確認の承認に関する決定が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 承認者ステージ ]</td> 
   <td>[!UICONTROL 配達確認の承認レポート ] で、このフィールドには、現在のステージの配達確認に関する情報が表示されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 承認 ]</td> 
   <td> <p>タスク、ドキュメント、タイムシートなどの特定の作業項目に対しては、管理者や他のユーザーが作業項目に対してサインオフする必要が生じる場合があります。 このサインオフのプロセスを承認と呼びます。 </p> <p>詳しくは、 <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">承認プロセスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 承認日 ]</td> 
   <td>[!UICONTROL 配達確認の承認 ] レポートのこのフィールドには、配達確認が承認された日付が表示されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 承認者 ]</td> 
   <td>特定の作業項目、またはタイムシートの時間エントリを承認するユーザーに対してサインオフする必要があるユーザーまたはジョブの役割。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 割り当て先 ]</td> 
   <td> <p>[!UICONTROL タスクまたはイシュー ] レポートでは、このフィールドにタスクの所有者、イシューまたは [!UICONTROLプライマリ担当者 ] が表示されます。 また、このフィールドでフィルターやグループ化をおこなうこともできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 割り当て ]</td> 
   <td>イシューまたはタスクに割り当てられたユーザー、ジョブの役割、またはチーム。 プロジェクト、ポートフォリオ、またはプログラムに割り当てを含めることはできません。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 割り当て ]</td> 
   <td> <p>[!UICONTROL タスク ] または [!UICONTROL タスク ] レポートで、このフィールドにタスクまたはタスクに割り当てられているすべてのエンティティ（ユーザー、ジョブの役割、チーム）のリストが表示されます。 [!UICONTROL 割り当てユーザー ] フィールドと [!UICONTROL 割り当て役割 ] フィールドを使用して、このフィールドでフィルタリングできます。 「チーム」フィールドを使用して、タスクまたはイシューに割り当てられたチームでフィルタリングできます。 このフィールドでレポートをグループ化することはできません。</p> <p>[!UICONTROL ごみ箱 ] に配置された作業項目は、[!UICONTROL 割り当て ] オブジェクトを参照する一部のレポートに引き続き表示されます。このレポートで、 [!DNL OR] filter 修飾子が使用されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 割り当ての役割 ]</td> 
   <td>
   <p>[!UICONTROL タスク ] または [!UICONTROL タスク ] レポートで、タスクまたはタスクに割り当てられたジョブの役割に関する情報が表示されます。 このフィールドには、[!UICONTROLプライマリの所有者 ] と、タスクまたはタスクに割り当てられた他のジョブの役割が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 割り当てステータス ]</td> 
   <td> <p>割り当て、タスク、または問題報告では、作業項目に割り当てられたユーザーが [!UICONTROL 作業項目 ] ボタンをクリックしたか、[!UICONTROL 完了 ] ボタンをクリックして作業を承認または完了したかが [!UICONTROL 割り当てステータス ] に表示されます。 次の [!UICONTROL 割り当てステータス ] が存在します。</p> 
    <ul> 
     <li><b>[!UICONTROL リクエスト済み ]</b>：ユーザーはタスクまたはイシューに割り当てられていますが、[!UICONTROL 作業時間 ] ボタンをクリックしてまだ作業を開始していません。</li> 
     <li><b>[!UICONTROL Working]</b>：ユーザーが「[!UICONTROL 操作 ]」ボタンをクリックし、現在項目の操作中です。 </li> 
     <li><b>[!UICONTROL 完了 ]</b>：ユーザーが「完了」ボタンをクリックし、項目の作業を完了した。 </li> 
    </ul> <p>詳しくは、 <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">[!UICONTROL 操作 ] ボタンと [!UICONTROL 完了 ] ボタンの概要</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 割り当てチーム ]</td> 
   <td>
   <p>[!UICONTROL タスク ] または [!UICONTROL タスク ] レポートで、このフィールドにタスクまたはタスクに割り当てられたチームに関する情報が表示されます。 「 」フィールドには、[!UICONTROLプライマリの所有者 ] と、タスクまたはタスクに割り当てられた他のチームが表示されます。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 割り当てユーザー ]</td> 
   <td>
   <p>[!UICONTROL タスク ] または [!UICONTROL タスク ] レポートで、このフィールドにタスクまたはタスクに割り当てられたユーザーに関する情報が表示されます。 このフィールドには、[!UICONTROLプライマリ所有者 ] と、タスクまたはタスクに割り当てられた他のユーザーが表示されます。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 属性 ]</td> 
   <td>属性は、 [!DNL Workfront] オブジェクト。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 監査領域 ]</td> 
   <td> <p>監査は、Workfrontで発生したアクションを記録するシステムメッセージです。 次の監査タイプが記録されます。</p> 
    <ul> 
     <li>[!UICONTROL スコープの変更 ]</li> 
     <li>[!UICONTROL 添付ファイルアクション ]</li> 
     <li>[!UICONTROL 一般編集 ]</li> 
     <li>[!UICONTROL ステータスの変更 ]</li> 
     <li>[!UICONTROL メモ ]</li> 
     <li>[!UICONTROL 結合エントリ ]</li> 
     <li>[!UICONTROL エラーエントリ ]</li> 
     <li>[!UICONTROL ステータスの変更 ]</li> 
     <li>[!UICONTROL 購読の変更 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 監査証跡 ]</td> 
   <td>記録された変更（[!UICONTROL 監査領域 ]）を通じて追跡されるイベントによって自動的に生成されるメモのコレクション。 各メモには、誰が何をしたか、何をしたか、いつ実行したかが記録されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 自動変更と変更時 ]</td> 
   <td> <p>[!UICONTROL Project Update] タイプの 1 つ。 これにより、夜間の再計算処理が実行されたときや、プロジェクト内のプロジェクトまたはタスクに対して更新が行われたときに、プロジェクトの予測および計画タイムラインが再計算されます。 </p> <p>詳しくは、 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプを選択 </a>.</p> </td> 
  </tr>

<tr> 
   <td><p>使用可否</p></td> 
   <td> <p>この用語は、「ユーザーの可用性」または「リソースの可用性」に関連して使用され、リソース（ユーザーまたはジョブの役割）が機能できる時間を示します。 </p> 
   <p>Workfrontは、複数のフィールドを使用し、システム内のリソース管理環境設定の設定に応じて、ユーザーの可用性を計算します。 詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理環境設定の指定</a>. </p>
   <p>リソースの可用性の詳細については、 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">リソース管理の概要</a></p>
   または、「容量」を使用して、リソースの可用性を指す場合もあります。 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL 自動のみ ]</td> 
   <td> <p>[!UICONTROL Project Update] タイプの 1 つ。 これにより、夜間の再計算処理が実行されたときに「予測」と「計画」のタイムラインが再計算されます。</p> <p>詳しくは、 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプを選択</a>.</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>日々の主要なビジネス目標の実行に貢献する「通常のビジネス」の仕事。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL バックログ ]</td> 
   <td>新しい問題に取り組む準備が整うまで、新しい問題が保たれる機敏な環境の領域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ベースライン ]</td> 
   <td>機敏な環境での反復を測定するためのデータのソース。</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL 請求レコード ]</td> 
   <td> <p>請求可能な売上高、時間または費用を記録します。 この情報は、外部の会計システムで請求書を作成する際に使用できます。</p> <p>詳しくは、 <a href="../../../manage-work/projects/project-finances/create-billing-records.md">請求レコードの作成</a>. </p> 
   </td> 
  </tr>

<tr> 
   <td>請求レコードのステータス</td> 
   <td> <p>請求レコードまたは時間レポートでは、請求レコードのステータスは請求レコードが請求済みか、請求なしかを示します。 プロジェクトを削除したり、請求済み請求レコードに関連する時間を編集したりすることはできません。 詳しくは、 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >請求レコードの作成</a>.</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL ブランディング ]</td> 
   <td><p>カスタマイズのプロセス [!DNL Workfront] を使用すると、会社を映し出すインターフェイスを、色とロゴを使用して実現できます。</p><p><strong>注意</strong><br>組織が [!DNL Adobe Experience Cloud]、ブランディングを使用できません。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL パンくずリスト ]</td> 
   <td> <p>ページ上部の領域で、アプリ内のユーザーの位置が階層的に表示されます。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">詳しくは、 <a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">パンくずリストの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予算ステータス ]</td> 
   <td> <p>これは廃止されたフィールドです。 このフィールドに表示される情報は、 [!DNL Workfront] が削除され、フィールドを更新できません。 </p> <p>このフィールドは、プロジェクトが [!UICONTROL 処理能力プランナー ] に追加されたかどうか、およびその予算の計算が完了したかどうかを示します。 [!UICONTROL Capacity Planner] が [!DNL Workfront]. </p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;not added to the capacity planner, its value is <i>Not Included</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">If the project is&nbsp;added to the Capacity Planner but is excluded from the budget calculation,&nbsp;the value is <i>Included but not Calculated</i>.&nbsp;</li>
     --> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> If the project is&nbsp;added to the Capacity Planner and included in the budget calculation, the value is <i>Included and Calculated</i>. </li>
     --> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予算完了日 ]</td> 
   <td> <p>これは廃止されたフィールドです。 このフィールドに表示される情報は、 [!DNL Workfront] が削除されました。 このフィールドは更新できません。 </p>
   <p> このフィールドは、[!UICONTROL プロジェクト ] および [!UICONTROL タスク ] のレポートとリストに引き続き表示されます。</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予算コスト ]</td>

<td> <p>これは、プロジェクトの予算リソースに関連するコストです。 </p>
   <p>フィールドは、 [!DNL Workfront] を次の名前で指定します。</p>
   <ul>
   <li><strong>[!UICONTROL 予算コスト ]</strong>:[!UICONTROL ビジネスケースサマリ ] パネル</li>
   <li><strong>[!UICONTROL コスト ]</strong>:[!UICONTROL コスト ] 別の情報表示の際の [!UICONTROL 使用率 ] 領域</li>
   <li><strong>[!UICONTROL プロジェクトの予算コスト ]</strong>：リストおよびレポートの</li>
   </ul>   
    <p>プロジェクトの予算コストは、次の式を使用して計算されます。</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>[!UICONTROL 予算コスト ] の計算と、この概念の様々な名前の理解については、 [!DNL Workfront]を参照してください。 <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">プロジェクトの予算コストの計算</a>. </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 予算時間 ]</td> 
   <td> <p>プロジェクトで完了する必要がある作業のリソースに予算される時間です。 このフィールドは、プロジェクトまたはプロジェクトリソースの [!UICONTROL ビジネスケース ]（または [!UICONTROL リソースプランナー ]）の [!UICONTROL リソース予算 ] 領域で予算設定された時間を参照します。</p> <p>詳しくは、 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">プロジェクトの [!UICONTROL 予算労務費 ] および [!UICONTROL 予算時間 ] の把握</a>. </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> ユーザーの予算設定については、 [!DNL Resource Planner]（記事を参照）。 <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">予算リソース ( [!DNL Resource Planner] [!UICONTROL Project] ビューと [!UICONTROL Role] ビューの使用</a>. </p> 
    <p>[!UICONTROL ビジネスケース ] の [!UICONTROL Resource Budgeting] 領域または [!UICONTROL Resource Planner] で予算化された時間は、次の領域に表示されます： [!DNL Workfront] 以下の名前の下に置きます。</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL Budgeted Hours] の表示名</strong></td> 
        <td><strong>領域： [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL 時間 ]</td> 
        <td>[!UICONTROL ビジネスケース ] の [!UICONTROL Resource Budgeting] 領域</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Hours] が閲覧した [!UICONTROL Resource Planner]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL 予算時間 ]</td> 
        <td> <p>[!UICONTROL 時間 ] ビューの使用率レポート</p> <p>[!UICONTROL 使用率 ] レポートについて詳しくは、 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[!UICONTROL リソース使用率 ] レポートの概要</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. 時間]</td> 
        <td> <p>[!UICONTROL 予算時間 ] レポート</p><p>予算時間レポートの [!UICONTROL 予算時間 ] オブジェクトは、廃止されたリソース管理ツールに関連する情報を参照します。 「[!UICONTROL Bud」のみ。 このレポートの「時間」フィールドは、プロジェクトの [!UICONTROL ビジネスケース ] の [!UICONTROL Resource Planner] または [!UICONTROL Resource Budgeting] 領域で予算設定された時間を参照します。 </p> <p>レポートの作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>.</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL リソースプランナーの予算時間数 ] </td> 
        <td> <p>次のレポートに含まれています：</p>
        <ul>
        <li>[!UICONTROL Project] レポート
        <li>[!UICONTROL プロジェクト（金融データ）] レポート
        <li>[!UICONTROL タスク ] レポート
        <li>[!UICONTROL 問題 ] レポート
        <li>[!UICONTROL 予算時間 ] レポート</li>
        </ul>
         <p>レポートの作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>.</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>[!UICONTROL Budgeted Hours] のその他の言及： [!DNL Adobe Workfront] は、Workfrontから削除された廃止された機能を使用して予算に計上された時間数を指します。 これらは表示のみのフィールドで、現在のリソース予算ツールを使用する際に、現在の情報では更新されません。 </p>
    <!--<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Hours from theResource Planner in the areas and reports listed below. </p>
     <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Hours view (in the BDG column)</li>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Hours view</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (the Bud. Hours field refers to hours budgeted for users; the Pln. Bud. Hours field refers to hours budgeted for roles or projects)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Project: Budgeted Hours field) </li>
        </ul>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The fields listed below display in the reports listed and are hours formerly budgeted in the&nbsp;Capacity Planner or the Legacy Resource Estimates area of the Business Case.</p>
         <p>Important: The Capacity Planner and Legacy&nbsp;Resource Estimates have been removed from Workfront. You cannot update any information that might display in these fields.</p>
        <ul>
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy&nbsp;Resource Estimates area of the Business Case (in the Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (in the Bud. Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report (in the Budgeted Hours field)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project (Financial&nbsp;Data) report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report (in the Project: Budgeted Hours field)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report (in the Project: Budgeted Hours field)</li>
      </ul> --> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予算労務費 ]</td> 
   <td> <p>これは、リソースマネージャとして、プロジェクトで完了する必要のある作業に対するジョブロールの予算に関連するコストです。 </p> <p>プロジェクトレポートの [!UICONTROL 予算労務費 ] は、次の式を使用して計算されます。</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>このフィールドは、次を参照している場合があります。</p> 
    <ul> 
     <li> <p>[!UICONTROL ビジネスケース ] の [!UICONTROL Resource Budgeting] 領域、またはプロジェクトのジョブロールのコストに関連付けられた [!UICONTROL Resource Planner] に表示される労務費。 [!UICONTROL 予算労務費 ] の計算の詳細は、この記事を参照してください。 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">[!UICONTROL プロジェクトの予算労務費の把握 ] および [!UICONTROL 予算時間 ]</a></p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>[!UICONTROL ビジネス事例 ] の [!UICONTROL Resource Budgeting] 領域に表示される労務費。この領域には、 [!DNL Scenario Planner] シナリオ・プランナを使用してプロジェクト・リソースを予算化する場合。 イニシアチブについて詳しくは、 <a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">シナリオプランナーのイニシアチブの概要</a>. </p> <p>The [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The [!DNL Scenario Planner] 概要</a>. </p> </li> 
     <p>の次の領域で、次の名前で表示されます。</p>
   <ul>
   <li><strong>[!UICONTROL 予算労務費 ]</strong>:[!UICONTROL ビジネスケース ] の [!UICONTROL Resource Budgeting] 領域。
   <li><strong>[!UICONTROL 予算コスト ]</strong>:[!UICONTROL 使用率 ] レポートの [!UICONTROL コスト ] ビュー
   <p>詳しくは、 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">リソース使用率情報の表示 </a>.</p>
   <li><strong>[!UICONTROL BDG]</strong>：内 [!DNL Resource Planner] プロジェクトまたは [!DNL Role] 表示（コスト別表示時）
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>：次のレポート内： 
   <ul>
    <li>[!UICONTROL Project] レポート</li>
    <li>[!UICONTROL プロジェクト（金融データ）] レポート</li>
    <li>[!UICONTROL タスク ] レポート</li>
    <li>[!UICONTROL 問題 ] レポート</li>
    <li>[!UICONTROL 予算時間 ] レポート</li> 
    </ul>
    <p>レポートの作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>.</p>
    <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Labor costs for hours budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner). This was available only in Adobe Workfront Classic. </p>
           <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
       </li> 
    </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost field based on the hours budgeted in the Resource Planner in the following areas and reports in&nbsp;Workfront: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Planner Cost view (in the BDG column)</li>
          <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Utilization report Cost view (in the Budgeted Cost column)</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budgeting area of the Business Case </li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate the Budgeted Labor Cost associated with resources budgeted in the Resource Planner in the Resource Planner Resource Budgeted Cost field in the following reports: </p>
       <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can locate a Budgeted Labor Cost field that contains information from a tool that has been deprecated in the reports listed below. You can no longer update the fields displayed in these reports and budgeting your resources on the projects does not update them: </p>
        <ul> 
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Budgeted Hour report </li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Project report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Task&nbsp;report</li>
           <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Issue report</li>
         </ul>      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating the Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;.&nbsp;</p>
    --> 
    </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL 予算開始日 ]</td> 
  <td> <p>これは廃止されたフィールドです。 このフィールドに表示される情報は、 [!DNL Workfront] が削除されました。 このフィールドは更新できません。</p>
  <p>これらの領域は、 [!DNL Workfront]. </p> 
  <p>このフィールドは、[!UICONTROL プロジェクト ] および [!UICONTROL タスク ] のレポートとリストに引き続き表示されます。</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL バーンダウングラフ ]</td> 
   <td>完了した作業時間と残りの作業時間を視覚的に表す折れ線グラフです。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ビジネスケース ]</td> 
   <td> <p>プロジェクトを [!UICONTROL Idea] ステータスから [!UICONTROL Planning] ステータスに移動する必要があるかどうかを評価するために使用されるツール。 つまり、[!UICONTROL ビジネスケース ] は、特にポートフォリオ内の他のプロジェクトと比較する場合に、プロジェクトを起動して完了することが重要かどうかを判断するのに役立ちます。</p> <p>詳しくは、 <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">プロジェクトの [!UICONTROL ビジネスケース ] の作成 </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ビジネスケースの予算時間 ]</td> 
   <td> <p>これは廃止されたフィールドです。 このフィールドに表示される情報は、 [!DNL Workfront] が削除されました。 このフィールドは更新できません。</p> <p>このフィールドは、プロジェクトおよび [!UICONTROL タスク ] リストとレポートに引き続き表示されます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 計算割り当て ]</td> 
   <td> <p>タスクの [!UICONTROL 期間 ] タイプの 1 つ。 これにより、タスクの [!UICONTROL 期間 ] と [!UICONTROL 作業に必要な日数 ] に基づいて、タスクに割り当てられたユーザーのタスクに割り当てられる 8 時間の作業日の割合が計算されます。</p> <p>詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク [!UICONTROL 期間 ] と [!UICONTROL 期間タイプ ] の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 計算作業 ]</td> 
   <td> <p>タスク [!UICONTROL 期間タイプ ] の 1 つ。 これにより、[!UICONTROL 期間 ] とユーザー [!UICONTROL 割り当て ] の割合（8 時間の稼働日に基づく）が指定されたタスクの [!UICONTROL 作業量（必須）] が計算されます。</p> <p>詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク [!UICONTROL 期間 ] と [!UICONTROL 期間タイプ ] の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カレンダー ]</td> 
   <td> <p>には 2 種類のカレンダーがあります [!DNL Workfront]:[!UICONTROL ホームカレンダー ] およびカレンダーレポート。</p> <p>[!UICONTROL ホームカレンダー ] は、ユーザーが使用可能な時間に対して、自分の作業負荷を管理できる個人用カレンダーです。 [!DNL Workfront]. また、[!UICONTROL Home Calendar] を [!DNL Outlook] ([!DNL Google] および [!DNL Microsoft] 統合に関する情報が含まれます )。 </p> <p>[!UICONTROL Home Calendar] について詳しくは、 <a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL ホームカレンダー ] ビュー</a>.</p> <p>カレンダーレポートは、イベントの日付やその他の重要な詳細（期日、作業状況、イベントが割り当てられたユーザーなど）を表示できる動的レポートです。</p> <p> カレンダーレポートの詳細については、 <a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">カレンダーレポートの概要</a>.</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL 開始可能 ]</td> 
   <td> <p>このフィールドは、タスクの作業を開始する準備ができているかどうかを示します。 タスクの [!UICONTROL Can Start] フィールドで作業を開始する準備が整ったら、[!UICONTROL True] に設定します。 </p> <p>詳しくは、 <a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">タスクの「[!UICONTROL Can Start]」の概要</a>.</p> 
   <!--
     <p>(NOTE: everything below is drafted because I created a new article linked above with all this information - it was getting kind of too big for just a table cell)</p>
    --> <!--
     <p>Workfront checks for the following things before it marks a task as True for the Can Start field:<br></p>
    --> 
    <!--
     <ul> 
      <li> If the task has a parent, it checks to see if the value of Can Start for the parent it set to True. If the value for the parent is False, then all the subtasks have the value of Can Start set to False, as well.&nbsp;</li> 
      <li> It also checks to see if the predecessors of the task as well as the predecessors of their parents are complete. If they are complete, the Can Start value for the task is set to True. If any of the task predecessors or their parents' predecessors are not complete, or have a status of Complete-Pending Approval, then the Can Start value for the task is set to False.&nbsp;</li> 
     </ul>
    --> 
    <!--
     <p>For information about task predecessors, see <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">Overview of task predecessors</a>.</p>
    --> <!--
     <p>Tip: If the Dependency Type between a task and its predecessors is Start-Start, the predecessor must start before the predecessor relationship is considered resolved and the successor tasks can start. For information about dependency types, see <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">Overview of task dependency types</a>. </p>
    --> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Capacity</td> 
    <td>The total availability (measure in either hours or FTE) of a designated user, resource pool, team, rob role, or company.</td> 
   </tr>
  -->

<tr> 
   <td> <p>キャパシティ</p> </td> 
   <td> <p>リソースを作業に割り当てることができる時間です。 「可用性」を参照してください。 </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL カテゴリ ]</p> </td> 
   <td> <p>カテゴリはカスタムフォームです。 このオブジェクトに関するレポートを作成し、他のオブジェクトレポートにも表示できます。 すべてのオブジェクトがカスタムフォームまたはカテゴリを持つことはできません。 次のオブジェクトは、カスタムフォームを持つことができます。 <br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL タスク ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL ドキュメント ]</li> 
     <li>[!UICONTROL 費用 ]</li> 
     <li>[!UICONTROL プログラム ]</li> 
     <li>[!UICONTROL ユーザー ]</li> 
     <li>[!UICONTROL 会社 ]</li> 
     <li>[!UICONTROL 反復 ]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カテゴリ名 ]</td> 
   <td> <p>次のオブジェクトのビューに列として追加されると、これらのオブジェクトに関連付けられているすべてのカスタムフォームのリストが表示されます。</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL タスク ]<br></li> 
     <li>[!UICONTROL の問題 ]<br></li> 
     <li>[!UICONTROLPortfolio]<br></li> 
     <li>[!UICONTROL ドキュメント ]<br></li> 
     <li>[!UICONTROL 費用 ]<br></li> 
     <li>[!UICONTROL プログラム ]<br></li> 
     <li>[!UICONTROL ユーザー ]<br></li> 
     <li>[!UICONTROL 会社 ]</li> 
     <li>[!UICONTROL 反復 ]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 変更管理 ]</td> 
   <td>計画作業を定義し、理解し、範囲、スケジュール、コスト、リソース要因の変化に合わせて調整することに重点を置いた練習領域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>プロジェクトに対して発生する問題の一種で、同意された範囲に対する要求された変更の概要を示します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変更のみ ]</td> 
   <td>プロジェクト [!UICONTROL 更新タイプ ] の 1 つ。 タスクに対する更新や、プロジェクトまたはタスクでの編集が行われた場合にのみ、[!UICONTROL Project Project Project Projected] および [!UICONTROL Planned] のタイムラインが更新されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>[!UICONTROL の問題 ] の種類の 1 つで、通常は、プロジェクトを完了する前に、計画外の作業が必要であることを示します。</p> <p>[!UICONTROL Issue] タイプの詳細については、この記事の「Default issue types」の節を参照してください <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">デフォルトの問題タイプをカスタマイズ</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 子タスク ]</td> 
   <td>[!UICONTROL 親タスク ] （[!UICONTROL サマリタスク ]）の [!UICONTROL サブタスク ] であるタスク。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 子 ]</td> 
   <td>[!UICONTROL 親タスク ] （[!UICONTROL サマリタスク ]）への [!UICONTROL サブタスク ] のコレクション。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コーチング ] と [!UICONTROL トレーニング ]</td> 
   <td>学習モジュール、認定、標準、または実践コミュニティ。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コミット ]</td> 
   <td>タスクの成果物に関する期待値を設定するユーザー向けの通信ツールです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コミット日 ]</td> 
   <td>ユーザーがタスクの成果物に関する期待事項を設定するための通信ツール。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] と [!UICONTROL Reporting]</td> 
   <td>プロジェクト、プログラムまたはポートフォリオの例外と正常性を確認するための基準</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 会社 ]</td> 
   <td> <p>[!UICONTROL 会社 ] は、 [!DNL Workfront]. </p> 
   <p> ユーザーまたはプロジェクトを 1 つの会社に関連付けることができます。 詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">会社の作成と編集</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 完了日 ]</td> 
   <td> <p>プロジェクト、タスク、またはタスクが完了する日付を指定します。 [!UICONTROL 完了日 ] には、複数のタイプがあります。 [!DNL Workfront]:</p> 
    <ul> 
     <li>[!UICONTROL 実際の完了日 ]。 詳しくは、 <a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">プロジェクト [!UICONTROL 実際の完了日 ] の概要 </a>.</li> 
     <li>[!UICONTROL 計画完了日 ]。 詳しくは、 <a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">プロジェクト [!UICONTROL 計画完了日 ] を設定</a> および <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">タスク [!UICONTROL 計画完了日 ] の概要</a>.</li> 
     <li>[!UICONTROL 予測完了日 ]。 詳しくは、 <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">プロジェクト、タスクおよび問題に関する [!UICONTROL 予定完了日 ] の概要</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 完了日 ]</td> 
   <td>[!UICONTROL テンプレート ] の開始を基準とした、[!UICONTROL テンプレートタスク ] または [!UICONTROL テンプレート ] が完了する予定の日。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 完了モード ]</td> 
   <td> <p>これは、プロジェクトが [!UICONTROL 完了 ] としてどのようにマークされるかを示します。 次の 2 つの値を持つことができます。</p> 
    <ul> 
     <li>[!UICONTROL 手動 ]：ユーザーは、プロジェクトのステータスを [!UICONTROL 完了 ] に変更する必要があります。</li> 
     <li>[!UICONTROL 自動 ]：プロジェクト内のすべてのタスクが 100%完了し、すべての問題が終了すると、プロジェクトのステータスは自動的に [!UICONTROL 完了 ] に変わります。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 条件 ]</td> 
   <td> <p>これは、タスク、イシュー、またはプロジェクトの進行状況を視覚的に表します。</p> <p>プロジェクトの場合、条件は、プロジェクト所有者が手動で設定することも、 [!DNL Workfront]（プロジェクトの進捗状況ステータスに基づく） </p> <p>プロジェクト条件に指定できる値は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL が問題を発生しています ]</li> 
    </ul> <p>プロジェクト条件の詳細については、「 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[!UICONTROL Project Condition] と [!UICONTROL Condition Type] の概要</a>.</p>
     <p>タスクと問題の条件を、レポートに表示できる数値に関連付けることができます。 以下のリストには、タスクとタスクの条件に対するデフォルトの名前と数値が表示されます。 システム管理者は、条件の名前を更新し、異なる数字の新しい条件を追加できます。 数値を条件に関連付けると、その数値は編集できなくなります。  </p> 
     <p>タスクの場合、条件はタスクの所有者が手動で設定します。 タスク条件に指定できる値は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL スムーズに進行中 ] (0)<br></li> 
     <li> [!UICONTROL いくつかの懸念事項 ] (1)<br></li> 
     <li>[!UICONTROL 主要な障害要因 ] (2)</li> 
    </ul> <p>タスク条件の詳細については、「 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">タスクと問題に関する [!UICONTROL 条件 ] の更新</a>.</p> <p>問題の場合、条件は問題の所有者が手動で設定します。 この問題の条件に指定できる値は次のとおりです。<br></p> 
    <ul> 
     <li>[!UICONTROL スムーズに進行中 ] (0)<br></li> 
     <li>[!UICONTROL いくつかの懸念事項 ] (1)<br></li> 
     <li>[!UICONTROL 主要な障害要因 ] (2)</li> 
    </ul> 
   <p><b>メモ</b></p>
    <p>[!UICONTROL ジャーナルエントリ ] レポートで [!UICONTROL 条件 ] フィールドがトラッキングされると、[!UICONTROL 新規 ] および [!UICONTROL 古い数値 ] には、名前の代わりに条件に関連付けられた数値が表示されます。 タスクまたはイシューに対して条件が最初に定義されていない状態で、後で更新した場合、更新を取り込むジャーナルエントリには、[!UICONTROL 条件 ] フィールドの [!UICONTROL 古い数値 ] が —2,147,483,648 と表示されます。 この記事の「[!UICONTROL 新しい数値 ]」、「[!UICONTROL 古い数値 ]」、「[!UICONTROL ジャーナルエントリ ]」も参照してください。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 条件の更新 ]</td> 
   <td> <p>このフィールドには、タスク、プロジェクトまたはタスクの現在の状態が表示されます。 このオプションは、タスク、プロジェクトまたはイシューの所有者が [!UICONTROL ステータスの更新 ] フィールドで新しい条件と共に提供した最新の更新を表示します。</p> <p>条件の更新に対しておこなわれたコメントは、[!UICONTROL 条件の更新 ] 列には表示されません。メインの更新のみが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制約日 ]</td> 
   <td> <p>[!UICONTROL の開始日 ] など、特定の日付に結び付けられた [!UICONTROL タスク制約 ] を使用している場合、その特定の日付はタスクの [!UICONTROL 制約日 ] になります。</p> <p>次のタスク制約で [!UICONTROL 制約日 ] フィールドが更新されます。</p> 
    <ul> 
     <li>[!UICONTROL は [] から始める必要があります</li> 
     <li>[!UICONTROL 終了日 ]</li> 
     <li>[!UICONTROL 次の日までに開始 ]</li> 
     <li>[!UICONTROL 次の日までに開始 ]</li> 
    </ul> <p>ヒント：   
     <ul> 
      <li> <p>[!UICONTROL 制約 ] が [!UICONTROL 固定日付 ] のタスクには [!UICONTROL 制約日 ] がありません。 </p> </li> 
      <li> <p> [!UICONTROL 制約日 ] は、レポートまたはカスタマイズされたビューでのみ表示できます。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制約日 ]</td> 
   <td> <p>[ 開始日 ] など、特定の日に関連付けられたテンプレートタスクで [ タスク制約 ] を使用している場合は、その日がテンプレートタスクの [ 制約日 ] になります。</p> <p>次のタスク制約で、「[!UICONTROL 制約日 ]」フィールドが更新されます。</p> 
    <ul> 
     <li>[!UICONTROL は [] から始める必要があります</li> 
     <li>[!UICONTROL 終了日 ]</li> 
     <li>[!UICONTROL 次の日までに開始 ]</li> 
     <li>[!UICONTROL 次の日までに開始 ]</li> 
    </ul> <p>ヒント： [!UICONTROL 制約日 ] は、レポートまたはカスタマイズされたビューでのみ表示できます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制約タイプ ]</td> 
   <td> <p>Task のスケジューリング傾向。 例えば、[!UICONTROL 可能な限り早く ] はタスクの開始をスケジュールし、[!UICONTROL 次の日まで ] はタスクの終了を [!UICONTROL 制約日 ] までにスケジュールします。</p> <p>詳しくは、 <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL タスク制約 ] の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コンテキストメニュー ]</td> 
   <td>画面の左側にあるメニューで、アクティブなコンテンツと関連付けてアイテムが変更されます。 例えば、ユーザーがプロジェクトを表示している場合、[!UICONTROL コンテキストメニュー ] にはプロジェクト関連の情報およびツールへのリンクが表示されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換された問題作成者 ]</td> 
   <td>問題がプロジェクトまたはタスクに変換されたときに、その問題の [!UICONTROLプライマリ連絡先 ] であるユーザーに関する情報を表示する、プロジェクトまたはタスクレポートのフィールドです。 このフィールドは「[!UICONTROL プロジェクトの詳細 ]」セクションにも表示され、変換後のイシューの [!UICONTROLプライマリ連絡先 ] の名前が表示されます。 この記事の「[!UICONTROLプライマリ連絡先 ]」も参照してください。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL コスト ]</td> 
   <td> <p>プロジェクト、タスクまたはイシューの完了時に費やす必要がある金額です。 </p> <p>プロジェクトに関連する労務、費用、リスクの様々なタイプのコストを追跡できます。 [!DNL Workfront] 参照 <a href="../../../manage-work/projects/project-finances/track-costs.md">コストの追跡</a>.</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コストタイプ ]</td> 
   <td>タスクの場合、[!UICONTROL コストタイプ ] はタスクによるコスト発生の方法を決定します。 例としては、[!UICONTROL 固定時間別 ]、[!UICONTROL ユーザー時間別 ]、[!UICONTROL ユーザー時間別+固定 ] などがあります。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクト間の依存関係 ]</td> 
   <td> <p>1 つのプロジェクトのタスクは、別のプロジェクトのタスクに依存します。</p> <p>詳しくは、 <a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">プロジェクト間の先行タスクの作成</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL カスタムデータ ]</td> 
   <td> <p>組織に固有のデータ。 組織は、 [!DNL Workfront] カスタムフォームとカスタムフィールドを作成してアプリケーションを作成する。 このカスタム情報により、KPI、監査、およびデマンドミックスに関するレポート作成を促進できます。 </p> <p>[!UICONTROL カスタムデータ ] は次のものにリンクできます。</p> 
    <ul> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL タスク ]</li> 
     <li>[!UICONTROL ユーザー ]</li> 
     <li>[!UICONTROL 会社 ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROL ドキュメント ]</li> 
     <li>[!UICONTROL 費用 ]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL プログラム ]</li> 
     <li>[!UICONTROL 反復 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カスタムデータ型 ]</td> 
   <td>[!UICONTROL カスタムデータ ] フィールドをテキスト、日付、数値、通貨のいずれでデータベースに格納するかを指定するオプションです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カスタム表示タイプ ]</td> 
   <td>カスタムフィールドの表示タイプ。 例としては、[!UICONTROL Drop-Down]、[!UICONTROL Text Field]、[!UICONTROL Text Area]、[!UICONTROL Radio Buttons] などがあります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カスタムフィールド ]</td> 
   <td>ユーザーが複数のオプションから選択できるカスタムデータの場合、これらの値はユーザーが選択できる値です。 カスタムオプションは、[!UICONTROL ドロップダウン ]、[!UICONTROL 複数選択ドロップダウン ]、[!UICONTROL ラジオボタン ] および [!UICONTROL チェックボックス ] でのみ有効です。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カスタムフォームラベル ]</td> 
   <td>[ カスタムオプション ] で [ カスタム表示タイプ ] を使用する場合、これは、[ カスタムオプション ] の [ ドロップダウン ] メニュー、[ チェックボックス ]、または [ ラジオボタン ] に表示される [ ユーザインタフェース ] テキストです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カスタム値 ]</td> 
   <td>カスタムオプションでカスタムフィールドを使用する場合、この値は特定のオプションに対してデータベースに格納されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL カスタムビュー ]</td> 
   <td>リスト内の各オブジェクトに対して表示されるデータフィールド（列）の定義。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Workfrontのインスタンスを使用する組織。</td> 
  </tr> 
 </tbody> 
</table>

## D - F

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>オブジェクト名</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL ダッシュボード ]</td> 
   <td> <p> このフィールドをレポートまたはレポートオブジェクトのリストに追加して、リストにレポートが表示されるダッシュボードを表示できます。 </p> <p> このフィールドを使用して、特定のダッシュボードにリストされているレポートをフィルタリングすることもできます。 </p> <p> レポートオブジェクトレポートにダッシュボード情報を含める方法の詳細については、この記事の「ダッシュボードに表示されるレポートについて」の節を参照してください。 <a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">レポートへのアクセスと整理</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL データ型 ]</td> 
   <td>「[!UICONTROL カスタムデータタイプ ]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 遅延日数 ]</td> 
   <td> <p>このフィールドには、[!UICONTROL 実際の完了日 ] がない場合に、[!UICONTROL 予定開始 ] と [!UICONTROL 今日 ] の日付差が表示されます。</p> <p>また、[!UICONTROL 実際の完了日 ] が存在する場合に、[!UICONTROL 実際の完了 ] と [!UICONTROL 予定完了 ] の間の日付の違いも表示します。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL デフォルトのスケジュール ]</td> 
   <td> <p>組織内のユーザーおよびプロジェクトに割り当てられる、カスタマイズ可能なデフォルトの勤務時間。 </p> <p>スケジュールは、ユーザーに割り当てられるタスクの計画日、開始日、完了日を計算するために使用されます。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 成果物 ]</td> 
   <td>プロジェクトの完了時に提供する必要がある定量化可能な商品またはサービス。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>インテークプロセスのスコア付けと優先順位付け。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 部門目標 ]</td> 
   <td>部門内の運用指標の改善に注力する特定の部門に固有の目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 依存関係 ]</td> 
   <td>一方のタスクが他方のタスクのステータスを変更する前に、一方のタスクを必要とする 2 つのタスク間のリンクも、ステータスを変更する場合があります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 依存関係の種類 ]</td> 
   <td> <p>タスクと先行タスクとの間のスケジューリング関係のタイプ。 1 つは [!UICONTROL Finish-Start] です。この場合、最初のタスクは、2 番目のタスクが開始する前に完了する必要があります。</p> <p>詳しくは、 <a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">タスク依存関係タイプの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ドキュメント ]</td> 
   <td>内のオブジェクトに添付されたファイル [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ドキュメントのバージョン ]</td> 
   <td> <p>同じドキュメントが同じオブジェクトにアップロードされるたびに、バージョン番号が割り当てられます。 ユーザーは、ドキュメントの以前のバージョンの複数のオプションを表示および変更できます。</p> <p>詳しくは、 <a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">ドキュメントバージョンの管理</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 期間 ]</td> 
   <td> <p>タスクの問題またはプロジェクトの完了に割り当てられる時間枠（[!UICONTROL 計画開始 ] から計画完了までの日数で決定）。</p> 
    <ul> 
     <li>タスクの場合、タスクの「期間」タイプが「単純」でない場合、「期間」は編集可能なフィールドです。 タスクの期間の種類が [ 簡易 ] の場合、またはタスクの制約が固定日付の場合、期間はWorkfrontが実行する計算です。</li> 
     <li>問題の場合、「期間」は常に編集可能なフィールドで、問題の解決に必要な日数の推定値を表す必要があります。</li> 
     <li>プロジェクトの場合、期間は次の方法で実行される計算です： [!DNL Workfront] これは、最も早いタスクの計画開始と、プロジェクトの最新タスクの [!UICONTROL 計画完了 ] の間の日数の差を表します。</li> 
    </ul> <p>タスクの [!UICONTROL 期間 ] と [!UICONTROL 予定期間 ] の違いについて詳しくは、この記事を参照してください <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">タスクの [!UICONTROL 予定期間 ] と [!UICONTROL 予定期間 ] の違い</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 時間（分単位）]</td> 
   <td>このフィールドには、[!UICONTROL 期間 ] フィールドと同じ情報が日数ではなく分単位で表示されます。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL 発生あたりの期間 ]</td> 
   <td> <p>これは、繰り返しタスクの親の [!UICONTROL タスクの詳細 ] ボックスと [!UICONTROL タスクの編集 ] ボックスに表示されます。 各繰り返しタスクの期間が表示されます。 繰り返しタスクの作成について詳しくは、 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">繰り返しタスクの作成</a>. </p> <p> <span>個々の定期タスクで変更された期間は、このフィールドに示される値を表示しません。</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 期間の種類 ]</td> 
   <td> <p>タスクの完了に必要な作業を、タスク期間を通じて担当者に割り当てる方法を示すタスクフィールドです。 これは、タスクの [!UICONTROL 期間 ]、[!UICONTROL 作業に必要な時間 ]、および割り当てられたリソースがタスクを完了するために費やす時間（[!UICONTROL 割り当て ]）との関係を表します。 </p> <p>このフィールドは、タスクの「[!UICONTROL 詳細 ]」タブに表示されます。 </p> <p>オプションは次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL 計算割り当て ]</li> 
     <li>[!UICONTROL 計算作業 ]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL シンプル ]</li> 
    </ul> <p>詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク [!UICONTROL 期間 ] と [!UICONTROL 期間タイプ ] の概要</a>.</p> 
    —&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>電力検索で時間を測定するために使用される単位。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>ユーザー数とタスクが完了するまでに要する時間との関係。 ユーザーを追加すると、タスクの完了に予定されている合計時間は短くなりますが、タスクの期間は変わりません。 例えば、タスクでピーナッツの樽をシェルしている場合、人数を増やすと予定時間が短縮されますが、担当者日数の期間は同じままになります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 経過時間 ]</td> 
   <td> <p>[!UICONTROL 経過時間 ] は、タスクの [!UICONTROL 期間 ] の時間の単位です。 タスクの [!UICONTROL 予定開始日 ] から [!UICONTROL 予定完了日 ] までの時間で、休日、週末、休日が含まれます。 つまり、経過時間は暦日の経過です。 </p> <p>[!DNL Workfront] は、タスクの期間に関して、次の経過時間単位をサポートします。</p> 
    <ul> 
     <li> <p>[!UICONTROL 経過分数 ]</p> </li> 
     <li> <p>[!UICONTROL 経過時間 ]</p> </li> 
     <li> <p>[!UICONTROL 経過日数 ]</p> </li> 
     <li> <p>[!UICONTROL 経過週間 ]</p> </li> 
     <li> <p>[!UICONTROL 経過月数 ]</p> </li> 
    </ul> <p>タスクの期間（経過時間など）の詳細については、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク [!UICONTROL 期間 ] と [!UICONTROL 期間タイプ ] の概要</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 終了日 ]</td> 
   <td> <p> [!UICONTROL レート ] レポートでは、プロジェクトレベルでのジョブの役割に対する新しい請求率が終了した日付です。 この日付より前のプロジェクトに関連する時間にこの請求率を掛けて、プロジェクトの売上高を計算します。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>タスク、プロジェクト、チーム、または組織に対するコミットメントと信念が減少している時期を示す [!UICONTROL 作業パフォーマンスインジケーター ] (WPI)。 これは、その信念とコミットメントを復活させるために行動する必要があることを示しています。 WPI は、簡単な質問をして測定されます。 「自分が何を期待していたのか、分かりましたか？ 君が任された仕事が組織に影響を与えたか？ 素晴らしい仕事をしたのか？」</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL エンタープライズ目標 ]</td> 
   <td>企業目標の指標に貢献する部門をまたいだ目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベント ]</td> 
   <td>プロジェクトまたはタスクに対する変更。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベントハンドラー ]</td> 
   <td>イベントの発生時に発生する自動化されたタスク。 一般的な例として、自動電子メール通知が挙げられます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イベント通知 ]</td> 
   <td>イベントハンドラーから生成された電子メール。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 費用 ]</td> 
   <td>タスクまたはプロジェクトに関する非労務費。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 外部 ]</td> 
   <td> <p>通常は、ライセンスの種類、またはそのようなライセンスを持つユーザーで、システム内の情報を確認する機能のみを持っています。</p> <p>詳しくは、 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] ライセンスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 外部システム ]</td> 
   <td>指定された記録システムの外部に保存および管理されるサービスまたはソフトウェア。</td> 
  </tr>

<tr> 
   <td>[!UICONTROL フィールド ]</td> 
   <td><p>任意のWorkfrontオブジェクト、またはそれに関連付けられている情報（データベースに表示されるもの）。 </p>
   <p>例えば、「project」、「user」、「hour」は、Workfrontオブジェクトとフィールドの両方です。 「名前」、「ステータス」、「所有者」、「開始日」は、上記のオブジェクトに関連付けられたWorkfrontフィールドです。 </p>

<p>オブジェクトを参照する場合、「objects」と「fields」は同じ意味で使用できます。</p>
   <p>レポートの範囲では、「フィールド」は、レポートに取り込むオブジェクトまたはオブジェクトに関する情報を指します。</p>

<p><b>メモ</b></p>

<p>テキストの詳細レポートでは、フィールドは、データベースに表示されるオブジェクトまたはその情報を参照します。</p>
   <p>ユーザーインターフェイスに表示される名前が、データベースのフィールドの名前と異なる場合があります。 例えば、「issue」はWorkfrontインターフェイスのオブジェクトの名前ですが、「opTask」はWorkfrontデータベースのオブジェクト（またはフィールド）の名前です。 </p> 
   <p> テキストモードのレポート、表示、フィルター、グループ化の記述時、または計算フィールドの作成時に、データベースに表示されるフィールドを使用することが重要です。</p>

<p>詳しくは、 <a href="../../../wf-api/general/api-explorer.md">API エクスプローラ</a> および <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">テキストモードの概要</a>.</p>

<p>デフォルトでは、Workfrontには、オブジェクトとその情報の両方を定義する一連のフィールドが用意されています。 また、カスタムフィールドを作成してオブジェクトを定義することもできますが、カスタムオブジェクトを作成することはできません。</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL フィルター ]</td> 
   <td> <p>画面に表示する情報を定義する、レポートの主要な構成要素またはリスト要素の 1 つ。 レポート要素について詳しくは、 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">レポート要素：フィルター、ビューおよびグループ化</a>.</p> <p>フィルターは、レポートまたは [!DNL Workfront] パネルリスト（プロジェクト、タスク、タスクなど）。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>の人件費、費用、収益データを管理するプロセス [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 固定コスト ]</td> 
   <td>プロジェクトに対して一定のコストを定義できます。 これは、プロジェクトの [!UICONTROL 計画コスト ] の一部で、プロジェクトの完了に必要な金額を表します。 コストの詳細については、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 固定売上高 ]</td> 
   <td>プロジェクトの売上高は、一定額で定義できます。 これは、プロジェクトの [!UICONTROL 計画売上高 ] の一部で、プロジェクトの完了時に入手できる金額を表します。 売上高について詳しくは、 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と売上高の概要</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フラグ ]</td> 
   <td> <p> これは [!UICONTROL ステータスアイコン ] と同じフィールドですが、次の表示でのみ使用できます。 </p> 
    <ul> 
     <li> [!UICONTROL テンプレート ] </li> 
     <li> [!UICONTROL 費用 ] </li> 
    </ul> <p> 詳しくは、 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">ビュー内のビルトインステータスアイコン</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ]</td> 
   <td>フォルダは、オブジェクトに関連付けられたドキュメントやレポートを整理するために使用します。</td> </tr>
  <tr>
  <td>[!UICONTROL FTE] （フルタイム相当）</td> 
   <td>これは、リソースが作業に使用できる時間を示す [ フルタイム相当 ] です。 
   [!UICONTROL FTE] フィールドは、次の領域に表示されます。 
  <ul>
   <li> ユーザーを編集または作成する際のユーザーのプロファイル </li>
   <li> [!UICONTROL リソースプランナー ] </li>
   <li> [!UICONTROL Scenario Planner] (Workfront Scenario Planner の追加ライセンスが必要 ) </li>
   <li> ユーザーリストとレポート </li> </ul>

<p>[!UICONTROL FTE] は、1 までの 10 進数で指定する必要があり、0 にはできません。 </p>
   <p> [!UICONTROL FTE] が 1（ユーザーのプロファイルで定義されている [!UICONTROL FTE] フィールドのデフォルト）の場合、リソース（ユーザーまたは役割）は、可用性を計算するスケジュールに基づいて、時間数全体で機能します。 </p>
   <p>Workfront管理者が、ユーザーの可用性を判断する際に使用するスケジュールを決定します。  </p>
   <ul>
   <li> [!UICONTROL デフォルトスケジュール ] を使用すると、Workfrontはプロファイル内のユーザーの [!UICONTROL FTE] を使用して可用性を計算します。 </li>
   <li> ユーザースケジュールを使用すると、Workfrontはユーザーのオフ時間、[!UICONTROL 作業時間 ] 値および [!UICONTROL デフォルトスケジュール ] の時間を使用して、ユーザーの [!UICONTROL FTE] を計算します。 </li> </ul>

<p>詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理環境設定の指定</a>.  </p>
   <p>でのスケジュール作成の詳細 [!DNL Workfront]を参照してください。 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールの作成</a>. </p>

<p><b>メモ</b></p>
   <p>[!UICONTROL Scenario Planner] のすべての計算に対して、Workfrontは値 1 [!UICONTROL FTE] = 8 時間を使用します。</p>
   <p>詳しくは、 <a href="../../../scenario-planner/get-started-with-scenario-planning.md">[!UICONTROL Scenario Planner] の概要</a>. </p>
   </td> </tr> 
   </tbody> 
   </table>

<!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Task field used by the planner to set how the work required is allocated to the assignees across the duration.</p>
<!--
FTE
The designated full time equivalency for users. A full-time user should have 100% FTE and part-time user should have a percentage that equals their working hours. 
-->

## G - I

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>オブジェクト名</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL ガントチャート ]</td> 
   <td> <p>プロジェクトのタスクが現在スケジュールされているときの、計画日または予定日に基づくカレンダービューのプロジェクト日の視覚的なタイムライン。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>目標に関する概念は次の 2 つです： [!DNL Workfront]: </p> 
    <ul> 
     <li> <p><b>プロジェクトの目標</b>：プロジェクトの関連する関係者が合意した一連のビジネス目標。 プロジェクトの目標は、プロジェクトのビジネス事例の一部です。 </p> <p>プロジェクト目標をリストやレポートに表示することはできませんが、API を使用してアクセスできます。 </p> <p>ビジネス事例のプロジェクト目標については、 <a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">ビジネスケース目標の作成 </a>. </p> </li> 
     <li> <p><b>戦略目標</b>：戦略的目標は、特定の期間、作業戦略を計画するために作成する目標です。 これらのタイプの目標は、 [!DNL Workfront Goals]. 組織が戦略目標を作成するには、追加のライセンスを購入し、この機能へのアクセス権が必要です。 [!DNL Workfront Goals] は、追加のライセンスでのみ使用できます。</p> 
     <p>詳しくは、 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概要 </a>. </p> 
     <p>目標またはプロジェクトレポートに戦略目標を表示し、API を使用してそれらにアクセスできます。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 目標階層 ]</td> 
   <td> <p>[!UICONTROL 目標 ] および [!UICONTROL プロジェクト ] レポートで、これは、戦略目標が他の目標と一致する場合に戦略目標が属する階層内の目標を表示するコレクションフィールドです。 目標は区切り文字▸区切りで区切られます。 </p> <p>このフィールドには、目標と目標の親のみが表示されます。 子の目標は表示されません。 </p> <p>での目標の調整に関する情報 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">の目標の整合の概要 [!DNL Workfront Goals]</a>. </p> 
   <p>このフィールドは、組織が [!DNL Workfront Goals]. を使用した戦略目標の管理の詳細 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概要 </a>. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 目標成功スコア ]</td> 
   <td> [!UICONTROL プロジェクトレポート ] では、このフィールドは、[!UICONTROL ビジネス ] ケースに関連付けられたプロジェクトレベルの目標を指すために使用されます。 現在、これは非推奨のフィールドで、機能に関連付けられていません。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 目標 ] </td> 
   <td> <p>[!UICONTROL プロジェクト ] レポートでは、これは、プロジェクトに関連付けられているすべての戦略目標を表示する収集フィールドです。 目標はコンマで区切ります。</p> <p>このフィールドは、組織が [!DNL Workfront Goals]. を使用した戦略目標の管理の詳細 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概要</a>. での戦略目標とプロジェクト目標の詳細 [!DNL Workfront]詳しくは、この記事の「[!UICONTROL 目標 ]」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL グローバルインターフェイス環境設定 ]</td> 
   <td>すべてのユーザーに影響するインターフェイス設定。 [!UICONTROL グローバルインターフェイス環境設定 ] は、[!UICONTROL ユーザーインターフェイス環境設定 ] で上書きできます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL グループ ]</td> 
   <td> <p>同じオブジェクトにアクセスできるユーザー（同じ部門またはビジネスユニットからの場合もあります）のコレクション。 ユーザーに加え、グループをポートフォリオ、プログラム、プロジェクトに関連付けることができます。<span> プロジェクトテンプレート</span> 会社、チーム、スケジュール、レイアウトテンプレート、およびタイムシートプロファイル。</p> <p>また、オブジェクトにグループ別の権限を付与することもできます。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">グループの概要</a>.</p> <p>次のいずれかのタイプのオブジェクトのリストまたはレポートで、[!UICONTROL Group] フィールドを使用して、特定のグループに関連付けられている特定のタイプのオブジェクト（ユーザー、ポートフォリオ、プログラム、プロジェクト）を一覧表示できます。 <span>プロジェクトテンプレート</span>、会社、チーム、スケジュール、レイアウトテンプレート、またはタイムシートプロファイル。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL グループ管理者 ]</td> 
   <td> <p>指定したユーザーグループのオブジェクト、アクセス、ユーザーを管理するユーザー。</p> <p> [!UICONTROL グループ ] レポートのこのフィールドには、グループで [!UICONTROL グループ管理者 ] として指定されたユーザーの名前が表示されます。 グループ管理者について詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 管理アクセス権を持つグループ ]</td> 
   <td> <p> [!UICONTROL レイアウトテンプレート ]、[!UICONTROL タイムシートプロファイル ]、または [!UICONTROL スケジュールレポート ] で、このフィールドには、グループ管理者がテンプレートを変更するためのアクセス権を持つグループが表示されます。 また、このフィールドでこのレポートをフィルタリングすることもできます。 </p> <p> 詳しくは、 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL グループ化 ]</td> 
   <td> <p>リスト内の情報を共通の基準で分類するために使用されるレポート要素。</p> <p>詳しくは、この記事の「[!UICONTROL グループ化 ]」の節を参照してください <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">レポート要素：フィルター、ビューおよびグループ化</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ハンドオフ日 ]</td> 
   <td> <p>タスクが作業可能になる日付。 [!UICONTROL ハンドオフ日 ] は計算日です。手動で設定することはできません。 <br>[!UICONTROL ハンドオフ日 ] について詳しくは、 <a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Task Handoff Date] の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ヘルプデスク ]</td> 
   <td>の部分 [!DNL Workfront] すべての問題キューを保持する [!UICONTROL ヘルプデスク ] を使用して、カスタマーサポートチケット、プロジェクトリクエスト、ヘルプデスクチケットなどを処理できます。 これは、[!UICONTROL 要求 ] 領域と同じです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 所有者 ]</td> 
   <td>[!UICONTROL 時間 ] レポートでは、[!UICONTROL 所有者 ] は時間が属するユーザーです。 これは、実際に時刻を記録しているユーザーとは異なります。 この 2 つのエンティティは、2 人の異なるユーザーになる場合があります。 <br>別のユーザーのログ時間の詳細については、「 <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">ログ時間</a>.</td> 
  </tr>

<tr> 
   <td>時間状態</td> 
   <td> <p>タスク、問題、プロジェクトに関してユーザーがログに記録する実際の時間に対してWorkfrontが設定する属性です。 </p>

Workfrontでは、時間エントリに次のいずれかのステータスを設定できます。
<ul>
   <li><b>送信済み</b>：プロジェクト、タスクまたはイシューにログオンしている時間。 請求レコードに含まれているか、まだ請求レコードに追加されていません。</li>
   <li><b>承認済み</b>：時間がログに記録され、プロジェクト所有者が承認しました。 請求レコードに含まれているか、まだ請求レコードに追加されていません。</li> 
   <li><b>未承認</b>：時間がプロジェクト所有者によって記録および却下されました。 請求レコードに含まれているか、まだ請求レコードに追加されていません。</li>
   <li><b>請求済み</b>：時間がログに記録され、請求レコードに追加され、請求レコードのステータスが「請求」とマークされています。 プロジェクト所有者の承認は必要ありませんでした。</li>
   <li><b>請求および承認済み</b>：時間がログに記録され、プロジェクト所有者が承認し、請求レコードのステータスが「請求」とマークされています。</li>
   </ul>


<p>時間が請求レコードに含まれる場合、時間ステータスは、時間が承認されたか、またはその時間が属する請求レコードが請求されたかを示します。 時間の入力時の時間ステータスは、時間リストまたはレポートにのみ表示されます。 </p>

<p>請求レコードに時間を追加する方法の詳細については、この記事の「請求レコードに時間を追加する」の節を参照してください。 <a href="../../../manage-work/projects/project-finances/create-billing-records.md" >請求レコードの作成</a>.</p>

<p>プロジェクトに関する承認時間の詳細については、 <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >プロジェクトの承認に時間を要する</a>.</p>

<p><b>ヒント</b></p>

<p>作業項目に直接ログインしていない一般的な時間には、時間ステータスは表示されません。 </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL 時間タイプ ]</td> 
   <td> <p>ユーザーがタスク、問題またはプロジェクトに対してログを記録する実際の時間に設定できる属性です。 これは、[!UICONTROL 休暇 ] や [!UICONTROL タイムオフ ] など、直接作業にリンクされていないログに記録された時間の属性でもあります。</p> <p>詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">時間タイプの管理</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>ID は、 [!DNL Workfront]. これは、 [!DNL Workfront] データベース。 レポート内の任意のオブジェクトの ID や、各オブジェクトのリストを表示できます。 </p> <p>ヒント：   <p>また、オブジェクトのページの URL に含まれる ID も確認できます。 例えば、プロジェクトの ID は、[!UICONTROL プロジェクトの詳細 ] ページにアクセスすると、次の URL に示す数字のようになります。</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 個々の目標 ]</td> 
   <td>チームの目標の指標に貢献するが、個人やキャリアの開発には関係しない個々の目標。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 継承されたアクセス ]</td> 
   <td>オブジェクトから別のオブジェクトにアクセスを伝達するための共有関数。 例えば、プログラムおよびポートフォリオレコードで定義された継承アクセス権がプロジェクトユーザーに与えられます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>Adobe Analytics の [!DNL Workfront Scenario Planner]を使用すると、プランを複数のイニシアチブに分割して、プランの管理を容易にすることができます。 <span>[!UICONTROL Initiative] レポートを作成し、[!UICONTROL Project] レポートで [!UICONTROL Initiative] 情報にアクセスできます。</span></p> <p>The [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The [!DNL Scenario Planner] 概要</a>. </p> <p>The [!DNL Initiative] レポートが [!DNL Workfront] インスタンス（会社がを購入していない場合） [!DNL Workfront Scenario Planner] ライセンス。 API から [!UICONTROL Initiatives] にアクセスすることはできません。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL イニシアチブジョブの役割 ]</span> </td> 
   <td> <p><span>[!UICONTROL イニシアチブジョブの役割 ] レポートタイプには、 [!DNL Workfront Scenario Planner].</span> </p> <p>The [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] 概要</a>. </p> <p><span>このレポートタイプは、 [!DNL Workfront] インスタンス（会社がを購入していない場合） [!DNL Workfront Scenario Planner] ライセンス。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> [!UICONTROL イニシアチブのジョブの役割 ] レポートには、イニシアチブのジョブの役割に関連する時間数が表示されます。</span> </p> <p>The [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] 概要</a>. </p> <p>このフィールドと [!UICONTROL Initiative Job Role] レポートタイプは、 [!DNL Workfront] インスタンス（会社がを購入していない場合） [!DNL Workfront Scenario Planner] ライセンス。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イニシアチブジョブの役割数 ]</td> 
   <td> <p>[!UICONTROL イニシアチブのジョブの役割 ] レポートには、イニシアチブに関連付けられている特定のジョブの役割の数が表示されます。</p> <p>The [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] 概要</a>. </p> <p>このフィールドと [!UICONTROL Initiative Job Role] レポートタイプは、 [!DNL Workfront] インスタンス（会社がを購入していない場合） [!DNL Workfront Scenario Planner] ライセンス。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative 最終公開日 ]</td> 
   <td> <p>[!UICONTROL Initiative]、[!UICONTROL Initiative Job Role]、および [!UICONTROL Project] の各レポートのフィールドで、プランイニシアチブがプロジェクトに最後に公開された日付を表示します。 イニシアチブをパブリッシュして、プロジェクトを作成したり、イニシアチブにリンクされたプロジェクトを更新したりできます。</p> <p>The [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] 概要</a>. </p> <p><span>イニシアチブの公開について詳しくは、</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">シナリオを公開して、でプロジェクトを作成および更新します。 [!DNL Workfront Scenario Planner]</a>. このフィールドは、 [!DNL Workfront] インスタンス（会社がを購入していない場合） [!DNL Workfront Scenario Planner] ライセンス。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL インライン検索 ]</td> 
   <td>検索は、フォームの完了中に、特定のフィールドに対して入力可能な項目を見つけるために実行されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL インターフェイスの設定 ]</td> 
   <td>カスタムビュー、フィルター、グループ化、リストコントロールなどを定義できるアプリケーションの領域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL が会社の目標 ]</p></td> 
   <td> <p>In [!DNL goal reports]に設定すると、各戦略目標の「[!UICONTROL True]/ [!UICONTROL False]」値が表示され、組織が目標に所有者として割り当てられているかどうかを示します。 </p> 
   <p>このフィールドは、組織が [!DNL Workfront Goals]. を使用した戦略目標の管理の詳細 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概要 </a>.</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL の問題 ]</td> 
   <td> <p>通常、タスクまたはプロジェクトの完了を妨げている問題があることを示す、計画外の作業項目です。 これは、さらなる作業労力の考慮のためにトリアージされ、評価されます</p> <p>[!UICONTROL の問題 ] は、[!UICONTROL ヘルプデスク ] のリクエストにもなります。 [!UICONTROL 変更管理 ]、[!UICONTROL リクエスト ]、[!UICONTROL バグ ] も [!UICONTROL 問題 ] です。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 問題管理 ]</td> 
   <td> <p>問題タイプの定義と、各タイプに関連付けられたルーティング、トラフィック、トラフィックの各プロセスを管理するプロセスとルール。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 問題の所有者 ]</td> 
   <td>問題のトリエージングと完了を担当するチームまたはユーザー。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 反復 ]</td> 
   <td>チームが事前に定義された成果物のセットを作成する期間。</td> 
  </tr> 
 </tbody> 
</table>

## J - L

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>オブジェクト名</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL ジョブの役割 ]</td> 
   <td> <p>ユーザーの日常の業務機能と責務を識別するために使用されます。 作業項目にジョブロールを割り当てて、特定のユーザーに割り当てずに、作業プロセスの完了に必要なスキルを特定できます。 </p> <p>1 人のユーザーに複数の役割を割り当てることができます。 例としては、グラフィックデザイナーやコンサルタントなどがあります。</p> <p>詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">ジョブの役割の作成と管理</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL ジャーナルエントリ ]</p> </td> 
   <td> <p>プロジェクト、タスク、問題およびその他のオブジェクトの [!UICONTROL 更新 ] 領域に表示される、追跡対象フィールドのシステム更新に関する情報を示すレポート可能なオブジェクトです。</p> <p>詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">[!UICONTROL 更新 ] 領域に関するレポート</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL かんばんフラグ ]</td> 
   <td> <p>[!UICONTROL Task] レポートまたは [!UICONTROL Issue] レポートでは、[!UICONTROL Kanban Flag] フィールドに [!UICONTROL Kanban Board] のストーリーに設定されているフラグステータスが表示されます。 指定できる値は、[!UICONTROL On Track]、[!UICONTROL Ready to Pull] および [!UICONTROL Is Blocked] です。</p> <p>[!UICONTROL かんばんストーリーボード ] のストーリーでフラグステータスを設定する方法については、この記事を参照してください <a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">[!UICONTROL かんばんボード ] のストーリーに対してフラグを使用します</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>企業が重要なビジネス目標をどの程度効果的に達成しているかを示す測定可能な値。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>先行タスクの [!UICONTROL 計画完了日 ] が経過してから、依存タスクが開始できるまでに経過する必要がある時間。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ラグタイプ ]</td> 
   <td> <p>[!UICONTROL Lag] の計算方法。 次のことが可能です。</p> 
    <ul> 
     <li>[!UICONTROL 日 ]（営業日）</li> 
     <li>[!UICONTROL カレンダー日 ] （休日を無視）</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL 曜日 ]</li> 
    </ul> <p>詳しくは、 <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">ラグタイプの概要</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 大きいサムネール ]</td> 
   <td> <p> [!UICONTROL ドキュメント ] のリストまたはレポートでは、ドキュメントのプレビューがサムネールで表示されます。 </p> <p>選択 <strong>[!UICONTROL 大きいサムネール ]</strong> をクリックすると、400 ピクセル幅のサムネールがレポートに表示されます。</p> <p>リストまたはレポートの列の幅を変更すると、サムネールのサイズが調整されます。</p> <p>この記事の「[!UICONTROL サムネール ]」も参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最近 10 人のビューア ]</td> 
   <td> <p>このフィールドには、レポートのリストに最近表示した最大 10 人のユーザーの名前が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>このフィールドには、オブジェクトの所有者が最後に入力した更新が表示されます。これは、オブジェクトに対する所有者の最新のアクティビティまたはインタラクションです。</p> <p>The [!DNL Last Condition Note] オブジェクトの最後のメモのメモテキストが削除されている場合、列は空になります。 オブジェクトに新しい注記を入力すると、その注記が最後の注記になり、列に再び表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最終財務更新日 ]</td> 
   <td>[!UICONTROL project] レポートでは、このフィールドは、プロジェクトの財務が最後に計算され、更新された日時を取り込みます。 プロジェクトの財政状況の詳細については、 <a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">プロジェクト財務の概要</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最終メモ ]</td> 
   <td> <p>このフィールドには、任意のユーザーがオブジェクトに最後に入力した更新が表示されます。 これは、オブジェクト上の最新のアクティビティまたはインタラクションです。</p> <p>オブジェクトの最後のメモのテキストが削除されている場合、[!UICONTROL 最後のメモ ] 列は空になります。 オブジェクトに新しい注記を入力すると、その注記が最後の注記になり、列に再び表示されます。</p>
   <p>このフィールドを [!UICONTROL タスク ] レポートに追加すると、問題、サブタスク、ドキュメントなどの子オブジェクトに更新が残ります。  — この列にはタスクのが表示されません。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最終閲覧者 ]</td> 
   <td> <p>このフィールドには、レポートリストで最後にレポートを表示したユーザーに関する情報が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最終閲覧日 ]</td> 
   <td> <p>レポートリストのこのフィールドには、レポートが最後に表示された日付が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL レイアウトテンプレート ]</td> 
   <td>特定のユーザーのワークスペースに表示されるタブとレポートを識別するために、システム管理者またはグループ管理者が定義します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レイアウトタイプ ]</td> 
   <td>[!UICONTROL カスタムビュー ] と組み合わせて、[!UICONTROL レイアウトタイプ ] は [!UICONTROL カスタムビュー ] のタイプを指定します。 現在は、リストのみを使用できます。 今後、[!UICONTROL 詳細 ]（オブジェクトの [!UICONTROL 詳細 ] ビュー）が使用可能になる可能性があります。</td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Cost</i>. </p> </td> 
  </tr>
  --> 
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Hours</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p> <p>The field is still visible in some reports and lists, but the information displayed cannot be updated. </p> <p>See <i>Budgeted Hours</i>. </p> <p>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        This field shows the number of hours budgeted for the project in the Legacy Resource Estimates area of the Business Case or in the Capacity Planner. 
       <br>If there&nbsp;are multiple job roles, this is a summary of the budgeted hours for all job roles. The Legacy Budgeted Hours are calculated after you have used the "Set budget to schedule" feature, or after you have defined how many of the Planned Hours should be budgeted, in the Resource Estimates area of the Business Case of the project or in the Capacity Planner.&nbsp; 
     </p> </td> </tr> -->
  <!--<tr data-mc-conditions=""> 
   <td>Legacy Budgeted Labor Cost</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> <p>The field is still visible in some reports and lists. </p> <p>See <i>Budgeted Labor Cost</i>. </p> 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In a project report, this field shows the labor cost associated with the project, taking into account the Cost per Hour rate of every job role and the amount of Legacy Budgeted Hours estimated in the Legacy Resource Estimates area of the Business Case that is needed for each role to complete the project.&nbsp;</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Legacy Budgeted Labor Cost in a project report is calculated using the following formula:</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code style="font-style: normal;">Legacy Budgeted Labor Cost = SUM(Job Role Cost per Hour * Legacy Budgeted Hours per Job Role)</code> </p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating Legacy Budgeted Labor Cost, see the article <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Understand Budgeted Labor Cost and Budgeted Hours for projects</a>&nbsp;&nbsp;</p>
    --> </td> 
  </tr> 
  <tr> 
   <!-- <td>Legacy Resource Pool</td> 
   <td> <p>This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed. This field cannot be updated. </p> 
   <p>Although not recommended, you may update the information in this report using the API.</p> 
   <p>See <i>Resource Pools</i> for updated fields. </p> 
   <p>The Legacy Resource Pool is a collection&nbsp;of job roles associated with a project or a user. The functionality of the Legacy Resource Pools is displayed in the tools available in the Legacy Resource Planning tab of the People area. This is a deprecated field.</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ライブラリタスク ]</td> 
   <td>アプリケーション全体で [!UICONTROL Tasks] と [!UICONTROL Template Tasks] の一貫した名前を付けるために使用される、単一のタスクのテンプレート。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ライセンスの種類 ]</td> 
   <td>[!UICONTROL アクセスレベル ] に割り当てられるライセンスのタイプ。 [!UICONTROL フルユーザー ]、[!UICONTROL 制限付きユーザー ]、[!UICONTROL リクエスター ] のいずれかです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ライセンス制限プラン ]</td> 
   <td> <p>[!UICONTROL グループ ] 表示またはレポートで、このフィールドには、各グループが [!UICONTROL ホームグループ ] として指定されているユーザーに割り当てることができる [!UICONTROL Plan] ライセンスの最大数が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ライセンス制限作業 ]</td> 
   <td> <p>[!UICONTROL グループ ] 表示またはレポートで、このフィールドには、各グループが [!UICONTROL ホームグループ ] として指定されているユーザーに割り当てることができる [!UICONTROL Work] ライセンスの最大数が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限付きユーザー ]</td> 
   <td>の作成を許可するライセンスタイプ [!DNL Access Level] には、表示のみの権限と、問題の送信、メモの入力およびドキュメントのアップロードを行う権限が含まれます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL リストコントロール ]</td> 
   <td> <p>[!UICONTROL インターフェイス設定 ] の一部で、カスタムフィルター、ビューおよびグループを個々のユーザーに、またはすべてのユーザーにグローバルにリンクできます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## M - O

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>オブジェクト名</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 手動のみ ]</td> 
   <td> <p>[!UICONTROL プロジェクト ] の [!UICONTROL 更新タイプ ] の 1 つ。 この設定を使用すると、「[!UICONTROL Reculed Timelines]」がクリックされた場合にのみ、[!UICONTROL Project Project Projected] および [!UICONTROL Planned] のタイムラインを更新できます。 この方法で設定されたプロジェクトは、再計算が少ないプロセス中や、プロジェクト内のプロジェクトまたはタスクが更新されたときに無視されます。</p> <p>詳しくは、 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクト [!UICONTROL 更新タイプ ] を選択 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>これは、現在ログインしているユーザーを指します。 </p> <p>他のユーザーとレポートを共有する際に、より一般的なレポートにするには、このフィールドをフィルターで使用することをお勧めします。 この方法では、1 つのレポートのみを作成できます。このレポートには、ログインしたユーザーに応じて常にカスタマイズされるので、ログインしたユーザーに応じて異なる情報が表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 最大ユーザー数 ]</td> 
   <td> <p>これは廃止されたフィールドです。 このフィールドに表示される情報は、 [!DNL Workfront] が削除され、フィールドを更新できません。 </p> <p>の以前のリリースでは [!DNL Workfront]の場合は、ジョブの役割を作成または編集する際にこのフィールドを更新できます。 各プロジェクトで役割に関連付けることができるユーザーの合計数が表示されていました。 プロジェクトに割り当てることのできるユーザーの数に制限はありません。値は 0 です。 </p>このフィールドは、一部のレポートおよびリストでは引き続き表示されますが、表示される情報は更新できません。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL マイルストーン ]</td> 
   <td> <p>タスクに関連付けて、タスクの完了時にプロジェクトの主要ポイントが達成されたことを示すマーカーです。 通常、マイルストーンを使用して、プロジェクトのフェーズの完了や一連の重要なアクティビティなど、重要なイベントを示すことができます。 [!UICONTROL マイルストーン ] は通常、親タスクに関連付けられています。 タスクに接続する前に、マイルストーンを作成する必要があります。 マイルストーンについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">マイルストーンパスを作成する</a> および <a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">タスクへのマイルストーンの関連付け</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL マイルストーンパス ]</td> 
   <td>[!UICONTROL マイルストーン ] の集まりです。 [!UICONTROL マイルストーンパス ] は、特定の種類の [!UICONTROL マイルストーン ] を持つプロジェクトと、異なる種類の [!UICONTROL マイルストーン ] を持つプロジェクトを区別するために、プロジェクトで使用されます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL マイルストーンタスク ]</td> 
   <td>測定するレポート可能なイベントを示すフラグが設定されたタスクです。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL モジュール ]</td> 
   <td>のシナリオ内の 1 つの手順 [!DNL Workfront Fusion] 関連するアプリに基づいて、が何らかの機能を実行する。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL マイプライマリの役割 ]</td> 
   <td> <p>これがフィルターで参照されると、ログインプライマリと同じ [!UICONTROLプライマリの役割 ] を持つユーザー、またはログインユーザーの [!UICONTROL ユーザーの役割 ] に割り当てられた作業項目が表示されます。</p> <p>他のユーザーとレポートを共有する際に、より一般的なレポートにするには、このフィールドをフィルターで使用することをお勧めします。 この方法では、1 つのレポートのみを作成できます。このレポートには、ログインしたユーザーに応じて常にカスタマイズされるので、ログインしたユーザーに応じて異なる情報が表示されます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL マイホームチーム ]</td> 
   <td> <p>これがフィルターで参照される場合、このフィールドには、ログインユーザーの [!UICONTROL ホームチーム ] に属するユーザー、またはログインユーザーの [!UICONTROL ホームチーム ] に割り当てられた作業項目が表示されます。 </p> <p>他のユーザーとレポートを共有する際に、より一般的なレポートにするには、このフィールドをフィルターで使用することをお勧めします。 この方法では、1 つのレポートのみを作成できます。このレポートには、ログインしたユーザーに応じて常にカスタマイズされるので、ログインしたユーザーに応じて異なる情報が表示されます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL 命名規則 ]</td> 
   <td>データを使用してプロジェクト、タスク、成果物の名前を作成する、組織全体のルールのセット。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL ネイティブ統合 ]</td> 
   <td>手動でのコーディングや API 設定を必要としない統合。 「標準」の統合とも呼ばれます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ナビゲーションメニュー ]</td> 
   <td>[!UICONTROL Workfront] のメイン領域へのリンクがあるアプリケーションの中央上のパネル。</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL 新しい数値 ]</td> 
   <td>[!UICONTROL ジャーナルエントリ ] レポートでは、[!UICONTROL 古い数値 ] に代わるフィールドの更新された値が表示されます。
   詳しくは、この記事の「[!UICONTROL 古い数値 ]」を参照してください。</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL 非稼働日 ]</td> 
   <td>割り当ての完了に割り当てられていない日。 通常は休日、休日、週末です。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL メモ ]</td> 
   <td>に対して行われたコメントまたは更新 [!DNL Workfront] オブジェクト。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL メモテキスト ]</td> 
   <td> <p>任意のオブジェクトに対してユーザーが入力した更新のテキストが表示されます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL リンクされた目標の数 ]</td> 
   <td> <p>[!UICONTROL プロジェクト ] レポートでは、これはプロジェクトに関連付けられている戦略目標の数です。 プロジェクトと戦略目標の関連付けについて詳しくは、 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">での目標へのプロジェクトの追加  [!DNL Adobe Workfront Goals]</a>.</p> 
   <p>戦略目標について詳しくは、この記事の「[!UICONTROL 目標 ]」も参照してください。</p> 
   <p>このフィールドは、組織が [!DNL Workfront Goals]. を使用した戦略目標の管理の詳細 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">[!UICONTROL Adobe Workfront Goals] の目標へのプロジェクトの追加</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL オブジェクト ]</td> 
   <td> <p>表示する情報 [!DNL Adobe Workfront] は、 [!DNL Workfront] データベース。 オブジェクトは、Workfrontの情報を動かすものです。 オブジェクトの例を次に示します。</p> 
    <ul> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL プログラム ]</li> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL タスク ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROL ドキュメント ]</li> 
     <li>[!UICONTROL ダッシュボード ]</li> 
     <li>[!UICONTROL レポート ]</li> 
     <li>[!UICONTROL グループ ]</li> 
     <li>[!UICONTROL チーム ]</li> 
     <li>[!UICONTROL ユーザー ]</li> 
     <li>[!UICONTROL 会社 ]</li> 
     <li>[!UICONTROL カスタムフォーム ]</li>
     <li>[!UICONTROL カスタムフィールド ]</li>  
     <li>[!UICONTROL 時間 ]</li> 
     <li>[!UICONTROL 請求率 ]</li> 
     <li>[!UICONTROL テンプレート ]</li> 
     <li>[!UICONTROL テンプレートタスク ]</li>

<p><b>メモ</b></p>
  <p>これは広範なリストではありません。 </p>

</ul> <p>詳しくは、 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">[!UICONTROL Adobe Workfront] のオブジェクトについて</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL オブジェクトタイプ ]</td> 
   <td>すべてのカスタムフォームを含むレポートまたはリストを作成する場合、このフィールドをビューまたはフィルターとして使用し、各フォームに関連付けられているオブジェクトの種類を確認できます。 </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL 古い数値 ]</td> 
   <td>[!UICONTROL ジャーナルエントリ ] レポートでは、更新前のフィールドの元の値が表示されます。 フィールドの値が更新されると、[!UICONTROL ジャーナルエントリ ] レポートに [!UICONTROL 新しい数値 ] と表示されます。 詳しくは、「[!UICONTROL 新しい数値 ]」も参照してください。</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL 変更のみ ]</td> 
   <td> <p>[!UICONTROL Project Update] タイプの 1 つ。 このオプションを選択すると、[!UICONTROL Project Project Projected] および [!UICONTROL Planned] タイムラインは、プロジェクトまたはプロジェクト内のタスクに対して更新または変更が行われた場合にのみ更新されます。 プロジェクトは毎晩更新されません。</p> <p>詳しくは、 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプを選択 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>[!UICONTROL Issue] の名前 ( [!DNL Workfront] データベース。テキストモードのレポートまたは計算済みのカスタムデータで使用されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 開く ]</td> 
   <td>未完了で作業中のイシューまたはタスク。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 組織図 ]</td> 
   <td>組織図の略称です。 組織の階層を示すグラフです。 また、[!UICONTROL ユーザー ] の詳細画面の「 」タブにも表示され、[!UICONTROL ユーザー ] の [!UICONTROL 会社 ] と [!UICONTROL レポート ] の関係を設定できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 組織の設定 ]</td> 
   <td>これにより、組織の [!UICONTROL 会社 ]、[!UICONTROL グループ ] および [!UICONTROL セキュリティプロファイル ] が定義されます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL その他のグループ ]</td> 
   <td> <p>ユーザーを一覧表示するレポートまたはビューで、このフィールドには各ユーザーがメンバーとなっているすべてのグループが表示されます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 通貨の上書き ]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL ジョブの役割 ] レポートでは、ジョブの役割に関連付けられている通貨を表します。 これは、[!UICONTROL Base Currency] の上書きです。これは、[!UICONTROL Setup] 領域で設定されているとおり、 [!DNL Workfront] 管理者。 </p> 
     <p>詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">ジョブの役割の作成と管理</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 通貨の請求/時間を上書き ]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL ジョブの役割 ] レポートでは、ジョブの役割の選択した [!UICONTROL 通貨の上書き ] を使用した、ジョブの役割の 1 時間あたりの請求率を表します。</p> 
     <p> 詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">ジョブの役割の作成と管理</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 通貨コスト/時間を上書き ]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL ジョブの役割 ] レポートでは、ジョブの役割の選択した [!UICONTROL 通貨の上書き ] を使用したジョブの役割の 1 時間あたりのコスト率を示します。 </p> 
     <p>詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">ジョブの役割の作成と管理</a>.</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 所有者 ]</td> 
   <td>指定されたオブジェクトの完了を担当するユーザー。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL 所有者タイプ ]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL 目標 ] レポートには、戦略目標に割り当てられている所有者のタイプが表示されます。 次に、目標所有者のタイプを示します。</p> 
     <ul> 
      <li> <p>[!UICONTROL ユーザー ]</p> </li> 
      <li> <p>[!UICONTROL チーム ] </p> </li> 
      <li> <p>[!UICONTROL グループ ]</p> </li> 
     </ul> 
     <p>目標所有者が組織の場合、このフィールドに値は表示されません。 </p> 
     <p>追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals] 概要</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## P - R

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>オブジェクト名</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL パラメーター ]</td> 
   <td> <p>[!UICONTROL パラメーター ] はカスタムフィールドです。 システム内のすべてのパラメーターまたはカスタムフィールドに関するレポートを作成できます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 親 ]</td> 
   <td>レポートで、このフィールドには、オブジェクトの親に関する情報が表示されます。 例えば、[!UICONTROL 問題 ] レポートでは、問題が記録されたタスクやプロジェクトに関する情報が表示され、タスクレポートでは直接親タスクやプロジェクトに関する情報が表示されます。 に親が含まれるオブジェクトの詳細 [!DNL Workfront]詳しくは、この記事の「オブジェクトの相互依存関係と階層」の節を参照してください。 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">でのオブジェクトについて [!DNL Adobe Workfront]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 親ラグ ]</td> 
   <td>[!UICONTROL 親タスク ] の開始から [!UICONTROL サブタスク ] の開始までの時間。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 親タスク ]</td> 
   <td>[!UICONTROL サマリタスク ] とも呼ばれます。 これはサブタスク（[!UICONTROL 子タスク ] とも呼ばれる）を持つタスクです。 親タスクの [!UICONTROL 期間 ]、[!UICONTROL 作業時間が必要 ] および [!UICONTROL 完了率 ] は、サブタスクから計算されます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL パートタイムリソース ]</td> 
   <td>システムで定義されたデフォルトのスケジュールより少ない容量を持つライセンスユーザー。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 完了率 ]</td> 
   <td> <p>タスク、プロジェクト、またはタスクに関連する作業の割合を示すプロジェクト、タスク、またはタスクのフィールド。</p> <p>問題や作業タスクについては、このフィールドを手動で更新できます。 </p> <p>プロジェクトおよび親タスクの場合、このフィールドはすべての作業タスクからのロールアップであり、手動で更新することはできません。 </p> <p>詳しくは、 <a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">プロジェクト [!UICONTROL 完了率 ] の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 権限 ]</td> 
   <td> <p>オブジェクトのユーザーに付与される権限。通常は、ユーザーが項目の作業を完了したり、項目を表示したりできるようにします。 次の権限を付与できます。</p> 
    <ul> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL タスク ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROLPortfolio]</li> 
     <li>[!UICONTROL プログラム ]</li> 
     <li>[!UICONTROL レポート ]</li> 
     <li>[!UICONTROL ダッシュボード ]</li> 
     <li>[!UICONTROL ドキュメント ]</li> 
     <li>[!UICONTROL カスタムForms]</li> 
     <li>[!UICONTROL 表示 ]</li> 
     <li>[!UICONTROL フィルター ]</li> 
     <li>[!UICONTROL グループ化 ]</li> 
    </ul> <p>詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">オブジェクトに対する共有権限の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プラン ]</td> 
   <td> <p>これは、 [!DNL Workfront] システム。 のすべての機能にアクセスするには、この権限が必要です。 [!DNL Workfront].</p> <p>詳しくは、 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] ライセンスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プラン ] ( [!DNL Scenario Planner])</td> 
   <td> <p>プランは、 [!DNL Workfront] シナリオプランナー。 近い将来および長期的な将来に向けた戦略の概要を示し、それぞれの大まかな成果を特定し、 [!DNL Workfront] シナリオプランナー。 </p> <p>表示できません [!DNL Scenario Planner] レポート内のプランの場合は、 [!DNL Workfront] API. </p> <p>The [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Scenario Planner] 概要</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>何かが発生するようにスケジュールされている時間枠。 でプロジェクト、タスクまたはイシューを作成する場合 [!DNL Workfront]を使用して、計画された開始日と終了日、およびそれらが発生する計画された期間を設定します。 これらの値は、項目の完了に要する時間の元の意図または推定を表します。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>これは、プロジェクトを完了すると組織に金銭上の利益がもたらされるかどうかを見積もるために、プロジェクトマネージャが手動で入力するものです。 この値の指定は、プロジェクトの [!UICONTROL ビジネスケース ] を組み立てる際に使用できます。 この値を更新するには、プロジェクトに対する [!UICONTROL 管理 ] 権限が必要です。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL 計画予算時間数 ]</td> 
   <td> <p>[!UICONTROL 予算時間 ] レポートでは、[!UICONTROL リソースプランナー ] のプロジェクトまたは [!UICONTROL ジョブロール ] に対して予算された時間数が表示されます。 </p> <p>[!UICONTROL Resource Planner] のプロジェクトまたはロールの予算作成の詳細は、この記事を参照してください <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">[!UICONTROL プロジェクト ] ビューと [!UICONTROL ロール ] ビューを使用した [!UICONTROL リソースプランナー ] の予算リソース</a>. [!UICONTROL Budgeted Hours] レポートの詳細については、この記事を参照してください <a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">レポート：予算時間</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 計画完了日 ]</td> 
   <td> <p>[!UICONTROL 計画完了日 ] は、手動で選択した日付に設定できます。 [!UICONTROL 計画完了日 ] を設定しない場合、 [!DNL Workfront] は自動的に設定します。 自動的に設定された場合、[!UICONTROL 計画完了日 ] は [!UICONTROL 計画開始日 ] + [!UICONTROL 期間 ] です。</p> <p>詳しくは、次の記事を参照してください。</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">タスク [!UICONTROL 計画完了日 ] の概要</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">プロジェクト [!UICONTROL 計画完了日 ] を設定</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 計画コスト ]</td> 
   <td> <p>プロジェクトの [!UICONTROL 計画労務費 ] と [!UICONTROL 計画費用 ] の合計。 これには、プロジェクトに [!UICONTROL 計画リスクコスト ] は含まれません。  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予定期間 ]</td> 
   <td> <p>タスクの [!UICONTROL 予定期間 ] は、通常、タスクの [!UICONTROL 期間 ] と同じです。 これは、タスクの [!UICONTROL 計画開始 ] と [!UICONTROL 計画完了日 ] の間の日数を表します。 </p> <p>タスクの [!UICONTROL 期間 ] タイプが [!UICONTROL 労力主導 ] の場合、[!UICONTROL 予定期間 ] は、タスクに割り当てたリソース数に基づいてタスクの [!UICONTROL 期間 ] と異なる場合があります。 </p> <p>例えば、[!UICONTROL 期間 ] タイプが [!UICONTROL 労力による ] のタスクの期間が 3 日間で、1 つのリソースをフルタイムスケジュールでタスクに割り当てた場合、[!UICONTROL 予定期間 ] も 3 日間になります。 3 つのリソースをフルタイムスケジュールで同じタスクに割り当てた場合、[!UICONTROL 期間 ] は 3 日間ですが、[!UICONTROL 予定期間 ] は 1 日になります。 [!UICONTROL 予定期間 ] では、新しい [!UICONTROL 予定期間 ] を反映するために、タスクの [!UICONTROL 予定開始 ] 日と [!UICONTROL 予定完了 ] 日も変更されます。 その結果、プロジェクトのタイムラインにも影響が及びます。 </p> <p>タスクの [!UICONTROL 期間 ] と [!UICONTROL 予定期間 ] の違いについて詳しくは、この記事を参照してください <a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">タスクの [!UICONTROL 予定期間 ] と [!UICONTROL 予定期間 ] の違い</a>.</p> <p>プロジェクトとイシューには [!UICONTROL 予定期間 ] がありません。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予定期間（分）]</td> 
   <td> <p>プロジェクトまたはイシューの [!UICONTROL 予定期間（分）] は、プロジェクトまたはイシューの [!UICONTROL 期間 ]（分）です。 </p> <p>タスクには [!UICONTROL 予定期間（分）] フィールドはありません。 </p> <p>[!UICONTROL テンプレートタスク ] には、[!UICONTROL 予定期間（分）] フィールドがあり、このフィールドにはタスクの [!UICONTROL 予定期間 ] が分単位で表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予定費用 ]</td> 
   <td> <p>プロジェクトまたはタスクでログに記録されたすべての費用の [!UICONTROL 計画金額 ] の合計。</p> <p><b>例</b></p>
   <p>タスク 1 の費用を作成し、「[!UICONTROL 計画金額 ]」フィールドに$600.00 と入力した場合、このタスクの [!UICONTROL 計画費用 ] は$600.00 になります。 </p> 
   <p>プロジェクトの場合、 [!DNL Workfront] では、次の式を使用して [!UICONTROL 計画費用 ] を計算します。</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予定時間数 ]</td> 
   <td> <p>このフィールドは [!UICONTROL Projects]、[!UICONTROL Tasks]、[!UICONTROL Tasks]、および [!UICONTROL Resource Planner]、[!UICONTROL Workload Balancer]、[!UICONTROL Utilization] レポートなどの問題領域、プロジェクト、タスク、タスク、問題管理ツールに表示されます。 </p> <p>プロジェクト所有者が、各タスクまたは問題が完了するまでに必要な時間数を示します。 プロジェクトの場合は、通常、これはプロジェクトのタスクからの [!UICONTROL 予定時間 ] の積み上げです。 </p> <p>[!UICONTROL 予定時間 ] フィールドには、表示元に応じて異なる情報が表示される場合があります。 予定時間については、 <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">計画時間の概要</a>.</p> <p>予定時間は、 [!DNL Workfront] データベース。 このフィールドを使用して計算を記述する場合は、時間が分単位で表示されることを考慮してください。<br></p> <p>デフォルトでは、計画時間は、作業項目の期間内のすべての日に均等に配分され、タスクに割り当てられたすべてのリソースにも均等に配分されます。 ユーザーは、作業項目の 1 日の計画時間数を更新したり、各担当者の個々の計画時間数を更新したりできます。</p> <p>このフィールドの更新は、プロジェクト、タスクおよび問題に対して異なります。 </p> 
    <ul> 
     <li> <p>問題が発生した場合は、このフィールドを手動で更新できます。 発行予定時間は、プロジェクト予定時間には追加されません。 </p> <p>ヒント：問題レポートでは、「[!UICONTROL 予定時間 ]」フィールドの 1 つが「[!UICONTROL 作業 ]」フィールドに置き換えられます。 「 」フィールドには、問題に関する計画時間数が表示されます。 詳しくは、この表の「作業」フィールドまたは「[!UICONTROL 作業 ]」フィールドを参照してください。 </p> </li> 
    </ul> 
    <ul> 
     <li> <p>タスクの場合、タスクの [!UICONTROL 期間タイプ ] が [!UICONTROL 計算割り当て ] または [!UICONTROL シンプル ] の場合は、このフィールドを手動で更新できます。 このフィールドは [!DNL Workfront] タスクの [!UICONTROL 期間タイプ ] が [!UICONTROL 計算作業時間 ] または [!UICONTROL 労力に基づく ] の場合。<br>[!UICONTROL タスク期間 ] について詳しくは、 <a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク [!UICONTROL 期間 ] と [!UICONTROL 期間タイプ ] の概要</a>.</p> </li> 
    </ul> 
    <ul> 
     <li> <p>プロジェクトの場合、 [!DNL Workfront] プロジェクトのすべてのタスクからすべての計画時間を追加して、計画時間を計算します。 </p> </li> 
    </ul> <p><b>ヒント</b></p> <p>[!UICONTROL 予定時間 ] を [!UICONTROL プロジェクト ]、[!UICONTROL タスク ]、または [!UICONTROL タスク ] のレポートに表示するには、テキストモードを使用し、追加のフィールドを参照します。 詳しくは、<code>work</code>"、"[!UICONTROL Work]"および"<code>workRequiredExpression</code>」フィールドが含まれています。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 計画労務費 ]</td> 
   <td> 
    <p>タスクの場合、ユーザーまたはロールの時間単価に、ユーザーまたはロールに割り当てられた時間数を掛けた値です。</p> <p>プロジェクトの場合、すべてのタスクの [!UICONTROL 計画労務費 ] の合計です。</p> <p>ユーザーまたは役割の割合が使用されるかどうかは、特定のタスクに対して選択されたコストの種類によって異なります。 </p> <p>詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md">コストの追跡</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予定収益 ]</td> 
   <td> <p>タスクおよびプロジェクトでは、[!UICONTROL 計画売上高 ] の値を [!DNL Workfront]. [!UICONTROL 計画収益 ] は、プロジェクト上のタスクの [!UICONTROL 計画時間 ] に関連する金額を表します。 プロジェクトの場合は、プロジェクトの [!UICONTROL 固定売上高 ] も含めることができます。 </p> <p>タスクの場合は、これは [!UICONTROL 予定時間 ] タスクに関連する売上高です。 すべてのタスクから計画時間は、プロジェクトの計画時間にロールアップされ、プロジェクト [!UICONTROL 計画時間 ] の計算に役立ちます。 </p> 
   <p>[!DNL Workfront] 次の式を使用して、タスクおよびプロジェクトの [!UICONTROL 計画収益 ] を計算します。</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>[!UICONTROL プロジェクトの詳細 ] 領域とプロジェクトレポートに表示されるプロジェクト [!UICONTROL 計画収益 ] は、[!UICONTROL 使用率 ] レポートに表示される計画収益とは異なります。 </p> <p>[!UICONTROL プロジェクトの詳細 ] 領域の [!UICONTROL 計画売上高 ] には、タスクの売上高とプロジェクトの固定売上高が反映されます。 [!UICONTROL 使用率レポート ] の [!UICONTROL 計画収益 ] には、プロジェクト内のタスクにのみ関連付けられた [!UICONTROL 計画収益 ] が表示されます。 </p> 
     <p><b>例</b></p>  
      <p>プロジェクトに 10 時間のタスクが 1 つあり、時間単価が$20 のコンサルタントに割り当てられ、プロジェクトに$100 の [!UICONTROL 固定売上高 ] がある場合、[!UICONTROL 使用率 ] レポートには時間に関連付けられた [!UICONTROL 予定売上高 ] に$200 が表示されますタスク )。 [!UICONTROL プロジェクトの詳細 ] セクションには、タスクからの$300（[!UICONTROL 計画売上高 ] およびプロジェクトの固定売上高）が表示されます。 </p> 
    <p>での売上高の追跡について詳しくは、 [!DNL Workfront] 参照 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">請求と売上高の概要</a>. </p> 
    <p>[!UICONTROL 使用率レポート ] での [!UICONTROL 予定収益 ] の計算について詳しくは、 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">リソース使用率情報の表示 </a>. </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 計画リスクコスト ]</td> 
   <td> <p>発生の確率を組み込んだ、プロジェクト上のすべてのリスクの [!UICONTROL 潜在的なコスト ] の合計。 この金額は、プロジェクトの [!UICONTROL 計画コスト ] には含まれません。</p> <p>プロジェクトの [!UICONTROL 計画リスクコスト ] は、次の式で計算されます。</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ポータルプロファイル ]</td> 
   <td>管理者が定義した、タブとポータルセクションの集まりで、 [!DNL Workfront] [!UICONTROL Home] およびその他のダッシュボード。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ポータルセクション ]</td> 
   <td>ダッシュボードまたはポータルページ上のタブの 1 つのコンポーネント。 通常は、単一のレポート、グラフ、カレンダー、または主要な情報のリストです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ポータルタブ ]</td> 
   <td>ポータルまたはダッシュボードのタブで、最大 3 つのポータルセクションを含む。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROLPortfolio]</td> 
   <td> <p>統一された特性を持つプロジェクトのコレクションです。 これらのプロジェクトは通常、同じリソース、予算、または時間帯を競い合います。 Portfolioをプログラムに分割し、Portfolioに追加する前にプロジェクトをプログラムに関連付けることができます。</p> <p>ポートフォリオについて詳しくは、 <a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">Portfolioの概要： [!DNL Adobe Workfront]</a>.</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio管理 ]</td> 
   <td>コレクションや関連するプログラムの管理、およびプロジェクトの取り組みに重点を置いたプラクティス領域。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio最適化 ]</td> 
   <td>A [!DNL Workfront] ポートフォリオ内のプロジェクトの評価と優先順位付けを支援するツール。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROLPortfolio所有者 ]</td> 
   <td>ポートフォリオの優先順位付けと予算を担当する関係者。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 潜在的なリスクコスト ]</td> 
   <td>これは、リストおよびレポートで見つけることができるプロジェクトフィールドです。 このリストには、プロジェクトに関連するリスクが発生した場合に発生する可能性のあるコストが示されます。 詳しくは、 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">潜在的なリスクコストの計算 </a>. </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 前任者 ]</td> 
   <td> <p>依存タスクの完了前に完了する必要があるタスク。 別のタスクの [!UICONTROL 依存関係 ] としてマークされたタスク。 先行タスクを使用すると、プランナーは、別のタスクが終了した後にタスクを開始するなど、順序依存ロジックを設定できます。</p> <p>詳しくは、 <a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">タスクの先行タスクの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLプライマリ会社 ]</td> 
   <td>ユーザー設定で指定された、ユーザーが属する会社。 会社をプロジェクトに関連付けることもできます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLプライマリ連絡先 ]</td> 
   <td><p>[!UICONTROLプライマリ連絡先 ] はイシューの作成者で、自動的に [!DNL Workfront] 誰かが問題を作成したとき。 次の場合は、手動でこのフィールドを更新できます： [!DNL Manage] 権限を問題に割り当てます。 1 つの問題に設定できるプライマリ連絡先は 1 つだけです。</p> 
   <p>プライマリの連絡先を変更した場合、元々プライマリー連絡先として指定されていたユーザーは、引き続き問題に対する [!UICONTROL 管理 ] アクセス権を持ちます。</p>
   <p>イシューをタスクまたはプロジェクトに変換する場合、の [!UICONTROLプライマリ連絡先 ] として指定されたユーザーが、プロジェクトまたはタスクの [!UICONTROL 変換後のイシュー作成者 ] になります。 問題の [!UICONTROLプライマリ連絡先 ] が問題の変換後に更新された場合、[!UICONTROL 変換された問題作成者 ] は、変換が発生した時点で問題の [!UICONTROLプライマリ連絡先 ] として保持されます。 この記事の「[!UICONTROL 変換された問題の作成者 ]」も参照してください。</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL 優先度 ]</td> 
   <td>タスク、イシューまたはプロジェクトに割り当てて、その重要度を指定できる値です。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プライベート ]</td> 
   <td>[!UICONTROL メモ ] または [!UICONTROL ドキュメント ] では、このオプションを使用すると、ほとんどのビューアでそのオブジェクトが非表示になります。 プライベートヘルプデスクキューの場合、[!UICONTROL ヘルプデスク ] エリアを通じて、キューチームのユーザーのみがそのキューに問題を送信できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロファイル ]</td> 
   <td>ユーザーアカウントに関するすべての情報。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL プログラム ]</td> 
   <td> <p>ポートフォリオ内のサブセット。同様のプロジェクトをグループ化して、明確に定義されたメリットを実現できます。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL プログラム管理 ]</td> 
   <td>プロジェクト間の依存関係、リスク、問題、要件、およびソリューションの管理により、プログラムの健全性を維持し、定義済みのプログラムのメリットを実現します。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL プログラム所有者 ]</td> 
   <td>プロジェクト目標が会社の目標に合致するように、アクティビティの監督および編成を担当する関係者。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>[!UICONTROL 目標 ] レポートには、戦略目標が完了にどの程度近いかに関する割合が表示されます。 進行状況の割合は数値で表示されます。 戦略目標の詳細については、この表の「[!UICONTROL 目標 ]」も参照してください。</p> <p>このフィールドは、組織が [!DNL Workfront] 目標。 を使用した戦略目標の管理の詳細 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md"> での目標へのプロジェクトの追加 [!DNL Adobe Workfront Goals] </a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 進行状況ステータス ]</td> 
   <td> <p>このフィールドには、プロジェクト、タスク、目標の進捗状況ステータスが表示されます。 詳しくは、次の記事を参照してください。</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">プロジェクトの進行状況ステータスの概要</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">タスクの進捗状況ステータスの概要</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">の目標進行状況と条件の概要 [!DNL Adobe Workfront Goals]</a> </p>
     <p>[!UICONTROL 目標 ] レポートと [!UICONTROL 進捗状況ステータス ] [!DNL goals] フィールドは、組織が [!DNL Workfront Goals]. での戦略目標の詳細 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概要</a>. </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>特定の期間内に完了する必要があり、特定の予算とリソース数を使用する必要がある大量の作業。 管理しやすいように、プロジェクトを一連のタスクに分割します。 すべてのタスクを完了すると、プロジェクトが完了します。 プロジェクトの計画については、 <a href="../../../manage-work/projects/planning-a-project/plan-project.md">プロジェクトの概要の計画</a>.</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクト割り当て予定時間数 ]</td> 
   <td> <p>[!UICONTROL イニシアチブジョブの役割 ] レポートでは、プロジェクトのタスクまたは問題に割り当てられたジョブの役割に関連する [!UICONTROL 予定時間 ] の数が表示されます。 このフィールドと [!UICONTROL Initiative Job Role] レポートタイプは、 [!DNL Workfront] インスタンス（会社がを購入していない場合） [!DNL Workfront Scenario Planner] ライセンス。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md">The [!DNL Workfront Scenario Planner] 概要</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクトの詳細 ]</td> 
   <td>プロジェクトの現在のステータスの詳細。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクトの予算コスト ]</td> 
   <td> <p> これは、リストおよびレポートに表示されるプロジェクトの [!UICONTROL 予算コスト ] です。</p><p>この記事の「[!UICONTROL 予算コスト ]」も参照してください。</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL プロジェクト管理 ]</td> 
   <td>プロジェクトの作成、分類、名前付けのしきい値を管理する一連のポリシー。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL プロジェクトのオーバーヘッド ]</td> 
   <td>[!UICONTROL 時間 ] レポートでは、このフィールドは [!UICONTROL プロジェクト時間 ] の時間タイプでログに記録された時間に関連する財務情報用に予約されます。 プロジェクトには独自の請求率を設定でき、1 時間がプロジェクトに直接記録された場合、それらの率は計算に使用されます。 プロジェクトの設定に基づいて、プロジェクトに異なる通貨を設定することもでき、その時間の通貨換算が可能です。 [!UICONTROL Project Overhead] オブジェクトを使用すると、 [!DNL Workfront] その情報を得るために</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクト所有者 ]</td> 
   <td>プロジェクトの範囲、タイムライン、割り当てを管理するユーザー。 変更管理、財務上の変更、成果物に対するデフォルトの承認者。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>プロジェクトスケジュールを作成および管理するプロセスです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクトスポンサー ]</td> 
   <td>各ユーザーが関連付ける必要がある指定された関係者のプロファイル。 In [!DNL Workfront]（これらは [!UICONTROL アクセスレベル ] として指定されます）</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクトチーム ]</td> 
   <td> <p>プロジェクトに割り当てられたユーザーまたは役割のコレクション</p> <p>詳しくは、 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">プロジェクトチームの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクトトラッキング ]</td> 
   <td>プロジェクトの正常性と範囲の測定に使用されるデータ</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>タスク、問題、またはプロジェクトの予定時間と完了率に基づく、作業が完了する時点のタイムスタンプの推定値です。</p> <p>これは、日付、またはタスク、タスク、タスクまたはプロジェクトの [!UICONTROL 期間 ] を指します。 通常は、ある作業が既に完了しているか、ある時間が経過した後で、作業項目の寿命に近い日付と期間を指定します。 </p> <p>例えば、タスクの [!UICONTROL Projected Completion Date] は [!DNL Workfront] は、タスクに対して行われた作業量、割り当てられた担当者数、開始日以降に経過した時間に基づいて、タスクが完了すると予測します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認の期限 ]</td> 
   <td> <p>[!UICONTROL ドキュメントのバージョン ] オブジェクト（[!UICONTROL ドキュメントのバージョン ] レポートや [!UICONTROL 配達確認の承認 ] レポートなど）が含まれるレポートでは、このフィールドに配達確認の期限の曜日、日付、時刻および年が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認の決定 ]</td> 
   <td> <p>[!UICONTROL ドキュメントのバージョン ] オブジェクト（[!UICONTROL ドキュメントのバージョン ] レポートや [!UICONTROL 配達確認の承認 ] レポートなど）を含むレポートで、このフィールドに配達確認の決定ステータス（保留中、必要な変更、承認済み）が表示されます</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認名 ]</td> 
   <td> <p>[!UICONTROL ドキュメントのバージョン ] オブジェクト（[!UICONTROL ドキュメントのバージョン ] レポートや [!UICONTROL 配達確認の承認 ] レポートなど）を含むレポートでは、このフィールドに配達確認の名前が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認ページ ]</td> 
   <td> <p>[!UICONTROL ドキュメントのバージョン ] オブジェクト（[!UICONTROL ドキュメントのバージョン ] レポートや [!UICONTROL 配達確認の承認 ] レポートなど）を含むレポートで、このフィールドに配達確認に含まれるページ数が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 配達確認の進行状況 ]</td> 
   <td> <p>[!UICONTROL ドキュメントのバージョン ] オブジェクト（[!UICONTROL ドキュメントのバージョン ] レポートや [!UICONTROL 配達確認の承認 ] レポートなど）を含むレポートで、配達確認の進行状況ステータスを表示します（[!UICONTROL 送信済み ]、[!UICONTROL 開封済み ]、[!UICONTROL コメント済み ]、[!UICONTROL 決定がおこなわれました ]）。</p> <p>詳しくは、 <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">配達確認の進行状況の概要</a> in <a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">配達確認の進行状況とステータスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 校正 ]</td> 
   <td>1 人または複数のユーザーが、画像、テキストドキュメント、ビデオまたはインタラクティブ Web コンテンツ内で変更するコンテンツに対してマークおよびコメントを付けるレビュープロセスです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL パブリック ]</td> 
   <td>[!UICONTROL メモ ] または [!UICONTROL ドキュメント ] で、このオプションを使用すると、他のユーザーや外部のユーザーがそのオブジェクトにアクセスできるようになります [!DNL Workfront]. [!UICONTROL ヘルプデスクキュー ] の場合、[!UICONTROL 公開 ] は、問題を送信できるすべてのユーザーが [!UICONTROL ヘルプデスク ] 領域を通じて問題を送信できることを意味します。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 品質 ]</td> 
   <td>組織内の仕事の質の認識。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL キュー ]</td> 
   <td>「[!UICONTROL Help Desk Queue]」とも呼ばれる。 これは、ユーザーが問題を送信できるように、[!UICONTROL ヘルプデスク ] 領域に公開されたプロジェクトです。 通常、キューは、バグ、プロジェクトリクエストなどの特定のトピックに対して作成されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL キューのプロパティ ]</td> 
   <td>これらの設定は、[!UICONTROL ヘルプデスク ] に公開されるプロジェクトの問題送信ルールを定義します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL キュートピック ]</td> 
   <td> <p>ユーザーが問題を送信してトピックを選択できる、[!UICONTROL Help Desk Queue] 上のプロパティ。 トピックでは、次のことが可能です。</p> 
    <ul> 
     <li>カスタムデータフォームに関連付ける。</li> 
     <li>選択したトピックに設定されたルーティング規則を使用して、問題をユーザー、役割、またはチームに自動的に割り当てます。</li> 
     <li>選択したトピックに設定されたルーティングルールを使用して、問題を別のプロジェクトまたはキューに移動します。</li> 
    </ul> <p>詳しくは、 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">キュートピックを作成</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ランク ]</td> 
   <td> <p>[!UICONTROL アクセスレベル ] レポートでは、[!UICONTROL アクセスレベル ] の [!UICONTROL ランク ] を手動で指定できます。 これは、 [!DNL Workfront] 管理者：各アクセスレベルに関連付けられている複雑さのレベルを視覚的に識別します。 例えば、より複雑な（[!UICONTROL プラン ] レベルの）アクセスレベルには小さい数値を指定し、より複雑でない（[!UICONTROL リクエスター ] レベルの）アクセスレベルには大きい数値を指定できます。 標準アクセスレベルのランク付けはできません。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 準備完了 ]</td> 
   <td> <p>タスクレポートのこのフィールドは、バックログで [!UICONTROL Agile] タスクが [!UICONTROL 準備完了 ] とマークされたかどうかを示します。 このフラグは [!UICONTROL Agile] タスク（[!UICONTROL Agile] チームに割り当てられたタスク）にのみ適用されます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL 繰り返し頻度 ]</td> 
   <td> <p>繰り返しタスクの親の [!UICONTROL タスクの詳細 ] または [!UICONTROL タスクの編集 ] ボックスに表示されるフィールドです。 繰り返しのタスクが発生する頻度です。 繰り返しタスクの作成について詳しくは、 <a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">繰り返しタスクの作成</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 参照番号 ]</td> 
   <td> <p>プロジェクト、タスクおよびタスクは、作成時に自動的に一意の参照番号に関連付けられます。 [!UICONTROL 参照番号 ] は、プロジェクト、タスク、問題の [!UICONTROL 詳細 ] ページ、またはリストやレポートで表示できます。 </p> <p><b>ヒント</b><p><br>参照番号は常に一意なので、2 つの項目が同じ名前の場合は、参照番号に従うことができます。 </p> <p>[!DNL Workfront] は、システムレベルで順次参照番号を自動的に生成します。 各プロジェクト、タスクまたはイシューは、シーケンス内で次に使用可能な番号を取得します。 <br></p> <p>例えば、ユーザー A がタスクを作成した場合、 [!DNL Workfront] は、タスクに「参照番号」(100) を自動的に割り当てる場合があります。 その直後にユーザー B が問題を作成した場合は、 [!DNL Workfront] 問題に 101 の参照番号を割り当てます。 参照番号は手動で編集できません。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 却下の問題 ]</td> 
   <td>プロジェクトまたはタスクレポートでは、これは、プロジェクトまたはタスクの承認が却下されたときに作成される問題です。 却下の問題について詳しくは、 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業項目の承認プロセスの作成</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 残りリスクコスト ]</td> 
   <td> <p>プロジェクトの [!UICONTROL 計画リスクコスト ] と、プロジェクトのすべてのリスクのすべての [!UICONTROL 実績コスト ] の合計との差を示すプロジェクトフィールド。 </p> <p>プロジェクトの [!UICONTROL 残りリスクコスト ] は、次の式を使用して計算されます。</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 再計画 ]</td> 
   <td>問題を修復または克服するためにプロジェクトの日付を変更する。 例えば、正確な日付を反映させるために、数ヶ月間保留状態のプロジェクトを再計画する必要があります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レポート ]</td> 
   <td>指定した 1 つに関する情報を含むグラフまたはテーブル [!DNL Workfront] オブジェクトとその関連属性。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL リクエスト ]</td> 
   <td> <p>単一の一元化されたキューでトリアージされ、進行中の作業とは無関係な問題の一種。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL リクエストキュー ]</td> 
   <td>トラフィックとトリエージのプロセスで管理される問題のバックログです。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL リクエストベロシティ ]</td> 
   <td>リクエストを取り込み、完了するまでの合計作業サイクル時間。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL リクエスター ]</td> 
   <td>通常は、ライセンスの種類です。 リクエスターライセンスを持つユーザーは、システム内で発生する新しい作業のリクエストを送信できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予約時間 ]</td> 
   <td>ユーザーの個人時間に指定された日数。ユーザーが作業に使用できなくなることを示します。 「[!UICONTROL 非稼働日数 ]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 問題の解決 ]</td> 
   <td> <p>問題レポートでは、このフィールドを表示またはフィルターで使用して、問題を解決する問題を参照します。 </p> <p>レポートでのオブジェクトの解決方法について詳しくは、 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">レポート内での解決可能なオブジェクト情報の表示と解決</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">オブジェクトの解決と解決の概要 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロジェクトを解決 ]</td> 
   <td> <p>問題レポートでは、このフィールドを表示またはフィルターで使用して、問題を解決するプロジェクトを参照します。 </p> <p>レポートでのオブジェクトの解決方法について詳しくは、 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">レポート内での解決可能なオブジェクト情報の表示と解決</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">オブジェクトの解決と解決の概要 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タスクを解決 ]</td> 
   <td> <p>問題レポートでは、このフィールドを表示またはフィルターで使用して、問題を解決するタスクを参照します。 </p> <p>レポートでのオブジェクトの解決方法について詳しくは、 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">レポート内での解決可能なオブジェクト情報の表示と解決</a> in <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">オブジェクトの解決と解決の概要 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL リソース ]</td> 
   <td>システム内に存在し、プロジェクトチームやタスクに割り当てられたユーザーやロール。</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL リソース管理 ]</td> 
   <td> <p>[!UICONTROL Resource Management] は、使用可能な状況に基づいてリソースの使用状況を正確に予測し、作業を予定どおりに予算通りに完了させるための一連のツールです。 </p> <p>リソース管理ツールを使用すると、リソースの長期的な容量と短期的なスケジューリングのニーズを計画できます。 </p> <p>でのリソース管理の詳細 [!DNL Workfront]を参照してください。 <a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">リソース管理の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager ID]</td> 
   <td><p>プロジェクトレポートでは、フィルターを作成して特定のリソースマネージャーを検索する際に、このオプションを使用できます。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL リソースマネージャー ]</td> 
   <td> <p>プロジェクトレポートまたはリスト表示では、これは、プロジェクトでリソース管理アクティビティを実行するように指定されたユーザーを表示する情報フィールドです。  レポートで「[!UICONTROL リソースマネージャー ]」を使用すると、プロジェクト上の各リソースマネージャーがコンマで区切られた状態で、リソースマネージャーのリストが表示されます。 特定のプロジェクトに対して、最大 30 人のリソースマネージャを指定できます。</p> <p>詳しくは、 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">プロジェクトまたはテンプレートに対するリソースマネージャの指定 </a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL リソースプランナーの予算時間数 ] </td> 
   <td>[!UICONTROL リソースプランナー ] でプロジェクトに予算された時間と、プロジェクトに関連付けられたリソース。 この記事の「[!UICONTROL Budgeted Hours]」も参照してください。 </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL リソースプランナー ] </td> 
   <td>上級者 [!DNL Workfront] プロジェクト、ジョブの役割、ユーザーをまたいでリソースを表示および管理できるツール。 詳しくは、 <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">リソースプランナーの概要</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL リソースプランナーの予算労務費 ]</td> 
   <td> <p>これらは、リソース・プランナを使用して、プロジェクト・ジョブ・ロールに予算された時間に関連する原価です。 </p> <p>この記事の「予算労務費」も参照してください。 </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL リソースプール ]</td> 
   <td> <p>資源プールは、プロジェクトに関連付けることができるユーザーの集まりです。同じ資源プール内のユーザーは、通常同じ部門に属し、同じスキルや補完的なスキルを持っているか、同じ予算で資金が提供されます。 複数のリソースプールをプロジェクトまたはユーザーに関連付けることができます。 リソースプールは、プロジェクトにのみ割り当てることも、複数のプロジェクトで共有することもできます。</p> 
   <p>リソースプールの詳細については、「 <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> リソースプールの概要 </a>.</p> 
   <p>プロジェクトレポートでは、リソースプールには、プロジェクトに関連付けられているすべてのプールが表示されます。 このオブジェクトはグループ化で使用できません。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL リソース使用率 ]</td> 
   <td>レポート：特定の期間内に利用可能な時間数と、レポート内の各ユーザーに対して予定されている時間数を表示します。 また、[!UICONTROL Average Hours Per Day] と配分率にも計算されます。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL 結果 ]</td> 
   <td>In [!DNL Workfront Goals]の場合、結果は目標の進行状況インジケーターです。 手動で更新する数値、割合値、または通貨金額を指定できます。 結果をレポートに表示することはできません。また、 [!DNL Workfront] API. アクティビティについて詳しくは、 <a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront目標の結果とアクティビティの概要</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL 売上高 ]</td> 
   <td>タスクまたはプロジェクトの請求可能な金額。 金額は、1 時間ごと、固定額またはその両方を組み合わせて指定できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 売上高タイプ ]</td> 
   <td>売上高タイプは、タスクが売上高を生み出す方法を決定します。 例としては、[!UICONTROL 固定時間別 ]、[!UICONTROL 役割時間別 ]、[!UICONTROL 役割時間別（Cap を含む）] などがあります。 での売上高の追跡について詳しくは、 [!DNL Workfront] 参照 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と売上高の概要</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レビュー担当者 ]</td> 
   <td>通常は、ライセンスの種類です。 [!UICONTROL Reviewer] ライセンスを持つユーザーは、システム内の作業項目を確認し、承認できます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL リスク ]</td> 
   <td> <p>これは、 [!DNL Workfront]:</p> 
    <ul> 
     <li> <p>プロジェクトのリスクを示すフィールド。 リスクのレベルに基づいて、プロジェクトの実行を優先順位付けできます。 プロジェクトには次のようなリスクレベルがあります。</p> <p>- [!UICONTROL 非常に低い ]</p> <p>- [!UICONTROL 低 ]</p> <p>- [!UICONTROL メディア ]</p> <p>- [!UICONTROL 高 ]</p> <p>- [!UICONTROL 非常に高い ]</p> <p>プロジェクトに対して示すリスクのレベルはカスタマイズできません。 </p> <p> プロジェクトのリスクを更新する方法については、この記事の「プロジェクト設定」の節を参照してください <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">プロジェクトを編集</a>. レポートでプロジェクトのリスクフィールドを表示できます。 </p> </li> 
     <li> <p>プロジェクトの存続中に発生する可能性のあるイベントで、プロジェクトのコスト、範囲、スケジュールに対する潜在的な影響を識別します。 プロジェクトに潜在的なリスクを定義し、プロジェクトのビジネスケースを構築する際に、そのリスクが発生する確率またはコストを関連付けます。 プロジェクトのビジネス事例にリスクを追加する方法については、「プロジェクトのリスクを作成および編集する」を参照してください。 </p> <p>[!UICONTROL ビジネスケース ] で定義されたリスクをレポートに表示することはできません。 レポートとリストには、複数のタイプのリスクコストのみを表示できます。 </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL リスクコスト ]</td> 
   <td> <p>プロジェクトのリスクに関連するコスト。 レポートに表示できるプロジェクトに関連するリスクコストは次のとおりです。</p> 
    <ul> 
     <li> <p>[!UICONTROL 実際のコスト ]：発生したリスクの実際のコストを示す、リスクのフィールド。 レポートやリストに加えて、リスクを編集または作成する際に [!UICONTROL リスクを編集 ] ボックスでそのリスクを探すことができます。 </p> <p>プロジェクト、タスクまたはタスクのコストについては、この記事の「[!UICONTROL 実際のコスト ]」を参照してください。 </p> </li> 
     <li> <p>[!UICONTROL 計画リスクコスト ]：プロジェクトのすべての [!UICONTROL 潜在的リスクコスト ] の合計を表示する、プロジェクト上のフィールド。 この記事の「[!UICONTROL 計画リスクコスト ]」も参照してください。 </p> <p>潜在的なリスクコストの詳細は、 <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">潜在的なリスクコストの計算 </a>. </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost]：すべてのリスクの [!UICONTROL Actual Costs] の合計と [!UICONTROL Planned Risk Cost] の差を表示する、プロジェクト上のフィールド。 この記事の「残りのリスクコスト」も参照してください。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL リスク管理 ]</td> 
   <td>リスクを特定、軽減、および監視するプロセス。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ロール ]</td> 
   <td>この記事の「[!UICONTROL ジョブの役割 ]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>問題の自動割り当てまたは移動 ( 通常は、キューのトピックまたはキューのデフォルトルート（ルーティングルール）となる方法による )。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ルーティングルール ]</td> 
   <td>ユーザー、ロール、またはチームに問題を自動的に割り当てたり、別のプロジェクトまたはキューに問題を移動したりする、プロジェクトとキューに関する設定。 ルーティングルールは、通常、受信する問題を自動的に割り当てるためにヘルプデスクキューで使用されます。</td> 
  </tr> 
 </tbody> 
</table>

## S - U

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>オブジェクト名</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 保存済みの検索結果 ]</td> 
   <td>検索条件が保存されている検索条件。 保存済みの検索結果を使用すると、検索条件を再入力しなくても、再度同じ操作を簡単に実行できます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL シナリオ ] ( [!DNL Workfront Fusion]) </td> 
   <td> <p>シナリオは、アプリやサービス間でデータを転送および変換する方法を示す一連の手順（モジュール）で構成されます。</p> <p>のシナリオについて詳しくは、 [!DNL Workfront Fusion]を参照してください。 <a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] シナリオの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シナリオ ] ( [!DNL Workfront Scenario Planner]) </td> 
   <td> <p>Adobe Analytics の [!DNL Scenario Planner]シナリオは、プランのコピーです。 </p> <p>The [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The [!DNL Scenario Planner] 概要</a>. </p> <p>シナリオの作成について詳しくは、 <a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">でのプランシナリオの作成と比較 [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スケジュール ]</td> 
   <td>週別の作業スケジュール（勤務時間を含む）と、休日（休日など）および例外日（土曜日の作業日など）を組み合わせたもの。 スケジュールは、プロジェクトとユーザーに適用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スケジュールの除外 ]</td> 
   <td>[!UICONTROL 変更済みシフト ] とも呼ばれます。 スケジュールで定義されている、通常の週別作業時間とは異なる、スケジュールされた日数。 例えば、土曜日が機能するようにスケジュールを設定した場合、月曜日から金曜日までの作業のみがスケジュールに設定されていると、[!UICONTROL スケジュールの適用除外 ] となります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 予定レポート ]</td> 
   <td> <p>レポートのレポートを作成する際に [!UICONTROL 予定レポート ] フィールドを使用してレポートの配信が予定されている場合は、レポートのスケジュールに関する情報を表示できます。 このフィールドには、レポートの各スケジュールに対して 1 つずつ、複数の値が箇条書きリストで表示されます。 レポートのスケジュール設定について詳しくは、この記事を参照してください。 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">レポート配信の概要</a>.</p> <p>このフィールドには複数の値が表示されるので、1 つのグループ化で使用することはできません。 フィルターまたはビューでのみアクセスできます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スコープの変更 ]</td> 
   <td>[!UICONTROL 監査証跡 ]。アクティブな場合、[!UICONTROL タスク期間 ] や [!UICONTROL 先行タスク ] が変更された場合など、プロジェクトまたはタスクの範囲に変更が加えられるたびにメモを生成します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL セクション ]</td> 
   <td>表示目的でカスタムデータを整理するために作成された、画面上の独自のヘッダーを持つ領域。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL セクション区切り ]</td> 
   <td>セクション間のギャップまたは境界。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL セキュリティ ]</td> 
   <td>ユーザーがシステム内の特定のオブジェクトを操作し、他のオブジェクトを操作できるようにする設定です。 この記事の「[!UICONTROL アクセスレベル ]」も参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 設定 ]</td> 
   <td>管理者がシステム設定と環境設定を行える領域。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 重大度 ]</td> 
   <td> <p>[!UICONTROL 重大度 ] は、作業の完了に対する項目の影響の可能性を示します。 例えば、重大度が高い問題は、タスクの完了を完全にブロックする可能性がありますが、重大度が低い問題は、単に表面的なものに過ぎません。</p> <p>詳しくは、 <a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref"> 問題の重大度を更新</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 重大度 ]</td> 
   <td>この記事の「[!UICONTROL 重大度 ]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 共有 ]</td> 
   <td>他のユーザーに特定の項目の表示または編集を許可するアクション [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLSlack日 ]</td> 
   <td>タスクビューまたはレポートでは、[!UICONTROLSlack日 ] は、タスクがプロジェクトの [!UICONTROL 完了日 ] に確実に影響を与える可能性がある正確な日付を表示します。 タスクの [!UICONTROLSlack日 ] について詳しくは、 <a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">タスクSlack日の概要</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スマート割り当て ]</td> 
   <td> <p>ユーザーにタスクまたは問題を割り当てる場合、 [!DNL Workfront] は、作業の完了に最適なユーザーとプロジェクトとの関係に基づいて、誰が作業を完了するかに関するレコメンデーション（[!UICONTROL スマート割り当て ]）をおこないます。</p> <p>詳しくは、 <a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">スマート割り当ての概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソース ]</td> 
   <td> <p>別のオブジェクトの親オブジェクトを示します。 例えば、タスクに添付されたドキュメントは [!UICONTROL Document] レポートまたはビューの [!UICONTROL Source] フィールドにタスクの名前を持ち、プロジェクトの下に記録されたイシューはイシューレポートまたはビューの [!UICONTROL Source] フィールドにプロジェクトの名前を持ちます。 </p> 
   <p>次のレポートには、親オブジェクトに関する情報を表示できる「ソース」列が表示されます。</p>
  <ul><li>問題レポート</li>
    <li>時間レポート</li>
    <li>ドキュメントレポート </li>
    </ul>
   <p>問題、時間、ドキュメントの親オブジェクトに対する権限をユーザーが持っていない場合、レポートが表示するように設定されている場合や、別のユーザーのアクセス権を持って配信される場合でも、レポートの「ソース」列には空白が表示されます。 </p>
   <p> レポートに親オブジェクトに関する情報を表示するには、親オブジェクトに列を追加して、親の名前を表示することをお勧めします。 </p>
    <p>例えば、次のいずれかをソース列を含むレポートに追加できます。 </p>
    <ul><li>プロジェクト名、タスク名、または問題名の列をドキュメントまたは時間レポートに適用します。</li>
    <li>[ プロジェクト名 ] 列または [ タスク名 ] 列を発行レポートに追加します。 </li> </ul>
    詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">別のユーザーのアクセス権を持つレポートの実行と配信</a>

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 開始日 ]</td> 
   <td> <p>項目の作業を開始するように設定された日付。 開始日は、 [!DNL Workfront]: </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL 実際 ]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>[!UICONTROL レートレポート ] では、プロジェクトレベルでのジョブの役割に対する新しい請求率が開始した日付です。 この日付以降のプロジェクトに関連する時間にこの請求率を掛けて、プロジェクトの売上高を計算します。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ステータス ]</td> 
   <td> <p>作業項目または戦略目標のワークフロー位置を示すために使用されるインジケーター。</p> <p>プロジェクトの場合、[!UICONTROL ステータス ] はプロジェクトの設定で、プロジェクトが次のどちらであるかを示します。</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL 保留中 ] </li> 
     <li>[!UICONTROL 完了 ] </li> 
     <li>[!UICONTROL 無効 ]</li> 
    </ul> <p>プロジェクトのステータスの詳細については、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">システムプロジェクトステータスのリストへのアクセス</a>.</p>
    <p>タスクの場合、[!UICONTROL ステータス ] はタスクの設定で、タスクが次のどちらであるかを示します。</p> 
    <ul> 
     <li>[!UICONTROL 新規 ]</li> 
     <li>[!UICONTROL 処理中 ]</li> 
     <li>[!UICONTROL 完了 ]</li> 
    </ul> <p>タスクステータスの詳細については、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">システムタスクステータスのリストへのアクセス</a></p> <p>問題の場合、[!UICONTROL ステータス ] は問題に関する設定で、この問題が次のどちらであるかを示します。</p> 
    <ul> 
     <li>[!UICONTROL 新規 ]</li> 
     <li>[!UICONTROL 処理中 ]</li> 
     <li>[!UICONTROL フィードバック待ち ]</li> 
     <li>[!UICONTROL 保留中 ]</li> 
     <li>[!UICONTROL 解決済み ]</li> 
     <li>[!UICONTROL で解決されません ]</li> 
     <li>[!UICONTROL は複製できません ]</li> 
     <li>[!UICONTROL 検証済みの完了 ]</li> 
     <li>[!UICONTROL 再開済み ]</li> 
    </ul> <p>問題のステータスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">システムの問題ステータスのリストへのアクセス</a>.</p> 
    <p>戦略目標の場合、[!UICONTROL ステータス ] は目標が次のどちらであるかを示す目標の設定です。</p> 
     <ul> 
      <li>[!UICONTROL アクティブ ]</li> 
      <li>[!UICONTROL 下書き ]</li> 
      <li>[!UICONTROL 非アクティブ ]</li> 
      <li>[!UICONTROL クローズ済み ]</li> 
     </ul> 
     <p>戦略目標の詳細については、この記事の「[!UICONTROL 目標 ]」または「[!UICONTROL 目標 ]」も参照してください。 </p> 
     <p>戦略目標の場合、このフィールドは組織が購入済みの場合にのみ表示されます [!DNL Workfront Goals]. を使用した戦略目標の管理の詳細 [!DNL Workfront Goals]を参照してください。 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概要</a>. </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ステータスの変更 ]</td> 
   <td>[!UICONTROL 監査証跡 ]。 ユーザーがプロジェクト、タスク、またはイシューのステータスを変更すると、メモが生成されます。</td> 
  </tr> 
  <tr> 
   <td>状態アイコン</td> 
   <td> <p>組み込みの [!UICONTROL Status Icons] フィールドをビューの列として追加し、次のようなオブジェクトの主要ポイントをより明確に表示できます。</p> 
    <ul> 
     <li>オブジェクトにドキュメントが添付されています</li> 
     <li>オブジェクトが承認プロセスに関連付けられています</li> 
     <li>オブジェクトには、追加のメモが関連付けられています</li> 
     <li>費用は請求可能または償還可能です </li> 
     <li>タスクがクリティカルパス上にあります</li> 
     <li>ユーザーが会社、チームに属している、または別のタイムゾーンにいる </li> 
    </ul> <p>次のオブジェクトのビューに「[!UICONTROL ステータスアイコン ]」フィールドを追加できます。 </p> 
    <ul> 
     <li>[!UICONTROL タスク ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL テンプレートタスク ]</li> 
     <li>[!UICONTROL テンプレート ]</li> 
     <li>[!UICONTROL 費用 ]</li> 
     <li>[!UICONTROL ドキュメント ]</li> 
     <li>[!UICONTROL ユーザー ]</li> 
    </ul> <p>詳しくは、 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">ビュー内のビルトインステータスアイコン</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ステータスの更新 ]</td> 
   <td> <p>このフィールドには、「[!UICONTROL ステータスの更新 ]」フィールドでオブジェクトの所有者が指定した最新のステータス更新が表示されます。 プロジェクトの場合は、プロジェクト所有者が行ったコメント、タスクやタスクに関するコメント、つまり担当者が行ったコメントを意味します。</p> 
   <p> ステータスの更新に関しておこなわれたコメントは、「[!UICONTROL ステータスの更新 ]」列に表示されません。</p> <p>「[!UICONTROL 新規 ]」、「[!UICONTROL In Process]」および「[!UICONTROL Complete]」のステータスを表示するには、[!UICONTROL Status] 列を使用します。</p> <p>ステータスについて詳しくは、「 <a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">タスクステータスを更新</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ステータス ]</td> 
   <td>この記事の「[!UICONTROL ステータス ]」を参照してください。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL ストーリーボード ]</td> 
   <td>ストーリーのステータス（俊敏な手法でのタスク）と、ストーリーが完了に向かってどのように進んでいるかを表すグラフです。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>ストーリーの難しさや複雑さの測定に使用される指標です。 アジャイルチームは、時間とポイントのどちらを使用するかを選択できます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>ストーリーの難しさや複雑さの測定に使用される指標です。 アジャイルチームは、時間とポイントのどちらを使用するかを選択できます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>組織や組織の動作を変更する長期の作業。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL 戦略的連携 ]</td> 
   <td>ポートフォリオやプログラム全体で企業目標を測定し、調整する。</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>これは、「テキストモード」インターフェイスを使用する際に、レポートの列で使用されます。 </p>
   <p>The <code>[!UICONTROL stretch]</code> は、ビューで不要な領域を占める列を識別するために使用されます。 一般的なユーザーのワークスペースのユーザーインターフェイスの幅は、約 850 ピクセルです。 つまり、4 列（それぞれ 150 ピクセル）のビューがあり、そのビューが 850 ピクセルのうち 600 ピクセルを占有している場合です。 UI には、ストレッチの割合が指定された列に追加される、250 個の追加のピクセルがあります。 </p>
   <p>追加のコード行を使用する場合、列の拡張は適用されます。 <code>[!UICONTROL usewidths=true]</code> ビュー内の列の少なくとも 1 つに対して 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL 購読者 ]</td> 
   <td> <p>プロジェクト、タスクまたはタスクを購読するユーザー。</p> <p>このフィールドをレポートで使用すると、購読者のリストが表示され、各購読者がコンマで区切られます。</p> <p>詳しくは、 <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">の項目を購読 [!DNL Adobe Workfront]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL サマリタスク ]</td> 
   <td>この記事の「[!UICONTROL 親タスク ]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL サブタスク ]</td> 
   <td>親タスクの下に配置される子タスク。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL システムガバナンス ]</td> 
   <td>システムの変更とメンテナンスを管理する一連のポリシー。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL システム統合 ]</td> 
   <td>異なるコンピューティングシステムとソフトウェアアプリケーションを物理的または機能的に連携させ、全体として機能させるプロセス。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL タスク ]</td> 
   <td> <p>最終目標を達成する（プロジェクトの完了）ためのステップとして実行する必要があるアクティビティ。</p> <p>詳しくは、 <a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">タスクの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タスク属性 ]</td> 
   <td>Task に関連付けられ、Task に関する特定の詳細を示すその他のフィールドまたはオブジェクト。 例として、[!UICONTROL 計画完了日 ] や [!UICONTROL ステータス ] があります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タスク制約 ]</td> 
   <td>「[!UICONTROL 制約タイプ ]」および「[!UICONTROL 制約日 ]」を参照してください。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL タスク管理 ]</td> 
   <td>タスクの作成、割り当て、終了、および表示のしきい値を管理する一連のポリシー。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL タスク所有者 ]</td> 
   <td>作業の見積もりとタスクの完了を担当するチームまたはユーザー</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL チーム ]</td> 
   <td> <p>同様の目標やビジネス目標に向けて作業するユーザーの集まり。 これらのユーザは、チームを作業項目に割り当てることで、作業項目に一括で割り当てることができます。</p> <p>チームについて詳しくは、 <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">チームの概要</a>.</p> <p>プロジェクトには [!UICONTROL プロジェクトチーム ] を割り当てることができます。このチームには、プロジェクトでの作業に関連するすべてのユーザーや役割が含まれます。</p> <p>プロジェクトチームの詳細については、 <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL テンプレート ]</td> 
   <td> <p>プロジェクトテンプレートは、最も繰り返し可能なプロジェクトの一般的な概要です。 プロジェクトテンプレートを作成する際にタスク、キュートピック、カスタムフォーム、ドキュメントまたは承認を定義して、新しいプロジェクトを作成する際に時間を節約できます。 </p> <p>既存のプロジェクトにテンプレートを添付したり、テンプレートを使用して新しいプロジェクトを作成したりできます。 テンプレートで指定されたすべての情報は、それを使用して作成されたプロジェクトに転送されます。 </p> <p>テンプレートについて詳しくは、 <a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">プロジェクトテンプレートの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL テンプレートタスク ]</td> 
   <td>テンプレートの一部であるタスク。 テンプレートタスクは、テンプレートを使用して作成されるプロジェクト内のタスクになります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スレッド ]</td> 
   <td>特定のトピックに関連する返信の [!UICONTROL メモ ] とそのコレクション。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL サムネール ]</td> 
   <td> <p> [!UICONTROL ドキュメント ] のリストまたはレポートでは、ドキュメントのプレビューがサムネールで表示されます。 </p> <p> 選択 <strong>[!UICONTROL サムネール ]</strong>  をクリックすると、33 ～ 66 ピクセルの幅のサムネールがレポートに表示されます。 </p> <p>リストまたはレポートの列の幅を変更すると、サムネールのサイズが調整されます。</p> <p>この記事の「[!UICONTROL 大きいサムネール ]」も参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイムオフ ]</td> 
   <td>[!UICONTROL タイムオフ ] レポートを作成して、ユーザーがプロファイルでタイムオフを示した時点を表示できます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイムシート ]</td> 
   <td> <p>ユーザーが、プロジェクト、タスク、問題に取り組んだ実際の時間、または会議やトレーニングなど、作業に関連しない他のアクティビティに費やした時間を入力できるタイムカードです。 作業に費やした時間を入力する以外に、時間が作業に関連するか、間接費に計上するかを指定する場合は、「時間タイプ」を使用して時間エントリを定義します。 タイムシートの詳細については、 <a href="../../../timesheets/timesheets/timesheets-overview.md">タイムシートの概要</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイムシートプロファイル ]</td> 
   <td> <p>[!UICONTROL タイムシートプロファイル ] は、 [!DNL Workfront] を使用して、関連付けられたユーザーのタイムシートを自動的に作成します。 </p> <p>各タイムシートの作成時に各タイムシートに適用する設定の数を構成できます。 これらの設定の一部は、タイムシートの作成頻度（週、週ごと、週ごと、月ごと、月ごと）、タイムシートの開始日、タイムシート承認者、記録された時間に関連付けることができる [!UICONTROL 時間の種類 ] です。</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>このフィールドでは、最上位のグループとそのサブグループに関するデータを識別し、リストまたはレポートでフィルタリングできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 上位の親名 ] </td> 
   <td> <p>このフィールドでは、リストまたはレポートの [!UICONTROL 表示 ] 内の最上位グループとそのサブグループに関するデータを識別できます。</p> <p>これは、[!UICONTROL Top Parent ID] フィールドを使用しておこなうこともできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 合計時間 ]</td> 
   <td> <p>[!UICONTROL プロジェクトレポート ] では、このフィールドには、プロジェクトの最後の財政計算時点での、プロジェクトの全時間の丸め合計が表示されます。 [!UICONTROL 実際の時間 ] は、プロジェクトにログオンした正確な時間を反映します。 通常、[!UICONTROL 実際の時間 ] は [!UICONTROL 合計時間 ] と一致する必要があります。 [!UICONTROL 合計時間 ] が [!UICONTROL 実際の時間 ] フィールドと大きく異なる場合は、プロジェクト上の財務を再計算する必要があります。</p> <p>プロジェクトの財務計算の詳細については、「 」を参照してください。 <a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">プロジェクトの財務を再計算</a>.</p> <p>タイムシート [!UICONTROL 標準 ] ビューでは、このフィールドは、タイムシートに表示される日付の項目に関して記録された合計時間数を参照します。 この組み込みビューのタイムシートの [!UICONTROL 合計時間 ] フィールドは、[!UICONTROL hoursDuration] フィールドを参照し、タイムシートの開始日と終了日の時間差を動的に計算します。 ユーザーがタイムシートの時間枠で使用可能な時間より長い時間を記録した場合、[!UICONTROL 合計時間 ] 列を赤で表示するために使用されます。 詳しくは、 <a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">タイムシートの合計時間を表示</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL トラッキングモード ]</td> 
   <td> <p>タスクの属性です。 これにより、タスクの予定タイムラインを更新する方法が決まりました。 例：</p> 
    <ul> 
     <li>[!UICONTROL ユーザーは更新が必要 ] タスクを手動で更新する必要があります。 それ以外の場合は、[!UICONTROL Behind Schedule]、[!UICONTROL Late] の順に変更されます。</li> 
     <li>[!UICONTROL 自動完了 ] は、期限（[!UICONTROL 予定完了日 ]）が過ぎると、タスクを自動的に完了します。</li> 
    </ul> <p>詳しくは、 <a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">タスクトラッキングモードの概要</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROLトリガー]</td> 
   <td>シナリオを開始するイベント。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL トラブルタスク ]</td> 
   <td>[!UICONTROL 遅延 ]、[!UICONTROL スケジュール遅延 ]、[!UICONTROL リスク状態 ] のいずれかの条件を持つ不完全なタスク。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 未割り当てタスク ]</td> 
   <td>ユーザー、役割、またはチームに割り当てられていないタスクです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 更新タイプ ]</td> 
   <td> <p>プロジェクトの推定タイムラインを再計算するタイミングを決定する、プロジェクトの設定です。 オプションは次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL 自動変更と変更時 ]</li> 
     <li>[!UICONTROL 自動のみ ]</li> 
     <li>[!UICONTROL 手動のみ ] </li> 
    </ul> <p>詳しくは、 <a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプを選択 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ユーザー ]</td> 
   <td>で作成されたアカウント [!DNL Workfront] ユーザーがログインしてシステムとやり取りできるようにする。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL ユーザーの委任 ]</p> </td> 
   <td> <p>次のことを示すレポート可能なオブジェクト。</p> 
    <ul> 
     <li>タスク、問題、プロジェクトの承認を委任したユーザー</li> 
     <li>タスク、問題、プロジェクトの承認を委任したユーザー</li> 
     <li>これらの委任が開始および終了したとき</li> 
    </ul> <p>詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">ユーザー委任レポートの作成</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ユーザーインターフェイス ]</td> 
   <td>のすべての視覚的およびインタラクティブな側面 [!DNL Workfront] アプリケーション。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ユーザーインターフェイスの環境設定 ]</td> 
   <td>[!UICONTROL ユーザーインターフェイスの設定 ] [!DNL Workfront] 管理者は、これらの設定を変更して、ユーザーインターフェイスの側面をカスタマイズできます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL 使用率 ]</td> 
   <td>割り当てられたスケジュール、PTO、現在のワークロードに基づくユーザーまたはロールの可用性。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ユーザー使用率 ]</td> 
   <td> <p>ユーザー（リソース）の割り当て方法または割り当て超過方法を示すレポートと組み合わせた検索。 この記事の「[!UICONTROL リソース使用率 ]」を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## V - Z

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>オブジェクト名</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Velocity]</td> 
   <td>作業サイクルの合計時間（作業の完了に要する時間）と、最初にコミットされた時間（作業とコミットの比率）での作業の頻度を示す尺度です。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL 表示 ]</td> 
   <td> <p>表示は、レポートの列を変更する場合や、プロジェクト、タスク、問題の一覧で使用する場合、またはアクセスレベルまたは権限共有レベルでの情報のみを表示するユーザーの権限を示す場合に使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アイコンを表示 ]</td> 
   <td> <p> これはステータスアイコンと同じフィールドですが、次の表示でのみ使用できます。 </p> 
    <ul> 
     <li> [!UICONTROL ドキュメント ] </li> 
    </ul> <p> 詳しくは、 <a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">ビュー内のビルトインステータスアイコン</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 先月表示 ]</td> 
   <td> <p>レポートリストには、そのレポートが先月に閲覧された回数が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 前四半期に表示 ]</td> 
   <td>レポートリストには、前四半期にそのレポートが表示された回数が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >レポートの使用状況の表示</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 昨年表示数 ]</td> 
   <td>レポートリストには、そのレポートが過去 1 年間に表示された回数が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 今月表示 ]</td> 
   <td> <p>レポートリストには、そのレポートが今月に閲覧された回数が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 今四半期に表示 ]</td> 
   <td>レポートリストには、そのレポートが今四半期に閲覧された回数が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 今年表示 ]</td> 
   <td>レポートリストには、そのレポートが今年に閲覧された回数が表示されます。<br>レポートリストの使用状況の詳細については、「 <a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">レポートの使用状況の表示</a>.</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> レポートで、[!UICONTROL テキストモード ] インターフェイスを使用する際に、各列の幅をピクセル単位で指定できるコード行。 Workfrontでは各フィールドに推奨される幅が提供されますが、フィールドの種類や形式に応じて異なりますが、調整を行うこともできます。
追加の <code>[!UICONTROL usewidths=true]</code> 列に指定された幅を適用するコードの行。 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>プロジェクト、タスク、またはタスクのレポートで、テキストモードで次のステートメントを使用すると、プロジェクト、タスク、またはタスクの予定時間が表示されます。</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>テキストモードの使用について詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">テキストモードの構文の概要</a>. </p> 
   <p><b>ヒント</b> 
   <p>問題レポートで、[!UICONTROL 予定時間 ] フィールドの 1 つを追加すると、 <code>work </code>フィールドをレポートに追加します。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>2 つの主なライセンスの種類の 1 つ。 これにより、[!UICONTROL プラン ] よりもアクセス権が小さくなりますが、システムで作成および更新をおこなうことができます。 これは、[!UICONTROL 外部 ]、[!UICONTROL レビュー担当者 ]、[!UICONTROL リクエスター ] の各ライセンスタイプよりも多くの機能を備えています。</p> <p>詳しくは、 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] ライセンスの概要</a>.</p> <p>Work は、プロジェクト、タスクまたは問題の [!UICONTROL 予定時間 ] 数を指す場合があります。 詳しくは、この表の「[!UICONTROL work]」フィールドを参照してください。 </p> <p>ヒント：問題レポートで、[!UICONTROL 予定時間 ] フィールドの 1 つを追加すると、 <code>work </code>フィールドをレポートに追加します。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 作業分類構造 ]</td> 
   <td>親/子の関係に基づいて、プロジェクトチームが実行するタスクの階層構造。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL 作業量 ] </td> 
   <td> 
    <p>プロジェクトマネージャーは、タスクの完了に必要な作業量を見積もる際に、[!UICONTROL 予定時間 ] の代わりにこのフィールドを使用することにします。 このフィールドは、次の条件を満たした場合にのみ表示されます。</p> 
     <ul> 
      <li> <p>タスクには [!UICONTROL シンプル期間タイプ ] が含まれています。 </p> <p>ヒント：タスク [!UICONTROL 期間タイプ ] を他のタイプに更新すると、このフィールドは非表示になります。 </p> </li> 
      <li>プロジェクトマネージャーが、[!UICONTROL 作業量を使用 ] で、プロジェクトのタスク [!UICONTROL 予定時間 ] フィールドを自動的に計算できるようにしました。 </li> 
     </ul> 
     <p>[!UICONTROL 予定時間 ] の代わりに [!UICONTROL 作業量 ] を使用してタスクの作業量を見積もる方法について詳しくは、 <a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>. </p> 
     <p>このフィールドは、タスクのレポートとリストに表示できます。</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL 作業項目 ]</td> 
   <td> <p>このフィールドは、 [!DNL Workfront]. </p> <p>[!UICONTROL 作業項目 ] レポートには、タスクと問題に関する情報が表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Mix]</td> 
   <td>ビジネスの実行に割り当てられた作業の割合と、ビジネスの変化に対する割合の [!UICONTROL 作業実績指標 ](WPI)。 Mix WPI は、戦略に実際の作業割り当てが適用されているかどうかを組織レベルで理解するのに役立ちます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 作業管理リソース ]</td> 
   <td>作業を受け取ったり、時間を追跡する資格のある、システム内のペルソナの指定。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 作業管理上の役割と責務 ]</td> 
   <td>指定された問題、タスク、プロジェクト、プログラム、またはポートフォリオの範囲、実行、承認を管理するための所有者と関係者を定義する。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 作業管理 SLA]</td> 
   <td>すべての関係者が合意した定量化可能な指標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 作業管理関係者 ]</td> 
   <td>作業リクエストの結果に対する関心が既にあるユーザーのコレクションです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management タッチポイント ]</td> 
   <td>関係者間の通信のデジタル化された記録。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 業績評価指標 ] </td> 
   <td> <p>比率、容量、速度、品質、エンゲージメントを組み合わせます。</p> <p>WPI は、[!UICONTROL Work Performance Indicator] の一般的な頭字語です。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 作業プロセス ]</td> 
   <td> <p>作業を受け取り、優先順位付けし、実行する方法。 作業の実行方法は、通常、「ワークフロー」または「プロジェクトプラン」（日付、先行者関係などを持つタスクのリスト）と呼ばれます。 </p> <p>作業プロセスの例としては、1 つのアセットの作成や複数アセットキャンペーンの配信などがあります。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ワークフローテンプレート ]</td> 
   <td>[!UICONTROL 配達確認の承認 ] レポートで、このフィールドに配達確認に関連付けられているワークフローテンプレートが表示されます。 テンプレートが添付されていない場合、列は空白になります。</td> 
  </tr>

<tr> 
   <td>[!UICONTROL 作業時間 ]</td> 
   <td>

<p>ユーザーが実際の作業に使用できる（オーバーヘッドを含まずに）フルタイム相当 ([!UICONTROL FTE]) 時間の割合を表します。 [!UICONTROL 作業時間 ] は、1 までの 10 進数で指定する必要があります。0 は指定できません。 例えば、実際の作業時間の 20%の可用性は 0.2 となります。</p>
   </p>フィールドのデフォルト値は 1 で、ユーザーが [!UICONTROL FTE] 全体を実際のプロジェクト関連の作業に費やすことを示します。  </p>
   <p>この数値を使用して、プロジェクト関連の実際の作業に対するユーザーの可用性が計算されます。 </p>
   <p> スケジュールの例外とタイムオフも、ユーザーの容量に影響を与える可能性があります。 </p>
   <p>Workfrontでスケジュールを作成する方法について詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールの作成</a>. </p>
    <p>Workfrontは、[!UICONTROL セットアップ ] 領域のリソース管理環境設定に応じて、ユーザーの可用性を計算します。 詳しくは、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">リソース管理環境設定の指定</a>. </p> 
   <p>ユーザーの [!UICONTROL 作業時間 ] は、ユーザーの編集時または作成時に更新できます。 詳しくは、 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">ユーザーのプロファイルの編集</a></p> 
   <b>ヒント</b> 
   <p>[!UICONTROL Work Time] の値を 1 に設定して、プロジェクト関連の作業でユーザーがフルタイムの同等の作業全体で使用できることを示します。</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 稼働時間 ]</td> 
   <td>Workfrontのドキュメントでは、この用語は、作業に割り当てられた時間をスケジュールに従って示すために使用されます。</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>プロジェクト、タスク、または問題報告で、テキストモードで次のステートメントを使用すると、プロジェクト、タスク、または問題の計画時間数が「時間」という単語の後に表示されます。</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>テキストモードの使用について詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">テキストモードの構文の概要</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
