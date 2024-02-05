---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの予定開始日の概要
description: タスクの予定開始日とは、タスク作成者が、その日にタスクの作業を開始する必要があると決定する日付です。タスクの予定日は、プロジェクトの日付とタイムラインに影響します。プロジェクトの予定開始日について詳しくは、プロジェクトの予定開始日の概要を参照してください。
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '626'
ht-degree: 100%

---

# タスクの予定開始日の概要

タスクの予定開始日とは、タスク作成者が、その日にタスクの作業を開始する必要があると決定する日付です。タスクの予定日は、プロジェクトの日付とタイムラインに影響します。プロジェクトの予定開始日について詳しくは、[プロジェクトの予定開始日の概要](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)を参照してください。

## タスクの予定開始日

タスクの予定開始日を指定することも、特定の基準に基づいて Adobe Workfront に任せて計算することもできます。 

* [タスクの予定開始日の手動設定](#manually-set-the-planned-start-date-of-a-task)
* [タスクの予定開始日の計算方法](#how-the-planned-start-date-is-calculated-for-a-task)

### タスクの予定開始日の手動設定 {#manually-set-the-planned-start-date-of-a-task}

タスクの予定開始日の設定は、タスクに割り当てたタスクの制約のタイプによって異なります。 

[プロジェクトでのタスクの作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)の記事で説明されるように、タスクを作成する際に予定開始日を手動で設定できます。

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

  タスクの制約について詳しくは、[タスクの制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)の記事を参照してください

* タスクの先行関係

  タスクの先行タスクについて詳しくは、[タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)の記事を参照してください。

* プロジェクトが開始日からスケジュールされている場合、プロジェクト開始日。
* タスクのプライマリ担当者の休暇スケジュール。

  プライマリ担当者がタスクの期間中に休暇を取る場合、「**ユーザーの休暇**」フィールドで&#x200B;**タスク期間にユーザーの休暇を考慮**&#x200B;の設定が選択されていると、タスクの予定日がそれに応じて調整されます。この設定は、新しいプロジェクトではプロジェクトの環境設定領域から継承されますが、設定はプロジェクトレベルで編集できます。

  例えば、「できるだけ早く」という制約を持つタスクが 6月1日に開始し、6月3日に完了するようにスケジュールされ、プライマリ担当者が 6月1日に「休暇」とマークされている場合、タスクの予定開始日は 6月2日になります。

  **ユーザーの休暇**&#x200B;の環境設定について詳しくは、[システム全体のプロジェクトの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)または[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)の記事を参照してください。

自動的に設定された場合、予定開始日は次の計算に基づいて決定されます。

```
Planned Start Date = Planned Completion Date - Task Duration
```

例えば、タスクの完了日が 9月16日で期間が 10 日の場合、予定開始日は 9月6日になります。

>[!NOTE]
>
>予定時間数と期間を自動的に調整するには、プロジェクトの更新タイプを「自動・変更時」または「自動」に設定する必要があります。\
>更新タイプについて詳しくは、[プロジェクトの更新タイプの選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。
