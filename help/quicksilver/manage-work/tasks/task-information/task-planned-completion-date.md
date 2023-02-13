---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの概要計画完了日
description: タスクの計画完了日とは、タスクが完了するように設定された日付です。
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 1%

---

# タスクの概要計画完了日

タスクの計画完了日とは、タスクが完了するように設定された日付です。

タスクの「計画完了日」を指定するか、特定の条件に応じてAdobe Workfrontまで残して計算できます。 

プロジェクトのタスクの計画完了日は、プロジェクトが開始日からスケジュールされる場合に、プロジェクトの計画完了日を決定します。 プロジェクトの計画完了日の詳細は、 [プロジェクトの完了予定日を設定](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>タスクの計画完了日は、次の方法で、タスクのコミット日またはタスクの予定完了日と異なります。
>
>* 「コミット日」は、タスクに割り当てられたユーザーがタスクを完了したと手動で推定する日付です。 詳しくは、次の記事を参照してください。
   * [コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [コミット日と計画完了日の間のインタラクション](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* 完了予定日とは、Workfrontが計算した日付で、タスクの遅延、タスクまたはその先行タスクのタイムライン、その他の要因を考慮して、タスクを現実的に完了できる実際の日付を決定します。 詳しくは、 [プロジェクト、タスクおよび問題に関する予定完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## タスクの計画完了日の手動設定

タスクの計画完了日を更新するには、タスクに対する編集アクセス権と管理権限が必要です。

タスクの計画完了日の設定は、タスクに割り当てたタスク制約の種類に応じて異なります。 

Workfrontの次の領域で、計画完了日を手動で設定できます。

* タスクを作成または編集するときに [ タスクの編集 ] ボックスを使用します。 詳しくは、 [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* 「タスクの詳細」領域で、 詳しくは、 [「タスクの詳細の概要」領域でタスク情報を管理します](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md).
* 「ホーム」領域で、タスクの表示時に「計画完了日」が表示される場合。 詳しくは、 [ホーム領域の作業項目を更新または編集する](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* タスクヘッダー内。 詳しくは、 [新しいオブジェクトヘッダー](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* タスク・リストまたはレポートで、「計画完了日」フィールドがビューに表示されます。

   詳しくは、 [リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

次のタスク制約のいずれかを選択すると、計画完了日を手動で指定できます。 

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
   <td> <p>指定日に終了</p> <p>これよりも遅く終了しない</p> <p>これよりも早く終了しない</p> </td> 
   <td> <p><span class="s1">「計画開始日」は、期間を同じにするために調整されます。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日付</p> </td> 
   <td> <p>「期間」は、計画開始日を同じにするために調整されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfrontがタスクの計画完了日を自動的に計算する方法

システムによって自動的に計算される場合、次のようにタスクの計画完了日に影響を与える可能性があります。

* タスクの制約

   タスク制約の詳細については、「 [タスク制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md).

* タスクの先行関係

   タスクの先行タスクの詳細については、「 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* プロジェクト完了日：プロジェクトが「完了日」からスケジュールされる日付。
* タスクのプライマリ担当者のスケジュールの時間。

   プライマリの担当者がタスクの期間中に予定されている時間を設定した場合、タスクの予定日は、 **タスク期間でのユーザーのオフ時間を考慮する** 設定が **ユーザーのタイムオフ** フィールドに入力します。 新しいプロジェクトは、この設定をプロジェクトの環境設定領域から継承しますが、設定はプロジェクトレベルで編集できます。

   例えば、「可能な限り早く」という制約を持つタスクが 6 月 1 日に開始し、6 月 3 日に完了するようにスケジュールされ、プライマリ担当者が 6 月 2 日に「タイムオフ」とマークされている場合、「予定完了日」は 6 月 4 日になります。

   詳しくは、 **ユーザーのタイムオフ** 環境設定については、記事を参照してください。 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) または [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

* タスクが承認に関連付けられている場合に承認設定に関連付けられた時間。 詳しくは、 [グローバル承認設定の指定](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

自動的に設定された場合、計画完了日は次の計算に基づいて決定されます。 

```
Planned Completion Date = Planned Start Date + Duration
```

例えば、タスクの開始日が 9 月 16 日で期間が 10 日の場合、計画完了日は 9 月 26 日になります。

>[!NOTE]
 計画時間と期間を自動的に調整するには、プロジェクトの「更新タイプ」を「自動」、「変更時」または「自動」に設定する必要があります。\
更新の種類の詳細については、「 [プロジェクトの更新タイプを選択](../../../manage-work/projects/manage-projects/select-project-update-type.md).
