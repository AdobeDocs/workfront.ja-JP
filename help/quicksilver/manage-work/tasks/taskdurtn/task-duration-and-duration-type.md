---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: タスクの期間と期間のタイプの概要
description: タスクの期間は、タスクの予定完了日と予定開始日の差です。期間は、タスクを完了するために使用できる時間枠を示します。
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1653'
ht-degree: 70%

---

# タスクの期間と期間のタイプの概要

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

タスクの期間は、タスクの予定完了日と予定開始日の差です。期間は、タスクを完了するために使用できる時間枠を示します。

タスクの期間タイプは、タスクに割り当てられたリソースの数、合計作業量およびタスクの合計期間の関係性を特定します。

## タスク期間の概要

タスクの実際の開始日と実際の完了日が、プロジェクトとプライマリ担当者のスケジュール、またはデフォルトのスケジュールの範囲外である場合、タスクの期間は 0 になります。

>[!BEGINSHADEBOX]

**例**
午前 9:00 に開始して午後 12:00 に終了するスケジュールがあり、タスクが午後 2:00 に開始して午後 4:00 に終了するようにスケジュールされている場合、タスクの期間はゼロになります。


>[!ENDSHADEBOX]

Adobe Workfrontで期間を計算する場合は、次の 2 つのシナリオがあります。

* タスクが 1 人のユーザーに割り当てられている場合：

   1. Workfrontでは、プロジェクトのスケジュールまたはタスクに割り当てられたユーザーのスケジュールが考慮されます。

      タスクが 1 人のユーザーに割り当てられたときにWorkfrontが使用するスケジュールは、Workfront管理者またはグループ管理者が決定します。 詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

   1. ユーザーまたはプロジェクトにスケジュールがない場合、Workfrontはシステムのデフォルトのスケジュールを使用します。

      手順は、Workfront が期間の計算に使用するスケジュールを理解した後の最初のシナリオと同様です。

* タスクが複数のユーザーに割り当てられている場合：

   1. Workfront は、プロジェクトのスケジュールまたはプライマリ担当者のスケジュールを考慮します。

      タスクが複数のユーザーに割り当てられる場合にWorkfrontが使用するスケジュールは、Workfront管理者またはグループ管理者が決定します。 詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

   1. プライマリ担当者またはプロジェクトにスケジュールがない場合、Workfrontはシステムのデフォルトのスケジュールを使用します。

  手順は、Workfront が期間の計算に使用するスケジュールを理解した後の最初のシナリオと同様です。

>[!NOTE]
>
>プロジェクトにおけるプライマリ担当者の休暇を考慮すると、タスクの予定日は調整される場合がありますが、タスクの期間は変わりません。プロジェクトを計画する際にプライマリ担当者の休暇を考慮する方法について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

## タスク期間の時間の単位

予定開始日から予定完了日までの通常の時間と経過時間の両方でタスク期間を指定できます。

リスト内でタスクの期間を更新する場合は、Workfront の時間の単位を示すために以下の略語を使用できます。

| 時間の単位 | 省略形 |
|---|---|
| 分 | M |
| 時間 | H |
| 日。これがデフォルトです。 | D |
| 週 | W |
| か月 | 月・木 |
| 経過時間数 (分) | EM |
| 経過時間数 | EH |
| 経過日数 | ED |
| 経過週数 | EW |
| 経過月数 | ET |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**例**

タスクの期間を 3 経過日とする場合は、タスク リストの [ 期間 ] フィールドに「3 ED」と入力します。  また、タスクの編集時に使用可能なドロップダウンメニューから、または「タスクの詳細」セクションで、期間の単位に適したオプションを選択することもできます。 タスクの編集について詳しくは、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

タスクの期間を指定する際は、次の点に注意してください。

* 経過時間は、タスクの期間の時間単位です。タスクの予定開始日から予定完了日までの時間で、休日、週末および休暇を含みます。つまり、経過時間はカレンダーの日数の経過です。
* 日は、システムで定義された営業日を表し、設定エリアで設定できます。 ほとんどの場合、1 日は 8 時間で構成されています。
* 定期的な時間（日または営業日）を考慮に入れて休日、週末、および休暇とそれらを除外からタスクの期間。
* タスクの期間を週単位で指定すると、Workfrontでは、「設定」の「プロジェクト環境設定」領域でWorkfront管理者が設定した 1 週間の標準的な作業日数と 1 日の標準的な時間数の設定に基づいて、期間（日と時間）が計算されます。
* Workfront では、期間を月単位で計算する際、1 か月にはデフォルトの 4 週間の期間を使用します。

## タスクの期間タイプの概要

タスクの期間タイプを管理すると、タスクのニーズに基づいて一貫したリソース割り当てを設定できます。

期間タイプで、次の疑問が解決できます。

* どのくらい忙しくなるのか
* 仕事の規模
* どのくらいの期間がかかるのか

![duration_type_triangle.png](assets/duration_type_triangle.png)

## 期間タイプを定義

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>期間タイプ</strong></p></th> 
   <th scope="col"> <p><strong>関数</strong> </p> </th> 
   <th scope="col"> <p><strong>リソースが与える影響</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>算出した割り当て</strong> </p> </th> 
   <td scope="col"> <p>タスクの各担当者の配分率を計算します。 </p> <p>この期間タイプを選択すると、タスクに対する個人の期間と予定時間数を入力できます。Workfront は、予定時間数をタスクの期間内の時間数で割り、次にタスクに割り当てられたリソース数で割って、各担当者への分配を計算します。</p> <p>詳しくは、<a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">期間タイプの概要：予定割り当て時間</a>を参照してください。</p> </td> 
   <td scope="col">タスクに担当者を追加または削除する際に、期間と予定時間数は変更されません。 </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>予定作業</strong> </p> </th> 
   <td scope="col"> <p>タスクを完了するために必要な予定時間数（工数）を決定します。</p> <p>通常は、タスクに割り当てられたリソースがタスクの期間全体に配分される場合に使用されます。</p> <p>この期間タイプを選択すると、タスクに対する個人の期間と予定時間数を入力できます。Workfront は、期間内の日数に、スケジュール内の作業時間数と、タスクに割り当てられた担当者数を掛けて、タスクの予定時間数を計算します。 </p> <p>タスクへの各担当者の配分率を手動で変更し、予定時間数を短縮できます。</p> <p>詳しくは、<a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">期間タイプの概要：予定作業</a>を参照してください。</p> </td> 
   <td scope="col"> <p>担当者がタスクに追加されると、予定時間数が増加します。 </p> <p>担当者がタスクから削除されると、予定時間数が減少します。</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>残存作業時間の優先</strong></p> </th> 
   <td scope="col"> <p>リソースの数に基づいて予定時間数を決定します。</p> <p>この期間タイプを選択すると、タスクに対する個人の期間と予定時間数を入力できます。Workfront は、期間内の日数にスケジュール内の作業時間数を掛けて、その数をタスクに割り当てられた担当者数で割って、タスクの予定時間数を算出します。 </p> <p>タスクへの各担当者の配分率を手動で変更することはできますが、予定時間数は変わりません。</p> <p>詳しくは、<a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">期間タイプの概要：残存作業時間の優先</a>を参照してください。</p> </td> 
   <td scope="col"> <p>担当者がタスクから削除されると、予定時間数が増加します。</p> <p>担当者がタスクに追加されると、予定時間数が減少します。 </p> <p>担当者の数やスケジュールの変更に関係なく、期間は変更されません。 </p> <p>期間は予定時間数と等しくなります。予定期間は、予定時間数を担当者数で割った値と等しくなります。</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>シンプル</strong> </p> </th> 
   <td scope="col"> <p>各担当者が配分される時間数に基づいて、予定時間数と期間（この期間タイプでは同じ）を決定します。 </p> <p>Workfront は、各担当者の予定割り当て時間数を合計して、予定時間数を計算します。 </p> <p>各担当者に配分される時間数を手動で変更し、それに応じて予定時間数と期間を変更することができます。すべての担当者に割り当てられた時間数の合計を選択した場合、その数は各担当者に均等に割り振られます。</p> <p>詳しくは、<a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">期間タイプの概要：シンプル</a>を参照してください。</p> </td> 
   <td scope="col"> <p>割り当て時間数の合計を選択すると、担当者間で時間が均等に配分されます。ただし、プロジェクトマネージャーは、各担当者の時間を手動で調整できます。 </p> <p>タスクの予定時間数と期間は、シンプル期間タイプをインラインで、またはタスクレベルで編集できます。 </p> <p>アジャイルチームがタスクに割り当てられている場合、期間タイプは自動的に「シンプル」に設定され、変更できません。アジャイルチームのタスク期間は 0 分以上である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 新しいタスクの期間タイプ

新しいタスクの期間タイプは、システムで設定された期間タイプと一致します。デフォルトの期間タイプは、予定割り当て時間です。Workfront 管理者またはグループ管理者は、使用するシステムまたはプロジェクトに関連付けられたグループのデフォルトの期間タイプを更新できます。詳しくは、[システム全体のタスクおよびイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

## 親タスクの元の期間

タスクの元の期間は、親タスクになる前にタスクが持っていた期間（分単位）です。

タスクが親タスクになると、最も早い子タスクの予定開始日から最も遅い子タスクの予定完了日までの期間が親タスクにロールアップされ、親タスクの期間になります。これにより、元のタスクの期間が置き換えられます。

子が経過日数の期間単位を使用し、その親が日数の期間単位を使用すると、Workfrontによる親タスクの期間の計算方法に不一致が生じる場合があります。

次の点に注意してください。

* 期間単位 Elapsed Days はカレンダー日を表し、常に 1 日 24 時間で構成されます。
* 期間単位（日数）は、システムで定義された稼働日を表し、構成可能です。 ほとんどの場合、それは 1 日 8 時間で構成されています。
* 親タスクの期間を計算する数式は次のとおりです。

  `Parent task duration = Planned Completion Date of the child task that is planned to end the latest - Planned Start Date of the child task that starts the earliest`

* 親タスクの期間を計算する場合、システムでは、最初に上記の式によって期間を計算してから、スケジュールを適用します。


詳しくは、[ タスクの元の期間と元の予定時間数の概要 ](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md) を参照してください。

## タスクの期間タイプの変更

タスクの期間タイプの変更について詳しくは、[タスクの期間タイプの更新](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)を参照してください。
