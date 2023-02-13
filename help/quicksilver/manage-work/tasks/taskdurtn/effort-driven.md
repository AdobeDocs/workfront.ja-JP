---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '''期間タイプの概要：労力主導型`'
description: Effort Driven は、Adobe Workfrontのタスクに設定できる期間タイプです。 Workfrontの期間のタイプに関する一般情報については、タスク期間の概要および期間のタイプを参照してください。
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# 期間タイプの概要：労力に基づく

Effort Driven は、Adobe Workfrontのタスクに設定できる期間タイプです。 Workfrontの期間のタイプに関する一般情報については、 [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 労力に基づく期間タイプの概要

Workfrontまたはグループ管理者は、システムまたはグループのデフォルトの「期間タイプ」を「労力に基づく」として設定できます。 この場合、すべての新しいタスクは、この期間タイプで作成されます。 システムレベルまたはグループレベルのプロジェクト環境設定の一部として、タスクや問題の環境設定を変更する方法については、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

このシナリオでは、プロジェクトマネージャーとして、タスクが実際に労力主導型タスクかどうかを検討する必要がない限り、プロジェクト計画を恣意的に短縮するリスクがあります。

労力を活用して次のことを実現：

* タスクで作業できるリソースの数に基づいて、計画期間を決定します。 期間は「予定時間」と等しくなります。 「計画期間」は、「計画時間」を担当者数で割った値と等しくなります。

   タスクに適用される労力のレベルによって、分業と期間が決まります。

* 複数のリソースが割り当てられた場合に、1 つのタスクに費やされた合計時間数を追跡します。

   リソースが追加されると、タスクの予定期間が短くなります。 （「多くの手で軽く作業する」という原則は、この期間タイプがタスクの計画期間に与える影響を示しています。）

次の節では、Workfrontが労力主導型タスクの計画期間を計算する方法と、この期間タイプのタスクにリソースを追加する効果について詳しく説明します。

## 「作業主導期間」タイプ式の概要

「期間タイプ」が「作業期間の駆動」のタスクに対する計画期間の計算式は、タスクに割り当てられた各リソースの割り当て率に応じて異なります。 作業主導型タスクの場合、Workfrontはタスクの計画時間を計算し、常にタスクの期間と同じになります。

```
Planned Hours (in hours) = Duration (in days)
```

タスクの期間は手動で調整できます。

Workfrontは、1 日の勤務時間が 8 時間であると想定しています。 Workfrontまたはグループ管理者が、セットアップの [ プロジェクトの基本設定 ] の [ 稼働日あたりの標準時間 ] 設定で 1 日あたりの時間を定義します。 システムレベルのプロジェクト環境設定の一部として、タスクと問題の環境設定を変更する方法については、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfrontは、タスクに割り当てられた各リソースのスケジュールを考慮して、タスクの各リソースの割り当て率を決定します。 スケジュールの作成と割り当てについて詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

次のシナリオを考慮します。

* [リソースはタスクに 100%割り当てられます](#resources-are-allocated-100-to-the-task)
* [リソースはタスクに対する様々な割合の時間に割り当てられます](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### リソースはタスクに 100%割り当てられます {#resources-are-allocated-100-to-the-task}

この式では、すべてのリソースがタスクに 100%割り当てられていることを前提としています。

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

この計算では、通常の稼働日の時間数が 8 であると想定しています。 数式にこの値が含まれるので、計画期間が日数で表示されます。

### リソースはタスクに対する様々な割合の時間に割り当てられます {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

割り当てられた各リソースには、一意のレベルの割り当てが可能なので、実際の数式では、次の割り当て値が考慮されます。

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

この計算では、通常の稼働日の時間数が 8 であると想定しています。 数式にこの値が含まれるので、計画期間が日数で表示されます。

## タスクにリソースを追加する効果

「工数主導期間タイプ」、「期間」、「計画時間」でタスクに担当者を追加または削除しても、変更はありません。 ただし、「予定期間」は変更されません。

次の例では、システム設定の [ プロジェクトの基本設定 ] で [Typical Hours per Work Day] が 8 に設定されています。 期間が 3 日なので、「計画時間」は 24 に設定されます（3 日 x 8 時間/稼働日= 24 計画時間）。

>[!NOTE]
>
>固定日付タスク制約を使用する場合、担当者を追加または削除しても計画期間は変わらず、代わりに期間と計画時間が調整されます。 固定日付以外のタスク制約を使用する場合、計画期間が調整されます。

次の表に、リソースをタスクに追加する際の計画期間の変化を示します。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>担当者数（100%ずつ割り当て）</strong> </p> </th> 
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
   <td> <p>24 時間</p> <p>（3 日 x 8 時間毎労働日=24 時間計画）</p> </td> 
   <td> <p>3 日</p> <p>（24 時間予定/1 担当者= 3 日）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 日</p> </td> 
   <td> <p>24 時間</p> <p>（3 日 x 8 時間毎労働日=24 時間計画）</p> </td> 
   <td> <p>1.5 日</p> <p>（24 時間計画/2 担当者= 12 時間または 1.5 日）</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 日</p> </td> 
   <td> <p>24 時間</p> <p>（3 日 x 8 時間毎労働日=24 時間計画）</p> </td> 
   <td> <p>1 日</p> <p>（24 時間/担当者 3 時間= 8 時間、1 日）</p> </td> 
  </tr> 
 </tbody> 
</table>

## タスクの期間タイプを「労力に基づく」に変更

タスクの期間の種類の変更について詳しくは、 [タスクの期間タイプの更新](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

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
