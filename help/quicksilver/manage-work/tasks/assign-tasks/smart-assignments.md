---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: スマート割り当ての概要
description: タスクとタスクの割り当てを管理する場合、スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。 スマート割り当てとは、ジョブに最も適したリソースを決定するアルゴリズムに基づいて作業項目をリソースに割り当てる際にAdobe Workfrontが表示する提案です。
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---

# スマート割り当ての概要


<span class="preview">このページで強調表示されている情報は、まだ一般に利用できない機能を示しています。 この機能は、すべての顧客のプレビュー環境でのみ使用できます。</span>

<span class="preview">現在のリリーススケジュールについて詳しくは、 [2024 年第 1 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>


タスクとタスクの割り当てを管理する場合、スマート割り当てを使用して、作業を完了するのに最適なリソースを特定できます。 スマート割り当てとは、ジョブに最も適したリソースを決定するアルゴリズムに基づいて作業項目をリソースに割り当てる際にAdobe Workfrontが表示する提案です。 スマート割り当ては、ユーザー、ジョブの役割、チームのいずれかになります。

>[!NOTE]
>
>ユーザーを提案する場合、スマート割り当てでは、ユーザーの可用性は考慮されません。 ただし、スケジュールに従って使用できる場合は、タスクの計画日と予定日に影響し、タスクが割り当てられた際に問題が発生します。 スケジュールについて詳しくは、この記事を参照してください。 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

この記事には、スマート割り当てに関する一般的な情報が含まれています。 スマート割り当てを使用してタスクとタスクをユーザーに割り当てる方法については、 [スマート割り当てを行う](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## スマート割り当ての概要

スマート割り当てを使用する際は、次の点に注意してください。

* このアルゴリズムは、タスクと問題に対して独立して機能します。 つまり、Workfrontは問題とタスクに関する基準に従って個別にリストを作成するので、問題の推奨ユーザーのリストがタスクの推奨ユーザーのリストと異なる場合があります。
* スマート割り当てでは、ジョブの役割やチームを推奨しません。 代わりに、タスクやイシューを完了するのに最適なユーザーの提案になります。
* 提案された割り当ては、常にアクティブなユーザーです。
* 最初にリストされたユーザーは、タスクに最も適した一致である必要があります。

## スマート割り当て候補の検索

スマート割り当ては、次のタスクまたはタスクを割り当てることができる領域で表示できます。

* 「割り当て」列の発行リストまたはレポート

  ![](assets/smart-assignments-issue-list.png)

* <span class="preview">「割り当て」列のタスクリストまたはレポート </span>

  <span class="preview">![](assets/smart-assignments-task-list.png)</span>

* 「割り当て」フィールドのタスクまたはイシューのヘッダー

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* 「割り当て」領域のタスクまたは問題の概要パネル

  ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* タスクまたはイシューを開いたときに [ 割り当て ] 領域の [ ホーム ] 領域に一覧表示された項目の [ 割り当て ] フィールド

  ![](assets/smart-assignments-in-home-nwe-350x216.png)

* タスクまたはイシューを割り当てる際に「この割り当て先」領域のワークロードバランサー

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## スマート割り当て条件


<div class="preview">

スマート割り当てのタスクに対する作業は、タスクに対する作業と問題に対する作業とでは異なります。

### タスクのスマート割り当て条件

タスクのスマート割り当ての計算は、2 つの段階で機能します。

#### タスクのスマート割り当て計算の第 1 段階

スマート割り当てを計算する第 1 段階では、Workfrontは割り当てごとに類似性スコアを計算します。

>[!NOTE]
>
>スマート割り当ての計算の第 1 段階は、次のタスク領域には適用されません。
>
>* ワークロードバランサーでの一括割り当て。
>* ボード上の接続済みカード。


類似性スコアの計算と、割り当てのリストの順序は、次の点を考慮に入れています。

* タスク、プロジェクト、ポートフォリオの名前が割り当てようとしているタスクと同じである既存の割り当てには、100%のスコアが割り当てられます。 既存の割り当てのタスクのプロジェクト名とポートフォリオ名も、割り当てようとしているタスクのプロジェクト名とポートフォリオと一致している必要があります。

* 他の割り当てのこの情報の一部のみが既存のタスクで一致する場合、スコアは 100%未満になる可能性があります。

  例えば、「My portfolio」という名前のプロジェクトに「My project」という名前のタスクを割り当て、「My project」という名前のポートフォリオに「My task」という名前の既存のタスクがある場合、「My task」に割り当てられたユーザーは、既存のタスク名と割り当て先が 95%になります現在は似ていますが、同一ではありません。

  >[!TIP]
  >
  >  Workfrontでは、タスク、プロジェクト、ポートフォリオの「名前」フィールドのみで一致を検索し、他のフィールドでは一致を検索しません。

* 同じ名前を持つシステム内の多数のタスクに割り当てられると、割り当てのスコアが高くなる場合があります。 例えば、名前に「AI」を含むシステム内のタスクの 50%に「Development」と呼ばれるチームが割り当てられ、名前に「AI」を含む別のタスクを割り当てる場合、「Development」チームのスコアは高くなります。 この場合、プロジェクト名やポートフォリオ名はそれほど重要ではありません。

* このスコアリングシステムを考慮すると、最初の 7 つの提案がスマート割り当てとして、スコアの降順で表示されます。 スコアが 40%未満の割り当ては表示されません。

* 複数の割り当てのスコアが同じ場合、割り当てが行われた日付の順に、最新の日付から順に表示されます。

  例えば、Rick が今日以前に類似のタスクに割り当てられ、Jennifer が 2 日前に類似のタスクに割り当てられた場合、Rick が最初に表示されます。

* この計算を使用して一致がない場合、スマート割り当ての第 2 段階が開始し、別のアルゴリズムを使用して計算されます。

#### タスクのスマート割り当て計算の第 2 段階

タスクのスマート割り当ての最初のステップで一致が見つからなかった場合、Workfrontではタスクのスマート割り当てを、タスクのイシューの計算と同じ方法で計算します。

詳しくは、 [タスクとタスクのスマート割り当て条件](#smart-assignments-criteria-for-tasks-and-issues) 」を参照してください。

### タスクとタスクのスマート割り当て条件

</div>

>[!NOTE]
>
><span class="preview">次の条件は、タスクのスマート割り当ての計算の最初の段階で一致が見つからなかった場合にのみ適用されます。 詳しくは、 [タスクのスマート割り当て計算の第 1 段階](#first-phase-of-smart-assignment-calculation-for-tasks) 」を参照してください。 デフォルトでは、次の条件が問題に常に適用されます。 </span>

次の条件の組み合わせに基づいて、「スマート割り当て」ドロップダウンリストでユーザーが推奨されます（最も重要な条件から最も重要でない条件の順に表示されます）。

1. 過去 30 日間に、割り当てを行ったユーザーによって他の作業項目に割り当てられたユーザー。 この条件に一致する最初の 50 人のユーザーが表示されます。 最も頻繁に割り当てられたユーザーが最初に表示されます。

2. 作業項目がチームまたはロールに割り当てられている場合は、以下の既存の割り当てを考慮して、提案されたユーザーのリストがさらにフィルタリングされます。 この場合、候補のリストには次のユーザーのみが表示されます。

   * ホームチームが作業項目に割り当てられたユーザー。
   * 作業項目に割り当てられた役割がプライマリロールのユーザーです。

>[!TIP]
>
>* タスクまたはタスクに割り当てられたロールまたはチームがない場合、Workfrontには過去 30 日間（最大 50 人のユーザー）に割り当てられたすべてのユーザーが表示されます。
>
>* 過去 30 日間に割り当てを行っていない場合は、割り当てられたチームに属しているユーザー、または作業項目に割り当てられたロールを持つユーザーのみが、スマート割り当てリストに表示されます。

<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
