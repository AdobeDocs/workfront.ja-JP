---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: コストの追跡
description: Adobe Workfront でプロジェクト、タスク、イシューのコストを追跡できます。
author: Lisa
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: d431ae178a157522e2b5d8d963da7b0623510d28
workflow-type: tm+mt
source-wordcount: '2480'
ht-degree: 76%

---

# コストの追跡

<!-- Audited: 02/2024 -->

Adobe Workfront でプロジェクト、タスク、イシューのコストを追跡できます。

## Workfront によるコストの計算方法

コストを追跡するには、ユーザーとジョブの役割を時間別コスト率に関連付ける必要があります。

コストレート（毎時）は、担当業務またはユーザーに関連付けられた作業単位ごとのコストの金額です。そのレートに対して作業に費やした時間を掛けると、プロジェクト、タスク、イシューのコストになります。

次のシナリオが存在します。

* タスクのコストタイプが「ユーザー（毎時）」の場合、ユーザーの 1 時間ごとのコストでタスクとプロジェクトのコストが計算されます。

  ユーザーとコストレートの関連付けについては、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

* タスクのコストタイプが「役割（毎時）」の場合、担当業務の 1 時間ごとのコストでタスクとプロジェクトのコストが計算されます。

  担当業務とレートの関連付けについては、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。

* Workfrontでは、問題の実際のコストのみが計算され、問題のコストタイプはありません。 詳しくは、 [Workfrontが問題のコストを追跡する方法](#how-workfront-tracks-costs-for-issues) 」を参照してください。

>[!TIP]
>
>プロジェクトのコストレートは上書きできません。ユーザーまたは担当業務の 1 時間あたりのコストを設定すると、システム内のすべてのコストはそのレートで計算されます。

## Workfront のコスト効率指数

Workfront では、プロジェクトのコスト効率を追跡できるように、プロジェクトのさまざまなコスト効率指標が計算されます。\
コスト効率指標の計算について詳しくは、次を参照してください。

* [コスト効果指数（CPI）の計算](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [コスト効率指数（CPI）の計算](../../../manage-work/projects/project-finances/calculate-csi.md)
* [スケジュール効率指数（SPI）の計算](../../../manage-work/projects/project-finances/calculate-spi.md)

## Workfront がタスクおよびプロジェクトのコストを追跡する方法

コストのタイプは、タスクとプロジェクトで異なります。

### Workfront によるコストの追跡方法 {#how-workfront-tracks-costs}

Workfrontでは、タスクやプロジェクトに関する複数のタイプのコストを追跡できます。 総コストは次の式で計算されます。

`Costs = Labor Costs + Expense Costs`

* **労力コスト** は、タスクとプロジェクトに関する時間と、タスクに関連付けられたリソースの 1 時間当たりのコストに関連付けられています。一般に、Workfront は次の労力コストを計算します。

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>予定労力コスト</td> 
     <td> <p>計算には次の式を使用します。</p><code>Planned Labor Costs = Planned Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>予算計上労力コスト</td> 
     <td> <p>計算には次の式を使用します。</p><code>Budgeted Labor Costs = Budgeted Hours * Cost per Hour rate</code> </td> 
    </tr> 
    <tr> 
     <td>実際の労力コスト</td> 
     <td> <p>計算には次の式を使用します。</p><code>Actual Labor Costs = Actual Hours * Cost per Hour rate</code> </td> 
    </tr> 
   </tbody> 
  </table>

  詳しくは、この記事の [Workfront による計画コスト、予算計上コスト、実際のコストの計算方法](#how-workfront-calculates-planned-budgeted-and-actual-costs)の節を参照してください。

* **費用コスト** は、プロジェクトおよびタスクの費用に関連付けられています。\
  プロジェクトを作成する際に、プロジェクト全体に対して予定費用を設定できます。また、費用を新規または既存のタスクに関連付けることもできます。詳しくは、[プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md)を参照してください。

* **固定コスト**&#x200B;は、プロジェクトの一定金額のコストとして定義されます。これは、プロジェクトの計画コストの一部で、プロジェクトの完了に必要な金額を表します。

  >[!TIP]
  >
  >テンプレートをプロジェクトに添付する際に、テンプレートの固定コストがプロジェクトの固定コストに追加されます。詳しくは、[プロジェクトへのテンプレートの添付の概要](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md)を参照してください。

### Workfront による予定コスト、予算計上コスト、実際のコストの計算方法 {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfront では、プロジェクト内の個々のタスクごとに予定コストと実際のコストが計算されます。Workfront では、これらの計算を個々のタスクで使用して、プロジェクトの予定コストと実際のコストが計算されます。

#### 予定コスト {#planned-cost}

プロジェクトの予定コストは、プロジェクトの予定作業（予定時間数）に関連付けられたコストです。

プロジェクトの予定コストは、次の式で計算されます。

`Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project`

例えば、タスクの「費用」タブには、$100 のマーケティング費用と$50 の管理費用の費用があります。 「財務」タブで、ユーザー（毎時）コストタイプを選択します。ユーザーがタスクに割り当てられ、ユーザーの時間率は 15 ドルです。ユーザーに割り当てられたこのタスクの作業時間は 5 時間です。プロジェクトの「費用」タブには、コンサルティングという費用に対して 100 ドルの予定コストがあります。このプロジェクトには、200 ドルの固定費もあります。

プロジェクトの予定コストは、次のように計算されます。

`$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525`

数式の時間別レートでは、レートの有効日付変更が考慮されます。

#### 予算計上コスト {#budgeted-cost}

プロジェクトの予算計上コストは、プロジェクトの予算計上作業（予算計上時間数）に関連付けられたコストです。

次の 2 つの条件が満たされる場合、プロジェクトの予定コストはプロジェクトの予算計上コストと同じになります。

* プロジェクト上のタスクの予定時間は、（リソースプランナの）予算時間に一致します。
* タスクの請求タイプは、役割（毎時）です。

次の条件が満たされる場合、プロジェクトの予算計上コストは次の式を使用して計算されます。

* プロジェクト上のタスクの予定時間が（リソースプランナの）予算時間と一致しません。
* タスクの請求タイプは、役割（毎時）です。

上記の条件が満たされる場合、Workfront では次の式を使用してプロジェクトの予算計上コストを計算します。

`Budgeted Project Cost = Budgeted Labor Cost + Budgeted Expense Cost of all tasks + Budgeted Expense Cost of the project`

#### 実際のコスト {#actual-cost}

プロジェクトの実際のコストは、プロジェクトの実際の作業（ログに記録された時間数）に関連付けられたコストです。

実際のコストは、次の式を使用して計算されます。

`Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project`

例えば、タスクの「費用」タブには、実際のコストが$110 のマーケティング費用と、実際のコストが$40 の管理費用があります。 役割（毎時）コストタイプを選択し、コンサルタントの担当業務をタスクに割り当てます。コンサルタントの担当業務の時給は 15 ドルで、コンサルタントの担当業務のタスクに 6 時間のログが記録されています。プロジェクトに関連付けられたコンサルティング費用（「費用」タブ）があり、実際のコストが 100 ドルで、ユーザープロファイルで 1 時間あたりのコスト率が 20 ドルになっているユーザーが、プロジェクトで 10 時間をログに記録します。このプロジェクトには、200 ドルの固定費もあります。

プロジェクトの実際のコストは、次のように計算されます。

`$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740`

数式の時間別レートでは、レートの有効日付変更が考慮されます。

>[!NOTE]
>
>プロジェクトの実際の費用コストは、次のように計算されます。
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>これらのコストは、実際のコストの計算では重複しません。例えば、固定コストがプロジェクトの実際の費用コストの一部である場合、実際のコストに別途追加されることはありません。

>[!NOTE]
>
>プロジェクトの時間を記録する場合、プロジェクトの実際の労力コストを計算する際に次のシナリオが存在します。
>
>* デフォルトでは、Workfront はユーザーの 1 時間あたりのコスト率を使用して実際の労力コストを計算します。
>* 時間のログを記録するユーザーがコストに関連付けられていない場合、Workfront はユーザーのプライマリロールの 1 時間あたりのコスト率を使用します。
>* Workfront管理者が **ジョブの役割を時間エントリに手動で割り当てる** [ セットアップ ] の [ タイムシートと時間の基本設定 ] 領域で設定を行い、プロジェクトのユーザーログ時間に関連付ける別の役割を選択すると、プロジェクトの実際のコストは、時間が記録されたときに指定した役割に基づいて計算されます。 特定の担当業務の時間の記録の有効化について詳しくは、[タイムシートと時間の環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)の記事を参照してください。

### Workfront によるタスクのコストタイプの計算方法 {#how-workfront-calculates-cost-types-for-tasks}

タスクの予定コストと実際のコスト、およびそれらのと労力コストは、各タスクのコストタイプで決定されます。

プロジェクト内の個々のタスクに対してコストタイプを設定できます。各コストタイプは、予定コストと実際のコストの値に影響を与えます。

タスクのコストタイプを変更する方法について詳しくは、[タスクのコストタイプを更新](../../../manage-work/tasks/task-information/update-task-cost-type.md)を参照してください。

次の表に、Workfrontで使用可能なタスクのコストタイプを示します。

<table style="table-layout:auto">
 <col> 
 <col> 
<tbody> 
  <tr> 
   <td> <p><strong>タスクのコストタイプ</strong> </p> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr>
  <tr> 
   <td> <p>ユーザー (毎時)</p> </td> 
   <td> <p>これは、タスクを作成する際のデフォルトのコストタイプです。</p> <p><strong>予定コスト</strong>は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>予定労力コストは次のように計算されます。<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>メモ： <p>ユーザー（毎時）コストタイプを使用して予定コストを計算する場合は、次の影響を考慮します。</p> 
     <ul> 
      <li>1 つのタスクに複数のリソースを割り当てると、Workfront では、各リソースに割り当てられたタスクの割合に基づいて予定コストの計算を調整します。</li>
      <li>日付が有効なコスト率の場合、予定労力コストは、タスクでカバーされる各期間の予定コストの合計です。</li>
      <li>「予定コスト」フィールドの値は、予定コストをタスク自体から表示するか、稼働率レポートから表示するかによって異なる場合があります。<br><strong>予定コストをタスク自体から表示する場合：</strong>「予定コスト」フィールドでは、担当業務レベルで設定された「コスト／時間」フィールドが考慮されます（「コスト／時間」フィールドがユーザーレベルで設定されていない場合）。<br><strong>予定コストを稼働率レポートから表示する場合：</strong>「予定コスト」フィールドでは、担当業務レベルで設定された「コスト／時間」フィールドは考慮されません。代わりに、「役職ロール」レベルで設定された「原価/人事」フィールドを「稼働率」レポートで考慮する場合は、タスクの「原価タイプ」を「時間別」に設定する必要があります。 </li> 
     </ul> </p> <p><strong>実際のコスト</strong>は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>実際の労力コストは次のように計算されます。</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>例えば、ユーザーのプロファイルの時間あたりのコストが $20 であるとします。タスクに対して 5 時間を記録した場合、そのタスクに対する実績のコストは $100 になります。ユーザーに時間当たりのコスト率が関連付けられていない場合、実際のコストは、プライマリ担当業務の時間当たりのコスト率に基づいて計算されます。担当業務がない場合や、担当業務の時間あたりのコスト率が定義されていない場合、タスクの実績コストは 0 になります。 </p> <p>注意：実績コストは、タスクの割り当て先に関係なく、時間を記録するユーザーの 1 時間あたりのコスト率に基づいて計算されます。 また、フォーミュラ内の請求時間率では、レートの有効な変更が考慮されます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>役割（毎時）</p> </td>
   <td> <p><strong>予定コスト</strong>は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>予定労力コストは次の方法で計算されます。</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>メモ：1 つのタスクに複数のリソースを割り当てると、Workfront では、各リソースに割り当てられたタスクの割合に基づいて、予定時間数が調整されます。また、数式の時間別レートでは、レートの有効な変更が考慮されます。</p> <p><strong>実際のコスト</strong>は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>タスクの実際の労力コストは次のように計算されます。</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>例えば、あるタスクが、1 つの担当業務に割り当てられている、または時間あたりのコストレートが $20 の担当業務を持つユーザーに割り当てられています。ユーザーがタスクに対して 5 時間と記録した場合、そのタスクに対する実際のコストは $100 になります。タスクに割り当てられたユーザーが、タスクに関連する担当業務を持っていない場合、実際のコストは、プライマリ担当業務の時間あたりのコストレートに基づいて計算されます。担当業務がない場合や、担当業務の時間あたりのコスト率が定義されていない場合、タスクの実績コストは 0 になります。 </p> <p>注意：ロールの実際の時間時間は、時間を記録するユーザーに関連付けられたロールではなく、タスクに関連付けられたユーザーのジョブロールに基づいて計算されます。 また、フォーミュラ内の請求時間率では、レートの有効な変更が考慮されます。</p> <p>Workfront管理者が <strong>ジョブの役割を時間エントリに手動で割り当てる</strong> [ セットアップ ] の [ タイムシートと時間の基本設定 ] 領域で設定を行い、タスクのユーザーログ時間によって、この時間に関連付ける別の役割が選択され、時間が記録されたときに指定した役割に基づいて、[ ロールの 1 時間あたりの実績コスト ] タスクが計算されます。 特定の担当業務に対する時間記録の有効化について詳しくは、<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">タイムシートと時間の環境設定を指定</a>の記事を参照してください。</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定 (毎時)</p> </td> 
   <td> <p><strong>予定コスト</strong>は次の数式で計算されます。</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>タスクの労力コストは次のように計算されます。</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>実際のコスト</strong>は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>実際の労力コストは次のように計算されます。</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>このコストタイプでは、個々のユーザーや担当業務は考慮されません。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>コストなし</p> </td> 
   <td> <p>このコストタイプはコストには影響しません。 親タスクにこの原価タイプがある場合、別の原価タイプのサブタスクは個々の原価タイプに従って計算され、それに応じて親タスクの原価が影響を受けます。 </p> <p>財務データへのアクセス権がないユーザーまたはテンプレートに対する財務権限を持たないユーザーが、そのテンプレートからプロジェクトを作成する場合、これはプロジェクトのタスクのデフォルトのコストタイプです。</p> <p>財務データへのアクセスの詳細については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセス権を付与</a>の記事を参照してください。</p> <p>プロジェクトに対する財務権限について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">オブジェクトに対する財務権限の共有</a>の記事を参照してください。</p> <p>テンプレートからプロジェクトを作成する方法について詳しくは、<a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">テンプレートを使用したプロジェクトの作成</a>の記事を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront でイシューのコストをトラッキングする方法 {#how-workfront-tracks-costs-for-issues}

イシューは、プロジェクトの次のタイプのコストには影響しません。

* 予定コスト
* 予算計上コスト

ただし、問題には **実際のコスト**（プロジェクトの実際のコストにも影響します）。

次の表では、イシューに対する割り当てのタイプに応じて、イシューに対する実際のコストの計算方法を説明します。

<table style="table-layout:auto"> 
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td> <p>ユーザーの割り当て</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>実際のコスト</strong>は次の数式で計算されます。</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>イシューに割り当てられているユーザーに関係なく、時間を記録するユーザーの時間あたりのコスト率がここで考慮されます。 </p> <p>時間を記録するユーザーのプロファイルに「時間当たりのコスト」レートがない場合、プライマリジョブロールの「時間当りのコスト」レートで問題の実際のコストが計算されます。</p> <p>時間を記録しているプライマリに、プロファイルに役割がない場合や、関連付けられている率がない場合、実際の時間数は、イシューに関する担当者のプライマリ担当業務の時間当たりのコスト率を使用して計算されます。その役割にレートが定義されていない場合、イシューの実際のコストはゼロになります。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>役割の割り当て</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>実際のコスト</strong>は次の数式で計算されます。</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>イシューに割り当てられている役割に関係なく、イシューの時間を記録するユーザーの時間あたりのコスト率がここで考慮されます。 </p> <p>時間のログに時間当たりのコスト率が関連付けられていない場合、イシューの実際のコストは、プライマリの役割の時間当たりのコスト率で計算されます。</p><p>時間を記録するユーザーのプロファイルに役割がない場合や、プロファイルに関連付けられている率がない場合、問題の実際のコストはゼロになります。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>割り当てなし</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>実際のコスト</strong>は次の数式で計算されます。</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>時間を記録するユーザーが自分のプロファイルに関連付けられた「1 時間当たりコスト」のレートを持たない場合、イシューの実際のコストはそのプライマリ担当業務の「1 時間当たりコスト」レートによって計算されます。 </p> <p>時間を記録するユーザーに、そのプロファイルに関連付けられた担当業務がない場合、またはプライマリ担当業務に「1 時間当たりのコスト」レートが定義されていない場合、イシューの実際のコストはゼロになります。 </p> </td> 
  </tr> 
 </tbody> 
</table>
