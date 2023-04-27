---
content-type: reference;how-to-procedural
product-area: projects
navigation-topic: financials
title: コストの追跡
description: Adobe Workfrontでプロジェクト、タスクおよび問題のコストを追跡できます。
author: Alina
feature: Work Management
exl-id: df3090ae-9721-4e9b-84b4-315890619801
source-git-commit: 7e78ca8c8ea7f037b55b06e7452ac5c562b99eca
workflow-type: tm+mt
source-wordcount: '2418'
ht-degree: 1%

---

# コストの追跡

Adobe Workfrontでプロジェクト、タスクおよび問題のコストを追跡できます。

## Workfrontがコストを計算する方法

コストを追跡するには、ユーザーとジョブの役割を時間別コスト率に関連付ける必要があります。

時間別原価率は、ジョブの役割またはユーザーに関連付けられた作業単位ごとの原価の金額です。 レートに作業に費やした時間を掛けると、プロジェクト、タスク、または問題に関するコストが生じます。

次のシナリオが存在します。

* タスクのコストタイプが「1 時間ごとのユーザー」の場合、ユーザーの 1 時間ごとのコストはタスクとプロジェクトのコストを計算します。

   ユーザーとコストレートの関連付けについて詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* タスクのコストタイプが「1 時間ごと」の場合、ジョブロールの 1 時間ごとの割合でタスクとプロジェクトのコストが計算されます。

   ジョブの役割とコストレートの関連付けについて詳しくは、 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfrontでは、問題と問題に対する実際のコストのみが計算され、コストタイプがありません。 詳しくは、 [Workfrontが問題のコストを追跡する方法](#how-workfront-tracks-costs-for-issues) 」を参照してください。

>[!TIP]
>
>プロジェクトのコストレートは上書きできません。 ユーザーまたはジョブロールの時間単価を設定すると、その単価はシステム内のすべての原価を計算します。

## Workfrontのコストパフォーマンスインデックス

Workfrontは、プロジェクトのコスト効果のインデックスを多数計算し、コスト効率を高めるためにプロジェクトを追跡できるようにします。\
コスト・パフォーマンス・インデックスの計算の詳細は、次を参照してください。

* [コスト効果指数 (CPI) の計算](../../../manage-work/projects/project-finances/calculate-cpi.md)
* [CSI(Calculate Cost Schedule Performance Index)](../../../manage-work/projects/project-finances/calculate-csi.md)
* [スケジュールパフォーマンスインデックスの計算 (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md)

## Workfrontがタスクおよびプロジェクトのコストを追跡する方法

* [Workfrontによるコストの追跡方法](#how-workfront-tracks-costs)
* [Workfrontが計画原価、予算原価および実績原価を計算する方法](#how-workfront-calculates-planned-budgeted-and-actual-costs)
* [Workfrontがタスクのコストタイプを計算する方法](#how-workfront-calculates-cost-types-for-tasks)

### Workfrontによるコストの追跡方法  {#how-workfront-tracks-costs}

Workfrontでは、タスクやプロジェクトに関する複数のタイプのコストを追跡できます。 総コストは次の式で計算されます。

```
Costs = Labor Costs + Expense Costs
```

* **人件費** は、タスクとプロジェクトに関する時間と、タスクに関連付けられたリソースの時間単価に関連付けられています。 一般に、Workfrontは次の人件費を計算します。

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>計画労務費</td> 
     <td> <p>計算には次の式を使用します。</p><pre>計画労務費=計画時間*時間単価</pre> </td> 
    </tr> 
    <tr> 
     <td>予算労務費</td> 
     <td> <p>計算には次の式を使用します。</p><pre>予算労務費=予算時間*時間単価</pre> </td> 
    </tr> 
    <tr> 
     <td>実際の人件費</td> 
     <td> <p>計算には次の式を使用します。</p><pre>実際の労務費=実績時間*時間単価</pre> </td> 
    </tr> 
   </tbody> 
  </table>

   詳しくは、 [Workfrontが計画原価、予算原価および実績原価を計算する方法](#how-workfront-calculates-planned-budgeted-and-actual-costs) 」の節を参照してください。

* **費用コスト** は、プロジェクトとタスクの費用に関連付けられています。\
   プロジェクトを作成する際に、プロジェクト全体に対して計画費を設定できます。 また、費用を新規または既存のタスクに関連付けることもできます。 詳しくは、 [プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **固定コスト** は、プロジェクトの一定金額のコストとして定義されます。 これは、プロジェクトの計画コストの一部で、プロジェクトの完了に必要な金額を表します。

   >[!TIP]
   >
   >テンプレートをプロジェクトにアタッチする場合、テンプレートの固定コストがプロジェクトの固定コストに追加されます。 詳しくは、 [プロジェクトへのテンプレートのアタッチの概要](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md).

### Workfrontが計画原価、予算原価および実績原価を計算する方法 {#how-workfront-calculates-planned-budgeted-and-actual-costs}

Workfrontは、プロジェクト内の個々のタスクごとに、計画コストと実績コストを計算します。 Workfrontでは、これらの計算を個々のタスクで使用して、プロジェクトの計画原価と実績原価を計算します。

* [予定コスト](#planned-cost)
* [予算計上コスト](#budgeted-cost)
* [実際のコスト](#actual-cost)

#### 予定コスト {#planned-cost}

プロジェクトの計画原価は、プロジェクト上の計画作業（計画時間）に関連付けられた原価です。

プロジェクトの計画コストは、次の式で計算されます。

```
Planned Project Cost = Planned Labor Cost of all tasks + Planned Expense cost of all tasks + Planned Expense Cost of the project + Fixed Cost of the project
```

例えば、タスクの「費用」タブに次の費用があるとします。100 ドルのマーケティング費用と 50 ドルの管理費用。 「財務」タブで、「ユーザー — 時間別」コストタイプを選択します。 ユーザーがタスクに割り当てられ、ユーザーの時間単価は$15 です。 このタスクの作業時間が 5 時間に割り当てられています。 プロジェクトの「費用」タブに、コンサルティングという費用に対して 100 ドルの計画コストがあります。 また、プロジェクトに 200 ドルの固定コストがあります。

プロジェクトの計画コストは次のように計算されます。

```
$100 (Consulting Expense) + $100 (Marketing Expense) + $50 (Administrative Expense) + $15(Hourly Rate)*5(Planned Hours Logged) + $200 (Fixed Cost) = $525
```

#### 予算計上コスト {#budgeted-cost}

プロジェクトの予算原価は、プロジェクトの予算作業（予算時間）に関連付けられた原価です。

次の 2 つの条件を満たす場合、プロジェクトの予算原価はプロジェクトの計画原価と同じになります。

* プロジェクト上のタスクの予定時間は、（リソースプランナの）予算時間に一致します
* タスクの「請求タイプ」は「1 時間ごとの役割」です。

次の条件を満たす場合、プロジェクトの予算コストは次の式を使用して計算されます。

* プロジェクト上のタスクの予定時間が（リソースプランナの）予算時間と一致しません
* タスクの請求タイプは「1 時間ごとの役割」です。

上記の条件を満たした場合、Workfrontは次の式を使用してプロジェクトの予算コストを計算します。
<pre>予算プロジェクト原価=予算労務費+全タスクの予算費+プロジェクトの予算費用</pre>

#### 実際のコスト {#actual-cost}

プロジェクトの実際のコストは、プロジェクト上の実際の作業に関連するコスト（ログに記録された時間数）です。

実際のコストは、次の式を使用して計算されます。

```
Actual Project Cost = Actual Labor Cost of all tasks + Actual Expense Cost of all tasks + Actual Labor Cost of the project + Actual Expense Cost of the project + Fixed Cost of the project
```

例えば、タスクの「費用」タブに次の費用があるとします。実際のコストが$110 のマーケティング費用と、実際のコストが$40 の管理費用。 「時間別の役割」コストタイプを選択し、コンサルタントジョブの役割をタスクに割り当てます。 コンサルタントジョブの役割の割合は 1 時間あたり$15 で、コンサルタントジョブの役割のタスクに 6 時間ログが記録されます。 プロジェクトに関連するコンサルティング費用（「費用」タブ）があり、実際のコストが$100 で、ユーザープロファイルログに 10 時間のユーザープロファイルに時間あたりのコスト率が$20 のユーザーがあります。 また、プロジェクトに 200 ドルの固定コストがあります。

プロジェクトの実際のコストは次のように計算されます。

```
$100 (Consulting Expense) + $110 (Marketing Expense) + $40 (Administrative Expense) +$15 (Hourly Rate)*6 (Actual Hours Logged) + $20 (Cost per Hour rate for the user logging time on the project)*10 (hours the user logs on the project) + $200 (Fixed Cost) = $740
```

>[!NOTE]
>
>プロジェクトの実費コストは次のように計算されます。
>`SUM (All Project Actual Expense Costs) + SUM (All Tasks Actual Expense Costs) + Project Fixed Cost`
>
>これらのコストは、実際のコストの計算では重複しません。 たとえば、固定コストがプロジェクトの実費コストに含まれている場合、実費には別途追加されません。

>[!NOTE]
>
>プロジェクトで時間を記録する場合、プロジェクトの実績労務費を計算する際には、次のシナリオが存在します。
>
>* デフォルトでは、Workfrontはユーザーの時間あたりのコスト率を使用して、実際の労務費を計算します。
>* 時間のログを記録するユーザーがコストに関連付けられていない場合、Workfrontはユーザーのプライマリロールの時間あたりのコスト率を使用します。
>* Workfront管理者が **ジョブの役割を時間エントリに手動で割り当て** [ タイムシートと時間の基本設定 ] 領域の設定を行い、プロジェクトのユーザーログ時間に関連付ける別の役割が選択されると、プロジェクトの実績コストは、時間が記録されたときに指定した役割に基づいて計算されます。 特定のジョブの役割のログ時間の有効化について詳しくは、この記事を参照してください。 [タイムシートと時間の基本設定を構成する](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).


### Workfrontがタスクのコストタイプを計算する方法 {#how-workfront-calculates-cost-types-for-tasks}

タスクの「計画原価」と「実績原価」と「労務原価」は、各タスクの「原価タイプ」で決定されます。

プロジェクト内の個々のタスクに対してコストタイプを設定できます。 各コストタイプは、「計画原価」と「実績原価」の値に影響を与えます。

タスクのコストタイプを変更する方法については、 [タスクのコストタイプを更新](../../../manage-work/tasks/task-information/update-task-cost-type.md).

次の表に、Workfrontで使用可能なタスクのコストタイプを示します。

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>タスクのコストタイプ</strong> </p> </th> 
   <th> <p><strong>説明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>ユーザー (毎時)</p> </td> 
   <td> <p>タスクを作成する際のデフォルトのコストタイプです。</p> <p><strong>計画コスト</strong> は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>計画労務費が次の方法で計算される場合：<br><code>Planned Labor Cost = Planned Hours * Cost per Hour Rate of the User assigned to the task</code></p> <p>メモ:   <p>「ユーザーの時間別コスト・タイプ」を使用して計画コストを計算する場合の次の影響を考慮します。</p> 
     <ul> 
      <li>1 つのタスクに複数のリソースを割り当てると、Workfrontでは、各リソースに割り当てられたタスクの割合に基づいて、計画コストの計算が調整されます。</li> 
      <li>「計画原価」フィールドの値は、タスク自体から計画原価を表示するか、稼働率レポートから計画原価を表示するかによって異なります。<br><strong>タスク自体から計画原価を表示する場合：</strong> 「計画原価」フィールドでは、「役職ロール」レベルで設定された「原価/人事」フィールドが考慮されます（「原価/人事」フィールドがユーザー・レベルで設定されていない場合）。<br><strong>プロジェクトの「稼働率」レポートから計画原価を表示する場合：</strong> 「計画原価」フィールドでは、「製造オーダー・ロール」レベルで設定された「原価/人事」フィールドは考慮されません。 代わりに、「役職ロール」レベルで設定された「原価/人事」フィールドを「稼働率」レポートで考慮する場合は、タスクの「原価タイプ」を「時間別」に設定する必要があります。 </li> 
     </ul> </p> <p><strong>実費</strong> は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>実際の労務費が次の基準で計算される場合：</p> <p><code>Actual Labor Cost = Actual Hours * Cost per Hour Rate of the User logging the hours</code> </p> <p>例えば、ユーザーのプロファイルの時間あたりのコスト率が$20 であるとします。 タスクに対して 5 時間を記録した場合、そのタスクに対する実績労務費は$100 になります。 ユーザーに「時間当たりの原価」レートが関連付けられていない場合、「実績原価」は、プライマリ・ジョブ・ロールの「時間当たりの原価」レートに基づいて計算されます。 ジョブロールがない場合や、ジョブロールの 1 時間あたりのコストレートが定義されていない場合、タスクの実績コストは 0 になります。 </p> <p>注意：実際のコストは、タスクに割り当てられているユーザーに関係なく、時間を記録するユーザーの 1 時間あたりのコスト率に基づいて計算されます。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>役割 (毎時)</p> </td> 
   <td> <p><strong>計画コスト</strong> は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost+ Task Planned Expense Cost</code> </p> <p>タスク計画労務費が次の方法で計算される場所</p> <p><code>Task Planned Labor Cost = Planned Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>注意：1 つのタスクに複数のリソースを割り当てると、Workfrontでは、各リソースに割り当てられたタスクの割合に基づいて、計算時間が調整されます。</p> <p><strong>実費</strong> は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Actual Cost = Task Actual Labor Cost + Task Actual Expense Cost</code> </p> <p>タスクの実績労務費が次の基準で計算される場合：</p> <p><code>Task Actual Labor Cost = Actual Hours * Cost per Hour Rate of the Job Role assigned to the task</code> </p> <p>例えば、1 つのタスクが 1 つのジョブの役割に割り当てられているか、1 時間あたりのコスト率が$20 のジョブの役割を持つユーザーに割り当てられているとします。 ユーザーがタスクに対して 5 時間ログを記録した場合、そのタスクの実績労務費は$100 になります。 タスクに割り当てられたプライマリに、タスクに関連するジョブロールがない場合、Actual Cost は、タスクジョブロールの 1 時間あたりのコスト率に基づいて計算されます。 ジョブロールがない場合や、ジョブロールの 1 時間あたりのコストレートが定義されていない場合、タスクの実績コストは 0 になります。 </p> <p>メモ:   <p> ロールの実際の時間時間時間タスクは、時間を記録するユーザーに関連付けられたロールではなく、タスクに関連付けられたユーザーのジョブロールに基づいて計算されます。</p> <p>Workfront管理者が <strong>ジョブの役割を時間エントリに手動で割り当て</strong> [ タイムシートと時間の基本設定 ] 領域の設定を行い、タスクのユーザーログ時間がこの時間に関連付ける別の役割を選択すると、時間が記録されたときに指定した役割に基づいて、[ 時間別の役割の実績コスト ] タスクが計算されます。 特定のジョブの役割のログ時間の有効化について詳しくは、この記事を参照してください。 <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">タイムシートと時間の基本設定を構成する</a>.</p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定 (毎時)</p> </td> 
   <td> <p><strong>計画コスト</strong> は次の数式で計算されます。</p> <p><code style="font-style: normal;">Task Planned Cost = Task Planned Labor Cost + Task Planned Expense Cost</code> </p> <p>タスク労務費の計算方法：</p> <p><code>Task Planned Labor Cost = Planned Hours * Fixed Hourly Cost of the Task</code> </p> <p><strong>実費</strong> は次の数式で計算されます。 </p> <p><code style="font-style: normal;">Task Actual Cost = Actual Task Labor Cost + Task Planned Expense Cost</code> </p> <p>タスクの実績労務費が次の基準で計算される場合：</p> <p><code>Task Actual Labor Cost = Actual Hours * Fixed Hourly Cost of the Task</code> </p> <p>このコストタイプでは、個々のユーザーやジョブの役割は考慮されません。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>コストなし</p> </td> 
   <td> <p>この原価タイプは原価には影響しません。 親タスクにこのコスト・タイプがある場合、別のコスト・タイプのサブタスクは個々のコスト・タイプに従って計算され、それに応じて親タスクのコストが影響を受けます。 </p> <p>財務データへのアクセス権がないユーザーまたはテンプレートに対する財務権限を持たないユーザーが、そのテンプレートからプロジェクトを作成する場合、これはプロジェクトのタスクのデフォルトのコストタイプです。</p> <p>財務データへのアクセスの詳細については、「 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセス権の付与</a>.</p> <p>オブジェクトに対する財務権限の詳細については、「 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">オブジェクトに対する財務権限の共有</a>.</p> <p>テンプレートからプロジェクトを作成する方法については、この記事を参照してください。 <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">テンプレートを使用したプロジェクトの作成</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because this was moved to its own how-to article linked above. Could be removed after some time.) </p>
<p>To configure the Cost Type of an individual task:</p>
<ol>
<li value="1">Go to the task where you want to configure the Cost Type. </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then expand the <strong>Finance</strong> area. </p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Double click <strong>Cost Type</strong> and select the cost type that you want to apply to the task. </p> </li>
<li value="4">Click <strong>Save.</strong></li>
</ol>
</div>
-->

## Workfrontが問題のコストを追跡する方法 {#how-workfront-tracks-costs-for-issues}

問題は、プロジェクトの次のタイプのコストに影響を与えません。

* 予定コスト
* 予算計上コスト

ただし、問題には **実費** これは、プロジェクトの実際のコストにも影響します。

次の表では、問題に対する割り当てのタイプに応じて、問題に対する実際のコストがどのように計算されるかを説明します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th colspan="4">実際のコストの発行</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>ユーザー割り当て</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>実費</strong> は次の数式で計算されます。</p> <p><code style="font-style: normal;">Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>問題に割り当てられているユーザーに関係なく、時間を記録するユーザーの 1 時間あたりのコスト率がここで考慮されます。 </p> <p>時間を記録するユーザーのプロファイルに「時間当たりのコスト」レートがない場合、プライマリジョブロールの「時間当りのコスト」レートで問題の実際のコストが計算されます。 時間を記録しているプライマリに、プロファイルに役割がない場合や、関連付けられている率がない場合、実際の時間数は、問題に関するユーザー担当者のプライマリ・ジョブ・ロールの時間当たりのコスト率を使用して計算されます。 その役割にレートが定義されていない場合、問題の実際のコストはゼロになります。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>役割の割り当て</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>実費</strong> は次の数式で計算されます。</p><code>Issue Actual Cost = Actual Hours * Cost per Hour Rate of user logging the hours</code> <p>問題に割り当てられている役割に関係なく、問題の時間を記録するユーザーの 1 時間あたりのコスト率がここで考慮されます。 </p> <p>時間のログに「時間当たりのコスト」レートが関連付けられていない場合、プライマリロールの「時間当たりのコスト」レートで問題の実際のコストが計算されます。<br>時間を記録するユーザーのプロファイルに役割がない場合や、プロファイルに関連付けられている率がない場合、問題の実際のコストはゼロになります。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p>割り当てなし</p> <p> </p> </td> 
   <td colspan="3"> <p><strong>実費</strong> は次の数式で計算されます。</p> <p><code>Issue Actual Cost = Actual Hours * Cost per Hour rate of the user logging the hours</code> </p> <p>時間を記録するプライマリに、プロファイルに「時間当たりのコスト」レートが関連付けられていない場合、ユーザージョブロールの「時間当たりのコスト」レートで問題の実際のコストが計算されます。 </p> <p>時間を記録するユーザーに、そのプロファイルに関連付けられたジョブロールがない場合、またはプライマリジョブロールに時間当たりのコスト率が定義されていない場合、問題の実際のコストはゼロになります。 </p> </td> 
  </tr> 
  <!--<tr data-mc-conditions=""> 
   <td colspan="4"> 
    <div> <MadCap:conditionalText data-mc-conditions="">
       If your Workfront administrator enabled the 
      <strong>Assign Job Roles to hour entries manually</strong> setting in the Timesheets &amp; Hours Preferences area, and the user logging time on the issue selects a different role to associate with this time, the Actual Cost of the issue calculates based on the role specified when the hours were logged. For information about enabling logging time for a specific job role, see the article 
      <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configure timesheet and hour preferences</a>. 
     </MadCap:conditionalText> 
    </div> </td> 
  </tr> 
  -->
 </tbody> 
</table>
