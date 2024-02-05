---
content-type: reference
navigation-topic: workfront-navigation
title: '  [!DNL Adobe Workfront]  の用語集'
description: The [!DNL Adobe Workfront] 用語集には、 [!DNL Adobe Workfront]. You can use the glossary when you want to find the definition of concepts you see in the [!UICONTROL Workfront] インターフェイス、レポート、または [!DNL Workfront] 定義された概念 [!DNL Workfront] ドキュメント。
author: Alina
feature: Get Started with Workfront
exl-id: 758072b3-775e-4771-9ae9-da0b38580c93
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '19889'
ht-degree: 89%

---


# [!DNL Adobe Workfront] の用語集

<!--Audited: 12/2023-->

>[!IMPORTANT]
>
>この記事は、[!DNL Adobe Workfront] アプリケーション、[!DNL Workfront] のドキュメント、または一般的に作業の計画と管理に関して出会う可能性がある用語を理解するための参考資料として使用してください。現在、この情報を更新中です。そのため、この表は完了していない可能性があります。情報が十分に網羅された判断した時点で、この免責条項を削除する予定です。

次の表は、Adobe Workfront でよく使用される用語の一覧です。

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
   <td>[!UICONTROL Access Level]</td> 
   <td>ユーザーが Workfront 内の様々なオブジェクトやツールを操作する方法を決定するユーザープロファイル。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Active Task]</td> 
   <td>現在進行中のプロジェクトで、先行タスクによって作業が妨げられておらず、将来の予定開始日を持つタスク制約を持たない未完了のタスク。つまり、今日からでも作業を開始できます。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Activity]</td> 
   <td>[!DNL Workfront Goals] の場合、アクティビティは目標の進捗状況インジケーターです。手動で更新するプログレスバー、または目標に関連付けられたプロジェクトを指定できます。アクティビティをレポートに表示することはできません。また、[!DNL Workfront] API を経由してアクティビティにアクセスすることはできません。アクティビティについて詳しくは、<a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront Goals の結果とアクティビティの概要</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Cost]</td> 
   <td> <p>タスクおよびイシューの場合、タスクまたはイシューに割り当てられたリソースの 1 時間あたりのコスト率に関して、実際に記録された時間に関連するコストです。プロジェクトの場合、これは、プロジェクトのタスクとイシューに関するすべての [!UICONTROL Actual Costs] の合計です。詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Expense Cost]</td> 
   <td> <p>プロジェクトまたはタスクに記録されたすべての費用の [!UICONTROL Actual Amounts] の合計です。</p> <b>例</b>
   <p>タスク 1 の費用を作成し、[!UICONTROL Actual Amount] フィールドに $600.00 と入力した場合、このタスクの [!UICONTROL Actual Expense Cost] は $600.00 になります。 </p> 
   <p>プロジェクトの場合、[!DNL Workfront] は次の式で [!UICONTROL Actual Expense Cost] を計算します。</p> <p><code>Project Actual Expense Cost = SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost</code> <br> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (drafting this because not sure if this is still correct)</p>
    --> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Hours]</td> 
   <td> <p>プロジェクト、タスク、またはイシューレポートでは、[!UICONTROL Actual Hours] は、プロジェクト、タスク、またはイシューに関して記録されたすべての時間の合計です。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span>タスク 1 の [!UICONTROL Updates] タブから「ログ時間」をクリックし、25 時間と入力した場合、タスク 1 の実際の時間は 25 時間になります。 </p> <p>[!DNL Workfront] 次の式を使用して、親タスクまたはプロジェクトの [!UICONTROL Actual Hours] を計算します。</p> 
    <ul> 
     <li> <p><code>For parent tasks = children [!UICONTROL Actual Hours] + [!UICONTROL Actual Hours] on the parent task. </code> </p> </li> 
     <li> <p><code>For projects = [!UICONTROL Actual Hours] logged on the project + [!UICONTROL Actual Hours] logged on standalone or children tasks in the project</code> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Labor Cost]</td> 
   <td> <p>タスクまたはプロジェクトに投入された労力に関連する [!UICONTROL Actual Cost]。 </p> <p>タスクの場合、[!DNL Workfront] は次の式を使用して [!UICONTROL Actual Labor Cost] を計算します。</p> <p><code>Task [!UICONTROL Actual Labor Cost] = Number of [!UICONTROL Actual Hours] on the task * User or Job Role [!UICONTROL Hourly Cost Rate]</code> </p> <p>タスクの [!UICONTROL Cost Type] が [!UICONTROL User Hourly] の場合、[!DNL Workfront] はユーザーレートを使用します。タスクが [!UICONTROL Cost Type] が [!UICONTROL Role Hourly] の場合、[!DNL Workfront] は [!UICONTROL Actual Labor Cost] を計算するために担当業務レートを使用します。 </p> <p>プロジェクトの場合、[!DNL Workfront] では、次の式を使用して [!UICONTROL Actual Labor Cost] を計算します。</p> <p><code>Project [!UICONTROL Actual Labor Cost] = SUM(All Tasks [!UICONTROL Actual Labor Cost]) </code> </p> <p>詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span>例えば、ユーザーが [!UICONTROL User Hourly] [!UICONTROL Cost Type] でタスクに対して 5 時間記録し、その時間単価が $100 の場合、[!UICONTROL Actual Labor Cost] は $500 になります。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Actual Revenue] </td> 
   <td> <p>プロジェクトまたはタスクの [!UICONTROL Actual Revenue] は、プロジェクトまたはタスクの [!UICONTROL Actual Hours] に関連する金額です。 </p> <p>[!DNL Workfront] での収益の追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Actual Start]</td> 
   <td>ユーザーが、割り当てられた作業で進行中のオブジェクトを変更したときのタイムスタンプ。</td> 
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
   <td>[!UICONTROL Agile] 方法論</td> 
   <td>部門横断的なチームでのニーズとソリューションのコラボレーションの進化に基づく方法論のひとつ。固定されたタイムラインに基づく柔軟性と変化を促進します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Agile Team]</td> 
   <td>従来のチームとは異なります。これは、見込み作業をバックログから取り出し、[!UICONTROL 反復 ] と呼ばれる一定の期間内に作業を行うからです。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL All My Teams]</td> 
   <td> <p>この情報が [!UICONTROL フィルター ] で参照される場合、このフィールドには、ログインユーザーが属する任意のチームに属するユーザー、またはログインユーザーが属するチームに割り当てられた作業項目が表示されます。 </p> <p>他のユーザーとレポートを共有する場合は、このフィールドをフィルターで使用して、より一般的なレポートにすることをお勧めします。このように、情報は常にログインユーザーに合わせてカスタマイズされるので、レポートを 1 つだけ作成して、ログインしてレポートを表示するユーザーに応じて異なる情報を表示することができます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Allocation Date]</td> 
   <td> <p>このフィールドは、次のタイプのレポートにあります。</p> 
    <ul> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
     --> 
     <li>[!UICONTROL Project]（財務データ）</li> 
     <li>[!UICONTROL Budgeted Hour]</li> 
    </ul> <p><!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Resource Estimates or 
      </MadCap:conditionalText>
     -->[!UICONTROL Project (Financial Data)]レポートの場合： </p> 
    <ul> 
     <li>リソースに割り当てられている[!UICONTROL Planned Hours]の量を<!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         how resources are budgeted for work, or 
       </MadCap:conditionalText>
      -->把握しようとする場合は、このレポートを作成します。</li> 
     <li> <p>[!UICONTROL Allocation Date]は、タスクへの[!UICONTROL Job Role]の配分が開始される週の最初の日（日曜日）です。リソース（[!UICONTROL Job Role]）には、割り当てられているタスクの[!UICONTROL Duration]中の週と同数の[!UICONTROL Allocation Dates]を設定できます。タスクが複数月にわたる場合、タスクの [!UICONTROL Duration]内であれば、月の最初の日を[!UICONTROL Allocation Date]にすることもできます。</p> <p>例えば、3 週間以上にわたるタスクにユーザーの[!UICONTROL Job Role]を割り当て、[!UICONTROL Planned Hours]を 90 時間にすることができます。これらの時間数はタスクの期間中に均等に配分され、毎日 6 時間の[!UICONTROL Planned Hours]が担当業務に割り当てられます。</p> <p><em> [!UICONTROL Daily Planned Hours] = [!UICONTROL Total Planned Hours] / タスクの[!UICONTROL Duration]中の[!UICONTROL Work Days]の数</em> </p> <p>その結果、[!UICONTROL Allocation Dates]は 3 つあり、タスクの[!UICONTROL Duration]中の毎週日曜日ごとに 1 つで、それぞれに特定の数の[!UICONTROL Planned Hours]が関連付けられています。<br>ある月の最終週の真ん中でタスクが開始され、新しい月の初めから 2 週間後に終了する場合、タスクには 4 つの[!UICONTROL Allocation Dates]があります。タスクの[!UICONTROL Duration]中の毎週日曜日ごとに 1 つと、新しい月の最初の日に 1 つです。</p> <p>この情報を最大限に活用するために、<!--
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          Resource Estimates or a 
        </MadCap:conditionalText>
       --> プロジェクト（財務データ）レポートを作成し、[!UICONTROL Allocation Date]のマトリックスグループを追加した後、結果を週別、月別、四半期別または年別にグループ化して最も正確なデータを得ることをお勧めします。<br>マトリックスグループ化の作成については、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md" class="MCXref xref">マトリックスレポートの作成</a>の記事を参照してください。</p> </li> 
    </ul> <p>[!UICONTROL Project (Financial Data)]レポートに財務情報が入力されるのは、関連付けられているデータが 5 年未満の場合のみです。例えば、2015年1月に担当業務がタスクに割り当てられ、今日が 2021年9月の場合、[!UICONTROL Project (Financial Data)]レポートでは、担当業務の[!UICONTROL Allocation Date]などの財務フィールドにデータは入力されません。 </p> 
    <div> 
     <p>[!UICONTROL Budgeted Hour]レポートの場合：</p> 
     <ul> 
      <li>リソースプランナーでリソースやプロジェクトに割り当てられる[!UICONTROL Budgeted Hours]の量を把握しようとする場合は、このレポートを作成します。</li> 
      <li> <p>[!UICONTROL Allocation Date]は、[!UICONTROL Resource Planner]で時間を予算計上した週の最初の日（日曜日）です。 </p> <p><b>ヒント</b></p> <p>1 週間が 2 か月にわたる場合は、レポートに 2 つの行が生成されます。1 つは週の最初の日（最初の月の 第 1 週の日曜日）に対応し、2 行目には 2 番目の月の最初の日が表示されます。 </p> <p>例えば、6月30日（日曜日）～7月6日（土曜日）の週に 8 時間を予算計上した場合、2 つの行には 6月30日と 7月1日の[!UICONTROL Allocation Date]が表示されます。 </p> </p> <p>[!DNL Resource Planner]でのリソースの予算計上については、<a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">[!DNL Resource Planner]の[!UICONTROL Project]ビューと[!UICONTROL Role]ビューを使用したリソースの予算計上</a>を参照してください。</p> <p>[!UICONTROL Budgeted Hour]レポートの作成については、<a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">レポート：予算計上時間数</a>を参照してください。 </p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Announcements]</td> 
   <td> <p>システム内でユーザーに情報を伝える方法。この情報は、多くの場合、[!DNL Workfront] から管理者に、または管理者からユーザーに送信されます。 </p> <p>詳しくは、<a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">お知らせの送信</a>を参照してください</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL App Integration]</td> 
   <td>アプリは通常、ソフトウェアアプリケーションへのコネクタを表しますが、データを操作する特別な機能を表すこともあります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver Decision]</td> 
   <td> <p>[!UICONTROL Proof Approval]レポートで、このフィールドには、アクティブでなくなったプルーフの承認に関する決定が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver stage]</td> 
   <td>[!UICONTROL Proof Approval report]で、このフィールドには、プルーフの現在のステージに関する情報が表示されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval]</td> 
   <td> <p>タスク、ドキュメント、タイムシートなどの所定の作業アイテムは、上司または他のユーザーが承認することが必要な場合があります。このサインオフのプロセスを承認と呼びます。 </p> <p>詳しくは、<a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">承認プロセスの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approval date]</td> 
   <td>[!UICONTROL Proof Approval]レポートで、このフィールドには、プルーフが承認された日付が表示されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Approver]</td> 
   <td>特定の作業アイテムについてサインオフする必要があるユーザーまたは担当業務や、タイムシートの時間エントリを承認するユーザーです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assigned To]</td> 
   <td> <p>[!UICONTROL Task or Issue] レポートで、このフィールドには、タスクまたはイシューの所有者、または [!UICONTROL Primary Assignee] が表示されます。また、このフィールドでフィルタリングやグループ化を行うこともできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment]</td> 
   <td>イシューまたはタスクに割り当てられたユーザー、担当業務、またはチーム。プロジェクト、ポートフォリオまたはプログラムには、割り当てることはできません。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignments]</td> 
   <td> <p>[!UICONTROL Task] または [!UICONTROL Issue] レポートで、このフィールドにはタスクやイシューに割り当てられているすべてのエンティティ（ユーザー、担当業務、チーム）のリストが表示されます。[!UICONTROL Assignment Users] フィールドと [!UICONTROL Assignment Roles] フィールドを使用して、このフィールドでフィルタリングできます。チームフィールドを使用して、タスクまたはイシューに割り当てられているチームでフィルタリングできます。このフィールドでレポートをグループ化することはできません。</p> <p>[!UICONTROL Recycle Bin] に配置された作業アイテムは、[!UICONTROL Assignment] オブジェクトを参照する一部のレポートに引き続き表示されます。このレポートでは、[!DNL OR] フィルター修飾子が使用されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Roles]</td> 
   <td>
   <p>[!UICONTROL Task] または [!UICONTROL Issue] レポートで、タスクやイシューに割り当てられた担当業務に関する情報が表示されます。このフィールドには、[!UICONTROL Primary Owners] と、タスクやイシューに割り当てられた他の担当業務が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Status]</td> 
   <td> <p>割り当てレポート、タスクレポート、イシューレポートでは、作業項目に割り当てられたユーザーが「[!UICONTROL Work On It]」ボタンまたは「[!UICONTROL Done]」ボタンをクリックして作業を承認または完了したかどうかが、[!UICONTROL Assignment Status] に表示されます。以下の [!UICONTROL Assignment Statuses] があります。</p> 
    <ul> 
     <li><b>[!UICONTROL Requested]</b>：ユーザーはタスクまたはイシューに割り当てられていますが、「[!UICONTROL Work On It]」ボタンをまだクリックしておらず、作業を開始していません。</li> 
     <li><b>[!UICONTROL Working]</b>：ユーザーが「[!UICONTROL Work On It]」ボタンをクリックし、現在作業中です。 </li> 
     <li><b>[!UICONTROL Done]</b>：ユーザーが「[!UICONTROL Done]」ボタンをクリックし、作業を完了しました。 </li> 
    </ul> <p>詳しくは、<a href="../../../workfront-basics/updating-work-items-and-viewing-updates/work-on-it-and-done-buttons-accept-complete-work.md" class="MCXref xref">「[!UICONTROL Work On It]」ボタンと「[!UICONTROL Done]」ボタンの概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Teams]</td> 
   <td>
   <p>[!UICONTROL task] レポートまたは [!UICONTROL issue] レポートで、このフィールドにはタスクやイシューに割り当てられたチームに関する情報が表示されます。このフィールドには、[!UICONTROL Primary Owners] と、タスクまたはイシューに割り当てられた他のチームが表示されます。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Assignment Users]</td> 
   <td>
   <p>[!UICONTROL Task] レポートまたは [!UICONTROL Issue] レポートで、このフィールドにはタスクまたはイシューに割り当てられたユーザーに関する情報が表示されます。このフィールドには、[!UICONTROL Primary Owners] と、タスクまたはイシューに割り当てられた他のユーザーが表示されます。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attribute]</td> 
   <td>属性は [!DNL Workfront] オブジェクトの特性です。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Area]</td> 
   <td> <p>監査は、Workfrontで発生したアクションを記録するシステムメッセージです。 以下の監査タイプが記録されます。</p> 
    <ul> 
     <li>[!UICONTROL Scope Change]</li> 
     <li>[!UICONTROL Attachment Action]</li> 
     <li>[!UICONTROL General Edit]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Note]</li> 
     <li>[!UICONTROL Combined Entry]</li> 
     <li>[!UICONTROL Error Entry]</li> 
     <li>[!UICONTROL Status Change]</li> 
     <li>[!UICONTROL Subscription Change]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Audit Trail]</td> 
   <td>記録される変更（[!UICONTROL Audit Areas]）を通じて追跡されるイベントによって自動的に生成されるメモのコレクション。それぞれのメモには、誰が当該のアクションを行ったか、何をしたか、いつ実行したかが記録されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Automatic And On Change]</td> 
   <td> <p>[!UICONTROL Project Update] タイプのうちの 1 つ。これにより、夜間の再計算処理が実行されたときや、プロジェクト内のプロジェクトまたはタスクが更新されたときに、プロジェクトの予測および計画タイムラインが再計算されます。 </p> <p>詳しくは、<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプの選択</a>を参照してください。</p> </td> 
  </tr>

<tr> 
   <td><p>使用可否</p></td> 
   <td> <p>この用語は、「ユーザーの空き時間」または「リソースの空き時間」に関連して使用され、リソース（ユーザーまたは担当業務）が作業できる時間を示します。 </p> 
   <p>Workfront は、システム内のリソース管理の環境設定に応じて、いくつかのフィールドを使用してユーザーの空き時間を計算します。詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理環境設定の指定</a>を参照してください。 </p>
   <p>リソースの空き時間の詳細については、<a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">リソース管理の概要</a>を参照してください。</p>
   リソースの空き時間を指すためには「キャパシティ」も使用されます。 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Automatic Only]</td> 
   <td> <p>[!UICONTROL Project Update] タイプのうちの 1 つ。これにより、夜間の再計算処理が実行されたときに「見込み」と「計画」のタイムラインが再計算されます。</p> <p>詳しくは、<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプを選択</a>を参照してください。</p> </td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL BAU]</td> 
   <td>日々の主要なビジネス目標の実行に貢献する「通常のビジネス」業務。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Backlog]</td> 
   <td>新しいイシューに取り組む準備ができるまで保持されるアジャイル環境のエリア。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Baseline]</td> 
   <td>アジャイルな環境でのイテレーションを測定するためのデータのソース。</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td>[!UICONTROL Billing Record]</td> 
   <td> <p>請求可能な売上高、時間、または費用を記録します。この情報は、外部の会計システムで請求書を作成する際に使用できます。</p> <p>詳しくは、<a href="../../../manage-work/projects/project-finances/create-billing-records.md">請求記録を作成</a>を参照してください。 </p> 
   </td> 
  </tr>

<tr> 
   <td>請求記録のステータス</td> 
   <td> <p>請求記録または時間レポートでは、請求記録のステータスは請求記録が請求済みか、請求なしかを示します。プロジェクトを削除したり、請求済み請求記録に関連する時間を編集したりすることはできません。詳しくは、<a href="../../../manage-work/projects/project-finances/create-billing-records.md" >請求記録を作成</a>を参照してください。</p>  
   </td> 
  </tr>


<tr> 
   <td>[!UICONTROL Branding]</td> 
   <td><p>[!DNL Workfront] をカスタマイズして、色やロゴを使用してインターフェイスに会社を反映した外観を与えるプロセス。</p><p><strong>メモ</strong><br>組織が [!DNL Adobe Experience Cloud] にオンボーディングされている場合、ブランディングは利用できません。</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Breadcrumbs]</td> 
   <td> <p>ページ上部のエリアで、アプリケーション内のユーザーの位置が階層的に表示されます。</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">詳しくは、<a href="../../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">パンくずリストの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget Status]</td> 
   <td> <p>これは非推奨のフィールドです。このフィールドに表示される情報はすべて、[!DNL Workfront] によって削除された機能に関連しているため、フィールドを更新できません。 </p> <p>このフィールドは、プロジェクトが [!UICONTROL Capacity Planner] に追加されたかどうか、およびその予算の計算が完了したかどうかを示します。[!UICONTROL Capacity Planner] は [!DNL Workfront] から削除されました。 </p> 
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
   <td>[!UICONTROL Budgeted Completion Date]</td> 
   <td> <p>これは非推奨のフィールドです。このフィールドに表示される情報はすべて、[!DNL Workfront]が削除した機能に関連しています。このフィールドは更新できません。 </p>
   <p> このフィールドは、[!UICONTROL project] および [!UICONTROL tasks] のレポートとリストに引き続き表示されます。</p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budgeted Cost]</td>

<td> <p>これは、プロジェクトの予算リソースに関連するコストです。 </p>
   <p>フィールドは、以下の名前の下の [!DNL Workfront] の次のエリアに表示されます。</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Cost]</strong>：[!UICONTROL Business Case Summary] パネル内</li>
   <li><strong>[!UICONTROL Cost]</strong>：[!UICONTROL Cost] ごとに情報を表示する場合の [!UICONTROL Utilization] エリア内</li>
   <li><strong>[!UICONTROL Project Budgeted Cost]</strong>：リストおよびレポート内</li>
   </ul>   
    <p>プロジェクトの [!UICONTROL Budgeted Cost] は、次の式を使用して計算されます。</p> 
    <p><code>[!UICONTROL Project Budgeted Cost] (or [!UICONTROL Budgeted Cost]) = [!UICONTROL Budgeted Expense Cost] + [!UICONTROL Budgeted Labor Cost] + [!UICONTROL Fixed Cost] of the project</code> </p> 
    <p>[!DNL Workfront] における [!UICONTROL Budgeted Cost] の計算と、この概念の様々な名前の理解について詳しくは、<a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">プロジェクトの予算計上コストを計算</a>を参照してください。 </p>
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Budgeted Hours]</td> 
   <td> <p>プロジェクトで完了する必要がある作業のリソースに予算される時間です。このフィールドは、プロジェクトまたはプロジェクトリソースの [!UICONTROL Business Case]（または [!UICONTROL Resource Planner]）の [!UICONTROL Resource Budgeting] エリアで予算設定された時間を参照します。</p> <p>詳しくは、<a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">プロジェクトの [!UICONTROL Budgeted Labor Cost] および [!UICONTROL Budgeted Hours] を理解</a>を参照してください。 </p> 
    <!-- 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Hours that were formerly budgeted in the Legacy Resource Estimates area of a project (or in the Capacity Planner)</p>
    <p>Important: This is a deprecated field. Any information that this field might display is related to a feature that Workfront has removed and the field cannot be updated. </p>
  -->
    <p> [!DNL Resource Planner] のユーザーの予算計上についての詳細は、<a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">[!UICONTROL Project] ビューと [!UICONTROL Role] ビューを使用する [!DNL Resource Planner] 内のリソースの予算計上</a>の記事を参照してください。 </p> 
    <p>[!UICONTROL Business Case] の [!UICONTROL Resource Budgeting] エリアまたは [!UICONTROL Resource Planner] で予算計上された時間は、以下の名前の下の [!DNL Workfront] の次のエリアに表示されます。</p> 
     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td><strong>[!UICONTROL Budgeted Hours] の表示名</strong></td> 
        <td><strong>以下のエリア [!DNL Workfront]</strong></td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Hours]</td> 
        <td>[!UICONTROL Business Case] の [!UICONTROL Resource Budgeting] エリア</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL BDG]</td> 
        <td>[!UICONTROL Hours] が閲覧した [!UICONTROL Resource Planner]</td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Budgeted Hours]</td> 
        <td> <p>稼働率レポート [!UICONTROL Hours] ビュー</p> <p>[!UICONTROL Utilization] レポートについての詳細は、<a href="../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md" class="MCXref xref">[!UICONTROL Resource Utilization] レポートの概要</a>の記事を参照してください。</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Bud. Hours]</td> 
        <td> <p>[!UICONTROL Budgeted Hour] レポート</p><p>予算計上時間数レポートの [!UICONTROL Budgeted Hour] オブジェクトは、非推奨であるリソース管理ツールに関連する情報を参照します。このレポートの「[!UICONTROL Bud. Hours]」フィールドのみが、プロジェクトの [!UICONTROL Resource Planner] またはプロジェクトの [!UICONTROL Business Case] の [!UICONTROL Resource Budgeting] エリアで予算計上された時間数を参照します。 </p> <p>レポートの作成についての情報は、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>の記事を参照してください。</p> </td> 
       </tr> 
       <tr> 
        <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
        <td> <p>次のレポートに含まれています。</p>
        <ul>
        <li>[!UICONTROL Project] レポート
        <li>[!UICONTROL Project (Financial Data)] レポート
        <li>[!UICONTROL Task] レポート
        <li>[!UICONTROL Issue] レポート
        <li>[!UICONTROL Budgeted Hour] レポート</li>
        </ul>
         <p>レポートの作成についての情報は、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>の記事を参照してください。</p> </td> 
       </tr> 
      </tbody> 
     </table> 
    <p>[!DNL Adobe Workfront] の [!UICONTROL Budgeted Hours] に関する他の明記では、Workfront から削除および非推奨の機能を使用して予算計上された時間数を指します。これらは、表示のみのフィールドで、現在のリソース予算計上ツールを使用する際に、現在の情報では更新されません。 </p>
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
   <td>[!UICONTROL Budgeted Labor Cost]</td> 
   <td> <p>これは、リソース管理者として、プロジェクトで完了する必要のある作業の担当業務に対して予算計上する時間数に関連するコストです。 </p> <p>プロジェクトレポートの [!UICONTROL Budgeted Labor Cost] は、次の式を使用して計算されます。</p> <p><code style="font-style: normal;">[!UICONTROL Budgeted Labor Cost] = SUM([!UICONTROL Job Role Cost] per [!UICONTROL Hour] * [!UICONTROL Budgeted Hours] per [!UICONTROL Job Role])</code> </p> <p>このフィールドは、次を参照している場合があります。</p> 
    <ul> 
     <li> <p>[!UICONTROL Business Case]の[!UICONTROL Resource Budgeting]エリア、またはプロジェクトの担当業務のコストに関連付けられた [!UICONTROL Resource Planner] に表示される労務費。[!UICONTROL Budgeted Labor Cost] の計算の詳細は、<a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">プロジェクトの [!UICONTROL Understand Budgeted Labor Cost] および [!UICONTROL Budgeted Hours]</a>の記事を参照してください。</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>シナリオプランナーを使用してプロジェクトリソースを予算計上する場合、[!DNL Scenario Planner] からプロジェクトにリンクされたイニシアチブで推定された[!UICONTROL People Costs]を反映する [!UICONTROL Business Case]の[!UICONTROL Resource Budgeting]エリアに表示される労力コスト。イニシアチブについての情報は、<a href="../../../scenario-planner/initiatives-overview.md" class="MCXref xref">シナリオプランナーのイニシアチブの概要</a>を参照してください。 </p> <p>[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] についての詳細は、<a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">[!DNL Scenario Planner] の概要</a>を参照してください。 </p> </li> 
     <p>次の領域に以下の名前で表示されます。</p>
   <ul>
   <li><strong>[!UICONTROL Budgeted Labor Cost]</strong>：[!UICONTROL Business Case]の[!UICONTROL Resource Budgeting]エリア内。
   <li><strong>[!UICONTROL Budgeted Cost]</strong>：[!UICONTROL Utilization] レポート [!UICONTROL Cost] ビュー内
   <p>詳しくは、<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">リソース稼働率情報の表示</a>を参照してください。</p>
   <li>コスト別表示時の [!DNL Resource Planner] プロジェクトまたは [!DNL Role] ビュー内の<strong>[!UICONTROL BDG]</strong>
   <li><strong>[!DNL Resource Planner Budgeted Labor Cost]</strong>：次のレポート内 
   <ul>
    <li>[!UICONTROL Project] レポート</li>
    <li>[!UICONTROL Project (Financial Data)] レポート</li>
    <li>[!UICONTROL Task] レポート</li>
    <li>[!UICONTROL Issue] レポート</li>
    <li>[!UICONTROL Budgeted Hour] レポート</li> 
    </ul>
    <p>レポートの作成についての詳細は、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>の記事を参照してください。</p>
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
   <td>[!UICONTROL Budgeted Start Date]</td> 
  <td> <p>これは非推奨のフィールドです。このフィールドに表示される情報はすべて、[!DNL Workfront]が削除した機能に関連しています。このフィールドは更新できません。</p>
  <p>これらのエリアは[!DNL Workfront]から削除されました。 </p> 
  <p>このフィールドは、[!UICONTROL project] および [!UICONTROL task] のレポートとリストに引き続き表示されます。</p>
   <!--
   <p>This field shows the date when the budgeting of resources starts, as defined in the Legacy Resource Estimates area of the Business Case of a project, or the Capacity Planner.</p>
   -->   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Burndown Chart]</td> 
   <td>完了した作業と残りの作業を視覚的に表現する折れ線グラフ。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case]</td> 
   <td> <p>プロジェクトを [!UICONTROL Idea] ステータスから [!UICONTROL Planning] ステータスに移行する必要があるかどうかを評価するために使用されるツール。言い換えれば、[!UICONTROL business case] は、特にポートフォリオ内の他のプロジェクトと比較する場合に、当該のプロジェクトを開始して完了することが重要かどうかを判断するのに役立ちます。</p> <p>詳しくは、<a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">プロジェクトの [!UICONTROL Business Case] を作成 </a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Business Case Budgeted Hours]</td> 
   <td> <p>これは非推奨のフィールドです。このフィールドに表示される情報はすべて、[!DNL Workfront]が削除した機能に関連しています。このフィールドは更新できません。</p> <p>このフィールドは、プロジェクトおよび [!UICONTROL task] リストとレポートに引き続き表示されます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Assignment]</td> 
   <td> <p>タスク [!UICONTROL 期間タイプ ] の 1 つ。 これにより、タスクの [!UICONTROL Duration] と [!UICONTROL Work Required] に基づいて、タスクに割り当てられたユーザーが 1 日 8 時間の労働時間のうち、そのタスクに割り当てられる割合が計算されます。</p> <p>詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの [!UICONTROL Duration] と [!UICONTROL Duration Type] の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calculated Work]</td> 
   <td> <p>タスクの [!UICONTROL Duration Types] のうちの 1 つ。これにより、[!UICONTROL Duration] とユーザーの[!UICONTROL Assignment]割合（1 日 8 時間の作業に基づく）を指定して、タスクの[!UICONTROL Work Required]が計算されます。</p> <p>詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの [!UICONTROL Duration] と [!UICONTROL Duration Type] の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Calendar]</td> 
   <td> <p>[!DNL Workfront] には 2 つのタイプのカレンダーがあります。[!UICONTROL Home Calendar] およびカレンダーレポートです。</p> <p>[!UICONTROL Home Calendar] は、ユーザーが[!DNL Workfront]の空き時間に対して、自分の作業負荷を管理できる個人用カレンダーです。また、[!UICONTROL Home Calendar] を [!DNL Outlook] ([!DNL Google] および [!DNL Microsoft] 統合に関する情報が含まれます )。 </p> <p>[!UICONTROL Home Calendar] について詳しくは、<a href="../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md" class="MCXref xref">[!UICONTROL Home Calendar] のビュー</a>を参照してください。</p> <p>カレンダーレポートは、ユーザーが期日、作業ステータス、イベントが割り当てられているユーザーなど、イベントの日付やその他の重要な詳細を表示できる動的なレポートです。</p> <p> カレンダーレポートについて詳しくは、<a href="../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md" class="MCXref xref">カレンダーレポートの概要</a>を参照してください。</p> </td> 
  </tr> 
   <tr> 
   <td>[!UICONTROL Can Start]</td> 
   <td> <p>このフィールドは、タスクの作業を開始する準備ができているかどうかを示します。開始の準備ができている場合、タスクの [!UICONTROL Can Start] フィールドが [!UICONTROL True] に設定されます。 </p> <p>詳しくは、<a href="../../../manage-work/tasks/task-information/can-start-task-overview.md" class="MCXref xref">タスクの「[!UICONTROL Can Start]」の概要</a>を参照してください。</p> 
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
   <td> <p>作業に割り当てることができるリソースの空き時間。「空き時間」を参照してください。 </p></td> 
  </tr>

<tr> 
   <td> <p>[!UICONTROL Category]</p> </td> 
   <td> <p>カテゴリはカスタムフォームです。このオブジェクトに関するレポートを作成し、他のオブジェクトレポートにも表示できます。すべてのオブジェクトがカスタムフォームやカテゴリを持つことができるわけではありません。以下のオブジェクトは、カスタムフォームを持つことができます。<br></p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Portfolio]</li> 
     <li>[!UICONTROL Document]</li> 
     <li>[!UICONTROL Expense]</li> 
     <li>[!UICONTROL Program]</li> 
     <li>[!UICONTROL User]</li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li></ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Category Name]</td> 
   <td> <p>次のいずれかのオブジェクトのビューに列として追加されると、それらのオブジェクトに関連付けられているすべてのカスタムフォームのリストが表示されます。</p> 
    <ul> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Task]<br></li> 
     <li>[!UICONTROL Issue]<br></li> 
     <li>[!UICONTROL Portfolio]<br></li> 
     <li>[!UICONTROL Document]<br></li> 
     <li>[!UICONTROL Expense]<br></li> 
     <li>[!UICONTROL Program]<br></li> 
     <li>[!UICONTROL User]<br></li> 
     <li>[!UICONTROL Company]</li> 
     <li>[!UICONTROL Iteration]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Management]</td> 
   <td>スコープ、スケジュール、コスト、リソースの要因の変化に対して、予定作業を定義し、理解し、適応させることに焦点を当てた実施領域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Change Order]</td> 
   <td>プロジェクトに対して発生するイシューの一種で、同意されたスコープに対して要求された変更の概要を示します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Only]</td> 
   <td>[!UICONTROL Update Types] プロジェクトの 1 つ。 プロジェクトまたはタスクでタスクまたは編集が実行された場合にのみ、[!UICONTROL Project Project Project Projected] および [!UICONTROL Planned] タイムラインが更新されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change Order]</td> 
   <td> <p>[!UICONTROL Issue] の種類の 1 つであり、通常、プロジェクトを完了する前に、計画外の量の作業が必要であることを示します。</p> <p>[!UICONTROL Issue] のタイプについて詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md" class="MCXref xref">デフォルトのイシュータイプをカスタマイズ</a>の記事で、「デフォルトのイシュータイプ」の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Child Task]</td> 
   <td>[!UICONTROL Parent Task]（[!UICONTROL Summary Task]）の [!UICONTROL Subtask] であるタスクです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Children]</td> 
   <td>[!UICONTROL Parent Task]（[!UICONTROL Summary Task]）の [!UICONTROL Subtasks] のコレクションです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coaching] と [!UICONTROL Training]</td> 
   <td>学習モジュール、認定、標準、または実践コミュニティです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit]</td> 
   <td>ユーザーがタスクの成果物に関する期待を設定するためのコミュニケーションツールです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Commit Date]</td> 
   <td>ユーザーがタスクの成果物に関する期待を設定するためのコミュニケーションツールです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Communication] と [!UICONTROL Reporting]</td> 
   <td>プロジェクト、プログラムまたはポートフォリオの例外と正常性を確認するための基準</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Company]</td> 
   <td> <p>[!UICONTROL Company] は、[!DNL Workfront] の組織単位です。 </p> 
   <p> ユーザーまたはプロジェクトを 1 つの会社に関連付けることができます。詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md">会社の作成と編集</a>を参照してください。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion date]</td> 
   <td> <p>プロジェクト、タスク、またはイシューが完了するように設定した日付です。[!DNL Workfront] の [!UICONTROL Completion dates] には複数のタイプがあります。</p> 
    <ul> 
     <li>[!UICONTROL Actual Completion Date]。詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">プロジェクトの [!UICONTROL Actual Completion Date] の概要</a>を参照してください。</li> 
     <li>[!UICONTROL Planned Completion Date]。詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">プロジェクトの [!UICONTROL Planned Completion Date] の設定</a>および<a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">タスクの [!UICONTROL Planned Completion Date] の概要</a>を参照してください。</li> 
     <li>[!UICONTROL Projected Completion Date]詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">プロジェクト、タスクおよびイシューの [!UICONTROL Projected Completion Date] の概要</a>を参照してください。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Day]</td> 
   <td>[!UICONTROL Template] の開始日を基準として、[!UICONTROL Template Task] または [!UICONTROL Template] が完了すると想定される日です。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Completion Mode]</td> 
   <td> <p>これは、プロジェクトが [!UICONTROL Complete] としてマークされる方法を示します。次の 2 つの値を持つことができます。</p> 
    <ul> 
     <li>[!UICONTROL Manual]：ユーザーは、プロジェクトステータスを [!UICONTROL Complete] に変更する必要があります。</li> 
     <li>[!UICONTROL Automatic]：プロジェクト内のすべてのタスクが 100％完了し、すべてのイシューがクローズされると、プロジェクトステータスは自動的に [!UICONTROL Complete] に変わります。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition]</td> 
   <td> <p>これは、タスク、イシュー、プロジェクトの進行状況を視覚的に表現したものです。</p> <p>プロジェクトの場合、条件はプロジェクト所有者が手動で設定することも、プロジェクトの進捗ステータスに基づいて[!DNL Workfront]により自動で設定することもできます。 </p> <p>プロジェクト条件に指定できる値は以下のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL On Target]</li> 
     <li>[!UICONTROL At Risk]</li> 
     <li>[!UICONTROL In Trouble]</li> 
    </ul> <p>プロジェクト条件の詳細については、「 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">[!UICONTROL Project Condition] と [!UICONTROL Condition Type] の概要</a>.</p>
     <p>タスクとイシューの条件を、レポートに表示できる数値に関連付けることができます。以下のリストには、タスクとイシューの条件に対するデフォルトの名前と数値が表示されます。システム管理者は、条件の名前をアップデートし、異なる数値の新しい条件を追加できます。数値を条件に関連付けると、その数値は編集できなくなります。  </p> 
     <p>タスクの場合、条件はタスク責任者が手動で設定します。タスク条件に指定できる値は以下のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly]（0）<br></li> 
     <li> [!UICONTROL Some Concerns]（1）<br></li> 
     <li>[!UICONTROL Major Roadblocks]（2）</li> 
    </ul> <p>タスク条件の詳細については、「 <a href="../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">タスクと問題に関する [!UICONTROL 条件 ] の更新</a>.</p> <p>イシューの場合、条件はイシュー所有者が手動で設定します。イシューの条件に指定できる値は以下のとおりです。<br></p> 
    <ul> 
     <li>[!UICONTROL Going Smoothly]（0）<br></li> 
     <li>[!UICONTROL Some Concerns]（1）<br></li> 
     <li>[!UICONTROL Major Roadblocks]（2）</li> 
    </ul> 
   <p><b>メモ</b></p>
    <p>[!UICONTROL Journal Entry] レポートで [!UICONTROL Condition] フィールドが追跡されると、[!UICONTROL New] および [!UICONTROL Old Number Values] には、名前の代わりに条件に関連付けられた数値が表示されます。もともとタスクまたはイシューに対して条件が定義されておらず、後でアップデートした場合、アップデートをキャプチャするジャーナルエントリには、[!UICONTROL Condition] フィールドの [!UICONTROL Old Number Value] が -2,147,483,648 と表示されます。この記事の「[!UICONTROL New Number Value]」、「[!UICONTROL Old Number Value]」、「[!UICONTROL Journal Entry]」も参照してください。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Condition Update]</td> 
   <td> <p>このフィールドには、タスク、プロジェクト、イシューの現在の状態が表示されます。このオプションは、タスク、プロジェクト、イシューの所有者が [!UICONTROL Update Status] フィールドに提供した最新のアップデートと、新しい条件が表示されます。</p> <p>条件のアップデートに対しておこなわれたコメントは、[!UICONTROL Condition Update] 列には表示されません。メインのアップデートのみが表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Date]</td> 
   <td> <p>[!UICONTROL Must Start On] など、特定の日付に結び付けられた [!UICONTROL Task Constraint] を使用している場合、その特定の日付はタスクの [!UICONTROL Constraint Date] になります。</p> <p>以下のタスクの制約で [!UICONTROL Constraint Date] フィールドがアップデートされます。</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>ヒント</b></p>   
     <ul> 
      <li> <p>[!UICONTROL Fixed Dates] の [!UICONTROL Constraint] を持つタスクには、[!UICONTROL Constraint Date] がありません。 </p> </li> 
      <li> <p> [!UICONTROL Constraint Date] は、レポートまたはカスタマイズされたビューでのみ表示できます。</p> </li> 
     </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Day]</td> 
   <td> <p>「指定日に開始」など、特定の日に関連付けられたテンプレートタスクでタスクの制約を使用している場合、その特定の日がテンプレートタスクの制約の条件日になります。</p> <p>以下のタスクの制約で、[!UICONTROL Constraint Day] フィールドがアップデートされます。</p> 
    <ul> 
     <li>[!UICONTROL Must Start On]</li> 
     <li>[!UICONTROL Must Finish On]</li> 
     <li>[!UICONTROL Start No Later Than]</li> 
     <li>[!UICONTROL Start No Earlier Than]</li> 
    </ul> <p><b>ヒント</b></p> <p>  [!UICONTROL 制約日 ] は、レポートまたはカスタマイズされたビューでのみ表示できます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Constraint Type]</td> 
   <td> <p>タスクのスケジュール傾向。 例えば、[!UICONTROL 可能な限り早く ] はタスクの開始をスケジュールし、[!UICONTROL 次の日まで ] はタスクの終了を [!UICONTROL 制約日 ] 以降にスケジュールします。</p> <p>詳しくは、<a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">[!UICONTROL Task Constraint] の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Contextual Menu]</td> 
   <td>画面の左側にあるメニューで、項目はアクティブなコンテンツとの関連付けで変化します。例えば、ユーザーがプロジェクトを表示している場合、[!UICONTROL コンテキストメニュー ] には、プロジェクトに関連する情報およびツールへのリンクが表示されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Converted Issue Originator]</td> 
   <td>イシューがプロジェクトまたはタスクに変換されるときに、イシューの [!UICONTROL Primary Contact] であるユーザーに関する情報を表示する、プロジェクトまたはタスクレポート内のフィールド。このフィールドは、[!UICONTROL Project Details] セクションにも表示され、変換後のイシューの [!UICONTROL Primary Contact] の名前が表示されます。この記事の「[!UICONTROL Primary Contact]」も参照してください。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Cost]</td> 
   <td> <p>プロジェクト、タスク、イシューの完了時に費やす必要がある金額です。 </p> <p>プロジェクトに関連する労力コスト、経費、リスクなど、様々なタイプのコストを追跡できます。[!DNL Workfront]でのコストの追跡については、<a href="../../../manage-work/projects/project-finances/track-costs.md">コストを追跡</a>を参照してください。</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cost Type]</td> 
   <td>タスクの場合、[!UICONTROL Cost Type] が、タスクによってコストがどのように発生するかを決定します。例としては、[!UICONTROL Fixed Hourly]、[!UICONTROL User Hourly]、[!UICONTROL User Hourly plus Fixed] などがあります。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cross-Project Dependencies]</td> 
   <td> <p>1 つのプロジェクトのタスクは、別のプロジェクトのタスクに依存しています。</p> <p>詳しくは<a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">プロジェクト間の先行タスクを作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Custom Data]</td> 
   <td> <p>組織に固有のデータ。組織は、カスタムフォームとカスタムフィールドを作成して、[!DNL Workfront] アプリケーションをカスタマイズすることができます。このカスタム情報により、KPI、監査、およびデマンドミックスに関するレポーティングを促進することができます。 </p> <p>[!UICONTROL Custom Data] は以下のものにリンクできます。</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Iterations]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Data Type]</td> 
   <td>[!UICONTROL Custom Data] フィールドをテキスト、日付、数値、通貨のいずれでデータベースに格納するかを指定するオプション。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Display Type]</td> 
   <td>カスタムフィールドのフィールドの表示タイプ。例としては、[!UICONTROL Drop-Down]、[!UICONTROL Text Field]、[!UICONTROL Text Area]、[!UICONTROL Radio Buttons] などがあります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Field]</td> 
   <td>ユーザーが複数のオプションから選択できるカスタムデータの場合、これらの値はユーザーが選択できる値です。 カスタムオプションは、[!UICONTROL Drop-Down]、[!UICONTROL Multi-Select Drop-Down]、[!UICONTROL Radio Buttons] および [!UICONTROL Checkboxes] でのみ有効です。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Form Label]</td> 
   <td>Custom Options で Custom Display Type を使用する場合、これは、その Custom Option のドロップダウンメニュー、チェックボックス、またはラジオボタンに表示されるユーザーインターフェイステキストです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Value]</td> 
   <td>カスタムオプションでカスタムフィールドを使用する場合、この値は、特定のオプションに対してデータベースに格納されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom View]</td> 
   <td>リスト内の各オブジェクトに対して表示されるデータフィールドまたは列の定義。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Customer]</td> 
   <td>Workfront のインスタンスを使用する組織。</td> 
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
   <td>[!UICONTROL Dashboards]</td> 
   <td> <p> このフィールドをレポートまたはレポートオブジェクトのビューに追加して、レポートがリストに表示されているダッシュボードを表示できます。 </p> <p> このフィールドを使用して、特定のダッシュボードにリストされているレポートをフィルタリングすることもできます。 </p> <p> レポートオブジェクトレポートにダッシュボード情報を含める方法について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/access-organize-reports.md" class="MCXref xref">レポートへのアクセスと整理</a>の記事にある「ダッシュボードにリストされるレポートの内容について」の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data Type]</td> 
   <td>「[!UICONTROL Custom Data Type]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Days Late]</td> 
   <td> <p>このフィールドには、[!UICONTROL Actual Completion Date] がない場合に、[!UICONTROL Planned Start] と [!UICONTROL Today] の日付差が表示されます。</p> <p>また、[!UICONTROL Actual Completion Date] が存在する場合に、[!UICONTROL Actual Completion] と [!UICONTROL Planned Completion] の間の日付差も表示します。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Default Schedule]</td> 
   <td> <p>組織内のユーザーおよびプロジェクトに割り当てられる、カスタマイズ可能なデフォルトの作業時間。 </p> <p>スケジュールは、ユーザーに割り当てられたタスクの予定日、開始日、完了日を計算するために使用されます。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Deliverable]</td> 
   <td>プロジェクトの完了時に提供する必要がある定量化可能な商品またはサービス。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Demand Management]</td> 
   <td>取り込みプロセスのスコア付けと優先順位付け。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Department Goals]</td> 
   <td>部門内の運用指標の改善に焦点を当てた、特定の部門に固有の目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency]</td> 
   <td>2 つのタスク間のリンクであり、一方のタスクがステータスを変更する前に、もう一方のタスクもステータスを変更する必要があるもの。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dependency Type]</td> 
   <td> <p>タスクとその先行タスクとの間のスケジューリング関係のタイプ。1 つの例は [!UICONTROL Finish-Start] です。この場合、最初のタスクは、2 番目のタスクが開始する前に完了させる必要があります。</p> <p>詳しくは、<a href="../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md" class="MCXref xref">タスク依存関係タイプの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document]</td> 
   <td>[!DNL Workfront] 内のオブジェクトに添付されたファイル。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Document Version]</td> 
   <td> <p>同じドキュメントが同じオブジェクトにアップロードされるたびに、バージョン番号が割り当てられます。ユーザーは、ドキュメントの以前のバージョンの複数のオプションを表示および変更できます。</p> <p>詳しくは、<a href="../../../documents/managing-documents/manage-document-versions.md" class="MCXref xref">ドキュメントバージョンを管理</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration]</td> 
   <td> <p>タスク、イシューまたはプロジェクトの完了に割り当てられる時間のウィンドウ（[!UICONTROL Planned Start] と予定完了日の間の日数によって決定されます）。</p> 
    <ul> 
     <li>タスクの場合、タスクの期間タイプが単純でない場合、期間は編集可能なフィールドです。タスクの期間タイプが単純な場合、またはタスクの制約が固定日付の場合、期間は Workfront が計算します。</li> 
     <li>イシューの場合、期間は常に編集可能なフィールドで、イシューの解決に必要な日数の見積りを表す必要があります。</li> 
     <li>プロジェクトの場合、期間は [!DNL Workfront] が計算します。プロジェクトの最も早いタスクの予定開始日と最終タスクの [!UICONTROL Planned Completion] の間の日数の差を表します。</li> 
    </ul> <p>タスクの [!UICONTROL Duration] と [!UICONTROL Planned Duration] の差について詳しくは、<a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md">タスクの [!UICONTROL Planned Duration] と [!UICONTROL Duration] の差</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Duration in Minutes]</td> 
   <td>このフィールドには、[!UICONTROL Duration] フィールドと同じ情報が日数ではなく分単位で表示されます。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc,QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Duration per Occurrence]</td> 
   <td> <p>これは、繰り返しタスクの親の [!UICONTROL Task Details] ボックスと [!UICONTROL Edit Task] ボックスに表示されます。各定期タスクの期間を表示します。繰り返しタスクの作成について詳しくは、<a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">繰り返しタスクを作成</a>を参照してください。 </p> <p> <span>個々の繰り返しタスクで変更された期間には、このフィールドに示された値は表示されません。</span> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Duration Type]</td> 
   <td> <p>タスクフィールドには、タスクを完了するために必要な作業が、タスク期間全体にわたって担当者にどのように割り当てられるかが示されます。これは、タスクの [!UICONTROL Duration]、[!UICONTROL Work Required]、および割り当てられたリソースがタスクを完了するために費やすべき時間、すなわち [!UICONTROL Allocation] の関係を表しています。 </p> <p>このフィールドは、タスクの「[!UICONTROL Details]」タブに表示されます。 </p> <p>タスクの「期間の種類」には、次のオプションがあります。</p> 
    <ul> 
     <li>[!UICONTROL Calculated assignment]</li> 
     <li>[!UICONTROL Calculated Work]</li> 
     <li>[!UICONTROL Effort Driven]</li> 
     <li>[!UICONTROL Simple]</li> 
    </ul> <p>詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの [!UICONTROL Duration] および [!UICONTROL Duration Type] の概要</a>を参照してください。</p> 
    --&gt; </td> 
   </tr> 
   <tr> 
   <td>[!UICONTROL Duration Unit]</td> 
   <td>パワー検索で時間を測定するために使用される単位。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Effort Driven]</td> 
   <td>ユーザー数とタスクが完了するまでに要する時間との関係。ユーザーを追加すると、タスクの完了に予定される合計時間は短くなりますが、タスクの期間は変わりません。例えば、ピーナッツの殻を剥くタスクの場合、人数を増やすと予定時間が短縮されますが、人日の期間は変わりません。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elapsed Time]</td> 
   <td> <p>[!UICONTROL Elapsed time] は、タスクの [!UICONTROL Duration] の時間の単位です。タスクの [!UICONTROL Planned Start Date] から [!UICONTROL Planned Completion Date] までの時間で、休日、週末、休日が含まれます。つまり、経過時間はカレンダーの日数の経過です。 </p> <p>[!DNL Workfront] タスクの期間に関して、次の経過時間単位をサポートします。</p> 
    <ul> 
     <li> <p>[!UICONTROL Elapsed Minutes]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Hours]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Days]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Weeks]</p> </li> 
     <li> <p>[!UICONTROL Elapsed Months]</p> </li> 
    </ul> <p>経過時間を含めたタスクの期間について詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスクの [!UICONTROL Duration] および [!UICONTROL Duration Type] の概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL End Date]</td> 
   <td> <p> [!UICONTROL Rate] レポートでは、プロジェクトレベルでの担当業務に対する新しい請求レートが終了する日付です。この日付より前のプロジェクトに関連する時間にこの請求レートを掛けて、プロジェクトの収益を計算します。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Engagement]</td> 
   <td>タスク、プロジェクト、チームまたは組織に対するコミットメントと信念の減少を示す [!UICONTROL Work Performance Indicator]（WPI）。これは、その信念とコミットメントを復活させるために行動する必要があることを示します。WPI は、「自分に何が期待されているか理解できましたか？」のような簡単な質問をすることで測定されます。あなたが担当した作業は、組織に対して何か影響がありましたか？仕事はうまくいきましたか？」</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Enterprise Goals]</td> 
   <td>企業目標の指標に貢献する部門をまたいだ目標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event]</td> 
   <td>プロジェクトまたはタスクに対する変更。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event Handler]</td> 
   <td>イベントの発生時に発生する自動化されたタスク。一般的な例として、自動メール通知が挙げられます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Event notification]</td> 
   <td>イベントハンドラーから生成されたメール。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Expenses]</td> 
   <td>タスクまたはプロジェクトに関する労力以外のコスト。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External]</td> 
   <td> <p>通常、これはライセンスの種類、またはそのようなライセンスを持つユーザーです。 このようなライセンスタイプを持つユーザーは、システム内の情報を確認するだけで済みます。 彼らは積極的に仕事に参加できない。</p> <p>詳しくは、<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]ライセンスの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL External System]</td> 
   <td>指定された記録システムの外部に保存および管理されるサービスまたはソフトウェア。</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Field]</td> 
   <td><p>データベースに表示される任意の Workfront オブジェクトまたはそれに関連付けられている情報。 </p>
   <p>例えば、「プロジェクト」、「ユーザー」、「時間」は、Workfront オブジェクトとフィールドの両方です。「名前」、「ステータス」、「所有者」、「開始日」は、上記のオブジェクトに関連付けられた Workfront フィールドです。 </p>

<p>オブジェクトを参照する場合、「オブジェクト」と「フィールド」という用語は同じ意味で使用できます。</p>
   <p>レポートの範囲では、「フィールド」は、レポートに取り込むオブジェクトまたはオブジェクトに関する情報を指します。</p>

<p><b>メモ</b></p>

<p>テキストの詳細レポートでは、フィールドは、データベースに表示されるオブジェクトまたはその情報を参照します。</p>
   <p>ユーザーインターフェイスに表示される名前が、データベースのフィールドの名前と異なる場合があります。 例えば、「イシュー」は Workfront インターフェイスのオブジェクトの名前ですが、「opTask」は Workfront データベースのオブジェクト（またはフィールド）の名前です。 </p> 
   <p> テキストモードのレポートの書き込み、表示、フィルターまたはグループ化の際、または計算フィールドの作成時に、データベースに表示されるフィールドを使用することが重要です。</p>

<p>詳しくは、<a href="../../../wf-api/general/api-explorer.md">API エクスプローラー</a>および<a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md">テキストモードの概要</a>を参照してください。</p>

<p>デフォルトでは、Workfront には、オブジェクトとその情報の両方を定義する一連のフィールドが用意されています。カスタムフィールドを作成してオブジェクトを定義することもできますが、カスタムオブジェクトを作成することはできません。</p> 
   </td> 
  </tr>

<tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Filter]</td> 
   <td> <p>画面に表示される情報を定義する、レポート要素またはリスト要素を構成する主要な部品の 1 つです。レポート要素について詳しくは、<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">レポート要素：フィルター、ビューおよびグループ化</a>を参照してください。</p> <p>フィルターは、プロジェクト、タスク、イシューなど、レポートまたは [!DNL Workfront] パネルのリストに表示される結果を決定します。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Financial Work Management]</td> 
   <td>[!DNL Workfront] で人件費、経費、収益データを管理するプロセスです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Cost]</td> 
   <td>プロジェクトの固定コストを定義できます。これは、プロジェクトの [!UICONTROL Planned Cost] の一部であり、プロジェクトを完了するために必要な金額を表します。コストについて詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Fixed Revenue]</td> 
   <td>プロジェクトの固定収益額を定義することができます。これはプロジェクトの [!UICONTROL Planned Revenue] の一部であり、プロジェクトが完了すると得られるであろう金額を表しています。収入について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Flags]</td> 
   <td> <p> これは [!UICONTROL Status Icons] と同じフィールドですが、次の表示でのみ使用できます。 </p> 
    <ul> 
     <li> [!UICONTROL Templates] </li> 
     <li> [!UICONTROL Expenses] </li> 
    </ul> <p> 詳しくは、<a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">ビュー内のビルトインのステータスアイコン</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td>フォルダーは、オブジェクトに関連付けられたドキュメントまたはレポートを整理するために使用されます。</td> </tr>
  <tr>
  <td>[!UICONTROL FTE]（フルタイム換算）</td> 
   <td>これはフルタイム換算であり、リソースを作業に使用できる時間を示します。
[!UICONTROL FTE] フィールドは、次のエリアに表示されます。 
  <ul>
   <li> ユーザーのプロファイル（ユーザーを編集または作成する際） </li>
   <li> [!UICONTROL Resource Planner] </li>
   <li> [!UICONTROL Scenario Planner]（Workfront Scenario Planner の追加ライセンスが必要） </li>
   <li> ユーザーリストとレポート </li> </ul>

<p>[!UICONTROL FTE] は、1 以下の小数で指定する必要があり、0 にはできません。 </p>
   <p> [!UICONTROL FTE] が 1（ユーザーのプロファイルで定義されている [!UICONTROL FTE] フィールドのデフォルト）の場合、リソース（ユーザーまたは役割）は、空き時間を計算したスケジュールに基づいて、時間数全体でその作業に携わることを意味します。 </p>
   <p>Workfront 管理者が、ユーザーの空き時間の判断にどのスケジュールを使用するかを決定します。  </p>
   <ul>
   <li> [!UICONTROL Default Schedule]では、Workfront はユーザーのプロファイル内にある [!UICONTROL FTE] を使用して空き時間を計算します。 </li>
   <li> ユーザーのスケジュールを使用すると、Workfront はユーザーの休暇、[!UICONTROL Work Time] 値および [!UICONTROL Default Schedule] の時間を使用して、ユーザーの [!UICONTROL FTE] を計算します。 </li> </ul>

<p>詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理の環境設定</a>を参照してください。  </p>
   <p>[!DNL Workfront] でのスケジュール作成について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールを作成</a>を参照してください。 </p>

<p><b>メモ</b></p>
   <p>[!UICONTROL Scenario Planner] のすべての計算に対して、Workfront は 1 [!UICONTROL FTE] = 8 時間という値を使用します。</p>
   <p>詳しくは、<a href="../../../scenario-planner/get-started-with-scenario-planning.md">[!UICONTROL Scenario Planner] の概要</a>を参照してください。 </p>
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
   <td>[!UICONTROL Gantt Chart]</td> 
   <td> <p>プロジェクトの日付をカレンダービューで示した視覚的なタイムラインです。プロジェクトのタスクが現在スケジュールされている、予定日または見込日に基づいています。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal]</td> 
   <td><p>[!DNL Workfront] には、目標の概念 2 つがあります。 </p> 
    <ul> 
     <li> <p><b>プロジェクト目標</b>：プロジェクトに関わる利益関係者と合意した一連のビジネス目標です。プロジェクト目標は、プロジェクトのビジネスケースの一部です。 </p> <p>プロジェクト目標をリストやレポートに表示することはできませんが、API を使用してアクセスできます。 </p> <p>ビジネスケースのプロジェクト目標について詳しくは、<a href="../../../manage-work/projects/define-a-business-case/create-business-case-goals.md">ビジネスケース目標の作成</a>を参照してください。 </p> </li> 
     <li> <p><b>戦略的目標</b>：戦略的目標は、特定の期間、作業戦略を計画するために作成する目標です。[!DNL Workfront Goals] を使用して、このタイプの目標を作成できます。戦略的目標を作成するには、組織が追加のライセンスを購入し、この機能へのアクセス権を持っていることが必要です。[!DNL Workfront Goals] は、追加のライセンスでのみ使用できます。</p> 
     <p>詳しくは、<a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals]概要</a>を参照してください。 </p> 
     <p>目標またはプロジェクトレポートに戦略目標を表示し、API を使用してそれらにアクセスできます。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Hierarchy]</td> 
   <td> <p>[!UICONTROL Goal] および [!UICONTROL Project] レポートで、これは、戦略目標が他の目標と一致する場合に戦略目標が属する階層内の目標を表示するコレクションフィールドです。目標は▸区切り文字で区切られます。 </p> <p>このフィールドには、目標と目標の親のみが表示されます。子の目標は表示されません。 </p> <p>[!DNL Workfront Goals] での目標の整合について詳しくは、<a href="../../../workfront-goals/goal-alignment/goal-alignment-overview.md">[!DNL Workfront Goals]</a> の目標の整合の概要を参照してください。 </p> 
   <p>このフィールドは、組織が [!DNL Workfront Goals] を購入した場合のみに表示されます。[!DNL Workfront Goals] を使用した戦略目標の管理について詳しくは、<a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] 概要</a>を参照してください。 </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Goal Success Score]</td> 
   <td> [!UICONTROL Project report] では、このフィールドは、[!UICONTROL Business] ケースに関連付けられたプロジェクトレベルの目標を指すために使用されます。現在、これは非推奨のフィールドで、機能に関連付けられていません。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Goals] </td> 
   <td> <p>[!UICONTROL Project] レポートでは、これはプロジェクトに関連付けられているすべての戦略目標を表示するコレクションフィールドです。目標はコンマで区切ります。</p> <p>このフィールドは、組織が [!DNL Workfront Goals] を購入した場合にのみ表示されます。[!DNL Workfront Goals] を使用した戦略目標の管理について詳しくは、<a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] 概要</a>を参照してください。[!DNL Workfront] での戦略目標とプロジェクト目標について詳しくは、この記事の「[!UICONTROL Goal]」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global Interface Preferences]</td> 
   <td>すべてのユーザーに影響するインターフェイス設定。[!UICONTROL Global Interface Preferences] は、[!UICONTROL User Interface Preferences] で上書きできます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Group]</td> 
   <td> <p>同じオブジェクトにアクセスできるユーザー（同じ部門またはビジネスユニットからの場合もあります）のコレクション。ユーザーに加えて、グループをポートフォリオ、プログラム、プロジェクト、<span> プロジェクトテンプレート、</span> 会社、チーム、スケジュール、レイアウトテンプレートおよびタイムシートプロファイルに関連付けることができます。</p> <p>また、オブジェクトにグループ別の権限を付与することもできます。詳しくは、<a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">グループの概要</a>を参照してください。</p> <p>次のいずれかのタイプのオブジェクトのリストまたはレポートで、[!UICONTROL Group] フィールドを使用して、特定のグループに関連付けられている特定のタイプのオブジェクト、ユーザー、ポートフォリオ、プログラム、プロジェクト、<span>プロジェクトテンプレート</span>、会社、チーム、スケジュール、レイアウトテンプレートまたはタイムシートプロファイルを一覧表示できます。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Group Administrator]</td> 
   <td> <p>指定したユーザーグループのオブジェクト、アクセスおよびユーザーを管理するユーザー。</p> <p> [!UICONTROL Group] レポートのこのフィールドには、グループで [!UICONTROL Group Administrators] に指定されたユーザーの名前が表示されます。グループ管理者について詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group with Administration Access]</td> 
   <td> <p> [!UICONTROL Layout Template]、[!UICONTROL Timesheet Profile] または [!UICONTROL Schedule report] で、このフィールドには、グループ管理者がテンプレートを変更するためのアクセス権を持つグループが表示されます。また、このフィールドでこのレポートをフィルタリングすることもできます。 </p> <p> 詳しくは、<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">レイアウトテンプレートの作成と管理</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Grouping]</td> 
   <td> <p>リスト内の情報を共通の基準で分類するために使用されるレポート要素。</p> <p>詳しくは、<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">レポート要素：フィルター、ビューおよびグループ化</a>の記事の「[!UICONTROL Groupings]」の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Handoff Date]</td> 
   <td> <p>タスクが作業可能になる日付。[!UICONTROL Handoff Date] は計算される日付で、手動で設定することはできません。<br>[!UICONTROL Handoff Date] について詳しくは、<a href="../../../manage-work/tasks/task-information/handoff-task-date.md" class="MCXref xref">[!UICONTROL Task Handoff Date] の概要</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Help Desk]</td> 
   <td>の [!UICONTROL リクエスト ] 領域を表す別の名前 [!DNL Workfront]. [!UICONTROL リクエスト ] 領域を使用して、カスタマーサポートチケット、プロジェクトリクエスト、ヘルプデスクチケットなどを処理できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Owner]</td> 
   <td>[!UICONTROL Hour] レポートでは、[!UICONTROL Owner] はその時間が属するユーザーです。これは、実際に時刻を記録しているユーザーとは異なります。 この 2 つのエンティティは、2 人の異なるユーザーになる場合があります。<br>別のユーザーへの時間の記録について詳しくは、<a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">時間を記録</a>の記事を参照してください。</td> 
  </tr>

<tr> 
   <td>時間ステータス</td> 
   <td> <p>タスク、イシューまたはプロジェクトに関してユーザーがログに記録する実際の時間に対して Workfront が設定する属性です。 </p>

Workfront では、時間エントリには次のいずれかのステータスを設定できます。
<ul>
   <li><b>送信済み</b>：プロジェクト、タスクまたはイシューに記録されている時間。これらは請求記録に含まれているか、まだ請求記録に追加されていません。</li>
   <li><b>承認済み</b>：時間がログに記録され、プロジェクト所有者によって承認されています。これらは請求記録に含まれているか、まだ請求記録に追加されていません。</li> 
   <li><b>未承認</b>：時間がログに記録され、プロジェクト所有者によって拒否されています。これらは請求記録に含まれているか、まだ請求記録に追加されていません。</li>
   <li><b>請求済み</b>：時間が記録され、請求記録に追加され、請求記録のステータスが請求済みとマークされています。プロジェクト所有者の承認は必要ありませんでした。</li>
   <li><b>請求済みおよび承認済み</b>：時間がログに記録され、プロジェクト所有者が承認し、請求記録のステータスが請求済みとマークされます。</li>
   </ul>


<p>時間が請求記録に含まれる場合、時間ステータスは、時間が承認されたかまたはその時間が属する請求記録が請求済みにされたかを示します。時間の入力時の時間ステータスは、時間リストまたはレポートにのみ表示されます。 </p>

<p>請求記録に時間を追加する方法について詳しくは、<a href="../../../manage-work/projects/project-finances/create-billing-records.md" >請求記録を作成</a>の記事の「請求記録への時間の追加」の節を参照してください。</p>

<p>プロジェクトの時間の承認について詳しくは、<a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" >プロジェクトの承認に時間を必須にする</a>を参照してください。</p>

<p><b>ヒント</b></p>

<p>作業アイテムに直接ログインしていない一般的な時間には、時間ステータスは表示されません。 </p> </td> 
  </tr>



<tr> 
   <td>[!UICONTROL Hour Type]</td> 
   <td> <p>ユーザーがタスク、イシューまたはプロジェクトに対してログを記録する実際の時間に設定できる属性です。これは、[!UICONTROL Vacation] や [!UICONTROL Time Off] など、直接作業にリンクされていないログに記録された時間の属性でもあります。</p> <p>詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">時間タイプの管理</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>ID は、[!DNL Workfront] ですべてのオブジェクトに関連付けられた英数字のインジケーターです。これは、[!DNL Workfront] データベースで各オブジェクトを一意に識別します。レポート内の任意のオブジェクトの ID または各オブジェクトのリストを表示できます。 </p> <p><b>ヒント</b></p>   <p>また、オブジェクトのページの URL に含まれる ID も確認できます。例えば、プロジェクトの ID は、[!UICONTROL Project Details] ページにアクセスする場合、次の URL に示す数字のようになります。</p> <p><code>https://&lt;your domain>.my.workfront.com/project/<b>5e29c8010027d8eb334762d4fff3ffca</b>/overview</code> </p> </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Individual Goals]</td> 
   <td>チームの目標の指標に貢献するが、個人やキャリアの開発には関係しない個人の目標。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Inherited Access]</td> 
   <td>オブジェクトから別のオブジェクトにアクセスを伝達するための共有関数。例えば、プログラム記録およびポートフォリオ記録で定義されたプロジェクトユーザーの継承アクセス権が挙げられます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Initiative]</td> 
   <td> <p>[!DNL Workfront Scenario Planner] では、計画を複数のイニシアチブに分割して、計画の管理を容易にすることができます。<span>[!UICONTROL Initiative] レポートを作成し、[!UICONTROL Project] レポートで [!UICONTROL Initiative] 情報にアクセスできます。</span></p> <p>[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">[!DNL Scenario Planner] 概要</a>を参照してください。 </p> <p>[!DNL Initiative] レポートは、会社が [!DNL Workfront Scenario Planner] ライセンスを購入していない場合、[!DNL Workfront] インスタンスでは表示されません。API から [!UICONTROL Initiatives] にアクセスすることはできません。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role]</span> </td> 
   <td> <p><span>[!UICONTROL Initiative Job Role] レポートタイプには、[!DNL Workfront Scenario Planner] でプランイニシアチブに関連付けられている担当業務に関する情報が表示されます。</span> </p> <p>[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md">[!DNL Scenario Planner] 概要</a>を参照してください。 </p> <p><span>このレポートタイプは、会社が [!DNL Workfront Scenario Planner] ライセンスを購入していない場合、[!DNL Workfront] インスタンスに表示されません。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Initiative Job Role Hours]</span> </td> 
   <td> <p><span> [!UICONTROL Initiative Job Role] レポートには、イニシアチブの担当業務に関連する時間数が表示されます。</span> </p> <p>[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md">[!DNL Scenario Planner] の概要</a>を参照してください。 </p> <p>このフィールドおよび [!UICONTROL Initiative Job Role] レポートタイプは、会社が [!DNL Workfront Scenario Planner] ライセンスを購入していない場合、[!DNL Workfront] インスタンスには表示されません。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role Count]</td> 
   <td> <p>[!UICONTROL イニシアチブジョブの役割 ] レポートには、イニシアチブに関連付けられている特定のジョブの役割の数が表示されます。</p> <p>[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md">[!DNL Scenario Planner] の概要</a>を参照してください。 </p> <p>このフィールドと [!UICONTROL Initiative Job Role] レポートタイプは、会社が [!DNL Workfront Scenario Planner] ライセンスを購入していない限り、[!DNL Workfront] インスタンスに表示されません。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Last Published Date]</td> 
   <td> <p>[!UICONTROL Initiative]、[!UICONTROL Initiative Job Role]、および [!UICONTROL Project] の各レポート内のフィールドで、プランイニシアチブがプロジェクトに最後に公開された日付を表示します。 イニシアチブを公開して、プロジェクトを作成したり、イニシアティブにリンクされたプロジェクトを更新したりできます。</p> <p>[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md">[!DNL Scenario Planner] の概要</a>を参照してください。 </p> <p><span>イニシアチブの公開について詳しくは、</span><a href="../../../scenario-planner/publish-scenarios-update-projects.md">[!DNL Workfront Scenario Planner]</a> でプロジェクトを作成および更新するためのシナリオを公開するをご覧ください。会社が [!DNL Workfront Scenario Planner] ライセンスを購入していない限り、このフィールドは [!DNL Workfront] インスタンスには表示されません。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Inline Search]</td> 
   <td>フォームに記入する過程で、特定のフィールドに入力できる項目を見つけるために実行される検索。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Interface Setup]</td> 
   <td>カスタムビュー、フィルター、グループ化、リストコントロールなどを定義できるアプリケーションの領域。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Is Company Goal]</p></td> 
   <td> <p>[!DNL goal reports] では、各戦略目標の「[!UICONTROL True]／[!UICONTROL False]」の値が表示され、組織が所有者として目標に割り当てられているかどうかが示されます。 </p> 
   <p>このフィールドは、組織が [!DNL Workfront Goals] を購入した場合のみに表示されます。[!DNL Workfront Goals] を使用した戦略目標の管理について詳しくは、<a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Adobe Workfront Goals] の概要</a>を参照してください。</p>
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue]</td> 
   <td> <p>通常、タスクまたはプロジェクトの完了を妨げる問題があることを示す予定外の作業アイテム。作業量をさらに検討するためにトリアージおよび評価</p> <p>[!UICONTROL Issue] は、[!UICONTROL Help Desk] リクエストである場合もあります。[!UICONTROL Change Orders]、[!UICONTROL Requests]、および [!UICONTROL Bugs] は [!UICONTROL Issues] でもあります。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Management]</td> 
   <td> <p>イシュータイプの定義と、各タイプに関連付けられたルーティング、トリアージ、またはトラフィックプロセスを管理するプロセスとルール。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Issue Owner]</td> 
   <td>イシューのトリアージと完了を担当するチームまたはユーザー。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Iteration]</td> 
   <td>チームが事前定義された一連の成果物を作成する期間。</td> 
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
   <td>[!UICONTROL Job Role]</td> 
   <td> <p>ユーザーの日常の職務と責任を識別するために使用されます。担当業務を作業アイテムに割り当てて、特定のユーザーに割り当てることなく、作業プロセスを完了するために必要なスキルを特定できます。 </p> <p>ユーザーは複数の役割を持つことができます（例：グラフィックデザイナーやコンサルタントなど）。</p> <p>詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成と管理</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL Journal Entry]</p> </td> 
   <td> <p>プロジェクト、タスク、イシュー、その他のオブジェクトの [!UICONTROL Updates] エリアに表示される追跡フィールドのシステム更新に関する情報を通知するレポート可能なオブジェクト。</p> <p>詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">[!UICONTROL Updates] エリアのレポート</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kanban Flag]</td> 
   <td> <p>[!UICONTROL Task] レポートまたは [!UICONTROL Issue] レポートの [!UICONTROL Kanban Flag] フィールドには、[!UICONTROL Kanban board] のストーリーに設定されているフラグのステータスが表示されます。可能な値は、[!UICONTROL On Track]、[!UICONTROL Ready to Pull]、および [!UICONTROL Is Blocked] です。</p> <p>[!UICONTROL Kanban story board] のストーリーにフラグステータスを設定する方法について詳しくは、記事<a href="../../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md" class="MCXref xref">[!UICONTROL Kanban board] のストーリーでフラグを使用</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>KPI</td> 
   <td>企業が主要なビジネス目標をどの程度効果的に達成しているかを示す測定可能な値。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag]</td> 
   <td>先行タスクの [!UICONTROL Planned Completion Date] が経過してから、依存タスクが開始できるようになるまでに経過する必要がある時間。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Lag Types]</td> 
   <td> <p>[!UICONTROL Lag] の計算メソッド。使用可能な値は次のとおりです。</p> 
    <ul> 
     <li>[!UICONTROL Days]（営業日）</li> 
     <li>[!UICONTROL Calendar Days]（祝日は無視）</li> 
     <li>[!UICONTROL Percent]</li> 
     <li>[!UICONTROL Day of Week]</li> 
    </ul> <p>詳しくは、 <a href="../../../manage-work/tasks/use-prdcssrs/lag-types.md" class="MCXref xref">ラグタイプの概要</a>.</p> </td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Large Thumbnail]</td> 
   <td> <p> [!UICONTROL Document] のリストまたはレポートでは、ドキュメントのプレビューがサムネールで表示されます。 </p> <p><strong>[!UICONTROL Large Thumbnail]</strong> を選択すると、400 ピクセル幅のサムネールがレポートに表示されます。</p> <p>リストまたはレポートの列の幅を変更すると、サムネールのサイズが調整されます。</p> <p>この記事の「[!UICONTROL Thumbnail]」も参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last 10 Viewers]</td> 
   <td> <p>レポートリストのこのフィールドには、最近レポートを表示した最大 10 人のユーザーの名前が表示されます。<br>レポートリストの使用状況について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況を表示</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Condition Note]</td> 
   <td> <p>このフィールドには、オブジェクトの所有者が最後に入力した更新が表示されます。これは、オブジェクトに対する所有者の最新のアクティビティまたはインタラクションです。</p> <p>[!DNL Last Condition Note] 列は、オブジェクトの最終メモのメモテキストが削除されている場合、空になります。オブジェクトに新規メモを入力すると、最終メモになり、列に再び表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Finance Update Date]</td> 
   <td>[!UICONTROL project] レポートでは、このフィールドは、プロジェクトの財務が最後に計算され、更新された日時を取り込みます。プロジェクトの財務について詳しくは、<a href="../../../manage-work/projects/project-finances/project-finances-overview-1.md" class="MCXref xref">プロジェクト財務の概要</a>を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Note]</td> 
   <td> <p>このフィールドには、任意のユーザーがオブジェクトに最後に入力した更新が表示されます。これは、オブジェクト上の最新のアクティビティまたはインタラクションです。</p> <p>オブジェクトの最終メモのテキストが削除されている場合、[!UICONTROL Last Note] 列は空になります。オブジェクトに新規メモを入力すると、それが最終メモになり、列に再び表示されます。</p>
   <p>このフィールドを [!UICONTROL Task] レポートに追加すると、タスクの子オブジェクト（イシュー、サブタスク、ドキュメントなど）に残った更新は、この列に表示されません。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed By]</td> 
   <td> <p>レポートリストでこのフィールドは、最後にレポートを表示したユーザーに関する情報が表示されます。<br>レポートリストの使用について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポート使用の表示</a>の記事を参照してください。<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Last Viewed Date]</td> 
   <td> <p>レポートリストのこのフィールドには、レポートが最後に表示された日付が表示されます。<br>レポートリストの使用について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポート使用の表示</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Layout Template]</td> 
   <td>特定のユーザーのワークスペースに表示されるタブとレポートを識別するために、システム管理者またはグループ管理者が定義します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Layout Type]</td> 
   <td>[!UICONTROL Custom Views] と組み合わせて、[!UICONTROL Layout Type] は [!UICONTROL Custom View] のタイプを指定します。現在は、リストのみを使用できます。今後、[!UICONTROL Detail]（オブジェクトの [!UICONTROL Detail] ビュー）が使用可能になる可能性があります。</td> 
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
   <td>[!UICONTROL Library Task]</td> 
   <td>アプリケーション全体で [!UICONTROL Tasks] と [!UICONTROL Template Tasks] の一貫した名前を付けるために使用される、単一のタスクのテンプレート。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Type]</td> 
   <td>[!UICONTROL Access Level] に割り当てられるライセンスのタイプ。[!UICONTROL Full User]、[!UICONTROL Limited User] または [!UICONTROL Requester] のいずれかです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Plan]</td> 
   <td> <p>[!UICONTROL Group] ビューまたはレポートで、このフィールドには、各グループが [!UICONTROL Home Group] として指定されているユーザーに割り当てることができる [!UICONTROL Plan] ライセンスの最大数が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL License Limit Work]</td> 
   <td> <p>[!UICONTROL Group] ビューまたはレポートで、このフィールドには、各グループが [!UICONTROL Home Group] として指定されているユーザーに割り当てることができる [!UICONTROL Work] ライセンスの最大数が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limited User]</td> 
   <td>[!DNL Access Level] の作成を許可するライセンスタイプには、表示のみの権限と、イシューの送信、メモの入力およびドキュメントのアップロードを行う権限が含まれます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List Controls]</td> 
   <td> <p>[!UICONTROL Interface Setup] の一部で、カスタムフィルター、ビューおよびグループ化を個々のユーザーにまたはすべてのユーザーにグローバルにリンクできます。</p> </td> 
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
   <td>[!UICONTROL Manual Only]</td> 
   <td> <p>[!UICONTROL Project] の [!UICONTROL Update Types] の 1 つ。この設定により、「[!UICONTROL Recalculated Timelines]」がクリックされた場合にのみ、[!UICONTROL Project Projected] および [!UICONTROL Planned] タイムラインが更新されるようになります。この方法で設定されたプロジェクトは、夜間の再計算プロセス中や、プロジェクト内の 1 つまたは複数のタスクが更新されたときに無視されます。</p> <p>詳しくは、<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクト [!UICONTROL Update Type] の選択</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Me]</td> 
   <td> <p>これは、現在ログインしているユーザーを指します。 </p> <p>他のユーザーとレポートを共有する場合は、このフィールドをフィルターで使用して、より一般的なレポートにすることをお勧めします。このように、情報は常にログインユーザーに合わせてカスタマイズされるので、レポートを 1 つだけ作成して、ログインしてレポートを表示するユーザーに応じて異なる情報を表示することができます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Max Users]</td> 
   <td> <p>これは非推奨のフィールドです。このフィールドに表示される情報はすべて、[!DNL Workfront] によって削除された機能に関連しているため、フィールドを更新できません。 </p> <p>[!DNL Workfront] の以前のリリースでは、職務の作成または編集時にこのフィールドを更新できました。各プロジェクトの役割に関連付けることができるユーザーの総数が表示されます。値 0 は、プロジェクトに割り当てることができるユーザーの数に制限はありません。 </p>このフィールドは一部のレポートおよびリストに引き続き表示されますが、表示される情報は更新できません。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone]</td> 
   <td> <p>タスクに関連付けて、タスクの完了時にプロジェクトの主要ポイントが達成されたことを示すマーカーです。 通常、マイルストーンを使用して、プロジェクトのフェーズの完了や、一連の重要なアクティビティなどの重要なイベントを示すことができます。[!UICONTROL Milestones] は通常、親タスクに関連付けられています。マイルストーンをタスクに添付する前に、マイルストーンを作成する必要があります。マイルストーンの詳細については、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md">マイルストーンパスの作成</a>および<a href="../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md">マイルストーンのタスクへの関連付け</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Milestone Path]</td> 
   <td>[!UICONTROL milestones] のコレクションです。[!UICONTROL マイルストーンパス ] は、特定の種類の [!UICONTROL マイルストーン ] を持つプロジェクトと、異なる種類の [!UICONTROL マイルストーン ] を持つプロジェクトを区別するために、プロジェクトで使用されます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Milestone Task]</td> 
   <td>測定すべき報告可能なイベントを示すフラグが付けられたタスク。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Module]</td> 
   <td>関連するアプリに基づいて何らかの機能を実行する、[!DNL Workfront Fusion] のシナリオ内の 1 つの手順。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Primary Role]</td> 
   <td> <p>これがフィルターで参照されると、ログインユーザーと同じ [!UICONTROL Primary Role] を持つユーザー、またはログインユーザーの [!UICONTROL Primary Role] に割り当てられた作業項目が表示されます。</p> <p>他のユーザーとレポートを共有する場合は、このフィールドをフィルターで使用して、より一般的なレポートにすることをお勧めします。このように、情報は常にログインユーザーに合わせてカスタマイズされるので、レポートを 1 つだけ作成して、ログインしてレポートを表示するユーザーに応じて異なる情報を表示することができます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL My Home Team]</td> 
   <td> <p>これがフィルターで参照される場合、このフィールドには、ログインユーザーの [!UICONTROL Home Team] に属するユーザー、またはログインユーザーの [!UICONTROL Home Team] に割り当てられた作業項目が表示されます。 </p> <p>他のユーザーとレポートを共有する場合は、このフィールドをフィルターで使用して、より一般的なレポートにすることをお勧めします。このように、情報は常にログインユーザーに合わせてカスタマイズされるので、レポートを 1 つだけ作成して、ログインしてレポートを表示するユーザーに応じて異なる情報を表示することができます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Naming convention]</td> 
   <td>データを使用してプロジェクト、タスク、成果物の名前を作成する、組織全体のルールのセットです。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Native Integration]</td> 
   <td>手動のコーディングや API 設定を必要としない統合。「標準」の統合とも呼ばれます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Navigation Menu]</td> 
   <td>[!UICONTROL Workfront] のメインエリアへのリンクがあるアプリケーションの上部中央のパネル。</td> 
  </tr> 
 </tr> 
  <tr> 
   <td>[!UICONTROL New Number Value]</td> 
   <td>[!UICONTROL Journal Entry] レポートでは、[!UICONTROL Old Number Value] を置き換えるフィールドの更新された値が表示されます。
詳しくは、この記事の「[!UICONTROL Old Number Value]」を参照してください。</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Non Work Day]</td> 
   <td>任意の割り当てを完了するために割り当てられていない日。通常は休日、休日、週末です。 「 」という用語が API エクスプローラーに表示されます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note]</td> 
   <td>[!DNL Workfront] オブジェクトに対して行われたコメントまたは更新。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Note Text]</td> 
   <td> <p>任意のオブジェクトに対してユーザーが入力した更新のテキストが表示されます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Number of Linked Goals]</td> 
   <td> <p>[!UICONTROL Project] レポートでは、これはプロジェクトに関連付けられた戦略目標の数です。プロジェクトを戦略目標に関連付ける方法については、<a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">[!DNL Adobe Workfront Goals]</a> でプロジェクトを目標に追加を参照してください。</p> 
   <p>戦略目標について詳しくは、この記事の [!UICONTROL Goal] も参照してください。</p> 
   <p>このフィールドは、組織が [!DNL Workfront Goals] を購入した場合のみに表示されます。[!DNL Workfront Goals] を使用した戦略目標の管理については、<a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">[!UICONTROL Adobe Workfront Goals] の目標にプロジェクトを追加</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object]</td> 
   <td> <p>[!DNL Adobe Workfront] で表示する情報は、[!DNL Workfront] データベース内で保存されるオブジェクトで表されます。オブジェクトは、Workfront の情報を駆動するものです。オブジェクトの例を以下に示します。</p> 
    <ul> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Groups]</li> 
     <li>[!UICONTROL Teams]</li> 
     <li>[!UICONTROL Users]</li> 
     <li>[!UICONTROL Companies]</li> 
     <li>[!UICONTROL Custom forms]</li>
     <li>[!UICONTROL Custom fields]</li>  
     <li>[!UICONTROL Hours]</li> 
     <li>[!UICONTROL Billing Rates]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Template tasks]</li>

<p><b>メモ</b></p>
  <p>これは包括的なリストではありません。 </p>

</ul> <p>詳しくは、<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">[!UICONTROL Adobe Workfront] のオブジェクトについて</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Object Types]</td> 
   <td>すべてのカスタムフォームを含むレポートまたはリストを作成する場合、このフィールドをビューまたはフィルターとして使用して、どのオブジェクトタイプがそれぞれのフォームに関連付けられているかを確認できます。 </td> 
  </tr> 
 <tr> 
   <td>[!UICONTROL Old Number Value]</td> 
   <td>[!UICONTROL Journal Entry] レポートでは、更新前のフィールドの元の値が表示されます。フィールドの値が更新されると、[!UICONTROL Journal Entry] レポートに [!UICONTROL New Number Value] と表示されます。詳しくは、「[!UICONTROL New Number Value]」も参照してください。</td> 
  </tr>
  <tr> 
   <td>[!UICONTROL On Change Only]</td> 
   <td> <p>[!UICONTROL Project Update] タイプのうちの 1 つ。このオプションを選択すると、[!UICONTROL Project Project Projected] および [!UICONTROL Planned] のタイムラインは、プロジェクトまたはプロジェクト内のタスクに対して更新または変更が行われた場合にのみ更新されます。 これはプロジェクトを毎晩更新するものではありません。</p> <p>詳しくは、<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新の種類の選択</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Op Task]</td> 
   <td> <p>[!DNL Workfront] データベース内の [!UICONTROL Issue] の名前であり、テキストモードのレポートや計算カスタムデータで使用されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Open]</td> 
   <td>未完了で作業中の問題またはタスク。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Org Chart]</td> 
   <td>組織図の略称。組織の階層を示すグラフです。また、[!UICONTROL User] の詳細画面のタブにも表示され、[!UICONTROL User] の [!UICONTROL Company] と [!UICONTROL Reporting] の関係を設定することができます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Organizational Setup]</td> 
   <td>これにより、組織の [!UICONTROL Companies]、[!UICONTROL Groups] および [!UICONTROL Security Profiles] が定義されます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Other Groups]</td> 
   <td> <p>ユーザーをリスト表示するレポートまたはビューで、このフィールドにはそれぞれのユーザーがメンバーとなっているすべてのグループが表示されます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL Job Role] レポートでは、これは担当業務に関連付けられている通貨を表します。これは、[!DNL Workfront] 管理者によって [!UICONTROL Setup] エリアで確立された [!UICONTROL Base Currency] の上書きです。 </p> 
     <p>詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成および管理</a>を参照してください。</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Billing/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL Job Role] レポートでは、これは担当業務の選択された [!UICONTROL Override Currency] を使用した、担当業務の 1 時間あたりの請求料金を表します。</p> 
     <p> 詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成および管理</a>を参照してください。</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Override Currency Cost/ Hour]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL Job Role] レポートでは、これは担当業務の選択された [!UICONTROL Override Currency] を使用した、担当業務の 1 時間あたりのコスト率を表します。 </p> 
     <p>詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成および管理</a>を参照してください。</p> 
    </div> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Owner]</td> 
   <td>指定されたオブジェクトの完了を担当するユーザー。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Owner Type]</span> </td> 
   <td> 
    <div> 
     <p>[!UICONTROL Goal] レポートでは、これには戦略目標に割り当てられている所有者のタイプが表示されます。以下に、目標の所有者のタイプを示します。</p> 
     <ul> 
      <li> <p>[!UICONTROL User]</p> </li> 
      <li> <p>[!UICONTROL Team] </p> </li> 
      <li> <p>[!UICONTROL Group]</p> </li> 
     </ul> 
     <p>目標の所有者が組織の場合、このフィールドに値は表示されません。 </p> 
     <p>追加のライセンスが必要です。[!DNL Workfront Goals] について詳しくは、<a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">[!DNL Adobe Workfront Goals]概要</a>を参照してください。 </p> 
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
   <td>[!UICONTROL Parameter]</td> 
   <td> <p>[!UICONTROL parameter] はカスタムフィールドです。システム内のすべてのパラメーターやカスタムフィールドに関するレポートを作成できます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent]</td> 
   <td>レポートでは、このフィールドには、オブジェクトの親に関する情報が表示されます。例えば、[!UICONTROL issue] レポートでは、イシューが記録されたタスクやプロジェクトに関する情報が表示され、タスクレポートでは、直接の親タスクやプロジェクトに関する情報が表示されます。[!DNL Workfront] で親を持つ可能性のあるオブジェクトについて詳しくは、「<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">[!DNL Adobe Workfront]</a>内のオブジェクトの理解」の記事にある「オブジェクトの相互依存性と階層」の節を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Lag]</td> 
   <td>[!UICONTROL Parent Task] の開始と [!UICONTROL Subtask] の開始の間に経過する必要がある時間。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent Task]</td> 
   <td>[!UICONTROL Summary Task] とも呼ばれます。これはサブタスク（[!UICONTROL Children Tasks] とも呼ばれる）を持つタスクです。親タスクの [!UICONTROL Duration]、[!UICONTROL Work Required] および [!UICONTROL Percent CompletePercent Complete] は、サブタスクから計算されます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Part-Time Resources]</td> 
   <td>システムに定義されているデフォルトのスケジュールよりも容量が少ないライセンスを取得したユーザー。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Percent Complete]</td> 
   <td> <p>タスク、プロジェクト、イシューに関連する作業の割合を示すプロジェクト、タスク、イシューのフィールド。</p> <p>イシューや作業タスクについては、このフィールドを手動で更新できます。 </p> <p>プロジェクトおよび親タスクの場合、このフィールドはすべての作業タスクからのロールアップであり、手動で更新することはできません。 </p> <p>詳しくは、<a href="../../../manage-work/tasks/task-information/project-percent-complete.md" class="MCXref xref">プロジェクトの [!UICONTROL Percent CompletePercent Complete] の概要を参照してください</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permission]</td> 
   <td> <p>オブジェクトに対してユーザーに付与される権限であり、通常は、ユーザーが項目に対する作業を完了したり、項目を表示したりできるようにするために付与されます。以下の権限を付与することができます。</p> 
    <ul> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Portfolios]</li> 
     <li>[!UICONTROL Programs]</li> 
     <li>[!UICONTROL Reports]</li> 
     <li>[!UICONTROL Dashboards]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Custom Forms]</li> 
     <li>[!UICONTROL Views]</li> 
     <li>[!UICONTROL Filters]</li> 
     <li>[!UICONTROL Groupings]</li> 
    </ul> <p>詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">オブジェクトに対する共有権限の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]</td> 
   <td> <p>これは、[!DNL Workfront] システムのフルライセンスタイプです。ユーザーが [!DNL Workfront] のすべての機能にアクセスするには、これが必要です。</p> <p>詳しくは、<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]ライセンスの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Plan]（[!DNL Scenario Planner] で）</td> 
   <td> <p>[!DNL Workfront] シナリオプランナーを使用する場合、計画はメインオブジェクトです。会社の短期的および長期的な将来の戦略の概要を示し、それぞれの高レベルの結果を特定して、それを計画として [!DNL Workfront] シナリオプランナーに追加できます。 </p> <p>結果を [!DNL Scenario Planner] の計画に表示することはできません。また、[!DNL Workfront] API を経由して計画にアクセスすることはできません。 </p> <p>[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md">[!DNL Scenario Planner] の概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned]</td> 
   <td> <p>何かが発生するようにスケジュールされている時間枠。プロジェクト、タスクやイシューを [!DNL Workfront] に作成する場合、予定開始日と予定完了日、およびそれらが発生する予定時間枠を確定します。これらの値は、当初の意図、または項目が完了するまでにかかる時間の見積もりを表します。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Benefit]</td> 
   <td>これは、プロジェクトマネージャーが、プロジェクトの完了が組織に金銭的利益をもたらすかどうかを見積もるための手動入力です。この値の指定は、プロジェクトの [!UICONTROL Business Case] をまとめる作業の一部として行うことができます。この値を更新するには、プロジェクトに対する [!UICONTROL Manage] 権限が必要です。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Planned Budgeted Hours]</td> 
   <td> <p>[!UICONTROL 予算時間 ] レポートでは、[!UICONTROL リソースプランナー ] のプロジェクトまたは [!UICONTROL ジョブロール ] に予算された時間数が表示されます。 </p> <p>[!UICONTROL リソースプランナー ] でのプロジェクトまたはロールの予算作成について詳しくは、この記事を参照してください <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">[!UICONTROL プロジェクト ] ビューと [!UICONTROL ロール ] ビューを使用した [!UICONTROL リソースプランナー ] の予算リソース</a>. [!UICONTROL Budgeted Hours] レポートについて詳しくは、<a href="../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">レポート：予算計上時間数</a>の記事を参照してください</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Completion Date]</td> 
   <td> <p>[!UICONTROL Planned Completion Date] は、手動で選択した日付に設定できます。[!UICONTROL Planned Completion Date] を設定しない場合、[!DNL Workfront] が自動的に設定します。自動的に設定された場合、[!UICONTROL Planned Completion Date] は [!UICONTROL Planned Start Date] + [!UICONTROL Duration] です。</p> <p>詳しくは、次の記事を参照してください。</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">タスクの [!UICONTROL Planned Completion Date] の概要</a> </p> </li> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-planned-completion-date.md" class="MCXref xref">プロジェクト [!UICONTROL Planned Completion Date] の設定</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Cost]</td> 
   <td> <p>プロジェクトの [!UICONTROL Planned Labor Cost] と [!UICONTROL Planned Expense Cost] の合計。これには、プロジェクトに [!UICONTROL Planned Risk Cost] は含まれません。  </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration]</td> 
   <td> <p>タスクの [!UICONTROL Planned Duration] は、通常、タスクの [!UICONTROL Duration] と同じです。これは、タスクの [!UICONTROL Planned Start] と [!UICONTROL Planned Completion Dates] の間の日数の差を表します。 </p> <p>タスクが [!UICONTROL Effort Driven] の [!UICONTROL Duration] タイプの場合、[!UICONTROL Planned Duration] は、タスクに割り当てたリソース数に基づいてタスクの [!UICONTROL Duration] と異なる場合があります。 </p> <p>例えば、[!UICONTROL 期間 ] タイプが [!UICONTROL 労力による ] のタスクの期間が 3 日で、フルタイムスケジュールを持つ 1 つのリソースをタスクに割り当てた場合、[!UICONTROL 予定期間 ] も 3 日になります。 3 つのリソースをフルタイムスケジュールで同じタスクに割り当てた場合、[!UICONTROL 期間 ] は 3 日間ですが、[!UICONTROL 予定期間 ] は 1 日になります。 [!UICONTROL Planned Duration] では、新しい [!UICONTROL Planned Duration] を反映するために、タスクの [!UICONTROL Planned Start] の日付と [!UICONTROL Planned Completion] の日付も変更されます。その結果、プロジェクトのタイムラインにも影響が及びます。 </p> <p>タスクの [!UICONTROL Duration] と [!UICONTROL Planned Duration] の違いについて詳しくは、<a href="../../../manage-work/tasks/task-information/planned-duration-vs-duration-for-tasks.md" class="MCXref xref">タスクの [!UICONTROL Planned Duration] と [!UICONTROL Duration] の違い</a>の記事を参照してください。</p> <p>プロジェクトとイシューには [!UICONTROL Planned Duration] がありません。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Duration Minutes]</td> 
   <td> <p>プロジェクトまたはイシューの [!UICONTROL Planned Duration Minutes] は、分単位のプロジェクトまたはイシューの [!UICONTROL Duration] です。 </p> <p>タスクには「[!UICONTROL Planned Duration Minutes]」フィールドはありません。 </p> <p>[!UICONTROL Template Tasks] には、[!UICONTROL Planned Duration Minutes] フィールドがあり、このフィールドにはタスクの [!UICONTROL Planned Duration] が分単位で表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Expense Cost]</td> 
   <td> <p>プロジェクトまたはタスクでログに記録されたすべての費用の [!UICONTROL Planned Amounts] の合計。</p> <p><b>例</b></p>
   <p>タスク 1 の費用を作成し、「[!UICONTROL Planned Amount]」フィールドに 600 ドルと入力した場合、このタスクの [!UICONTROL Planned Expense Cost] は 600 ドルになります。 </p> 
   <p>プロジェクトの場合、[!DNL Workfront] では、次の式を使用して [!UICONTROL Planned Expense Cost] を計算します。</p> <p><code>Project [!UICONTROL Planned Expense Cost] = SUM (All Project [!UICONTROL Planned Expense Costs]) + SUM (All Tasks [!UICONTROL Planned Expense Costs])</code> </p> 
   <!--
     <p>Important: If the value in the Actual Amount field for an expense is negative, Workfront will ignore that expense record. For example, if the value in the Planned Amount field is $200.00 but the value in the Actual Amount field is -$300.00, the system will ignore this entire expense record which means you would not include the $200.00 planned value or the -$300.00 actual value in any calculations for Planned Expense Cost or Actual Expense Cost. (Drafting this because not sure if this is correct anymore)</p>
    --> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Hours]</td> 
   <td> <p>このフィールドは [!UICONTROL projects] エリア、[!UICONTROL tasks] エリアおよびイシューエリア、プロジェクト、タスクまたはイシューのレポート、[!UICONTROL Resource Planner]、[!UICONTROL Workload Balancer]、[!UICONTROL Utilization] レポートのリソース管理ツールに表示されます。 </p> <p>プロジェクト所有者が、各タスクまたは問題が完了するまでに必要な時間数を示します。 プロジェクトの場合は、通常、これはプロジェクトのタスクからの [!UICONTROL Planned Hours] のロールアップです。 </p> <p>「[!UICONTROL Planned Hours]」フィールドには、表示する場所に応じて異なる情報が表示される場合があります。予定時間数について詳しくは、<a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">予定時間数の概要</a>を参照してください。</p> <p>予定時間数は、[!DNL Workfront] データベースに分単位で保存されます。このフィールドを使用して計算を記述する場合は、時間が分単位で表示されることを考慮してください。<br></p> <p>デフォルトでは、予定時間数は、作業項目の期間内のすべての日に均等に配分され、タスクに割り当てられたすべてのリソースにも均等に配分されます。ユーザーは、作業項目の 1 日の計画時間数を更新したり、担当者ごとに個々の計画時間数を更新したりできます。</p> <p>このフィールドの更新は、プロジェクト、タスクおよびイシューによって異なります。 </p> 
    <ul> 
     <li> <p>イシューの場合は、このフィールドを手動で更新できます。イシュー予定時間数は、プロジェクト予定時間数には追加されません。 </p> <p><b>ヒント</b></p> <p>問題レポートでは、「[!UICONTROL 予定時間 ]」フィールドの 1 つが「[!UICONTROL 作業 ]」フィールドに置き換えられます。フィールドには、イシューに関する予定時間数が表示されます。詳しくは、この表の「作業」フィールドまたは「[!UICONTROL Work]」フィールドを参照してください。 </p> </li> 
    </ul> 
    <ul> 
     <li> <p>タスクの場合、タスクの [!UICONTROL Duration Type] が [!UICONTROL Calculated Assignment] または [!UICONTROL Simple] の場合は、このフィールドを手動で更新できます。このフィールドは、タスクの [!UICONTROL Duration Type] が [!UICONTROL Calculated Work] または [!UICONTROL Effort Driven] の場合は、[!DNL Workfront] によって計算されます。<br>[!UICONTROL Task Duration] について詳しくは、<a href="../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref">タスク [!UICONTROL Duration] と [!UICONTROL Duration Type] の概要</a>の記事を参照してください。</p> </li> 
    </ul> 
    <ul> 
     <li> <p>プロジェクトの場合、[!DNL Workfront] は、プロジェクトのすべてのタスクからすべての予定時間数を追加して、予定時間数を計算します。 </p> </li> 
    </ul> <p><b>ヒント</b></p> <p>[!UICONTROL Planned Hours] を [!UICONTROL project] レポート、[!UICONTROL task] レポートまたは [!UICONTROL issues] レポートに表示するには、テキストモードを使用して追加のフィールドを参照します。詳しくは、この表の「<code>work</code>」フィールド、「[!UICONTROL Work]」フィールドおよび「<code>workRequiredExpression</code>」フィールドを参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Labor Cost]</td> 
   <td> 
    <p>タスクの場合、ユーザーまたは役割の時間単価に、ユーザーまたは役割に割り当てられた時間数を掛けた値です。</p> <p>プロジェクトの場合、すべてのタスクの [!UICONTROL Planned Labor Costs] の合計です。</p> <p>ユーザーまたは役割の率が使用されるかどうかは、特定のタスクに対して選択されたコストタイプによって異なります。 </p> <p>詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md">コストのトラック</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Revenue]</td> 
   <td> <p>タスクとプロジェクトでは、[!DNL Workfront] に [!UICONTROL Planned Revenue] の値を表示できます。[!UICONTROL Planned Revenue] は、プロジェクトのタスクの [!UICONTROL Planned Hours] に関連付けられた金額を表します。プロジェクトの場合は、プロジェクトの [!UICONTROL Fixed Revenue] を含めることもできます。 </p> <p>タスクの場合、これはタスクの [!UICONTROL Planned Hours] に関連付けられた収益です。すべてのタスクの予定時間数はプロジェクトの予定時間数にまとめられて、プロジェクト [!UICONTROL Planned Hours]の計算に使用されます。 </p> 
   <p>[!DNL Workfront] 次の式を使用して、タスクとプロジェクトの[!UICONTROL Planned Revenue]を計算します。</p> 
   <p><code>Task [!UICONTROL Planned Revenue] = [!UICONTROL Planned Hours] * Billing hourly rate</code> </p> <p><code>Project [!UICONTROL Planned Revenue] = SUM (All tasks [!UICONTROL Planned Revenue]) + [!UICONTROL Fixed Revenue]</code> </p> 
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    --> 
    <p>[!UICONTROL Project Details]エリアおよびプロジェクトレポートに表示されるプロジェクト[!UICONTROL Planned Revenue]は、[!UICONTROL Utilization]レポートに表示される予定収益とは異なります。 </p> <p>[!UICONTROL Project Details]エリアの[!UICONTROL Planned Revenue]には、タスクの収益とプロジェクトの固定収益が反映されます。[!UICONTROL Utilization Report]の[!UICONTROL Planned Revenue]には、プロジェクト内のタスクにのみ関連付けられた[!UICONTROL Planned Revenue]が表示されます。 </p> 
     <p><b>例</b></p>  
      <p>プロジェクトに 10 時間のタスクが 1 つあり、そのタスクがコンサルタントに時給 20 ドルで割り当てられ、プロジェクトの[!UICONTROL Fixed Revenue]が 100 ドルの場合、[!UICONTROL Utilization]レポートには[!UICONTROL Planned Revenue]として 200 ドルが表示されます（[!UICONTROL Planned Revenue]はタスクの時間に関連付けられています）。「[!UICONTROL Project Details]」セクションには、300 ドル（タスクからの[!UICONTROL Planned Revenue]とプロジェクトの固定収益）が表示されます。 </p> 
    <p>[!DNL Workfront] での収益の追跡については、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md">請求と収益の概要</a>を参照してください。 </p> 
    <p>[!UICONTROL Utilization report]での[!UICONTROL Planned Revenue]の計算については、<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">リソース稼働率情報の表示</a>を参照してください。 </p> 
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Planned Risk Cost]</td> 
   <td> <p>発生確率を考慮した、プロジェクトのすべてのリスクの[!UICONTROL Potential Cost]の合計。この金額は、プロジェクトの[!UICONTROL Planned Cost]には含まれません。</p> <p>プロジェクトの[!UICONTROL Planned Risk Cost]は、次の式で計算されます。</p> <p><code>Planned Risk Cost = SUM(Potential Risk Cost * Probability / 100)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Profile]</td> 
   <td>管理者が定義した、タブおよびポータルセクションのコレクションで、[!DNL Workfront] アプリケーション[!UICONTROL Home]やその他のダッシュボードに表示されるものです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Section]</td> 
   <td>ダッシュボードまたはポータルページにあるタブの 1 つのコンポーネントです。通常は、単一のレポート、グラフ、カレンダーまたは主要情報のリストです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Portal Tab]</td> 
   <td>ポータルまたはダッシュボードにあるタブで、最大 3 つのポータルセクションが含まれているものです。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Portfolio]</td> 
   <td> <p>統一的な特性を持つプロジェクトのコレクションです。これらのプロジェクトは通常、同じリソース、予算または時間枠を得るために競い合うことになります。ポートフォリオに追加する前に、ポートフォリオをプログラムに分割し、プロジェクトをプログラムに関連付けることができます。</p> <p>ポートフォリオについて詳しくは、<a href="../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md">[!DNL Adobe Workfront]</a> のポートフォリオの概要を参照してください。</p> 
   </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Management]</td> 
   <td>コレクションまたは関連するプログラムおよびプロジェクト作業の管理に重点を置いた実務エリアです。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Optimizer]</td> 
   <td>ポートフォリオ内のプロジェクトの評価と優先付けを支援する [!DNL Workfront] ツールです。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Portfolio Owner]</td> 
   <td>ポートフォリオの優先付けと予算を担当する関係者です。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Potential Risk Cost]</td> 
   <td>リストおよびレポートにあるプロジェクトフィールドです。プロジェクトに関連するリスクが発生した場合の潜在コストを示します。詳しくは、<a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">潜在リスクコストの計算</a>を参照してください。 </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Predecessor]</td> 
   <td> <p>依存タスクの完了前に完了する必要があるタスク。 別のタスクの [!UICONTROL 依存関係 ] としてマークされたタスクでもあります。 先行タスクを使用すると、別のタスクが終了してからタスクを開始するなどの、シーケンス依存関係ロジックをプランナーで設定できます。</p> <p>詳しくは、<a href="../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md" class="MCXref xref">タスクの先行タスクの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Company]</td> 
   <td>ユーザー設定で指定された、ユーザーが所属する会社です。会社は、プロジェクトに関連付けることもできます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Primary Contact]</td> 
   <td><p>[!UICONTROL Primary Contact]はイシューの作成者であり、イシューが作成されると [!DNL Workfront] によって自動的に指定されます。イシューの[!DNL Manage]権限が付与されている場合は、このフィールドを手動で更新できます。1 つのイシューのプライマリ連絡先は 1 つだけです。</p> 
   <p>プライマリ連絡先を変更しても、当初プライマリ連絡先として指定されたユーザーは引き続きイシューに対する[!UICONTROL Manage]アクセス権を持ちます。</p>
   <p>イシューをプライマリまたはプロジェクトに変換する場合、そのイシューの [!UICONTROL タスク連絡先 ] として指定されたユーザーが、プロジェクトまたはタスクの [!UICONTROL 変換後のイシュー作成者 ] になります。 イシューの変換後にイシューの [!UICONTROL Primary Contact] が更新された場合、[!UICONTROL Converted Issue Originator] は、変換が行われた時点のイシューの [!UICONTROL Primary Contact] として保持されます。この記事の [!UICONTROL Converted Issue Originator] も参照してください。</p> 
   </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Priority]</td> 
   <td>タスク、イシューまたはプロジェクトに割り当てて、その重要度を指定できる値です。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Private]</td> 
   <td>[!UICONTROL Note] または [!UICONTROL Document] では、このオプションを使用すると、ほとんどのビューアでそのオブジェクトが非表示になります。非公開ヘルプリクエストキューの場合、[!UICONTROL リクエスト ] 領域を通じて、プロジェクトチームのユーザーのみがそのキュー（またはプロジェクト）にイシューを送信できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Profile]</td> 
   <td>ユーザーアカウントに関するすべての情報です。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Program]</td> 
   <td> <p>ポートフォリオ内のサブセットで、類似したプロジェクトをグループ化し、明確に定義された利益を達成できます。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Management]</td> 
   <td>プロジェクト間の依存関係、リスク、イシュー、要件およびソリューションを管理して、プログラムの健全性を維持し、定義済みのプログラムの利益を達成します。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Program Owner]</td> 
   <td>プロジェクトの目標と会社の目標が合致していることを確認するために、アクティビティの監督および編成を担当する関係者です。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>[!UICONTROL Progress]</span> </td> 
   <td> <p>[!UICONTROL Goal] レポートでは、戦略目標が達成にどの程度近づいているかを割合で表示します。進行状況の割合は数値で表示されます。戦略目標について詳しくは、この表の「[!UICONTROL Goal]」も参照してください。</p> <p>このフィールドは、組織が [!DNL Workfront] Goals を購入した場合にのみ表示されます。[!DNL Workfront Goals] を使用した戦略目標の管理について詳しくは、<a href="../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md">[!DNL Adobe Workfront Goals] の目標にプロジェクトを追加</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Progress Status]</td> 
   <td> <p>プロジェクト、タスク、目標レポートで、このフィールドにはプロジェクト、タスクまたは戦略的目標の進捗ステータスが表示されます。詳しくは、次の記事を参照してください。</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/projects/planning-a-project/project-progress-status.md" class="MCXref xref">プロジェクトの進捗ステータスの概要</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">タスクの進捗ステータスの概要</a> </p> </li> 
     <li> <p><a href="../../../workfront-goals/goal-management/calculate-goal-progress.md">[!DNL Adobe Workfront Goals]</a> の目標の進行状況と条件の概要 </p>
     <p>「[!DNL goals]」フィールドの [!UICONTROL Goal] レポートと [!UICONTROL Progress Status] は、組織が [!DNL Workfront Goals] を購入している場合にのみ表示されます。[!DNL Workfront Goals] の戦略目標については、<a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] の概要</a>を参照してください。 </p> </li>
    </ul> </td> 
  </tr> 
  <td>[!UICONTROL Project]</td> 
   <td> <p>特定の期間内に完了する必要があり、特定の予算とリソース数を使用する必要がある大量の作業。管理しやすくするには、プロジェクトを一連のタスクに分割します。すべてのタスクを完了すると、プロジェクトが完了します。プロジェクトの計画について詳しくは、<a href="../../../manage-work/projects/planning-a-project/plan-project.md">プロジェクトの計画の概要</a>を参照してください。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Assignment Planned Hours]</td> 
   <td> <p>[!UICONTROL Initiative Job Role] レポートには、プロジェクトのタスクまたはイシューに割り当てられたジョブの役割に関連付けられた [!UICONTROL Planned Hours] の数字が表示されます。このフィールドおよび [!UICONTROL Initiative Job Role] レポートタイプは、会社が [!DNL Workfront Scenario Planner] ライセンスを購入していない場合、[!DNL Workfront] インスタンスには表示されません。[!DNL Workfront Scenario Planner] について詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md">[!DNL Workfront Scenario Planner] の概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Details]</td> 
   <td>プロジェクトの現在のステータスの詳細。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Budgeted Cost]</td> 
   <td> <p> リストおよびレポートに表示されるプロジェクトの [!UICONTROL Budgeted Cost] です。</p><p>この記事の「[!UICONTROL Budgeted Cost]」も参照してください。</p></td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Project Management]</td> 
   <td>プロジェクトの作成、分類、名前付けのしきい値を管理する一連のポリシーです。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Project Overhead]</td> 
   <td>[!UICONTROL Hour] レポートで、このフィールドは [!UICONTROL Project Time] の時間タイプでログに記録された時間に関連する財務情報用に予約されています。プロジェクトには独自の請求レートを設定でき、時間がプロジェクトに直接記録される場合は、設定された請求レートが計算に使用されます。また、プロジェクトの設定に基づいてプロジェクトに異なる通貨を使用することができ、その時間に合わせて通貨換算を行うこともできます。[!UICONTROL Project Overhead] オブジェクトを使用すると、[!DNL Workfront] でその情報を取得できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Owner]</td> 
   <td>プロジェクトの範囲、タイムライン、割り当てを管理するユーザー。変更依頼、財務上の変更、成果物に対するデフォルトの承認者。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Planning]</td> 
   <td>プロジェクトスケジュールを作成および管理するプロセス。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Sponsor]</td> 
   <td>各ユーザーが関連付ける必要がある指定された関係者のプロファイル。[!DNL Workfront] では、これらは [!UICONTROL Access Levels] として指定されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project Teams]</td> 
   <td> <p>プロジェクトに割り当てられたユーザーまたは役割のコレクション</p> <p>詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-team-overview.md">プロジェクトチームの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Project tracking]</td> 
   <td>プロジェクトの正常性と範囲の測定に使用されるデータ</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Projected]</td> 
   <td> <p>タスク、イシュー、またはプロジェクトの予定時間数と完了率に基づく、作業が完了する時点のタイムスタンプの推定値。</p> <p>これは、タスク、イシューまたはプロジェクトの 日付または [!UICONTROL Duration] を指します。通常は、ある作業が既に完了しているか、ある時間が経過した後で、作業アイテムの寿命により忠実な日付と期間を指定します。 </p> <p>例えば、タスクの [!UICONTROL Projected Completion Date] は、タスクに対して行われた作業量、割り当てられた担当者数、開始日以降に経過した時間に基づいて、[!DNL Workfront] がタスクが完了すると予測した日付です。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Deadline]</td> 
   <td> <p>[!UICONTROL Document Version] オブジェクト（[!UICONTROL Document Version] レポートや [!UICONTROL Proof Approval] レポートなど）が含まれるレポートでは、このフィールドにプルーフの期限の曜日、日付、時刻および年が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Decision]</td> 
   <td> <p>[!UICONTROL Document Version] オブジェクト（[!UICONTROL Document Version] レポートや [!UICONTROL Proof Approval] レポートなど）が含まれるレポートでは、このフィールドにプルーフの決定ステータス（保留中、変更が必要、承認済み）が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Name]</td> 
   <td> <p>[!UICONTROL Document Version] オブジェクト（[!UICONTROL Document Version] レポートや [!UICONTROL Proof Approval] レポートなど）が含まれるレポートでは、このフィールドにプルーフ名が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Pages]</td> 
   <td> <p>[!UICONTROL Document Version] オブジェクト（[!UICONTROL Document Version] レポートや [!UICONTROL Proof Approval] レポートなど）が含まれるレポートでは、このフィールドにプルーフに含まれるページ数が表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proof Progress]</td> 
   <td> <p>[!UICONTROL Document Version] オブジェクト（[!UICONTROL Document Version] レポートや [!UICONTROL Proof Approval] レポートなど）が含まれるレポートでは、プルーフの進捗ステータス（[!UICONTROL Sent]、[!UICONTROL Opened]、[!UICONTROL Commented]、[!UICONTROL Decision Made]）を表示します。</p> <p>詳しくは、<a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md" class="MCXref xref">プルーフの進捗状態とステータスの概要</a>の中の<a href="../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md#understanding-progress-and-status" class="MCXref xref">プルーフの進捗状態の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Proofing]</td> 
   <td>1 人または複数のユーザーが、画像、テキストドキュメント、ビデオまたはインタラクティブ Web コンテンツ内で変更するコンテンツに対してマークおよびコメントを付けるレビュープロセスです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Public]</td> 
   <td>[!UICONTROL Note] または [!UICONTROL Document] でこのオプションを使用すると、他のユーザーや [!DNL Workfront] 外部のユーザーがそのオブジェクトにアクセスできるようになります。[!UICONTROL ヘルプリクエストキュー ] の場合、[!UICONTROL 公開 ] は、プロジェクトにイシューを送信できるすべてのユーザーが [!UICONTROL リクエスト ] 領域を通じてイシューを送信できることを意味します。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Quality]</td> 
   <td>組織内の仕事の質の認識。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue]</td> 
   <td>「Help Desk Queue」または「[!UICONTROL Help Request Queue]」とも呼ばれる。 これは、ユーザーが問題を送信できるように、[!UICONTROL 要求 ] 領域に公開されたプロジェクトです。 通常、キューは特定のトピックに対して作成されます（[!UICONTROL バグ ]、[!UICONTROL プロジェクトリクエスト ] など）。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Properties]</td> 
   <td>これらの設定は、[!UICONTROL 要求 ] 領域に公開されるプロジェクトの問題送信ルールを定義します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Queue Topic]</td> 
   <td> <p>ユーザーが問題を送信してトピックを選択できる、[!UICONTROL Help Request Queue] 上のプロパティ。 トピックには次のようなものがあります。</p> 
    <ul> 
     <li>カスタムデータフォームに関連付ける。</li> 
     <li>選択したトピックに設定されたルーティングルールを通じて、問題をユーザー、役割、またはチームに自動的に割り当てます。</li> 
     <li>選択したトピックに設定されたルーティングルールを通じて、問題を別のプロジェクトまたはキューに移動します。</li> 
    </ul> <p>詳しくは、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">キュートピックの作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rank]</td> 
   <td> <p>[!UICONTROL Access Level] レポートでは、[!UICONTROL Access Level] の [!UICONTROL Rank] を手動で指定できます。これは、[!DNL Workfront] 管理者として、各アクセスレベルに関連付けられている複雑さのレベルを視覚的に識別するのに役立ちます。例えば、複雑さの高い（[!UICONTROL Plan] レベルの）アクセスレベルには小さい数値を指定し、複雑さの低い（[!UICONTROL Requester] レベルの）アクセスレベルには大きい数値を指定できます。標準アクセスレベルのランク付けはできません。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ready]</td> 
   <td> <p>タスクレポートのこのフィールドは、バックログで [!UICONTROL Agile] タスクが [!UICONTROL Ready] とマークされたかどうかを示します。このフラグは、[!UICONTROL Agile] タスク（[!UICONTROL Agile] チームに割り当てられたタスク）にのみ適用されます。 </p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Recurrence Frequency]</td> 
   <td> <p>繰り返しタスクの親の [!UICONTROL Task Details] ボックスまたは [!UICONTROL Edit Task] ボックスに表示されるフィールドです。これは、繰り返しの中のタスクが発生する頻度です。繰り返しタスクの作成について詳しくは、<a href="../../../manage-work/tasks/create-tasks/create-recurring-tasks.md" class="MCXref xref">繰り返しタスクを作成</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reference Number]</td> 
   <td> <p>プロジェクト、タスクおよびイシューは、作成時に自動的に一意の参照番号に関連付けられます。[!UICONTROL Reference Number] は、プロジェクト、タスク、イシューの [!UICONTROL Details] ページ、またはリストやレポートで表示できます。 </p> <p><b>ヒント</b><p><br>参照番号は常に一意なので、2 つの項目が同じ名前の場合は、参照番号に従うことができます。 </p> <p>[!DNL Workfront] は、システムレベルで順次参照番号を自動的に生成します。 各プロジェクト、タスクまたはイシューは、次に使用可能な番号をシーケンス内で取得します。 <br></p> <p>例えば、ユーザー A がタスクを作成した場合、[!DNL Workfront] は、タスクに 100 の参照番号を自動的に割り当てる場合があります。その直後にユーザー B がイシューを作成した場合、[!DNL Workfront] はイシューに 101 の参照番号を割り当てます。参照番号は手動で編集できません。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rejection Issue]</td> 
   <td>プロジェクトまたはタスクレポートでは、これは、プロジェクトまたはタスクの承認が却下されたときに作成されるイシューです。拒否イシューについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">作業項目の承認プロセスを作成</a>を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remaining Risk Cost]</td> 
   <td> <p>プロジェクトの [!UICONTROL Planned Risk Cost] と、プロジェクトにおけるすべてのリスクの [!UICONTROL Actual Costs] の合計との差を示すプロジェクトフィールド。 </p> <p>プロジェクトの [!UICONTROL Remaining Risk Cost] は、次の式を使用して計算されます。</p> <p><code>[!UICONTROL Remaining Risk Cost] = Project [!UICONTROL Planned Risk Cost] - SUM([!UICONTROL Actual Cost] for all risks)</code> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Replanning]</td> 
   <td>問題を修復または克服するためにプロジェクトの日付を変更する。 例えば、正確な日付を反映させるために、数ヶ月間保留状態のプロジェクトを再計画する必要があります。 これは、プロジェクトの日付またはタスクの日付を手動で調整する操作です。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Report]</td> 
   <td>指定した 1 つの [!DNL Workfront] オブジェクトおよびその関連属性に関する情報を含むグラフまたはテーブル。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request]</td> 
   <td> <p>単一の一元化されたキューでトリアージされ、進行中の作業とは無関係なイシュー。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Request Queue]</td> 
   <td>トラフィックとトリアージのプロセスで管理されるイシューのバックログ。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Request velocity]</td> 
   <td>リクエストを取り込み、完了するまでの合計作業サイクル時間。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Requester]</td> 
   <td>通常は、ライセンスタイプです。リクエスターライセンスを持つユーザーは、システム内で発生する新しい作業のリクエストを送信できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reserved Time]</td> 
   <td>ユーザーの個人時間に指定された日数。ユーザーが作業できなくなることを示します。 「[!UICONTROL Non Work Days]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Issue]</td> 
   <td> <p>イシューレポートでは、このフィールドをビューまたはフィルターで使用して、解決するイシューを参照します。 </p> <p>レポートでのオブジェクトの解決方法について詳しくは、<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解決可能なオブジェクトと解決オブジェクトの概要</a>の<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">レポート内で解決可能なオブジェクトと解決オブジェクトの情報を表示</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Project]</td> 
   <td> <p>イシューレポートでは、このフィールドをビューまたはフィルターで使用して、イシューを解決するプロジェクトを参照します。 </p> <p>レポートでの解決オブジェクトの表示について詳しくは、<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解決可能なオブジェクトと解決オブジェクトの概要</a>の<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">レポート内で解決可能なオブジェクトと解決オブジェクトの情報を表示</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resolve Task]</td> 
   <td> <p>イシューレポートでは、このフィールドをビューまたはフィルターで使用して、イシューを解決するタスクを参照します。 </p> <p>レポートでの解決オブジェクトの表示については、<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解決オブジェクトと解決可能オブジェクトの概要</a>の<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md#resolvable-and-resolving-data-in-reports" class="MCXref xref">レポートでの解決可能オブジェクトおよび解決オブジェクト情報の表示</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource]</td> 
   <td>に存在するユーザーまたはロール [!DNL Workfront] およびは、プロジェクトチーム、タスクおよびタスクに割り当てられます。 プロジェクト、タスクまたは問題に関連する作業を完了する責任を負います。 </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Resource Estimates</td> 
    <td>This report captures information about an area in&nbsp;Workfront that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>. </td> 
   </tr>
   <td>Resource Grid</td> 
   <td>A visual table showing the allocation of resources.</td> 
  </tr> -->
  <tr> 
   <td>[!UICONTROL Resource Management]</td> 
   <td> <p>[!UICONTROL Resource Management]は、リソースの空き時間に基づいてリソースの使用状況を正確に予測して、実行する必要がある作業を予算内で時間どおりに完了できるようにするエンタープライズツールセットです。 </p> <p>リソース管理ツールを使用すると、リソースの長期的な容量と短期的なスケジュール設定のニーズを計画できます。 </p> <p>[!DNL Workfront] でのリソース管理については、<a href="../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md">リソース管理の基本を学ぶ</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Manager IDs]</td> 
   <td><p>プロジェクトレポートでは、フィルターを作成して特定のリソース管理者を検索する際に、このオプションを使用できます。 </p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Managers]</td> 
   <td> <p>プロジェクトレポートまたはリストビューでは、これは、プロジェクトでリソース管理アクティビティを実行するように指定されたユーザーを表示する情報フィールドです。レポートで「[!UICONTROL Resource Managers]」を使用すると、プロジェクトのリソース管理者のコンマ区切りリストが表示されます。特定のプロジェクトに対して、最大 30 人のリソース管理者を指定できます。</p> <p>詳しくは、<a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md">プロジェクトまたはテンプレートに対するリソース管理者の指定</a>の記事を参照してください。</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Hours] </td> 
   <td>[!UICONTROL Resource Planner]でプロジェクトに予算計上された時間数とプロジェクトに関連付けられたリソース。この記事の「[!UICONTROL Budgeted Hours]」も参照してください。 </td> 
  </tr>  
  <tr> 
   <td>[!UICONTROL Resource Planner] </td> 
   <td>プロジェクト、担当業務またはユーザーを横断してリソースを表示および管理できる高度な [!DNL Workfront] ツールです。詳しくは、<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">リソースプランナーの概要</a>を参照してください。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Planner Budgeted Labor Cost]</td> 
   <td> <p>これは、リソース・プランナを使用して、プロジェクト・ジョブ・ロールに予算された時間に関連する原価です。 </p> <p>この記事の「予算計上労力コスト」も参照してください。 </p> </td>

</tr> 
  <tr> 
   <td>[!UICONTROL Resource Pools]</td> 
   <td> <p>リソースプールは、プロジェクトに関連付けることができるユーザーの集まりです。 同じリソースプール内のユーザーは、通常、同じ部門に属しているか、同じスキルを持っているか、補完的なスキルを持っているか、同じ予算で資金を提供されています。 複数のリソースプールをプロジェクトまたはユーザーに関連付けることができます。リソースプールは、1 つのプロジェクトにのみ割り当てることも、複数のプロジェクトで共有することもできます。</p> 
   <p>リソースプールについて詳しくは、<a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">リソースプールの概要</a>を参照してください。</p> 
   <p>プロジェクトレポートでは、リソースプールには、プロジェクトに関連付けられているすべてのプールが表示されます。このオブジェクトはグループ化で使用できません。</p> 
  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Resource Utilization]</td> 
   <td>特定の期間中に利用可能な時間数と、レポートの各ユーザーにスケジュールされた時間数を表示するレポート。また、[!UICONTROL Average Hours Per Day]と配分率の計算にも使用されます。</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>[!UICONTROL Result]</td> 
   <td>[!DNL Workfront Goals] の場合、結果は目標の進捗状況インジケーターです。手動で更新する数値、割合値または通貨金額にすることができます。結果をレポートに表示することはできません。また、[!DNL Workfront] API を介して結果にアクセスすることもできません。アクティビティについて詳しくは、<a href="../../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md" class="MCXref xref">Adobe Workfront Goals の結果とアクティビティの基本を学ぶ</a>を参照してください。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Revenue]</td> 
   <td>タスクまたはプロジェクトの請求可能な金額。この金額は、1 時間ごと、固定額またはその両方を組み合わせて指定できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Revenue Type]</td> 
   <td>収益タイプは、タスクがどのように収益を生み出すかを指定します。例えば、[!UICONTROL Fixed Hourly]、[!UICONTROL Role Hourly]、[!UICONTROL Role Hourly w/Cap]などがあります。[!DNL Workfront] での収益の追跡については、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reviewer]</td> 
   <td>通常は、ライセンスタイプです。[!UICONTROL Reviewer] ライセンスを持つユーザーは、システム内の作業項目を確認し、承認できます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk]</td> 
   <td> <p>これは、[!DNL Workfront] の次の概念を指す場合があります。</p> 
    <ul> 
     <li> <p>プロジェクトのリスクの可能性を示す、プロジェクトに関するフィールド。リスクのレベルに基づいて、プロジェクトに優先順位を付けて実行できます。プロジェクトで発生し得るリスクのレベルは次のとおりです。</p> <p>- [!UICONTROL Very Low]</p> <p>- [!UICONTROL Low]</p> <p>- [!UICONTROL Medium]</p> <p>- [!UICONTROL High]</p> <p>- [!UICONTROL Very High]</p> <p>プロジェクトに示すリスクのレベルはカスタマイズできません。 </p> <p> プロジェクトのリスクの更新については、<a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">プロジェクトの編集</a>の記事で「プロジェクト設定」の節を参照してください。レポートでプロジェクトのリスクフィールドを表示できます。 </p> </li> 
     <li> <p>プロジェクトの実施中に発生する可能性のあるイベントで、プロジェクトのコスト、範囲またはスケジュールに対する潜在的な影響を明らかにするもの。プロジェクトへの潜在的なリスクを定義し、プロジェクトのビジネスケースを作成する際に、そのリスクの発生確率またはコストを関連付けます。プロジェクトのビジネスケースへのリスクの追加については、「プロジェクトのリスクの作成と編集」を参照してください。 </p> <p>[!UICONTROL Business Case]で定義されたリスクをレポートに表示することはできません。レポートとリストには、いくつかのタイプのリスクコストのみを表示できます。 </p> </li> 
    </ul> </td>

</tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Cost]</td> 
   <td> <p>プロジェクトのリスクに関連するコスト。プロジェクトに関連するリスクコストのうち、レポートに表示できるものは次のとおりです。</p> 
    <ul> 
     <li> <p>[!UICONTROL Actual Cost]：発生したリスクの実際のコストを表示する、リスクのフィールド。レポートやリストに加えて、リスクの編集または作成時に[!UICONTROL Edit Risk]ボックスで、そのリスクを特定することができます。 </p> <p>プロジェクト、タスクまたはタスクのコストについては、この記事の「[!UICONTROL Actual Cost]」を参照してください。 </p> </li> 
     <li> <p>[!UICONTROL Planned Risk Cost]：プロジェクトのすべての[!UICONTROL Potential Risk Costs]の合計を表示する、プロジェクトのフィールド。この記事の「[!UICONTROL Planned Risk Cost]」も参照してください。 </p> <p>潜在リスクコストについては、<a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">潜在リスクコストの計算</a>を参照してください。 </p> </li> 
     <li> <p>[!UICONTROL Remaining Risk Cost]：すべてのリスクの[!UICONTROL Actual Costs]の合計と[!UICONTROL Planned Risk Cost]の差を表示する、プロジェクトのフィールド。この記事の「残存リスクコスト」も参照してください。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Risk Management]</td> 
   <td>リスクを特定、軽減および監視するプロセス。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td>この記事の「[!UICONTROL Job Role]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing]</td> 
   <td>問題の自動割り当てまたは移動 ( 通常は、キューのトピックまたはキューのデフォルトルート（ルーティングルール）となるため )。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Routing Rule]</td> 
   <td>ユーザー、役割、チームに問題を自動的に割り当てたり、別のプロジェクトまたはキュートピックに問題を移動したりする、プロジェクトおよびキュートピックに関する設定。 ルーティングルールは、通常、受信イシューを自動的に割り当てるためにヘルプリクエストキューで使用されます。</td> 
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
   <td>[!UICONTROL Saved Search]</td> 
   <td>検索条件が保存されている検索。保存済みの検索結果を使用すると、検索条件を再入力しなくても、再度同じ検索を簡単に実行できます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Scenario]（[!DNL Workfront Fusion] の場合） </td> 
   <td> <p>シナリオは、アプリまたはサービス間でデータを転送および変換する方法を示す一連の手順（モジュール）で構成されます。</p> <p>[!DNL Workfront Fusion] のシナリオについては、<a href="../../../workfront-fusion/scenarios/scenario-overview.md" class="MCXref xref">[!DNL Adobe Workfront Fusion] シナリオの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scenario]（[!DNL Workfront Scenario Planner]の場合） </td> 
   <td> <p>[!DNL Scenario Planner] の場合、シナリオはプランのコピーです。 </p> <p>[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">[!DNL Scenario Planner] の概要</a>を参照してください。 </p> <p>シナリオの作成について詳しくは、<a href="../../../scenario-planner/create-and-compare-scenarios-for-a-plan.md">[!DNL Scenario Planner]</a> でプランのシナリオを作成および比較を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule]</td> 
   <td>週別の作業スケジュール（勤務時間を含む）と、休暇（休日など）および例外日（土曜日の作業日など）を組み合わせたもの。スケジュールをプロジェクトおよびユーザーに関連付けることができます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Schedule Exemption]</td> 
   <td>[!UICONTROL Modified Shift] とも呼ばれます。スケジュールで定義されている、通常の週別作業時間とは異なる、スケジュールされた日数。例えば、月曜日から金曜日までの作業のみがスケジュールに設定されている場合、土曜日に作業するようにスケジュールを設定すると、[!UICONTROL Schedule Exemption] となります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scheduled Report]</td> 
   <td> <p>各種レポートのレポートを作成する際に、[!UICONTROL Scheduled Report] フィールドを使用してレポートの配信が予定されている場合は、レポートのスケジュールに関する情報を表示できます。このフィールドには、レポートの各スケジュールに対して 1 つずつ、複数の値が箇条書きリストで表示されます。レポートのスケジュール設定について詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">レポート配信の概要</a>の記事を参照してください。</p> <p>このフィールドには複数の値が表示されるので、1 つのグループ化で使用することはできません。フィルターまたはビューでのみアクセスできます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Scope Change]</td> 
   <td>[!UICONTROL 監査証跡 ]。アクティブの場合、[!UICONTROL タスク期間 ] や [!UICONTROL 先行タスク ] が変更された場合など、プロジェクトまたはタスクの範囲が変更されるたびにメモを生成します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section]</td> 
   <td>表示目的でカスタムデータを整理するために作成された、画面上の独自のヘッダーを持つエリア。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Section Break]</td> 
   <td>セクション間の空白または境界線。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Security]</td> 
   <td>ユーザーがシステム内の特定のオブジェクトを操作し、他のオブジェクトを操作できるようにする設定です。 この記事の「[!UICONTROL Access Levels]」も参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Setup]</td> 
   <td>管理者がシステム設定と環境設定を行える領域。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severity]</td> 
   <td> <p>[!UICONTROL Severity] は、項目が作業の完了にどの程度影響を与える可能性があるのかを示します。例えば、重大度が高い問題は、タスクの完了を完全にブロックする可能性がありますが、重大度が低い問題は、表面的なものに過ぎません。</p> <p>詳しくは、<a href="../../../manage-work/issues/issue-information/update-issue-severity.md" class="MCXref xref">イシューの重要度を更新</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Severities]</td> 
   <td>この記事の「[!UICONTROL Severity]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sharing]</td> 
   <td>他のユーザーに [!DNL Workfront] での特定の項目の表示または編集を許可するアクション。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Slack Date]</td> 
   <td>タスクのビューまたはレポートでは、[!UICONTROL Slack Date] は、タスクがプロジェクトの [!UICONTROL Completion Date] に確実に影響を与える可能性がある正確な日付を表示します。タスクの [!UICONTROL Slack Date] について詳しくは、<a href="../../../manage-work/tasks/task-information/task-slack-date.md" class="MCXref xref">タスクの余裕日の概要</a>を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Smart Assignments]</td> 
   <td> <p>ユーザーにタスクまたは問題を割り当てる場合 [!DNL Workfront] は、作業の完了に最適なユーザーとプロジェクトとの関係に基づいて、誰が作業を完了するかに関するレコメンデーション（[!UICONTROL スマート割り当て ]）をおこないます。</p> <p>詳しくは、<a href="../../../manage-work/tasks/assign-tasks/smart-assignments.md" class="MCXref xref">スマート割り当ての概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source]</td> 
   <td> <p>別のオブジェクトの親オブジェクトを示します。例えば、タスクに添付されたドキュメントは、[!UICONTROL Document] レポートまたはビューの [!UICONTROL Source] フィールドにタスクの名前を持ち、プロジェクトの下に記録されたイシューは、イシューレポートまたはビューの [!UICONTROL Source] フィールドにプロジェクトの名前を持ちます。 </p> 
   <p>次のレポートにはソース列が表示され、親オブジェクトに関する情報を表示できます。</p>
  <ul><li>イシューレポート</li>
    <li>時間レポート</li>
    <li>ドキュメントレポート </li>
    </ul>
   <p>イシュー、時間、ドキュメントの親オブジェクトに対する権限をユーザーが持っていない場合、レポートが表示するように設定されている場合や、別のユーザーのアクセス権を使用して配信される場合でも、レポートのソース列は空白となります。 </p>
   <p> レポートに親オブジェクトに関する情報を表示するには、親の名前を表示できる親オブジェクト用の列を追加することをお勧めします。 </p>
    <p>例えば、次のいずれかを「ソース」列でレポートに追加できます。 </p>
    <ul><li>「プロジェクト名」列、「タスク名」列または「イシュー名」列をドキュメントまたは時間レポートに。</li>
    <li>「プロジェクト名」列または「タスク名」列をイシューレポートに。 </li> </ul>
    詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md">別のユーザーのアクセス権を使用したレポートの実行と配信</a>を参照してください。

</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Start Date]</td> 
   <td> <p>アイテムの作業を開始するように設定された日付。[!DNL Workfront] で扱う開始日には、次のように複数のタイプがあります。 </p> 
    <ul> 
     <li>[!UICONTROL Planned]</li> 
     <li>[!UICONTROL Actual]</li> 
     <li>[!UICONTROL Projected] </li> 
    </ul> <p>[!UICONTROL Rate report]では、プロジェクトレベルでの担当業務の新しい請求料率が始まる日付です。この日付以降のプロジェクト関連の時間数にこの請求料率を乗算して、プロジェクトの収益を計算します。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status]</td> 
   <td> <p>作業アイテムまたは戦略目標のワークフロー位置を示すために使用されるインジケーター。</p> <p>プロジェクトの場合、[!UICONTROL ステータス ] はプロジェクトの設定で、プロジェクトが次のどちらであるかを示します。</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL On Hold] </li> 
     <li>[!UICONTROL Complete] </li> 
     <li>[!UICONTROL Dead]</li> 
    </ul> <p>プロジェクトのステータスの詳細については、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md">システムプロジェクトステータスのリストへのアクセス</a>.</p>
    <p>タスクの場合、[!UICONTROL ステータス ] はタスクが次のどちらであるかを示すタスクの設定です。</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Complete]</li> 
    </ul> <p>タスクのステータスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md">システムタスクステータスのリストへのアクセス</a></p> <p>問題の場合、[!UICONTROL ステータス ] は問題に関する設定で、この問題が次のどちらであるかを示します。</p> 
    <ul> 
     <li>[!UICONTROL New]</li> 
     <li>[!UICONTROL In Progress]</li> 
     <li>[!UICONTROL Awaiting Feedback]</li> 
     <li>[!UICONTROL On Hold]</li> 
     <li>[!UICONTROL Resolved]</li> 
     <li>[!UICONTROL Won't Resolve]</li> 
     <li>[!UICONTROL Cannot Duplicate]</li> 
     <li>[!UICONTROL Verified Complete]</li> 
     <li>[!UICONTROL Reopened]</li> 
    </ul> <p>問題のステータスについて詳しくは、 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">システムの問題ステータスのリストへのアクセス</a>.</p> 
    <p>戦略目標の場合、[!UICONTROL Status]は目標の設定の一つで、目標が次のうちどの状態にあるかを示すものです。</p> 
     <ul> 
      <li>[!UICONTROL Active]</li> 
      <li>[!UICONTROL Draft]</li> 
      <li>[!UICONTROL Inactive]</li> 
      <li>[!UICONTROL Closed]</li> 
     </ul> 
     <p>戦略目標について詳しくは、この記事の「[!UICONTROL Goal]」または「[!UICONTROL Goals]」も参照してください。 </p> 
     <p>戦略目標の場合、このフィールドは組織が [!DNL Workfront Goals] を購入済みの場合にのみ表示されます。[!DNL Workfront Goals] を使用した戦略目標の管理については、<a href="../../../workfront-goals/goal-management/wf-goals-overview.md">[!DNL Workfront Goals] の概要</a>を参照してください。 </p>
    </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Change]</td> 
   <td>[!UICONTROL Audit Trail]の一つ。ユーザーがプロジェクト、タスクまたはイシューのステータスを変更すると、メモが生成されます。</td> 
  </tr> 
  <tr> 
   <td>ステータスアイコン</td> 
   <td> <p>組み込みの [!UICONTROL Status Icons] フィールドをビューの列として追加すると、次のようなオブジェクトの主要ポイントをより明確に表示できます。</p> 
    <ul> 
     <li>オブジェクトにドキュメントが添付されている</li> 
     <li>オブジェクトが承認プロセスに関連付けられている</li> 
     <li>オブジェクトに追加のメモが関連付けられている</li> 
     <li>費用は請求可能または払い戻し可能</li> 
     <li>タスクがクリティカルパス上にある</li> 
     <li>ユーザーが会社、チームに属している、または別のタイムゾーンにいる</li> 
    </ul> <p>次のオブジェクトのビューに [!UICONTROL Status Icons] フィールドを追加できます。</p> 
    <ul> 
     <li>[!UICONTROL Tasks]</li> 
     <li>[!UICONTROL Issues]</li> 
     <li>[!UICONTROL Projects]</li> 
     <li>[!UICONTROL Template Tasks]</li> 
     <li>[!UICONTROL Templates]</li> 
     <li>[!UICONTROL Expenses]</li> 
     <li>[!UICONTROL Documents]</li> 
     <li>[!UICONTROL Users]</li> 
    </ul> <p>詳しくは、<a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">ビュー内の組み込みステータスアイコン</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Status Update]</td> 
   <td> <p>このフィールドには、プロジェクト、タスク、または問題報告で、「[!UICONTROL 更新 ]」領域でオブジェクトの所有者が提供した最新のステータス更新が表示されます。 プロジェクトの場合は、プロジェクト所有者が行ったコメント、タスクやタスクに対するコメント、つまり担当者が行ったコメントを意味します。</p> 
   <p> オブジェクトのステータスを更新する際におこなわれたコメントは、「[!UICONTROL ステータスの更新 ]」列に表示されません。</p> <p>「[!UICONTROL New]」、「[!UICONTROL In Process]」、「[!UICONTROL Complete]」のステータスを表示するには、[!UICONTROL Status] 列を使用します。</p> <p>ステータスについて詳しくは、<a href="../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">タスクステータスを更新</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Statuses]</td> 
   <td>この記事の「[!UICONTROL Status]」を参照してください。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Storyboard]</td> 
   <td>ストーリー（アジャイル方法論でのタスク）のステータスと、ストーリーが完了に向かってどのように進んでいるかを表すグラフ。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Hours]</td> 
   <td>ストーリーの難易度や複雑さの測定に使用する指標。アジャイルチームは、時間とポイントのどちらを使用するかを選択できます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Story Points]</td> 
   <td>ストーリーの難易度や複雑さの測定に使用する指標。アジャイルチームは、時間とポイントのどちらを使用するかを選択できます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Strategic]</td> 
   <td>組織や組織の仕組みを変更する長期の作業。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Strategic Alignment]</td> 
   <td>ポートフォリオやプログラム全体で会社の目標を測定し、調整します。</td> 
  </tr>

<tr> 
   <td><code>[!UICONTROL stretch]</code></td> 
   <td><p>これは、テキストモードインターフェイスを使用する際に、レポートの列で使用されます。 </p>
   <p><code>[!UICONTROL stretch]</code> は、ビューで不要な領域を占める列を識別するために使用されます。一般的なユーザーのワークスペースのユーザーインターフェイスの幅は、約 850 ピクセルです。つまり、ビューに 4 つの列（各 150 ピクセル）があり、
そのビューが 850 ピクセルのうち 600 ピクセルを占有している場合です。UI には、伸縮率が指定された列に追加される、250 個の追加のピクセルがあります。 </p>
   <p>ビュー内の少なくとも 1 つの列に対して追加のコード行 <code>[!UICONTROL usewidths=true]</code> を使用すると、列の伸縮が適用されます。 
   </td> 
  </tr>

<tr> 
   <td>[!UICONTROL Subscribers]</td> 
   <td> <p>プロジェクト、タスクまたはタスクを購読するユーザー。</p> <p>このフィールドをレポートで使用すると、サブスクライバーのリストが表示され、各サブスクライバーがコンマで区切られます。</p> <p>詳しくは、<a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">[!DNL Adobe Workfront]</a> で項目を登録の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Summary Task]</td> 
   <td>この記事の「[!UICONTROL Parent Task]」を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subtask]</td> 
   <td>親タスクの下に配置される子タスク。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL System Governance]</td> 
   <td>システムの変更とメンテナンスを管理する一連のポリシー。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL System Integration]</td> 
   <td>様々なコンピューティングシステムとソフトウェアアプリケーションを物理的または機能的に連携させ、全体として機能させるプロセス。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task]</td> 
   <td> <p>最終目標（プロジェクトの完了）を達成するためのステップとして実行する必要があるアクティビティ。</p> <p>詳しくは、<a href="../../../manage-work/tasks/task-information/tasks-overview.md" class="MCXref xref">タスクの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Attribute]</td> 
   <td>タスクに関連付けられ、タスクに関する特定の詳細を示すその他のフィールドまたはオブジェクト。 例として、[!UICONTROL Planned Completion Date] や [!UICONTROL Status] などがあります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Task Constraint]</td> 
   <td>「[!UICONTROL Constraint Type]」および「[!UICONTROL Constraint Date]」を参照してください。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Management]</td> 
   <td>タスクの作成、割り当て、終了、表示のしきい値を管理する一連のポリシー。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Managed"> 
   <td>[!UICONTROL Task Owner]</td> 
   <td>タスクの見積もりとタスクの完了を担当するチームまたはユーザー</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Ad hoc"> 
   <td>[!UICONTROL Team]</td> 
   <td> <p>同様の目標やビジネス目標に向けて作業するユーザーの集まり。チームを作業項目に割り当てることで、これらのユーザーを作業項目に一括で割り当てることができます。</p> <p>チームについて詳しくは、<a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">チームの概要</a>を参照してください。</p> <p>プロジェクトには [!UICONTROL Project Team] を割り当てることができます。このチームには、プロジェクトでの作業に関連するすべてのユーザーや役割が含まれます。</p> <p>プロジェクトチームについて詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">プロジェクトチームの概要</a>を参照してください。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode,SnippetConitions_MaturityModel.Ad hoc"> 
    <td>Team Goals</td> 
    <td>Team goals which contribute to the metrics of enterprise or department goals.</td> 
   </tr>
  --> 
  <tr> 
   <td>[!UICONTROL Template]</td> 
   <td> <p>プロジェクトテンプレートは、最も繰り返し可能なプロジェクトの一般的な概要です。プロジェクトテンプレートを作成する際に、タスク、キュートピック、カスタムフォーム、添付ドキュメントまたは承認を定義することで、新しいプロジェクトを作成する際に時間を節約できます。 </p> <p>既存のプロジェクトにテンプレートを添付したり、テンプレートを使用して新しいプロジェクトを作成したりできます。テンプレートで指定されたすべての情報は、それを使用して作成されたプロジェクトに転送されます。 </p> <p>テンプレートについて詳しくは、<a href="../../../manage-work/projects/create-and-manage-templates/project-template-overview.md">プロジェクトテンプレートの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Template Task]</td> 
   <td>テンプレートの一部であるタスクです。 テンプレートタスクは、テンプレートを使用して作成されるプロジェクト内のタスクになります。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thread]</td> 
   <td>特定のトピックに関連する返信の [!UICONTROL Note] とそのコレクション。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Thumbnail]</td> 
   <td> <p> [!UICONTROL Document] のリストまたはレポートでは、ドキュメントのプレビューがサムネールで表示されます。 </p> <p> <strong>[!UICONTROL Thumbnail]</strong> を選択すると、33 ～ 66 ピクセル幅のサムネイルがレポートに表示されます。 </p> <p>リストまたはレポートの列の幅を変更すると、サムネールのサイズが調整されます。</p> <p>この記事の「[!UICONTROL Large Thumbnail]」も参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Time Off]</td> 
   <td>[!UICONTROL Time Off] レポートを作成して、ユーザーがプロファイルで休暇を示した時点を表示できます。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet]</td> 
   <td> <p>ユーザーが、プロジェクト、タスク、イシューに取り組んだ実際の時間数、または会議やトレーニングなど、作業に関連しない他のアクティビティに費やした時間を入力できるタイムカード。作業に費やした時間を入力する以外に、その時間を作業関連時間として表示するか、オーバーヘッド時間に計上するかを指定する場合は、「時間タイプ」を使用して時間エントリを定義します。タイムシートについて詳しくは、<a href="../../../timesheets/timesheets/timesheets-overview.md">タイムシートの概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Timesheet Profile]</td> 
   <td> <p>[!UICONTROL Timesheet Profile] は、関連付けられたユーザーのタイムシートを [!DNL Workfront] で自動作成するのに使用するテンプレートです。 </p> <p>各タイムシートの作成時に、適用する設定の数を構成できます。これらの設定には、タイムシートの作成頻度（毎週、隔週、毎月 2 回、毎月）、タイムシートの開始日、タイムシート承認者、記録された時間に関連付けることができる [!UICONTROL Hour Types] があります。</p> </td> 
  </tr> 
  <tr > 
   <td>[!UICONTROL Top Parent ID] </td> 
   <td> <p>このフィールドでは、最上位のグループとそのサブグループに関するデータを識別し、リストまたはレポートでフィルタリングできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Top Parent Name] </td> 
   <td> <p>このフィールドでは、リストまたはレポートの [!UICONTROL View] 内の最上位グループとそのサブグループに関するデータを識別できます。</p> <p>これは、[!UICONTROL Top Parent ID] フィールドを使用して行うこともできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Hours]</td> 
   <td> <p>[!UICONTROL project report] では、このフィールドには、プロジェクトの最後の財政計算時点での、プロジェクトの全時間の丸め合計が表示されます。[!UICONTROL Actual Hours] は、プロジェクトにログオンした正確な時間を反映します。通常、[!UICONTROL Actual Hours] は [!UICONTROL Total Hours] と一致します。[!UICONTROL 合計時間 ] が [!UICONTROL 実際の時間 ] フィールドと大きく異なる場合は、プロジェクト上の財務を再計算する必要があります。</p> <p>プロジェクトの財務の再計算について詳しくは、<a href="../../../manage-work/projects/project-finances/recalculate-project-finances.md" class="MCXref xref">プロジェクトの財務を再計算</a>を参照してください。</p> <p>タイムシートの [!UICONTROL Standard] ビューでは、このフィールドは、タイムシートに表示される日付の項目に関して記録された合計時間数を参照します。このビルトインビューのタイムシートの [!UICONTROL Total Hours] フィールドは、[!UICONTROL hoursDuration] フィールドを参照し、タイムシートの開始日と終了日の時間差を動的に計算します。ユーザーがタイムシートの時間枠で利用可能な時間よりも長い時間を記録した場合に、「[!UICONTROL Total Hours]」列を赤で表示するために使用されます。詳しくは、<a href="../../../timesheets/create-and-manage-timesheets/view-total-hours-timesheets.md" class="MCXref xref">タイムシートの合計時間数の表示</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tracking Mode]</td> 
   <td> <p>タスクの属性。 これにより、タスクの予定タイムラインを更新する方法とタイミングが決まります。 例：</p> 
    <ul> 
     <li>[!UICONTROL ユーザーは更新が必要 ] では、タスクを手動で更新する必要があります。 それ以外の場合は、「[!UICONTROL Behind Schedule]」、「[!UICONTROL Late]」になります。</li> 
     <li>[!UICONTROL 自動完了 ] は、期限（[!UICONTROL 予定完了日 ]）が過ぎると、タスクを自動的に完了します。</li> 
    </ul> <p>詳しくは、<a href="../../../manage-work/tasks/task-information/task-tracking-mode.md" class="MCXref xref">タスクトラッキングモードの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Optimized"> 
   <td>[!UICONTROL Trigger]</td> 
   <td>シナリオを開始させるイベント。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Trouble Task]</td> 
   <td>[!UICONTROL 遅延 ]、[!UICONTROL スケジュール遅延 ]、[!UICONTROL リスク状態 ] のいずれかの条件を持つ不完全なタスク。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Unassigned Task]</td> 
   <td>どのユーザー、役割、またはチームにも割り当てられていないタスクです。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Update Type]</td> 
   <td> <p>プロジェクトの推定タイムラインを再計算するタイミングを決定する、プロジェクトの設定です。 [!UICONTROL 更新タイプ ] には、次の値を指定できます。</p> 
    <ul> 
     <li>[!UICONTROL Automatic and On Change]</li> 
     <li>[!UICONTROL Automatic Only]</li> 
     <li>[!UICONTROL Manual Only] </li> 
    </ul> <p>詳しくは、<a href="../../../manage-work/projects/manage-projects/select-project-update-type.md" class="MCXref xref">プロジェクトの更新タイプの選択</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User]</td> 
   <td>ユーザーがログインしてシステムとやり取りできるようするために [!DNL Workfront] で作成されたアカウント。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>[!UICONTROL User Delegation]</p> </td> 
   <td> <p>次の内容を示すレポート可能なオブジェクト。</p> 
    <ul> 
     <li>タスク、イシュー、プロジェクトの承認をデリゲートしたユーザー</li> 
     <li>タスク、イシュー、プロジェクトの承認をデリゲートされたユーザー</li> 
     <li>デリゲーションの開始および終了日時</li> 
    </ul> <p>詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-user-delegation-report.md" class="MCXref xref">ユーザーのデリゲーションレポートの作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface]</td> 
   <td>[!DNL Workfront] アプリケーションのあらゆる視覚的およびインタラクティブな側面。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Interface Preferences]</td> 
   <td>[!UICONTROL User Interface Setup][!DNL Workfront] 管理者はこれらの設定を変更して、ユーザーインターフェイスをカスタマイズできます。</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConitions_MaturityModel.Integrated"> 
   <td>[!UICONTROL Utilization]</td> 
   <td>割り当てられたスケジュール、PTO、現在のワークロードに基づくユーザーまたは役割の可用性。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User Utilization]</td> 
   <td> <p>ユーザー（リソース）の割り当て方法や過剰に割り当てられているかどうかを示すレポートと組み合わされた点検。この記事の [!UICONTROL Resource Utilization] を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## V 〜 Z

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
   <td>作業サイクルの合計時間（作業の完了に要する時間）と、当初コミットした時間内に作業が完了する頻度（作業とコミットの比率）を示す指標。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL View]</td> 
   <td> <p>ビューとは、レポート内の列またはオブジェクトのリスト内の列を変更できるレポート要素を指します。</p> 
   <p> 「表示」は、オブジェクトのアクセスレベルに応じて、またはそのオブジェクトの権限共有レベルで、そのオブジェクトの情報のみを表示するユーザーの権利を指します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL View Icons]</td> 
   <td> <p> これは、ステータスアイコンと同じフィールドですが、次のビューでのみ使用できます。 </p> 
    <ul> 
     <li> [!UICONTROL Documents] </li> 
    </ul> <p> 詳しくは、<a href="../../../reports-and-dashboards/reports/using-built-in-reports/built-in-status-icons-views.md" class="MCXref xref">ビュー内のビルトインステータスアイコン</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Month]</td> 
   <td> <p>レポートリストには、過去 1 カ月間にレポートが閲覧された回数が表示されます。<br>レポートリストの使用情報について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Quarter]</td> 
   <td>レポートリストでは、前四半期にそのレポートが閲覧された回数が表示されます。<br>レポートリストの使用情報について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" >レポートの使用状況の表示</a>の記事を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views Last Year]</td> 
   <td>レポートリストでは、昨年にそのレポートが閲覧された回数が表示されます。<br>レポートリストの使用情報について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>の記事を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Month]</td> 
   <td> <p>レポートリストでは、今月にそのレポートが閲覧された回数が表示されます。<br>レポートリストの使用情報について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Quarter]</td> 
   <td>レポートリストでは、今四半期にそのレポートが閲覧された回数が表示されます。<br>レポートリストの使用情報について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md" class="MCXref xref">レポートの使用状況の表示</a>の記事を参照してください。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Views This Year]</td> 
   <td>レポートリストでは、今年そのレポートが閲覧された回数が表示されます。<br>レポートリストの使用情報について詳しくは、<a href="../../../reports-and-dashboards/reports/report-usage/view-report-usage.md">レポートの使用状況の表示</a>の記事を参照してください。</td> 
  </tr>

<tr>
  <td> <code>[!UICONTROL width]</code>
  </td>
<td> レポートで、[!UICONTROL Text Mode]インターフェイスを使用する際に、各列の幅をピクセル単位で指定できるコード行。Workfront には、各フィールドの推奨幅が用意されていますが、
フィールドのタイプや形式に応じて、調整を行うこともできます。
追加の <code>[!UICONTROL usewidths=true]</code> コード行を使用して、列に指定された幅を強制する必要があります。 
  </td>

</tr>

<tr> 
   <td><code>[!UICONTROL work]</code> </td> 
   <td> <p>プロジェクト、タスクまたはイシューレポートで、テキストモードで次のステートメントを使用すると、プロジェクト、タスクまたはイシューの予定時間数が表示されます。</p>
   <code><p>valuefield=work</p>
   <p>valueformat=HTML</p></code> 
   <p>テキストモードの使用については、<a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">テキストモードの構文の概要</a>を参照してください。 </p> 
   <p><b>ヒント</b> 
   <p>イシューレポートで、[!UICONTROL Planned Hours]フィールドの 1 つを追加すると、<code>work </code>フィールドがレポートに追加されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work]</td> 
   <td> <p>2 つの主なライセンスタイプのうちの一つ。これは、[!UICONTROL Plan]よりもアクセス権限が弱いものの、システムで作成や更新を行うことができます。Work ライセンスを持つユーザーは、[!UICONTROL External]、[!UICONTROL Reviewer]、[!UICONTROL Requester] の各ライセンス所有者よりも多くの機能を持ちます。</p> <p>詳しくは、<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] ライセンスの概要</a>を参照してください。</p> <p>作業は、プロジェクト、タスクまたはイシューの[!UICONTROL Planned Hours]の数値を指す場合があります。詳しくは、この表の「[!UICONTROL work]」フィールドを参照してください。 </p> <p><b>ヒント</b></p> <p> イシューレポートで、[!UICONTROL Planned Hours]フィールドの 1 つを追加すると、<code>work </code>フィールドがレポートに追加されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Breakdown Structure]</td> 
   <td>親／子関係に基づく、プロジェクトチームで実行するタスクの階層構造。</td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Effort] </td> 
   <td> 
    <p>プロジェクトマネージャーは、タスクの完了に必要な作業量を見積もる際に、[!UICONTROL Planned Hours]の代わりにこのフィールドを使用できます。このフィールドは、次の条件を満たした場合にのみ表示されます。</p> 
     <ul> 
      <li> <p>タスクには[!UICONTROL Simple Duration Type]が含まれています。 </p> <p><b>ヒント</b></p> <p> タスク [!UICONTROL 期間タイプ ] を他のタイプに更新すると、このフィールドは非表示になります。 </p> </li> 
      <li>プロジェクトマネージャーが [!UICONTROL Use Work Effort]を有効にし、プロジェクトのタスクの[!UICONTROL Planned Hours]フィールドを自動的に計算できるようにした場合。 </li> 
     </ul> 
     <p>[!UICONTROL Planned Hours]の代わりに[!UICONTROL Work Effort]を使用してタスクの作業量を見積もる方法について詳しくは、<a href="../../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">作業量の概要</a>を参照してください。 </p> 
     <p>このフィールドは、タスクのレポートとリストに表示できます。</p> 
    </td> 
   </tr> 
  <tr> 
   <td>[!UICONTROL Work Item]</td> 
   <td> <p>このフィールドは、[!DNL Workfront] のタスクまたはイシューを参照します。 </p> <p>[!UICONTROL Work Item]レポートには、タスクとイシューの両方に関する情報が表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management mix]</td> 
   <td>ビジネスの実行に割り当てられた作業の、ビジネスの変更に対する割合を示す[!UICONTROL Work Performance Indicator]（WPI）。Mix WPI を使用すれば、戦略に実際の作業割り当てが適用されているかどうかを組織レベルで理解することができます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Resource]</td> 
   <td>作業を受け取ったり、時間を追跡したりすることができる、システム内のペルソナの指定。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Role and Responsibilities]</td> 
   <td>指定されたイシュー、タスク、プロジェクト、プログラム、またはポートフォリオの範囲、実行、承認を管理するための所有者と関係者を定義します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management SLA]</td> 
   <td>すべての関係者が合意した定量化可能な指標。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Management Stakeholder]</td> 
   <td>作業リクエストの結果に対する利害関係があるユーザーのコレクション。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work management touchpoints]</td> 
   <td>関係者間のコミュニケーションのデジタル化された記録。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Performance Indicators] </td> 
   <td> <p>割合、キャパシティ、速度、品質、エンゲージメントなどの組み合わせ。</p> <p>WPI は、Work Performance Indicator の頭字語です。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Work Process]</td> 
   <td> <p>作業を受け渡し、優先順位付けし、実行する方法。作業の実行方法は、通常、「ワークフロー」または「プロジェクトプラン」（日付、先行タスク関係などがあるタスクのリスト）と呼ばれます。 </p> <p>作業プロセスの例としては、1 つのアセットの作成や複数のアセットキャンペーンの配信などがあります。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Workflow template]</td> 
   <td>[!UICONTROL Proof Approval]レポートのこのフィールドに、プルーフに関連付けられているワークフローテンプレートが表示されます。テンプレートが添付されていない場合、この欄は空白になります。</td> 
  </tr>

<tr> 
   <td>[!UICONTROL Work Time]</td> 
   <td>

<p>ユーザーが実際の作業に使用できる（オーバーヘッドを含まない）フルタイム相当の（[!UICONTROL FTE]）時間の割合を表します。[!UICONTROL Work Time]は、1 までの 10 進数で指定する必要があります。0 は指定できません。例えば、実際の作業可能時間が 20%の場合は 0.2 になります。</p>
   </p>フィールドのデフォルト値は 1 で、これはユーザーが [!UICONTROL FTE] 時間全体を実際のプロジェクト関連の作業に費やすことを示します。  </p>
   <p>この数値を使用して、プロジェクト関連の実際の作業に対するユーザーの作業可能時間が計算されます。 </p>
   <p> スケジュールの例外と休暇も、ユーザーのキャパシティに影響を与える可能性があります。 </p>
   <p>Workfront でスケジュールを作成する方法について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md">スケジュールの作成</a>を参照してください。 </p>
    <p>Workfrontは、[!UICONTROL 設定 ] 領域のリソース管理環境設定に応じて、ユーザーの可用性を計算します。 詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md/">リソース管理環境設定の指定</a>を参照してください。 </p> 
   <p>ユーザーの[!UICONTROL Work Time]は、ユーザーの編集時または作成時に更新できます。詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md">ユーザーのプロファイルの編集</a>を参照してください。</p> 
   <b>ヒント</b> 
   <p>[!UICONTROL Work Time]の値を 1 に設定すると、ユーザーがフルタイム相当の時間をすべてプロジェクト関連の作業に使用できることを示します。</p> 
   </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Working time]</td> 
   <td>Workfront のドキュメントでは、この用語は、スケジュールに従って作業に割り当てられた時間を示します。</td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL workRequiredExpression]</code> </td> 
   <td> <p>プロジェクト、タスクまたはイシューのレポートで、次のステートメントをテキストモードで使用すると、プロジェクト、タスクまたはイシューの予定時間数の数値の後に「時間」という単語が表示されます。</p>
   <code>
   <p>valuefield=workRequiredExpression</p>
   <p>valueformat=HTML</p>
   </code>
    <p>テキストモードの使用については、<a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">テキストモードの構文の概要</a>を参照してください。 </p> </td> 
  </tr> 
 </tbody> 
</table>
