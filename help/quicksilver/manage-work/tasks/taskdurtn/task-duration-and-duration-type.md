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
source-git-commit: d98bb6b6bb8ff3bff6f367f1376948d5104887e5
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 94%

---

# タスクの期間と期間のタイプの概要

<!-- Audited: 12/2023 -->

タスクの期間は、タスクの予定完了日と予定開始日の差です。期間は、タスクを完了するために使用できる時間枠を示します。

タスクの期間タイプは、タスクに割り当てられたリソースの数、合計作業量およびタスクの合計期間の関係性を特定します。

## タスク期間の概要

タスクの [ 実績開始日 ] と [ 実績完了日 ] が、プロジェクトのスケジュール、主担当者、または既定のスケジュールのスケジュール外にある場合、タスクの [ 期間 ] は 0 になります。

**例：**&#x200B;午前 9 時に開始し、午後 12 時に終了するスケジュールと、午後 2 時に開始し、午後 4 時に終了するようにスケジュールされているタスクがある場合、タスクの期間は 0 になります。

Adobe Workfrontで期間を計算する際には、次の 2 つのシナリオが考えられます。

* タスクがユーザーWorkfrontに割り当てられている場合、は次のいずれかのスケジュールを使用し、この順序で期間を計算します。

   1. Workfront がユーザーのスケジュールを考慮します。
   1. ユーザーがスケジュールに関連付けられていない場合、Workfront はプロジェクトのスケジュールを考慮します。
   1. プロジェクトがスケジュールに関連付けられていない場合、Workfront はシステムのデフォルトスケジュールを考慮します。スケジュールについて詳しくは、[スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

* タスクが複数のユーザーに割り当てられている場合：

   1. Workfront は、プロジェクトのスケジュールまたはプライマリ担当者のスケジュールを考慮します。

  タスクが複数のユーザーに割り当てられている場合、Workfront が使用するスケジュールは、Workfront 管理者が決定します。詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

  手順は、Workfront が期間の計算に使用するスケジュールを理解した後の最初のシナリオと同様です。

>[!NOTE]
>
>プロジェクトにおけるプライマリ担当者の休暇を考慮すると、タスクの予定日は調整される場合がありますが、タスクの期間は変わりません。プロジェクトを計画する際にプライマリ担当者の休暇を考慮する方法について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

## タスク期間の時間の単位

タスクの期間は、通常時間と、予定開始日から予定完了日までの経過時間の両方で指定できます。

リスト内でタスクの期間を更新する場合は、Workfront の時間の単位を示すために以下の略語を使用できます。

| 時間の単位 | 省略形 |
|---|---|
| 分 | M |
| 時間 | H |
| 日。これがデフォルトです。 | D |
| 週 | W |
| か月 | T |
| 経過時間数 (分) | EM |
| 経過時間数 | EH |
| 経過日数 | ED |
| 経過週数 | EW |
| 経過月数 | ET |

{style="table-layout:auto"}

**例：**&#x200B;タスクの期間が 3 経過日数であることを示す場合は、タスクリストの「期間」フィールドに「3 ED」と入力します。また、タスクの編集時や「タスクの詳細」セクションで、使用可能なドロップダウンメニューから、期間単位を選択することもできます。タスクの編集について詳しくは、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

タスクの期間を指定する際は、次の点に注意してください。

* 経過時間は、タスクの期間の時間単位です。タスクの予定開始日から予定完了日までの時間で、休日、週末および休暇を含みます。つまり、経過時間はカレンダーの日数の経過です。
* 通常の時間は、休日、週末および休暇を考慮し、これらをタスクの期間から除外します。

* タスクの期間を週単位で指定すると、Workfront は、Workfront 管理者が「設定」のプロジェクト環境エリアで設定した「1 週間の標準的な稼働日数」と「稼働日の標準的な時間数」の設定に基づいて、期間を日単位と時間単位で計算します。
* Workfront では、期間を月単位で計算する際、1 か月にはデフォルトの 4 週間の期間を使用します。

## タスクの期間タイプの概要

タスクの期間タイプを管理すると、タスクのニーズに基づいて一貫したリソースの割り当てを設定できます。

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

## タスクの期間タイプの変更

タスクの期間タイプの変更について詳しくは、[タスクの期間タイプの更新](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)を参照してください。
