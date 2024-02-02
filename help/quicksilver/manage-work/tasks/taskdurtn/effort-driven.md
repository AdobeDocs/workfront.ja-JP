---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 「期間タイプの概要：残存作業時間の優先」
description: 残存作業時間の優先は、Adobe Workfront のタスクに設定できる期間タイプです。Workfront の期間タイプに関する一般情報については、タスク期間の概要と期間タイプを参照してください。
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '821'
ht-degree: 100%

---

# 期間タイプの概要：作業優先

残存作業時間の優先は、Adobe Workfront のタスクに設定できる期間タイプです。Workfront の期間タイプに関する一般情報については、[タスク期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

## 残存作業時間の優先の期間タイプの概要

Workfront またはグループ管理者は、システムまたはグループのデフォルトの期間タイプを残存作業時間の優先に設定できます。この場合、すべての新しいタスクは、この期間タイプで作成されます。システムレベルまたはグループレベルのプロジェクト環境設定の一部として、タスクやイシューの環境設定を変更する方法については、[システム全体のタスクとイシュー環境を設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

このシナリオでは、プロジェクトマネージャーとして、タスクが実際に残存作業時間の優先のタスクかどうかを検討する時間を取らない限り、プロジェクトプランが恣意的に短縮されるリスクがあります。

残存作業時間の優先は以下の目的で使用します：

* タスクに取り掛かる際に利用できるリソースの数に基づいて、予定期間を決定します。期間は予定時間数と等しくなります。予定期間は、予定時間数を担当者数で割った値と等しくなります。

  タスクに振り向けられる労力のレベルによって、分業と期間が決まります。

* 複数のリソースが割り当てられた場合に、1 つのタスクに費やされた合計時間数を追跡します。

  リソースが追加されると、タスクの予定期間が短くなります。（「人手が多ければ仕事は軽くなる」の原則が、この期間タイプがタスクの計画期間に与える影響を表しています。）

以降の節では、Workfront が残存作業時間の優先のタスクの予定期間を計算する方法と、この期間タイプのタスクに対するリソース追加の効果について詳しく説明します。

## 残存作業時間の優先の期間タイプの数式の概要

期間タイプが残存作業時間の優先のタスクに対する予定期間の計算式は、タスクに割り当てられた各リソースの割り当て率に応じて異なります。残存作業時間の優先のタスクの場合、Workfront はタスクの予定時間数を計算し、その時間数は常にタスクの期間と同じになります。

```
Planned Hours (in hours) = Duration (in days)
```

タスクの期間は手動で調整できます。

Workfront は、1 日の勤務時間は 8 時間と想定しています。Workfront またはグループ管理者は、設定のプロジェクト環境設定で、作業日あたりの標準時間数の設定によって 1 日あたりの時間を定義します。システムレベルのプロジェクト環境設定の一部として、タスクやイシューの環境設定を変更する方法について詳しくは、[システム全体のタスクとイシューの環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

>[!TIP]
>
>Workfront は、タスクに割り当てられた各リソースのスケジュールを考慮して、タスクに対する各リソースの割り当て率を決定します。スケジュールの作成とユーザーへの割り当てについて詳しくは、[スケジュールを作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

次のシナリオを考慮してください。

* [リソースがタスクに 100％割り当てられている](#resources-are-allocated-100-to-the-task)
* [リソースがタスクに対し時間について様々な割合で割り当てられている](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### リソースがタスクに 100％割り当てられている {#resources-are-allocated-100-to-the-task}

この式は、すべてのリソースがタスクに 100％割り当てられることを前提としています。

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

この計算は、通常の作業日の時間数を 8 としています。数式にはこの値が含まれているので、予定期間は日数で表示されます。

### リソースがタスクに対し時間について様々な割合で割り当てられている {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

割り当てられた各リソースには、一意のレベルの割り当てが可能なので、実際の数式では、次の割り当て値が考慮されます。

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

この計算は、通常の作業日の時間数を 8 としています。数式にはこの値が含まれているので、予定期間は日数で表示されます。

## タスクにさらにリソースを追加したときの効果

残存作業時間の優先の期間タイプであるタスクに担当者を追加または削除しても、期間と予定時間数は、変更されません。ただし、予定期間は変更されます。

次の例では、システム設定のプロジェクト環境設定で、作業日あたりの標準時間数が 8 に設定されています。期間が 3 日なので、予定時間数は 24（3 日 x 8 時間/作業日 = 24 時間予定）に設定されます。

>[!NOTE]
>
>固定日付のタスク制約を使用すると、担当者を追加または削除しても予定期間は変わらず、代わりに期間と予定時間数が調整されます。固定日付以外のタスク制約を使用すると、予定期間が調整されます。

次の表に、リソースをタスクに追加する際の予定期間の変化を示します。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>担当者数（100％ずつ割り当て）</strong> </p> </th> 
   <th> <p><strong>期間</strong> </p> </th> 
   <th> <p><strong>予定時間数</strong> </p> </th> 
   <th><strong>予定期間</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 日</p> </td> 
   <td> <p>24 時間</p> <p>（3 日 x 8 時間/作業日 = 24 時間予定）</p> </td> 
   <td> <p>3 日</p> <p>（24 時間予定 / 担当者 1 人 = 3 日）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 日</p> </td> 
   <td> <p>24 時間</p> <p>（3 日 x 8 時間/作業日 = 24 時間予定）</p> </td> 
   <td> <p>1.5 日</p> <p>（24 時間予定 / 担当者 2 人 = 12 時間または 1.5 日）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 日</p> </td> 
   <td> <p>24 時間</p> <p>（3 日 x 8 時間/作業日 = 24 時間予定）</p> </td> 
   <td> <p>1 日</p> <p>（24 時間予定 / 担当者 3 人 = 8 時間または 1 日）</p> </td> 
  </tr> 
 </tbody> 
</table>

## タスクの期間タイプを残存作業時間の優先に変更

タスクの期間タイプの変更について詳しくは、[タスクの期間タイプを更新](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
