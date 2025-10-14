---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの予定開始日の概要
description: タスクの予定開始日とは、タスク作成者が、その日にタスクの作業を開始する必要があると決定する日付です。タスクの予定日は、プロジェクトの日付とタイムラインに影響します。プロジェクトの予定開始日について詳しくは、プロジェクトの予定開始日の概要を参照してください。
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: 0ff02569d3c7fb532a2faafc46fe4235ce77acd4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 63%

---

# タスクの予定開始日の概要

<!-- Audited: 6/2025 -->

タスクの予定開始日とは、タスク作成者が、その日にタスクの作業を開始する必要があると決定する日付です。タスクの予定日は、プロジェクトの日付とタイムラインに影響します。プロジェクトの予定開始日について詳しくは、[プロジェクトの予定開始日の概要](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)を参照してください。

## タスクの予定開始日

タスクの「予定開始日」を指定するか、特定の条件に応じてタスクを計算する場合は、Adobe Workfrontに任せることができます。 

* [タスクの予定開始日の手動設定](#manually-set-the-planned-start-date-of-a-task)
* [タスクの予定開始日の計算方法](#how-the-planned-start-date-is-calculated-for-a-task)

### タスクの予定開始日の手動設定 {#manually-set-the-planned-start-date-of-a-task}

タスクの予定開始日を設定するかどうかは、タスクに割り当てたタスク制約の種類に応じて異なります。 

タスクの作成時に予定開始日を手動で設定できます。 詳しくは、[&#x200B; プロジェクトでのタスクの作成 &#x200B;](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) を参照してください。

次のタスクの制約のいずれかを選択すると、予定開始日を手動で指定できます。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>タスクの制約タイプ</strong> </p> </th> 
   <th> <p><strong>予定完了日の手動変更の影響</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>指定日に開始</p> <p>指定日以降に開始</p> <p>指定日までに開始</p> </td> 
   <td> <p><span class="s1">予定完了日は、期間を同じにするために調整されます。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日付</p> </td> 
   <td> <p>期間は、予定完了日を同じにするために調整されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### タスクの予定開始日の計算方法 {#how-the-planned-start-date-is-calculated-for-a-task}

システムによって自動的に計算される場合、次の項目がタスクの予定開始日に影響する可能性があります。

* 設定のタスクとイシューのエリアにある開始日の環境設定

  Workfront 管理者やグループ管理者は、新規タスクをプロジェクトの予定開始日と同じ日に開始するか、タスクを作成した日に開始するかを決定できます。

  タスクとイシューの環境設定について詳しくは、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

* タスクの制約

  タスク制約の詳細については、「[&#x200B; タスク制約の概要 &#x200B;](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)」を参照してください。

* タスクの先行関係

  先行タスクについて詳しくは、[タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

* プロジェクトが開始日からスケジュールされている場合、プロジェクト開始日。
* タスクのプライマリ担当者の休暇スケジュール。

  プライマリ担当者がタスク期間中に休暇をスケジュールした場合、「ユーザーの休暇」フィールドで「タスク期間のユーザーの休暇を考慮」設定を選択すると、タスクの予定日が調整されます。 この設定は、新しいプロジェクトではプロジェクトの環境設定領域から継承されますが、設定はプロジェクトレベルで編集できます。

  例えば、「できるだけ早く」の制約を持つタスクが 6 月 1 日に開始して 6 月 3 日に完了するようにスケジュールされていて、プライマリ担当者が 6 月 1 日を休暇としてマークしている場合、タスクの予定開始日は 6 月 2 日になります。

  ユーザーの休暇の環境設定については、[&#x200B; システム全体のプロジェクト環境設定を設定 &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) または [&#x200B; プロジェクトを編集 &#x200B;](../../../manage-work/projects/manage-projects/edit-projects.md) を参照してください。

自動的に設定された場合、予定開始日は次の計算に基づいて決定されます。

```
Planned Start Date = Planned Completion Date - Task Duration
```

例えば、タスクの完了日が 9月16日で期間が 10 日の場合、予定開始日は 9月6日になります。

>[!NOTE]
>
> また、予定時間数と期間を自動的に調整するには、プロジェクトの更新タイプを [ 自動 ] と [ 変更時 ] または [ 自動 ] に設定する必要があります。\
>更新の種類の詳細については、[&#x200B; プロジェクトの更新の種類を選択する &#x200B;](../../../manage-work/projects/manage-projects/select-project-update-type.md) を参照してください。
