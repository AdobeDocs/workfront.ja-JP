---
product-area: resource-management
navigation-topic: resource-utilization
title: リソース稼働率情報の表示
description: 稼働率レポートで、リソースの稼働率を表示できます。
author: Alina, Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '7254'
ht-degree: 99%

---

# リソース稼働率情報の表示

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

稼働率レポートで、リソースの稼働率を表示できます。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

稼働率レポートにアクセスするには、次の条件を満たす必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：任意</p>
       <p>または</p>
       <p>現在：Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次の項目に対する表示以上のアクセス権：</p> 
    <ul> 
     <li> <p>リソース管理 </p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>ポートフォリオ</p> </li> 
     <li> <p>プログラム</p> </li> 
     <li> <p>財務データ（コスト別に情報を表示する場合）</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リソースエリアの「稼働率」セクションにアクセスするためのプロジェクト、ポートフォリオ、およびプログラムへのアクセスを表示</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>プロジェクトへのアクセスを管理して、プロジェクトの「稼働率」セクションにアクセスする</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## 稼働率レポートの概要 {#overview-of-the-utilization-report}

稼動率レポートを使用すると、プロジェクト、プログラムまたはポートフォリオの進行状況、コスト、売上高を 1 つのレポートに表示できます。また、収益とコストを比較することもできます。

リソースエリアで稼働率レポートを表示して、複数のプロジェクト間の稼働率を表示したり、1 つのプロジェクトのレベルで表示して、そのプロジェクトに関連するそれぞれのリソース（担当業務およびユーザー）の稼働率を表示したりできます。

稼働率レポートへのアクセスと使用について詳しくは、[稼動率レポートを使用して、進捗、コスト、収益をトラック](#track-progress-cost-and-revenue-with-the-utilization-report)の節を参照してください。

### 時間のトラック（進行状況） {#track-hours-progress}

予算計上時間数と予定時間数を実際の時間と比較して表示することで、進行状況をトラックできます。

プロジェクト、プログラムまたはポートフォリオの進行状況をトラッキングする場合、タスクとイシューに対する進行状況が稼働率レポートに含まれます。

時間をトラッキングする時に使用可能な稼働率レポートには、次の情報が含まれます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>時間表示時の列タイトル</strong> </th> 
   <th><strong>関数</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>予算計上時間数</strong> </td> 
   <td scope="col"> <p>該当するプロジェクトに対する予算計上時間数。該当するプロジェクトの全期間の予算計上時間数を表示するか、指定した日付範囲のみの予算計上時間数を表示できます（個別の週または月を指定できます）。 </p> <p>予算計上時間数は、ビジネスケースのリソース予算計上エリアまたはリソースプランナーで使用可能な情報から入力されます<em>。</em></p> <p>予算計上時間数は、次の行の稼働率レポートに表示されます。</p> 
    <ul> 
     <li> 予算計上時間数は、稼働率レポートで担当業務別および個々のユーザー別に、次のように要約されます。<br><strong>個々のユーザー：</strong>各ユーザーの予算計上時間数は、稼働率レポートに要約されます。これらの予算計上時間数は、該当するプロジェクトでユーザーが割り当てられたタスクおよびイシューに関連付けられます。（対応する担当業務の行を展開すると、その担当業務を持つユーザーのリストを表示できます。）<br><strong>担当業務：</strong>予算計上時間数は、稼働率レポートの担当業務別に要約されます。<br>予算計上時間数は、次のシナリオの結果、特定の担当業務に表示されます。
     <ul>
     <li>担当業務は、予算計上時間数が関連付けられているタスクまたはイシューに割り当てられるユーザーの主な担当業務として定義されます。 </li> 
       <li>1 つのプロジェクトの稼動率情報を表示するときに、タスクやイシューに割り当てがない場合、担当業務が割り当てられていない別のユーザーが割り当てられている場合、別の担当業務に割り当てられた別のユーザーが割り当てられている場合、または別のチームが割り当てられている場合に、時間を割り当てられたユーザーの担当業務が使用されます。</li> 
       <li>複数のプロジェクト、プログラム、ポートフォリオの稼働率情報を表示する場合、時間が割り当てられたユーザーの担当業務は、その役割がプロジェクト内のタスクまたはイシューに割り当てられている場合にのみ使用されます。 </li> 
       <li>担当業務が予算計上時間数に関連付いたタスクまたはイシューに割り当てられると、タスクまたはイシューに割り当てられたユーザーには、システムで定義された担当業務がありません。</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>未割り当て時間数</strong>：予算計上時間数は、タスクまたはイシューに関連し、タスクまたはイシューに割り当てられているユーザーまたは役割がない場合、「未割り当て時間数」セクションの稼働率レポートに表示されます。<br>このセクションは、プロジェクトにこの説明に一致する時間がある場合、および 1 つのプロジェクトの稼働率レポートを表示する場合にのみ表示されます。 </p> <p>このセクションは、この説明に一致するプロジェクトに時間がかかっている場合と、プロジェクトによる使用率レポートの表示時にのみ表示されます。 </p> </li> 
    </ul> <p>予算計上時間数について詳しくは、<a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md">プロジェクトの予算計上労力コストと予算計上時間数について</a>の記事の<a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md#locate-the-budgeted-hours-of-a-project">プロジェクトの予算計上時間数の検索</a>の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>予定時間数</strong> </td> 
   <td scope="col">
<p>
各タスクおよびイシューの割り当てに関連付けられた、該当のプロジェクトの予算計上時間数。該当するプロジェクトの全期間に対する、プロジェクトのすべての割り当ての合計予定時間数を表示できます。また、指定した日付範囲に対する予定時間数の合計を表示することもできます（個々の週または月を指定できます）。
</p>
<p>
<strong>ヒント</strong>
</p>
<p>
期間が 0 の項目からの予定時間数は考慮されません。 
</p>
<p>
稼働率レポートの予定時間数では、タスクまたはイシューの期間中に予定時間数が再割り当てされたかどうかが考慮されます。 
</p>
<p>
ワークロードバランサーを使用してユーザーの日次時間割り当てを変更した場合、稼働率レポートで選択した日付にタスクの期間またはイシューの期間が一部しか含まれていなければ、稼働率レポートのデータに影響することがあります。 
</p>
<p>
ユーザー割り当ての変更については、<a href="../workload-balancer/manage-user-allocations-workload-balancer.md">ワークロードバランサーでのユーザー割り当ての管理</a>を参照してください。


</p>
<p>
予定時間数は、稼働率レポートで次の行のいずれかに表示されます。
</p>
<ul>

<li>予定時間数は、稼働率レポートで担当業務別および個々のユーザー別に、次のように、要約されます。 
<ul>

<li><strong>個々のユーザー</strong>：各ユーザーの予定時間数は、稼働率レポートに要約されます。 これらの予定時間数は、該当するプロジェクトでユーザーが割り当てられたタスクおよびイシューに関連付けられます。 （対応する担当業務の行を展開すると、その担当業務を持つユーザーのリストを表示できます。）

<li><strong>担当業務</strong>：予定時間数は 1 つのプロジェクトの稼働率レポートで、担当業務別に要約されます。<br>予定時間数は、次のシナリオの結果として、特定の担当業務に表示されます。  
<ul>

<li>担当業務は、予定時間数が関連付けられているタスクまたはイシューに割り当てられる、ユーザーのプライマリ担当業務として定義されます。

<li>1 つのプロジェクトの稼働率情報を表示する場合、次のシナリオでは、担当業務に関連する時間は担当業務では表示されません。   
<ul>

<li>タスクまたはイシューに割り当てがありません

<li>担当業務割り当てのないユーザーが割り当てられています

<li>ユーザーに別の担当業務が割り当てられています

<li>チームがタスクまたはイシューに割り当てられています
</li>   
</ul>

<li>複数のプロジェクト、プログラム、ポートフォリオの稼働率情報を表示する場合、時間が割り当てられたユーザーの担当業務は、その役割がプロジェクト内のタスクまたはイシューに割り当てられている場合にのみ使用されます。複数のプロジェクトの稼働率レポートを表示する場合、担当業務の時間が別々に表示されることはありません。

<li>担当業務は、予定時間数が関連付けられたタスクまたはイシューに割り当てられ、タスクまたはイシューに割り当てられたユーザーには、システムで定義された担当業務はありません。
</li>  
</ul>

<li><strong>未割り当て時間数</strong>：予定時間数は、タスクまたはイシューに関連し、タスクまたはイシューに割り当てられているユーザーまたは役割がない場合、「未割り当て時間数」セクションの稼働率レポートに表示されます。このセクションは、この説明に一致するプロジェクトに時間がかかっている場合と、単一プロジェクトの稼働率レポートの表示時にのみ表示されます。<br>予定時間数について詳しくは、<a href="../../manage-work/tasks/task-information/planned-hours.md">予定時間数の概要</a>を参照してください。
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>実際の時間数</strong> </td> 
   <td> <p> 該当するプロジェクトのタスク、イシュー<span>および、プロジェクトに</span>ログオンした合計時間数。該当するプロジェクトの全期間の実際の合計時間数を表示することも、指定した日付範囲（個別の週または月を指定できます）の実際の合計時間数のみを表示することもできます。 </p> <p><strong>警告</strong>：稼動率レポートには、少なくとも 1 つの割り当てがあるプロジェクト、子タスク、イシューおよび親タスクに記録された時間が含まれます。割り当てのない親タスクに記録された時間は含まれません。 親タスクを作業タスクとして使用せず、子タスクのみをリソースに割り当てることをお勧めします。 </p> <p>実際の時間数は、稼働率レポートの次のいずれかの行に表示されます。</p> 
    <ul> 
     <li> 実際の時間数は、次のように、プロジェクトの稼働率レポートで、担当業務別およびそれぞれのユーザー別に要約されます。<br><strong>個々のユーザー：</strong>実際の時間数は、稼働率レポートの時間を記録したユーザーの行に表示されます。 （対応する担当業務の行を展開すると、その担当業務を持つ時間を記録したユーザーのリストを表示できます。）<br><strong>担当業務：</strong>これらの役割に関連するユーザーが記録した実際の時間数は、稼働率レポートの対応する担当業務の行に要約されます。<br>実際の時間数は、次のシナリオの結果として、特定の担当業務に表示されます。 
      <ul> 
       <li>担当業務は、時間を記録したユーザーのプライマリ担当業務として定義されます。</li> 
       <li>タスクまたはイシューに割り当てがありません</li> 
       <li>担当業務割り当てのない別のユーザーが割り当てられています</li> 
       <li>別のユーザーに別の担当業務が割り当てられています</li> 
       <li> <p>チームが割り当てられます。</p> </li> 
      </ul></li>  
     <p>時間数を記録しているユーザーの担当業務がユーザーのプロファイルに関連付けられていない場合、稼働率レポートに使用される担当業務は、時間数が記録されているタスクまたはイシューに割り当てられた担当業務か、タスクまたはイシューのプライマリ所有者に関連付けられている担当業務です。 </p> 
     <li><strong>その他の時間数：</strong>実際の時間数は、稼働率レポートの「その他の時間数」セクションか、時間数を記録したユーザーの行に表示されます。<br>時間数を記録したユーザーの担当業務がシステムで定義されていない場合に、このセクションに時間数が表示されます。<br>このセクションは、この説明と合致する時間数がプロジェクトにある場合にのみ表示されます。 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>予算計上差異（時間数の場合）</strong> </td> 
   <td> <p>予算計上時間数の合計から、含まれるプロジェクトの実際の時間数の合計を差し引いた値。表示されるのは、含まれるプロジェクトの全期間の予算計上差異の合計か、指定した日付範囲（個々の週または月を指定できます）のみの予算計上差異の合計です。 </p> <p>正の値の場合は、緑で表示されます。これは、予算計上時間数の合計が実際の時間数よりも多いことを示しています。</p> <p>負の値の場合は、赤で表示されます。これは、予算計上時間数の合計が実際の時間数よりも少ないことを示しています。</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>予定差異（時間数の場合）</strong> </td> 
   <td> <p>予定時間数の合計から、含まれるプロジェクトの実際の時間数の合計を差し引いた値。表示されるのは、含まれるプロジェクトの全期間の予定差異の合計か、指定した日付範囲（個々の週または月を指定できます）のみの予定差異の合計です。</p> <p>正の値の場合は、緑で表示されます。これは、予定時間数の合計が実際の時間数よりも多いことを示しています。</p> <p>負の値の場合は、赤で表示されます。これは、予定時間数の合計が実際の時間数よりも少ないことを示しています。</p> </td> 
  </tr> 
 </tbody> 
</table>

### コストの追跡 {#track-cost}

予算計上コストと予定コストを実際のコストと比較して表示することで、コストを追跡できます。

プロジェクト、プログラムまたはポートフォリオのコストを追跡する場合、稼働率レポートの情報はタスクから取得されます。タスクのコスト情報は、稼働率レポートで常に入手できます。タスクのコストは、タスクのコストタイプに基づいて計算されます。タスクのコストタイプについて詳しくは、[コストの追跡](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)で [Workfront によるタスクのコストタイプの計算方法](/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-cost-types-for-tasks)を参照してください。

稼働率レポートにコスト情報を表示する方法は、次のいずれかです。

* 特定の週か月、またはプロジェクト全体、プログラム全体、ポートフォリオ全体
* プロジェクトの役割別または個人別

稼働率レポートの通貨は、プロジェクトで設定された通貨によって決まります。プロジェクトの通貨を調整する方法については、[プロジェクトの通貨の変更](../../manage-work/projects/project-finances/change-project-currency.md)を参照してください。

コストの追跡時に稼働率レポートで入手できる情報は次のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>コスト表示時の列タイトル</strong> </th> 
   <th> <p><strong>機能</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>予算計上コスト</strong> </td> 
   <td scope="col"> <p>含まれるプロジェクトの予算計上コスト。表示されるのは、含まれるプロジェクトの全期間の予算計上コストの合計か、指定した日付範囲（個々の週または月を指定できます）のみの予算計上コストの合計です。</p> <p>稼働率レポートの予算計上コストは役割別のコストに的を絞っているので、Workfront の他のエリア内の予算計上労力コストと同じ計算になります。予算計上労力コストの計算方法については、<a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">プロジェクトの予算計上労力コストと予算計上時間数について</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>予定コスト</strong> </td> 
   <td scope="col"> <p>含まれるプロジェクトの合計予定コスト。含まれるプロジェクトの全期間の予定コストの合計か、または指定した日付範囲のみの予定コストの合計を表示することができます（個々の週または月を指定できます）。</p> <p>週、月および四半期表示では、予定コストは、担当業務またはユーザーのコスト率が日付上有効な選択した期間の平均として計算されます。</p><p>プロジェクトの予定コストの計算方法について詳しくは、<a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">コストの追跡</a>の<a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">Workfront による予定コスト、予算計上コスト、実際のコストの計算方法</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"><strong>実際のコスト</strong> </td> 
   <td scope="col"> <p>含まれるプロジェクトの実際のコストの合計。表示されるのは、含まれるプロジェクトの全期間にわたる実際のコストの合計か、指定した日付範囲（個別の週または月を指定できます）のみの実際のコストの合計です。</p> <p>プロジェクトの実際のコストの計算方法について詳しくは、<a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">コストの追跡</a>の<a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">Workfront による予定コスト、予算計上コスト、実際のコストの計算方法</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td><strong>予算計上差異（コストの場合）</strong> </td> 
   <td scope="col"> <p>予算計上コストの合計から、含まれるプロジェクトの実際のコストの合計を差し引いた値。表示されるのは、含まれるプロジェクトの全期間の予算計上差異の合計か、指定した日付範囲（個々の週または月を指定できます）のみの予算計上差異の合計です。</p> <p>正の値の場合は、緑で表示されます。これは、予算計上コストの合計が実際のコストよりも多いことを示しています。</p> <p>負の値の場合は、赤で表示されます。これは、予算計上コストの合計が実際のコストよりも少ないことを示しています。</p> </td>
  </tr> 
  <tr> 
   <td><strong>予定差異（コストの場合）</strong> </td> 
   <td> <p>予定コストの合計から、含まれるプロジェクトの実際のコストの合計を差し引いた値。表示されるのは、含まれるプロジェクトの全期間の予定差異の合計か、指定した日付範囲（個々の週または月を指定できます）のみの予定差異の合計です。 </p> <p>正の値の場合は、緑で表示されます。これは、予定コストの合計が実際のコストよりも多いことを示しています。</p> <p>負の値の場合は、赤で表示されます。これは、予定コストの合計が実際のコストよりも少ないことを示しています。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 収益の追跡 {#track-revenue}

予算計上収益と予定収益を実収益と比較して表示することで、収益を追跡できます。

プロジェクト、プログラムまたはポートフォリオの収益を追跡する場合、タスクからの収益のみが稼働率レポートに含まれます。

収益の追跡時に稼働率レポートで入手できる情報は、次の表のとおりです。

特定のフィールドと Workfront によるフィールドの計算方法について詳しくは、[コストの追跡](../../manage-work/projects/project-finances/track-costs.md)および[請求と収益の概要](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)も参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>収益表示時の列タイトル</strong> </th> 
   <th> <strong>機能</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>予算計上収益</strong> </td> 
   <td scope="col"> <p>予算計上時間数の合計に、含まれるプロジェクトの役割請求レートを掛けた値。表示されるのは、含まれるプロジェクトの全期間の予算計上収益の合計か、指定した日付範囲（個々の週または月を指定できます）のみの予算計上収益の合計です。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>予定収益</strong> </td> 
   <td scope="col"> <p>稼働率レポートの予定収益は、プロジェクトのタスクに割り当てられたリソースに配分された予定時間数に関連付けられた収益です。</p> <p>Workfront では、次の式を使用して、稼働率レポートのプロジェクト予定収益を計算します。</p> <p><code>Project Planned Revenue = SUM (All Tasks Planned Revenue)</code> </p> 
   <p><b>メモ</b>
   <p>稼働率レポートに表示されるプロジェクト予定収益は、プロジェクト詳細エリアおよびプロジェクトレポートに表示される予定収益とは異なります。 </p> <p>プロジェクト詳細エリアの予定収益には、タスクの収益とプロジェクトの固定収益が反映されています。稼働率レポートの予定収益には、プロジェクトのタスクに関連付けられた予定収益のみが表示されます。 </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>プロジェクトに 10 時間のタスクが 1 つあり、そのタスクがコンサルタントに時給 20 ドルで割り当てられ、プロジェクトの固定収益が 100 ドルの場合、稼働率レポートには予定収益（タスクの時間数に関連付けられた予定収益）として 200 ドルが表示されます。「プロジェクト詳細」セクションには、300 ドル（タスクからの予定収益とプロジェクトの固定収益）が表示されます。 </p> 
     </div> <p>稼働率レポート以外のタスクおよびプロジェクトの予定収益について詳しくは、<a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。</p> </p> <p>含まれるプロジェクトの予定収益が稼働率レポートで計算および表示される際には、タスクに設定された収益タイプが考慮されます。 </p> <p>プロジェクト内の各タスクの収益タイプに応じて、次のシナリオが存在します。 </p> <p><strong>固定収益：</strong>タスクの割り当てに関係なく、タスクの収益は常に、タスクに指定された定額を使用して計算されます。</p> <p><b>重要</b>

Workfront の他のエリアとは異なり、稼働率レポートでは、固定収益をタスクの予定時間数で均等に割ることで、固定収益タスクの予定収益が計算されます。 </p> <p>例えば、タスクの収益が 200 ドルだとします。タスクの予定時間数が 4 時間の場合、各時間の収益は 50 ドルになります。これがユーザーおよび役割レベルで配分されます。この配分は、稼働率レポートに固有のものです。</p> <p><b>メモ</b>

固定収益タスクがあり、タスクに予定時間数がない場合、収益を各時間に配分する方法がないので、収益は稼働率レポートに表示されません。固定収益があるタスクに関する予定時間数があり、割り当てがない場合、収益は「未割り当て収益」として表示されます。 </p> <p><strong>役割 (毎時)：</strong>タスクの収益は、特定の役割に設定された請求レートに、その役割に関連付けられた予定時間数を掛けて計算されます。Workfront では次の数式が使用されます。</p> <p><code>役割 (毎時) の予定収益 = SUM(すべてのタスクにおける役割の予定時間数) * 役割の請求レート</code></p><p><b>メモ</b>：式中の請求時給では、有効なレートの変更の日付が考慮されます。</p>   <p><strong>ユーザー (毎時)：</strong>タスクの収益は、特定のユーザーに設定された請求レートに、そのユーザーに関連付けられた予定時間数を掛けて計算されます。Workfront では次の数式が使用されます。</p> <p><code>ユーザー (毎時) の予定収益 = SUM(すべてのタスクにおけるユーザーの予定時間数) * ユーザーの請求レート</code> </p> <p><b>メモ</b>：式中の請求時給では、有効なレートの変更の日付が考慮されます。</p> <p><b>役割 (毎時) + 固定またはユーザー (毎時) + 固定</b> </p> <p><b>重要</b>

Workfront の他のエリアとは異なり、稼働率レポートでは、固定収益をタスクの予定時間数で均等に割ることで、予定収益を計算します。 </p> <p>次のケースが存在します。 </p>
<ul>
<li> <p><strong>役割 (毎時) + 固定：</strong>タスクの収益は、特定の役割に設定された請求レートに、その役割に関連付けられた予定時間数を掛けた値を使用して計算されます。さらに、タスクに指定された定額が役割のレートに追加されます。Workfront では次の数式が使用されます。</p> <p><code>役割 (毎時) + 固定の予定収益 = [SUM(すべてのタスクにおける役割の予定時間数) * 役割の請求料率] + SUM(タスクの上限または定額 / タスクの予定時間数)</code> </p> </li>
<li> <p><strong>ユーザー (毎時) + 固定：</strong>特定のユーザーに設定された請求レートに、そのユーザーのタスクの予定時間数を掛けた値。さらに、タスクに指定された定額がユーザーのレートに追加されます。Workfront では次の数式が使用されます。</p> <p><code>ユーザー (毎時) + 固定の予定収益 = [SUM(すべてのタスクにおけるユーザーの予定時間数) * ユーザーの請求レート] + SUM(タスクの上限または定額 / タスクの予定時間数)</code> </p> </li>
</ul> <p><b>役割 (毎時) (上限付き) またはユーザー (毎時) (上限付き)</b> </p> <p><b>重要</b>

Workfront の他のエリアとは異なり、予定収益が上限を超える場合、上限額を超える金額は固定収益と見なされます。予定収益は、固定収益をタスクの予定時間数で均等に割り、上限金額と役割またはユーザーの時間収益に加算して計算されます。<br></p> <p>次のケースが存在します。 </p>
<ul>
<li> <p><strong>役割 (毎時) (上限付き)：</strong>タスクは役割 (毎時) と同様に時間単位で請求されますが、指定できる最大上限額があります。Workfront では次の数式が使用されます。</p> <p><code>役割 (毎時) (上限付き) の予定収益 = [SUM(すべてのタスクおよびイシューにおける役割の予定時間数) * 役割の請求レート] + タスクの上限額 + SUM(タスクの上限額を超えた金額 / タスクの予定時間数)</code> </p> </li>
<li> <p><strong>ユーザー (毎時) (上限付き)：</strong>タスクはユーザー (毎時) と同様に時間単位で請求されますが、指定できる最大上限額があります。Workfront では次の数式が使用されます。 </p> <p><code>ユーザー (毎時) (上限付き) の予定収益 = [SUM(すべてのタスクにおけるユーザーの予定時間数) * ユーザーの請求レート] + タスクの上限額 + SUM(タスクの上限額を超えた金額 / タスクの予定時間数)</code> </p> </li>
</ul> <p>予定収益の計算時に考慮される役割またはユーザーについて詳しくは、<a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td><strong>実収益</strong> </td>
   <td> <p>実収益は、タスクおよびプロジェクトの実際の時間数に関連付けられた収益です。実収益について詳しくは、<a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md">請求と収益の概要</a>の<a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#track-revenue-amounts">収益金額の追跡</a>を参照してください。</p>

<p>稼働率レポートで、含まれるプロジェクトの実収益を計算する方法は、次のように、タスクに設定された収益タイプによって異なります。</p> <p><strong>固定収益：</strong>タスクの割り当てに関係なく、タスクの収益は常に、タスクに指定された定額を使用して計算されます。</p> <p><b>重要</b>

Workfront の他のエリアとは異なり、稼働率レポートでは、固定収益をタスクで記録された時間数で均等に割ることで、実収益が計算されます。 </p> <p> </p> <p>例えば、タスクの実収益が 200 ドルだとします。タスクの実際の時間数が 4 時間の場合、各時間の実収益は 50 ドルになります。これがユーザーおよび役割レベルで配分されます。この配分は、稼働率レポートに固有のものです。</p> <p><b>メモ</b>

固定収益タスクがあり、タスクに実際の時間数がない場合、収益を各時間に配分する方法がないので、実収益は稼働率レポートに表示されません。 </p> <p><strong>役割 (毎時)：</strong>タスクの収益は、特定の役割に設定された請求レートと実際の時間数を掛けて計算されます。</p> <p>Workfront では次の数式が使用されます。</p> <p><code>役割 (毎時) の実収益 = SUM(すべてのタスクにおける役割の実際の時間数) * 役割の請求レート</code> </p> <p><b>メモ：</b>式中の請求時給では、有効なレートの変更の日付が考慮されます。</p> <p><strong>ユーザー (毎時)：</strong>タスクの収益は、特定のユーザーに設定された請求レートに、そのユーザーのタスクに対して記録された時間数を掛けて計算されます。Workfront では次の数式が使用されます。</p> <p><code>ユーザー (毎時) の実収益 = SUM(すべてのタスクにおけるユーザーの実際の時間数) * ユーザーの請求レート</code></p> <p><b>メモ：</b>式中の請求時給では、有効なレートの変更の日付が考慮されます。</p> <p><b>役割 (毎時) + 固定またはユーザー (毎時) + 固定</b> </p> <p><b>重要</b>

Workfront の他のエリアとは異なり、稼働率レポートでは、固定収益をタスクで記録された時間数で均等に割ることで、実収益が計算されます。 </p> <p>次のケースが存在します。 </p>
<ul>
<li> <p><strong>役割（時間単位）+ 固定：</strong>特定の役割に設定された請求レートに、その役割を持つユーザーがタスクに対して記録した時間数を掛けたもの。さらに、タスクに指定された定額が役割のレートに追加されます。 </p> <p>Workfront では次の数式が使用されます。</p> <p><code>役割予定収益（時間単位）+ 固定予定収益 = [SUM（全タスクの役割からの実際の時間数） * 役割請求レート] + SUM（タスクの請求金額 / タスクの実際の時間数）</code> </p> </li>
<li> <p><strong>ユーザー（時間単位）+ 固定：</strong>特定のユーザーに設定された請求レートと、そのユーザーがタスクに対して記録した時間数を掛けた値を使用して計算されます。さらに、タスクに指定された定額がユーザーのレートに追加されます。 </p> <p>Workfront では次の数式が使用されます。</p> <p><code>ユーザー（時間単位）+ 固定実収益 = [SUM（全タスクの役割からの実際の時間数） * ユーザー請求レート] + SUM（タスクの請求金額 / ユーザーのタスクの時間数）</code> </p> </li>
</ul> <p><b>役割（時間単位）またはユーザー（時間単位）（キャップあり）</b> </p> <p><b>重要</b>

Workfront の他のエリアとは異なり、予定収益が上限を超える場合、上限額を超える金額は固定収益と見なされます。予定収益は、固定収益をタスクの予定時間数で均等に割り、上限金額と役割またはユーザーの時間収益に加算して計算されます。<br></p> <p>次のケースが存在します。</p>
<ul>
<li> <p><strong>役割 (毎時) (上限付き)：</strong>タスクは役割 (毎時) と同様に時間単位で請求されますが、指定できる最大上限額があります。Workfront では次の数式が使用されます。</p> <p><code>役割実収益（時間単位）（キャップあり）= [SUM（全タスクおよびイシューの役割からの実際の時間数） * 役割請求レート] + タスクのキャップ額 + SUM（タスクのキャップ額を超えた額 / タスクの実際の時間数）</code></p> </li>
<li> <p><strong>ユーザー（時間単位）（キャップあり）：</strong>タスクはユーザー（時間単位）と同様に時間単位で請求されますが、指定できる最大キャップ額があります。</p> <p> Workfront では次の数式が使用されます。</p> <p><code>ユーザー実収益（時間単位）（上限あり）= [SUM（全タスクおよびイシューの役割からの実際の時間数） * ユーザー請求レート] + タスクのキャップ額 + SUM（タスクのキャップ額を超えた額 / タスクの実際の時間数）</code> </p> </li>
</ul>
<p><strong>プロジェクトの収益</strong>：プロジェクトに対して記録された時間に関連付けられた収益は、時間をログに記録したユーザーの主な担当業務の時間当たりの請求金額を考慮して計算されます。プロジェクトに時間を記録することはお勧めしません。 </p>
<p><b>メモ</b>

ユーザーが担当業務に関連付けられていない場合、または主要役割の時間当たりの請求額がゼロの場合、Workfront はユーザーの時間当たりの請求額を使用して実収益を計算します。ユーザーのプロファイルに時間あたりの請求額がない場合、実収益は 0 になります。 </p>
</td> 
  </tr> 
  <tr> 
   <td><strong>予算計上差異（収益用）</strong> </td> 
   <td> <p>含まれるプロジェクトの合計実収益から予算計上収益を引いた値。<br>含まれるプロジェクトの全期間の予算計上差異の合計か、または指定した日付範囲の予算計上差異の合計のみを表示できます（個々の週または月を指定できます）。</p> <p>正の値の場合は、緑で表示されます。これは、合計予算計上収益が実収益よりも大きいことを示します。</p> <p>負の値の場合は、赤で表示されます。これは、合計予算計上収益が実収益よりも少ないことを示します。</p> </td>
  </tr> 
  <tr> 
   <td><strong>予定差異（収益用）</strong> </td> 
   <td> <p>含まれるプロジェクトの合計実収益から合計予定収益を引いた値。<br>含まれるプロジェクトの全期間の予算計上差異の合計か、または指定した日付範囲の予算計上差異の合計のみを表示できます（個々の週または月を指定できます）。 </p> <p>正の値の場合は、緑で表示されます。これは、予定収益の合計が実収益よりも大きいことを示します。</p> <p>負の値の場合は、赤で表示されます。これは、予定収益の合計が実収益よりも少ないことを示します。</p> </td>
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### 収益と予定コストおよび実際のコストとの比較 {#compare-revenue-against-planned-and-actual-costs}

予定収益と共に、予定コストまたは実際のコストを表示できます。利益（％）も表示されます（利益は収益 - コスト / 収益として計算されます）。

収益対予定コストおよび実コストの比較をする場合は、以下の情報が稼働率レポートで使用可能です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>収益対コスト（予定）を表示する際の列のタイトル</strong> </th> 
   <th> <strong>関数</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>予定コスト</strong> </td> 
   <td scope="col"> 含まれるプロジェクトの合計予定コスト。含まれるプロジェクトの全期間の予定コストの合計か、または指定した日付範囲のみの予定コストの合計を表示することができます（個々の週または月を指定できます）。 </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>予定収益</strong> </td> 
   <td scope="col"> <p>予定収益は、タスクの予定時間数に関連付けられた収益です。 </p> <p>稼働率レポートで、含まれるプロジェクトの予定収益を計算および表示する方法は、タスクに設定された収益タイプによって異なります。詳しくは、この記事にある<a href="#track-revenue" class="MCXref xref">収益の追跡</a>の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>利益</strong> </td> 
   <td scope="col"> <p>利益率は次のように計算されます。</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>メモ</b>

予定収益が 0 に等しい場合、利益は 0 と表示されます。 </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>収益対コスト（実績）を表示する際の列タイトル</strong> </p>  </td> 
   <td scope="col"><p><strong>機能</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>実際のコスト</strong> </td> 
   <td scope="col"> <p>含まれるプロジェクトの実際のコストの合計。表示されるのは、含まれるプロジェクトの全期間にわたる実際のコストの合計か、指定した日付範囲（個別の週または月を指定できます）のみの実際のコストの合計です。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>実収益</strong> </td> 
   <td> <p>実収益は、タスクの実際の時間数に関連付けられた収益です。</p> <p>実収益は、タスクが「完了」（または「完了」と同等のステータス）とマークされた後にのみ、稼働率レポートに表示されます。</p> <p>稼働率レポートで、含まれるプロジェクトの実収益を計算する方法は、タスクに設定された収益タイプによって異なります。詳しくは、この記事にある<a href="#track-revenue" class="MCXref xref">収益の追跡</a>の節を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>利益</strong> </td> 
   <td> <p>利益率は次のように計算されます。</p> <p>(実収益 - 実際のコスト) / 実収益 * 100。 </p> <p><b>メモ</b>

実収益が 0 の場合、利益は 0 と表示されます。 </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## 稼動率レポートを使用して、進捗状況、コストおよび収益を追跡します。 {#track-progress-cost-and-revenue-with-the-utilization-report}

プロジェクト、プログラムまたはポートフォリオの進捗状況やコストを追跡できます。

特定の週や月またはプロジェクトの全期間の情報を稼働率レポートに表示できます。

稼働率レポートを使用して 1 つ以上のプロジェクトの進捗状況やコストを追跡するには、次の手順に従います。

1. 個々のプロジェクト、複数のプロジェクト、プログラム、ポートフォリオのどの稼働率情報を表示するかに応じて、以下のいずれかを行います。

   * 1 つのプロジェクトの稼働率情報を表示するには：

      1. 稼働率情報を表示するプロジェクトに移動し、**さらに表示／稼働率**&#x200B;とクリックします。
      1. 個々のプロジェクトを表示する場合は、稼働率情報が自動的に表示され、フィルターを適用する必要はありません。\
         稼働率レポートをフィルタリングする場合は、フィルターを適用してから、「**実行**」をクリックします。\
         稼働率レポートをフィルタリングする方法について詳しくは、この記事の[稼働率情報のフィルタリング](#filter-utilization-information)を参照してください。\
         個々のユーザーと役割の稼働率情報が表示されます（ユーザーは、関連付けられている役割内にグループ化されます）。

   * 複数のプロジェクトの稼働率情報を表示するには：

     {{step1-to-utilization-report}}

      1. 稼働率レポートにフィルターを適用し、「**実行**」をクリックします。
稼働率レポートを実行する前に、フィルターで 1 つ以上のプロジェクトを指定する必要があります。稼働率レポートをフィルタリングする方法について詳しくは、この記事の[稼働率情報のフィルタリング](#filter-utilization-information)を参照してください。\
         稼働率情報は、個々の役割およびプロジェクトごとに表示されます（役割は、関連するプロジェクト内でグループ化されます）。

   * プログラムの稼働率情報を表示するには、次の操作を行います。

     {{step1-to-utilization-report}}

      1. **表示**／**プログラム**&#x200B;をクリックします。
      1. 稼働率レポートにフィルターを適用し、「**実行**」をクリックします。\
         稼働率レポートを実行する前に、フィルターで 1 つ以上のプログラムを指定する必要があります。稼働率レポートをフィルタリングする方法について詳しくは、この記事の[稼働率情報のフィルタリング](#filter-utilization-information)を参照してください。\
         稼働率情報は、個々のプロジェクトおよびプログラムごとに表示されます（プロジェクトは、関連するプログラム内でグループ化されます）。

   * ポートフォリオの稼働率情報を表示するには、次の操作を行います。

     {{step1-to-utilization-report}}

      1. **表示**／**ポートフォリオ**&#x200B;をクリックします。
      1. 稼働率レポートにフィルターを適用し、「**実行**」をクリックします。\
         稼働率レポートを実行する前に、フィルターで 1 つ以上のポートフォリオを指定する必要があります。稼働率レポートをフィルタリングする方法について詳しくは、この記事の[稼働率情報のフィルタリング](#filter-utilization-information)を参照してください。\
         稼働率情報は、個々のプロジェクト、プログラム、ポートフォリオごとに表示されます（プロジェクトは関連するプログラム内でグループ化され、プログラムは関連するポートフォリオ内でグループ化されます）。

1. 稼働率レポートの右上隅で、「**ビュー**」をクリックし、メニューで次から選択します。

   * **コスト**
   * **時間**
   * **収益**
   * **収益対コスト（予定）**
   * **収益対コスト（実際）**

   選択したオプションに応じて、レポートで使用できる列と情報が決まります。
   ![オプションの表示](assets/utilization-view-dropdown.png)

1. （オプション）稼働率情報を表示する日付範囲を選択します。特定の週または月の情報を&#x200B;**全体**&#x200B;列の左側に表示できます。プロジェクト、プログラムまたはポートフォリオ全体の情報は、常に&#x200B;**全体**&#x200B;列に表示されます。\
   詳しくは、この記事の[情報を表示する日付範囲の調整](#adjust-the-date-range-for-which-information-is-displayed)を参照してください。

1. （オプション）任意の列タイトルをクリックすると、その列の情報に基づいて稼働率レポートを並べ替えることができます。並べ替えは、レポートに複数の項目が含まれている場合にのみ機能します。例えば、複数のプロジェクト（またはポートフォリオやプログラム）を表示している場合に、レポートの結果を並べ替えることができます。一度に 1 つのプロジェクト（または 1 つのポートフォリオや 1 つのプログラム）しか表示していない場合は、結果を並べ替えることはできません。
1. 稼働率レポートの各列について確認するには、この記事の[稼働率レポートの概要](#overview-of-the-utilization-report)の節に記載されている情報を参照してください。

## 稼働率情報をフィルタリング {#filter-utilization-information}

プロジェクトの稼働率レポートに表示される内容をフィルタリングできます。タスク、イシュー、役割およびカスタムデータをフィルタリングできます。フィルターを適用すると、選択した基準に基づく情報が稼働率レポートに表示されます。

新規フィルターを作成するか、以前に作成したフィルターを適用できます。

### フィルターを作成または変更 {#create-or-modify-a-filter}

フィルターを作成すると、稼働率レポートにアクセスできるすべての Workfront ユーザーが作成したフィルターにアクセスできるようになります。同様に、既存のフィルターを変更すると、稼働率レポートにアクセスできるすべてのユーザーに対してフィルターの変更が適用されます。

フィルターを作成または変更するには、次の操作を行います。

1. 稼働率レポートを開きます。
これを行うには、[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

1. 「**フィルター**」アイコンをクリックして、フィルターオプションを表示します。
1. （条件付き）既存のフィルターを変更するには、**フィルター**&#x200B;ドロップダウンメニューをクリックして、変更するフィルターを選択します。
1. フィルターを作成または変更するには、次の情報を指定します。

   * **ポートフォリオ：**&#x200B;稼働率レポートに含める情報が格納されているポートフォリオの名前を入力し、ドロップダウンリストにその名前が表示されたらクリックします。\
     このプロセスを繰り返して、複数のポートフォリオの情報を稼働率レポートに含めます。\
     システムのすべてのポートフォリオをフィルターに含めるには「**すべて追加**」をクリックします（このオプションは、システム内のポートフォリオが 10 件未満の場合にのみ使用できます）。

   * **プログラム：**&#x200B;稼動率レポートに含める情報が格納されているプログラムの名前を入力し、ドロップダウンリストにその名前が表示されたらクリックします。\
     このプロセスを繰り返して、複数のタスクの情報を稼働率レポートに含めます。\
     フィルターで既にポートフォリオを指定している場合、指定するプログラムは、既にフィルターに含まれているポートフォリオに属している必要があります。指定していない場合、プログラムのデータは稼動率レポートに含まれません。\
     システムのすべてのプログラムをフィルターに含めるには、「**すべて追加**」をクリックします（このオプションは、システム内のプログラムが 20 件未満の場合にのみ使用できます）。

   * **プロジェクト：**&#x200B;稼動率レポートに含める情報が格納されているプロジェクトの名前を入力し、ドロップダウンリストにその名前が表示されたらクリックします。\
     このプロセスを繰り返して、複数のプロジェクトの情報を稼働率レポートに含めます。\
     フィルターで既にポートフォリオまたはプログラムを指定している場合、指定するプロジェクトは、既にフィルターに含まれているポートフォリオまたはプログラムのいずれかに属している必要があります。指定していない場合、プロジェクトのデータは稼動率レポートに含まれません。\
     システムのすべてのプロジェクトをフィルターに含めるには、「**すべて追加**」をクリックします（このオプションは、システム内のプロジェクト数が 250 件未満の場合にのみ使用できます）。

   * **タスク：**&#x200B;稼動率レポートに含める情報が格納されているタスクの名前を入力し、ドロップダウンリストにその名前が表示されたらクリックします。\
     このプロセスを繰り返して、複数のタスクの情報を稼働率レポートに含めます。\
     フィルターで既にポートフォリオ、プログラム、またはプロジェクトを指定している場合、指定するタスクは、既にフィルターに含まれているポートフォリオ、プログラム、またはプロジェクトのいずれかに属している必要があります。指定していない場合、タスクのデータは稼動率レポートに含まれません。

   * **イシュー：**&#x200B;稼動率レポートに含める情報が格納されているイシューの名前を入力し、ドロップダウンリストにその名前が表示されたらクリックします。\
     このプロセスを繰り返して、複数のイシューの情報を稼働率レポートに含めます。\
     フィルターで既にポートフォリオ、プログラム、またはプロジェクトを指定している場合、指定するイシューは、既にフィルターに含まれているポートフォリオ、プログラム、またはプロジェクトのいずれかに属している必要があります。指定していない場合、イシューのデータは稼動率レポートに含まれません。\
     イシューのコスト情報は、稼働率レポートに含まれない場合があります。イシューのコスト情報が稼働率レポートに含まれる場合について詳しくは、この記事の[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

   * **役割：**稼動率レポートに表示する役割の名前を入力し、ドロップダウンリストに表示されたらその名前をクリックします。この手順を繰り返して、その他の役割を追加します。
稼働率レポートには、指定した役割の情報のみが表示されます。例えば、タスクに含まれる実際の時間数が 10 時間であるとします。そのうち 6 時間はデザイナーの役割から、4 時間は開発者の役割からのものです。デザイナーの役割で稼働率レポートをフィルタリングすると、開発者の役割の 4 時間がレポートから除外されます。

   * **フィルタールールを追加：**「**フィルタールールを追加**」をクリックしたあと、テキストフィールドをクリックし、フィルタリングするフィールド名を入力します。フィールドが使用可能な場合は、関連付けることが可能な各オブジェクトに対してが設定されます。フィールド名をクリックして、フィルターに追加します。

     >[!IMPORTANT]
     >
     >フィールドラベルではなく、フィールド名を入力する必要があります。フィールドラベルは、オブジェクトに添付されたカスタムフォームに表示されます。カスタムフィールドのラベルと名前の違いについて詳しくは、[カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

     列に表示されるフィールドについて詳しくは、[Adobe Workfront の用語集](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。\
     フィルターとフィルターの条件修飾子を選択します。使用可能な修飾子について詳しくは、[フィルターと条件修飾子](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)を参照してください。

1. 新しいフィルターを作成するには、「**フィルターを保存**」をクリックします。\
   または\
   既存のフィルターを変更するには、「**フィルターを保存**」ボタンの横にある矢印をクリックし、「**新規フィルターを保存**」をクリックします。
「**フィルター名**」フィールドにフィルター名を指定し、「**保存**」をクリックします。
稼働率領域は、フィルターに含めた情報でフィルタリングされます。

### 保存済みフィルターを適用 {#apply-a-saved-filter}

1. 稼働率レポートを開きます。
これを行うには、[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

1. 「**保存したフィルター**」をクリックし、ドロップダウンリストから適用するフィルターを選択します。

### フィルターを複製 {#duplicate-a-filter}

1. 稼働率レポートを開きます。
これを行うには、[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

1. 「**保存したフィルター**」をクリックし、複製するフィルターの上にポインタを合わせて、**複製**&#x200B;アイコンをクリックします。

   ![複製アイコン](assets/utilization-filter-duplicate.png)

   フィルターを複製ダイアログボックスが表示されます。

1. 「**フィルター名**」フィールドに新しいフィルター名を入力し、「**保存**」をクリックします。

### フィルターの名前を変更する {#rename-a-filter}

フィルターの名前を変更すると、稼働率レポートにアクセスできるすべての Workfront ユーザーに対して、入力した新しい名前が表示されます。

フィルターの名前を変更するには、次の手順に従います。

1. 稼働率レポートを開きます。
これを行うには、[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

1. 「**保存したフィルター**」をクリックし、名前を変更するフィルターの上にポインタを合わせて、**名前を変更**&#x200B;アイコンをクリックします。

   ![フィルター名を変更アイコン](assets/utilization-filter-rename.png)

   フィルター名を変更ダイアログボックスが表示されます。

1. 「**フィルター名**」フィールドに新しいフィルター名を入力し、「**保存**」をクリックします。

### フィルターを削除 {#delete-a-filter}

フィルターを削除すると、稼働率レポートにアクセスできるすべての Workfront ユーザーのフィルターが削除されます。

フィルターを削除するには、次の手順に従います。

1. 稼働率レポートを開きます。
これを行うには、[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

1. 「**保存したフィルター**」をクリックし、削除するフィルターの上にポインタを合わせて、**削除**&#x200B;アイコンをクリックします。

   ![削除アイコン](assets/utilization-filter-delete.png)

1. フィルターを削除するかどうかを確認するメッセージが表示されたら、「**削除**」をクリックします。

## 情報を表示する日付範囲を調整 {#adjust-the-date-range-for-which-information-is-displayed}

稼働率情報を表示する日付範囲を調整できます。 過去の日付または未来の日付を選択できます。 加えた変更は、自分だけに表示されます。

1. 稼働率レポートを開きます。
これを行うには、[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

1. 「**書き出し**」ボタンの横にある日付範囲をクリックします。

   デフォルトでは、現在の週が選択されています。

1. 次のオプションから選択します。

   * **週：**&#x200B;特定の週（日曜日から土曜日）を選択するには、このオプションを選択します。
   * **月：**&#x200B;特定の月を選択するには、このオプションを選択します。

   選択した日付範囲は、稼働率レポートの&#x200B;**全体**&#x200B;列の左側に表示されます。\
   Workfront は、週または月表示のどちらを表示するかを記憶します。 次回稼働率レポートにアクセスすると、選択したオプションに応じて、現在の週または現在の月が表示されます。

## 稼働率情報を書き出し

プロジェクト、プログラム、ポートフォリオの稼働率情報を Workfront から書き出すことができます。XLSX、TSV、PDF 形式でのみ、情報を書き出すことができます。

Microsoft Excel で表示すると、負の数値が括弧で囲まれて表示されます。

稼働率情報を書き出すには、以下の手順に従います。

1. 稼働率レポートを開きます。
これを行うには、[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

1. レポートの左上にある「**書き出し**」をクリックします。

1. 次のオプションから選択します。

   * **PDF：**&#x200B;レポートを PDF 形式で書き出します。 レポートを印刷する予定がある場合は、この形式が推奨されます。\
     **レター - 縦**、**レター - 横**&#x200B;または&#x200B;**その他のサイズ**（リーガル（8.5 インチ x 14 インチ）、台帳（11 インチ x 17 インチ）および A4 での書き出しのオプションがあります）のいずれかを選択します。
使用しているオペレーティングシステムによっては、ファイルを開くか保存するかを選択できます。 関連するアプリケーションでファイルを開くか、ご使用のコンピューターに保存します。

   * **Excel：**レポートを XLSX 形式で書き出します。 Excel でのデータをさらに分析する予定がある場合は、この形式をお勧めします。
使用しているオペレーティングシステムによっては、ファイルを開くか保存するかを選択できます。 関連するアプリケーションでファイルを開くか、ご使用のコンピューターに保存します。

   * **タブ区切り：**レポートを TSV 形式で書き出します。データをサードパーティのソフトウェアに書き出し、さらに分析を行う場合は、この形式をお勧めします。
使用しているオペレーティングシステムによっては、ファイルを開くか保存するかを選択できます。 関連するアプリケーションでファイルを開くか、ご使用のコンピューターに保存します。

1. 書き出されたファイルの使用方法を理解するには、[データを書き出し](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)の記事の情報を参照してください。

## グラフで稼働率情報を表示

稼働率レポートのデータをグラフビューで表示できます。

1. 稼働率レポートを開きます。
これを行うには、[稼動率レポートを使用した進捗、コスト、収益の追跡](#track-progress-cost-and-revenue-with-the-utilization-report)を参照してください。

1. 稼動率レポートの右上隅で&#x200B;**グラフ**&#x200B;アイコンをクリックします。

   ![グラフアイコン](assets/utilization-chart.png)

   稼動率レポートが、グラフ形式で表示されます。

1. （オプション）**表示**&#x200B;ドロップダウンメニューから適切なオプションを選択することで、プロジェクト、プログラムまたはポートフォリオを表示するようにグラフを設定します。
1. （オプション）レポートの特定の時点にポインタを合わせると、その時点のデータが表示されます。

   ![データポイントの上にポインタを合わせます。](assets/utilization-chart-hover.png)

1. （オプション）フィルターを調整して、グラフに表示する情報を変更します。フィルターの調整について詳しくは、この記事の[稼働率情報のフィルタリング](#filter-utilization-information)を参照してください。
1. （オプション）グラフレポートの時間枠を設定する方法について詳しくは、この記事の[情報を表示する日付範囲の調整](#adjust-the-date-range-for-which-information-is-displayed)を参照してください。
