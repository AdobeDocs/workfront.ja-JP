---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの計画開始日の概要
description: タスクの計画開始日とは、タスクの作成者がタスクの作業を開始するように決定した日付です。 計画タスクの日付は、プロジェクトの日付とタイムラインに影響を与えます。 プロジェクトの計画開始日の詳細は、「プロジェクトの概要計画開始日」を参照してください。
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 2%

---

# タスクの計画開始日の概要

タスクの計画開始日とは、タスクの作成者がタスクの作業を開始するように決定した日付です。 計画タスクの日付は、プロジェクトの日付とタイムラインに影響を与えます。 プロジェクトの計画開始日については、 [プロジェクトの概要計画開始日](../../../manage-work/projects/planning-a-project/project-planned-start-date.md).

## タスクの計画開始日

タスクの「予定開始日」を指定することも、特定の条件に応じてAdobe Workfrontまで計算することもできます。 

* [タスクの計画開始日を手動で設定する](#manually-set-the-planned-start-date-of-a-task)
* [タスクの計画開始日の計算方法](#how-the-planned-start-date-is-calculated-for-a-task)

### タスクの計画開始日を手動で設定する {#manually-set-the-planned-start-date-of-a-task}

タスクの計画開始日の設定は、タスクに割り当てたタスク制約の種類によって異なります。 

タスクの作成時に、手動で計画開始日を設定できます。詳しくは、この記事を参照してください [プロジェクトでのタスクの作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

次のタスク制約のいずれかを選択すると、計画開始日を手動で指定できます。 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>タスク制約タイプ</strong> </p> </th> 
   <th> <p><strong>計画完了日の手動変更の影響</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>指定日に開始</p> <p>指定日以後に開始</p> <p>指定日までに開始</p> </td> 
   <td> <p><span class="s1">「計画完了日」は、期間を同じにするために調整されます。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日付</p> </td> 
   <td> <p>「期間」は、計画完了日を同じ日付に保つために調整されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### タスクの計画開始日の計算方法 {#how-the-planned-start-date-is-calculated-for-a-task}

システムによって自動的に計算される場合、次のようにタスクの計画開始日に影響を与える可能性があります。

* セットアップの「タスクと問題」領域の「開始日」環境設定

   Workfrontまたはグループの管理者は、新しいタスクの開始日を、プロジェクトの予定開始日と同じ日付にするか、タスクを作成した日にするかを決定できます。

   タスクと問題の環境設定について詳しくは、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* タスクの制約

   タスク制約の詳細については、「 [タスク制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)

* タスクの先行関係

   タスクの先行タスクの詳細については、「 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* プロジェクト開始日：プロジェクトが開始日からスケジュールされる日付です。
* タスクのプライマリ担当者のスケジュールの時間。

   プライマリの担当者がタスクの期間中に予定されている時間を設定した場合、タスクの予定日は、 **タスク期間でのユーザーのオフ時間を考慮する** 設定が **ユーザーのタイムオフ** フィールドに入力します。 新しいプロジェクトは、この設定をプロジェクトの環境設定領域から継承しますが、設定はプロジェクトレベルで編集できます。

   例えば、「可能な限り早く」という制約を持つプライマリが 6 月 1 日に開始し、6 月 3 日に完了するようにスケジュールされていて、担当者が 6 月 1 日にタイムオフのマークを付けている場合、「計画開始日」は 6 月 2 日になります。

   詳しくは、 **ユーザーのタイムオフ** 環境設定については、記事を参照してください。  [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) または [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

自動的に設定された場合、計画開始日は次の計算に基づいて決定されます。 

```
Planned Start Date = Planned Completion Date - Task Duration
```

例えば、タスクの「完了日」が 9 月 16 日で、期間が 10 日の場合、「計画開始日」は 9 月 6 日です。

>[!NOTE]
>
> また、計画時間と期間が自動的に調整されるように、プロジェクトの「更新タイプ」も「自動および変更時」または「自動」に設定する必要があります。\
更新の種類の詳細については、「 [プロジェクトの更新タイプを選択](../../../manage-work/projects/manage-projects/select-project-update-type.md).
