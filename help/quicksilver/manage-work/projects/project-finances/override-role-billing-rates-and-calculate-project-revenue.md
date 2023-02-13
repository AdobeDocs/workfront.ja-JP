---
product-area: projects
navigation-topic: financials
title: ジョブ・ロール請求率の上書きとプロジェクトの収益の計算の概要
description: 請求率を使用して、プロジェクトに費やした時間で乗算したプロジェクトの売上高を計算できます。 請求率と売上高の詳細については、「請求と売上高の概要」を参照してください。
author: Alina
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3644'
ht-degree: 0%

---

# ジョブ・ロール請求率の上書きとプロジェクトの収益の計算の概要

請求率を使用して、プロジェクトに費やした時間で乗算したプロジェクトの売上高を計算できます。 請求率と売上高について詳しくは、 [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## 役割請求率および役割時間別収益タイプの概要

Adobe Workfrontの管理者は、ユーザーとジョブの役割の両方に請求率を関連付けることができます。\
ユーザーの作成と請求率への関連付けについて詳しくは、 [ユーザーを追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). ジョブの役割の作成と請求率との関連付けについて詳しくは、この記事を参照してください。 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

ユーザーに関連付けられた請求率は上書きできません。

ジョブの役割に関連付けられた請求率は、会社レベルまたはプロジェクトレベルで上書きできます。

役割の請求率に基づいてプロジェクトの収益を計算するには、 **売上高タイプ** プロジェクト上のタスクのうち、次のいずれかである必要があります。

* 役割 (毎時)
* 役割 (毎時) (上限付き)
* 時間別ロールと固定ロール

詳しくは、 **売上高タイプ** および請求率： [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 収益の計算時の請求レート上書きの階層

ジョブロールには、次の方法で請求率を関連付けることができます。

* Workfront管理者は、ジョブロールの作成時に、ジョブロールに関連付けられたシステムレベルの請求率を定義できます。\
   ジョブの役割の作成について詳しくは、 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Workfront管理者は、会社の作成時に同じ職務ロールの会社レベルの請求率を定義できます。\
   Workfrontがこの会社に関連付けられたプロジェクトの売上高を計算する際には、役割がタスクに割り当てられたときに、このジョブの役割のシステムレベルの請求率ではなく、会社の請求率が使用されます。\
   会社レベルでの役割率の変更は、その会社に関連するすべてのプロジェクトに影響を与えます。

   >[!NOTE]
   >
   >会社の請求率を更新する必要がある場合、プロジェクトの料金は自動的には更新されません。 新しい会社レートがプロジェクトに反映される前に、プロジェクトから会社を削除し、会社のレートを更新し、その後、会社をプロジェクトに再度関連付ける必要があります。 プロジェクトに会社を添付する手順については、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

   会社に固有の役割の請求率の作成の詳細については、 [会社の作成と編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Workfront管理者は、プロジェクトの編集時にオプションを有効にして、ユーザーが手動でプロジェクトの財務を再計算する際に、会社レベルの請求率に変更を適用できます。\
   詳しくは、 [プロジェクト・レベルの請求率を会社レベルの請求率で上書き](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

* プロジェクトマネージャーは、プロジェクトレベルで、同じジョブの役割の請求率を定義できます。\
   プロジェクトで変更されたジョブの役割率は、そのプロジェクトにのみ影響します。

   プロジェクトのロールレートの上書きについては、 [プロジェクト・レベルでの役割請求率の上書き](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>ジョブロールがシステムレベル、会社レベル、およびプロジェクトレベルの請求率に関連付けられている場合、Workfrontは、ジョブロールレートを使用する際に、プロジェクトレベルのジョブロールの請求率を使用してタスクの売上高を計算します。 すべてのタスクの売上高は、プロジェクトの売上高にまでロールアップされます。

## プロジェクト・レベルでの役割請求率の上書き

プロジェクトマネージャーは、特定のプロジェクトのジョブロールに対する請求率を指定できます。 このプロジェクトレベルの請求率は、このジョブロールのシステムレベルの請求率を上書きします。 Workfrontは、ジョブロールのプロジェクトレベルの請求率を使用して、システムレベルの請求率を使用する代わりに、売上高を計算します。

プロジェクト・レベルでの役職請求率の上書き方法の詳細は、 [プロジェクト・レベルでの役割請求率の上書き](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

プロジェクトの売上高の計算に使用されるジョブの役割の詳細については、「ユーザーと役割の割り当てに基づくタスクの収益計算」の節を参照してください。 [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>実際の収益の場合、請求としてマークされた請求レコードに追加された時間に適用される請求率は、請求レコードの請求後に発生する請求率の上書きの影響を受けません。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## プロジェクトの「 Billing Rates 」セクションの概要

プロジェクトに関連付けられた役割の請求率の上書きを指定すると、すべての役割と上書きが **請求率** 」タブをクリックします。

リスト内の次の情報に注意してください。 **請求率**:

* [ジョブロールのグループ化](#job-role-grouping)
* [プロジェクト請求率の値](#project-billing-rate-value)
* [デフォルトの請求率の値](#default-billing-rate-value)
* [会社の請求率の値](#company-billing-rate-value)
* [複数の請求率値と期間](#multiple-billing-rate-values-and-timeframes)

### ジョブロールのグループ化 {#job-role-grouping}

請求率は、 **請求率** 領域をそれぞれの役割別に表示します。

### プロジェクト請求率の値 {#project-billing-rate-value}

ジョブの役割に対応するグループ化ラインで、そのジョブの役割の請求率を、 **プロジェクト請求率** 列。 ジョブの役割に複数の上書き率がある場合、現在の日付に対応する上書き率が **プロジェクト請求率** 列。

### デフォルトの請求率の値 {#default-billing-rate-value}

ジョブロールのグループ化ラインで、そのジョブロールの請求率が、 **デフォルトの請求率** 列。

>[!NOTE]
>
>ジョブロールに対するプロジェクト請求率がある場合、 **デフォルトの請求率** は、プロジェクトの売上高の計算には適用されません。 次の項目のみ **プロジェクトの請求率** が適用され、売上高が計算されます。

### 会社の請求率の値 {#company-billing-rate-value}

ジョブロールのグループ化ラインで、そのジョブロールの請求率を、 **会社の請求率** 列。 つまり、このプロジェクトに関連する会社が存在し、このジョブの役割がその会社に対して異なる請求率を持つことを意味します。 プロジェクトレートと同じ場合でも、会社の請求率が表示されます。

>[!NOTE]
>
>ジョブロールに対するプロジェクト請求率がある場合、 **会社の請求率** は、プロジェクトの売上高の計算には適用されません。 次の項目のみ **プロジェクトの請求率** が適用され、売上高が計算されます。

### 複数の請求率値と期間 {#multiple-billing-rate-values-and-timeframes}

特定のジョブロールに対して複数の上書き請求率がある場合、そのジョブロールのグループ化の下にその請求率が表示されます。 インライン編集を使用すると、上書き率と **開始** **日付** および **終了日** の請求率が上書きされます。

>[!NOTE]
>
>次の項目は指定できません： **開始日** を最初の上書き率に設定し、 **終了日** 最後の上書き率を示します。 Workfrontは、最初の上書き率が **終了日** が最初の上書きの条件となり、最後の上書き率が、 **開始日** の値が最後の上書きに設定されています。\
>プロジェクトの計画開始日より前に 1 時間が記録された場合は、最初の請求率が使用されます。\
>プロジェクトの計画完了日の後に 1 時間が記録された場合は、最後の請求率が使用されます。

## 計画収益の計算

* [1 回限りの請求レート上書きに基づいて計画収益を計算](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [複数の請求レート上書きに基づいて計画収益を計算](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [タスクの期間全体での計画時間の配分](#distribution-of-planned-hours-across-the-duration-of-a-task)

### 1 回限りの請求レート上書きに基づいて計画収益を計算 {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

1 回限りの請求レート上書きに基づいて計画収益を計算する際は、次の点を考慮してください。

* 次の場合に **売上高タイプ** のタスクが **1 時間ごとの役割** Workfrontは、タスクの計画時間にタスクに関連付けられたジョブロールの請求率を掛け算して、タスクの計画収益を計算します。

* ジョブロールの請求率がプロジェクトレベルで上書きされた場合、Workfrontは、プロジェクトの上書き率を使用して計画収益を計算します。
* タスクに複数のアサイメントがある場合、計画収益は、各アサイメントの役割の請求率と各アサイメントの計画時間配賦を乗算して計算されます。

>[!NOTE]
>
>複数の割り当てがある場合、割り当てごとの計画時間はタスクの計画時間とは異なります。

計画収益の計算に使用される役割の詳細は、この記事の「ユーザーおよび役割の割り当てに基づくタスクの収益計算について」の節を参照してください [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### 複数の請求レート上書きに基づいて計画収益を計算 {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

複数の請求レート上書きに基づいて計画収益を計算する際は、次の点を考慮してください。

* 次の場合に **売上高タイプ** のタスクが **1 時間ごとの役割** Workfrontは、タスクの計画時間にタスクに関連付けられたジョブロールの請求率を掛け算して、タスクの計画収益を計算します。

   計画収益の計算に使用される役割の詳細は、この記事の「ユーザーおよび役割の割り当てに基づくタスクの収益計算について」の節を参照してください [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* 複数の請求レートの上書きの場合、タスクの期間中に計画時間が掛けられるレートが変化します。 デフォルトでは、Workfrontは、タスクの期間全体に計画時間を均等に配分し、タスクの 1 日あたりの時間数を均等に割り当てます。 計算時 **計画収益** タスクの場合、Workfrontは「計画時間/日」にその日の請求率を掛け算します。 複数の請求率がある場合、その率は毎日異なる可能性があります。

   例えば、1 時間ごとの役割を持つタスクがあるとします **売上高タイプ**. タスクの期間は 5 日で、「計画時間」の値は 40 時間です。 1 日あたりの予定時間は 8 時間です。 タスクに Project Manager のジョブロールを割り当て、タスクの過去 3 日間のこのジョブロールの請求率を上書きします。この場合、最初の 2 日間はレート 1 の請求率、このジョブロールの残り 3 日間はレート 2 の請求率になります。

   計算する数式 **計画収益** このタスクの内容は次のとおりです。

   ```
   Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
   ```

Workfrontでの 1 日あたりの予定時間数の見つけ方について詳しくは、 [タスクの期間全体での計画時間の配分](#distribution-of-planned-hours-across-the-duration-of-a-task) 」を参照してください。

>[!NOTE]
>
>タスクに複数の担当者がいる場合、「計画時間数」は各担当者に配分され、その後タスクの期間中は各日に配分されます。 この場合、計画収益は、各担当者の 1 日の時間数と、タスクの期間中に変更される可能性のある各ジョブロールの請求率（複数の請求率の場合）を考慮して計算されます。

### タスクの期間全体での計画時間の配分 {#distribution-of-planned-hours-across-the-duration-of-a-task}

タスクの期間における計画時間の配分を理解する際は、次の点を考慮してください。

* デフォルトでは、Workfrontは、計画時間をタスクの期間全体に均等に配分し、プロジェクトスケジュールの可用性に基づいて、タスクの 1 日ごとに計画時間数を均等に割り当てます。

   タスクの期間全体での計画時間の配分の詳細については、この記事の「タスクの期間全体での計画時間の配分について」の節を参照してください。 [計画時間の概要](../../../manage-work/tasks/task-information/planned-hours.md).

   >[!NOTE]
   >
   >1 日あたりの計画時間数は、タスクの期間中の各日の計画時間数の割り当てです。 タスクに割り当てが 1 つある場合、この数は割り当てごとの予定時間数を表します。 タスクに複数の割り当てがある場合、割り当てごとの予定時間数は、タスクの [ 予定時間数/日 ] とは異なります。 複数の割り当てを持つタスクの日別予定時間数は、Workfrontに表示されません。
   >
   >
   >1 日あたりの計画時間に、その日のタスクに割り当てられたジョブロールの請求率を掛け合わせて、そのタスクの 1 日あたりの計画収益を計算します。 この方法で計算されたすべての日別計画売上高の合計は、そのタスクの計画売上高と等しくなります。

## 実際の売上高を計算

* [1 回限りの請求レート上書きに基づいて実際の収益を計算](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [複数の請求レートの上書きに基づいて実際の収益を計算](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### 1 回限りの請求レート上書きに基づいて実際の収益を計算 {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

1 回限りの請求レート上書きに基づいて実際の収益を計算する際は、次の点を考慮してください。

* 次の場合に **売上高タイプ** のタスクが **1 時間ごとの役割**, Workfront **実際の時間** 計算するタスクに関連付けられたジョブロールの請求率によるタスクの **実際の売上高** タスクの 実績時間は、タスクに直接記録される時間です。

   計算に使用されるジョブの役割の詳細 **実際の売上高**&#x200B;詳しくは、この記事の「ユーザーと役割の割り当てに基づくタスクの収益計算について」を参照してください。 [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* ジョブロールの請求率がプロジェクトレベルで上書きされた場合、Workfrontはプロジェクトの上書き率を使用して実際の収益を計算します。 プロジェクトのジョブロールの請求率を上書きする場合、 **実際の売上高** 新しい調整率を使用してプロジェクトのが自動的に再計算されます。

   プロジェクトのロールレートの上書きについては、 [プロジェクト・レベルでの役割請求率の上書き](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>元の料金で請求された元の請求率を上書きする前に、プロジェクトに既にログオンしている時間を保持する場合は、それらを **請求レコード**&#x200B;を指定する場合、 **請求レコード** as **請求済み**. それ以外の場合は、 **実際の売上高** 請求レートが上書きされる前に記録された時間から、プロジェクトの財務が再計算されると、新しいレートを使用して再計算されます。\
>請求レコードに時間を含め、 **請求済み**（記事を参照） [請求レコードの作成](../../../manage-work/projects/project-finances/create-billing-records.md).

### 複数の請求レートの上書きに基づいて実際の収益を計算 {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

複数の請求レート上書きに基づいて実際の収益を計算する際は、次の点を考慮してください。

* 次の場合に **売上高タイプ** のタスクが **1 時間ごとの役割**, Workfront **実際の時間** 計算するタスクに割り当てられたジョブロールの請求率を持つタスクの **実際の売上高** タスクの 実績時間は、タスクに直接記録される時間です。

* 複数の請求レートの上書きの場合、 **実際の時間** を掛けて計算します **実際の売上高** は、タスクの実行中に変更される場合があります。 Workfrontは、時間枠が **入力日** タスクの計算に記録された時間数 **実際の売上高。**

   例えば、タスクの **売上高タイプ** / **1 時間ごとの役割** プロジェクトマネージャーのジョブロールに割り当てられます。 6 月 19 日から 6 月 25 日までの日付に対して、このジョブロールの請求率をレート 1 で上書きします。 6 月 26 日以降は、請求率をレート 2 で上書きします。 6 月 20 日の場合は 2 時間、6 月 28 日の場合は 3 時間です。

   Workfrontが **実際の売上高** 次の式を使用してこのタスクを実行します。

   ```
   Actual Revenue = 2 * Rate 1 + 3 * Rate 2
   ```

   計算に使用されるジョブの役割の詳細 **実際の売上高**&#x200B;詳しくは、この記事の「ユーザーと役割の割り当てに基づくタスクの収益計算について」を参照してください。 [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## 複数の請求率に基づいて売上高を計算する際のタイムゾーンの影響

Workfront内の他のエンティティとの間でタイムゾーンの違いが生じた場合、ユーザーには他のユーザーとは異なる 1 日あたりの予定時間が表示されます。 次のシナリオでは、別のユーザーが表示する情報とユーザーの 1 日あたりの予定時間情報をゆがめる可能性があります。

* 2 人のユーザーが 2 つの異なるタイムゾーン用にコンピューターを設定している場合
* Workfrontの 2 つのユーザープロファイルは、2 つの異なるタイムゾーンに設定されている場合があります
* ユーザープロファイルに関連付けられているタイムゾーンが、Workfrontのシステムのタイムゾーンと異なる場合があります
* ユーザープロファイルに関連付けられているタイムゾーンは、プロジェクトのスケジュールのタイムゾーンとは異なる場合があります。

この場合、タイムゾーンで同じ設定を共有していない 2 人のユーザーの間で、1 日あたりの予定時間数が異なる場合があります。 また、プロジェクトで複数の請求レートの上書きを使用する場合は、異なる計画収益数が表示されます。

* [異なるタイムゾーンのユーザーに対する計画収益の計算](#calculate-planned-revenue-for-users-in-different-time-zones)
* [異なるタイムゾーンのユーザーの実際の売上高を計算する](#calculate-actual-revenue-for-users-in-different-time-zones)

### 異なるタイムゾーンのユーザーに対する計画収益の計算 {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>異なるタイムゾーンのユーザーが同じプロジェクトで作業している場合は、週のプロジェクトの請求率の上書きを変更しないことをお勧めします。 ユーザーのスケジュール内のタイムゾーンとWorkfrontシステムのタイムゾーンの時間差が原因で、プロジェクトの予定売上高に誤った値が表示される場合があります。 ほとんどのスケジュールでは、週末を計画時間の計算から除外できます。 ジョブロールの請求率上書きで変更が発生した場合、タスクの期間の途中と同時に発生する可能性がある場合は、週末より週末の間に変更を行う方がよいです。

異なるタイムゾーンのユーザーの計画収益を計算する際は、次の点を考慮してください。

* 次を持つタスクの場合： **売上高タイプ** / **1 時間ごとの役割** ジョブロールに割り当てられます。 **計画収益** は、 **予定時間** タスクの割り当てをジョブロールの請求率で指定します。

* この **予定時間** は、 **期間** タスクの

* この **期間** は、 **計画開始** **日付** そして **計画完了日** タスクの これは、**計画開始日** および **計画完了日** タスクのタイムゾーンは、タスクを表示するユーザーのタイムゾーンによって異なる場合があります。異なるタイムゾーンの 2 人のユーザーの場合、1 日あたりの予定時間数は異なる場合があります。

* ジョブロールの請求率が変更されていない場合、または請求率上書きが 1 つのみの場合、1 日あたりの計画時間数はプロジェクトの計画収益を変更しません。 この場合、2 人の異なるタイムゾーンの 2 人のユーザーが異なる計画時間/日を表示した場合でも、プロジェクトの全体的な計画売上高は、2 人のユーザーで同じになります。

   ただし、複数の請求率の上書きがある場合、 **計画収益** 2 つの異なるタイムゾーンの 2 人のユーザーでは、1 日あたりの計画時間数（2 人のユーザーで異なる可能性があります）と請求率の上書き（各ユーザーが独自のタイムゾーンのタスクを見ている場合は同じ日に異なる可能性があります）に依存しています。

* 正確な **計画収益** amount は、Workfrontインスタンスのタイムゾーンと同じタイムゾーンを持つユーザーが表示するものです。 Workfront管理者が、「システム顧客情報」領域でWorkfrontタイムゾーンを定義します。\
   システムのタイムゾーンの定義の詳細については、を参照してください。 [システムの基本情報を設定する](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 異なるタイムゾーンのユーザーの実際の売上高を計算する {#calculate-actual-revenue-for-users-in-different-time-zones}

異なるタイムゾーンのユーザーの実際の売上高を計算する際は、次の点を考慮してください。

* 次の場合に **売上高タイプ** のタスクが **1 時間ごとの役割**, Workfront **実際の時間** タスクに割り当てられたジョブロールの請求率を使用して、 **実際の売上高**. 実績時間は、タスクに直接記録される時間です。

* 複数の請求レートの上書きがある場合、Workfrontは、時間枠が **入力日** タスクの計算に記録された時間数 **実際の売上高**.

* タイムスタンプが **入力日** ログに記録された時間数と、複数の請求レートの上書きの日付範囲にタイムスタンプがない場合 **実際の売上高** の計算は、ユーザーに関連付けられたタイムゾーンの影響を受けません。

計算に使用されるジョブの役割の詳細 **実際の売上高**&#x200B;詳しくは、この記事の「ユーザーと役割の割り当てに基づくタスクの収益計算について」を参照してください。 [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## プロジェクトの財務を再計算

財務は、プロジェクトに対して記録された時間内に変更が発生したときに、プロジェクトで計算されます。

プロジェクトの存続中にレートが変更された場合は、プロジェクトの「財務の再計算」オプションを使用して、手動でプロジェクトのコストと収益を再計算できます。 また、一部のアクションは自動再計算をトリガーにしています。

プロジェクトの財務計算の詳細については、「 [プロジェクトの財務を再計算](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## API を使用して新しい請求率を追加

API を使用してジョブロールの新しい請求率を追加するには、 *setRatesForRole* アクション **率** オブジェクトを *PUT法*.
アクションと、 **率** オブジェクトは、API バージョン 8.0 で使用できます。既にプロジェクトのジョブロールに対して複数の請求率が定義されていて、新しい日付範囲で新しい請求率を追加する場合は、既存の料率と追加率の両方を同じ API 呼び出しに含める必要があります。 これは、オブジェクトのコレクションを更新する方法と似ています。

次の API 呼び出しは **attachableID** が **プロジェクト ID** を追加します。 **RoleID** が **ジョブの役割 ID** 新しい請求率を追加する対象となる。<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;rates&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Workfront API の使用について詳しくは、 [API の基本](https://experience.workfront.com/s/article/API-Basics-638808549).
