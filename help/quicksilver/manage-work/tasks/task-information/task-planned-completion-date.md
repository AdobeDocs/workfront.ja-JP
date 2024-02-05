---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの予定完了日の概要
description: タスクの予定完了日とは、タスクが完了するように設定された日付です。
author: Alina
feature: Work Management
exl-id: b0522db5-9c68-4b1a-82c8-5a9e613eb2ff
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '775'
ht-degree: 100%

---

# タスクの予定完了日の概要

タスクの予定完了日とは、タスクが完了するように設定された日付です。

タスクの予定完了日を指定することも、Workfront に任せて、特定の基準に基づいて計算することもできます。 

プロジェクトを開始日からスケジューリングした場合、プロジェクトのタスクの予定完了日は、プロジェクトの予定完了日を決定します。プロジェクトの予定完了日について詳しくは、[プロジェクトの予定完了日の設定](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)を参照してください。

>[!NOTE]
>
>タスクの予定完了日は、次の点で、タスクのコミット日またはタスクの見込み完了日と異なります。
>
>* コミット日は、タスクに割り当てられたユーザーがタスクの完了を手動で見積もった日付です。詳しくは、次の記事を参照してください。
>
>* [コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>* [コミット日と予定完了日の間のインタラクション](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md)。
>
>* 見込み完了日とは、Workfront によって計算された日付で、タスクの遅延、タスクまたはその先行タスクのタイムライン、その他の要因を考慮して、タスクを現実的に完了できる実際の日付です。詳しくは、[プロジェクト、タスクおよびイシューの見込み完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。
>

## タスクの予定完了日を手動で設定

タスクの予定完了日を更新するには、タスクの編集権限と管理権限が必要です。

タスクの予定完了日の設定は、タスクに割り当てたタスク制約の種類に応じて異なります。 

予定完了日は、Workfront の次の領域で手動で設定できます。

* タスクを作成または編集するときに「タスクの編集」ボックスを使用。詳しくは、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。
* タスクの詳細領域。詳細については、[タスクの詳細の概要領域でタスク情報を管理](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)を参照してください。
* ホーム領域（タスクの表示時に予定完了日が表示される場合）。詳しくは、[ホーム領域の作業項目の更新または編集](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)を参照してください。
* タスクヘッダー内。詳しくは、[新しいオブジェクトヘッダー](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)を参照してください。
* タスクリストまたはレポートで、「予定完了日」フィールドがビューに表示される場合。

  詳しくは、[リスト内のタスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)を参照してください。

次のタスク制約のいずれかを選択すると、予定完了日を手動で指定できます。

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
   <td> <p>指定日に終了</p> <p>これよりも遅く終了しない</p> <p>これよりも早く終了しない</p> </td> 
   <td> <p><span class="s1">予定開始日は、期間を同じ長さにするために調整されます。</span> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>固定日付</p> </td> 
   <td> <p>期間は、予定開始日を同じにするために調整されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront でタスクの予定完了日が自動的に計算される仕組み

システムによって自動的に計算される場合、次が要素がタスクの予定完了日に影響を与える可能性があります。

* タスクの制約

  タスク制約について詳しくは、[タスク制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)を参照してください。

* タスクの先行関係

  タスクの先行タスクの詳細については、[タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

* プロジェクト完了日（プロジェクトが「完了日」からスケジュールされる場合）。
* タスクのプライマリ担当者の休暇スケジュール。

  「**ユーザーの休暇**」フィールドで「**タスク期間のユーザーの休暇を考慮する**」設定が選択されている場合、タスクの期間中にプライマリ担当者の休暇が予定されていると、タスクの予定日はそれに応じて調整されます。この設定は、新しいプロジェクトではプロジェクトの環境設定領域から継承されますが、設定はプロジェクトレベルで編集できます。

  例えば、「可能な限り早く」という制約を持つタスクが 6 月 1 日に開始し、6 月 3 日に完了するようにスケジュールされ、プライマリ担当者が 6 月 2 日に「休暇」とマークされている場合、「予定完了日」は 6 月 4 日になります。

  **ユーザー休暇**&#x200B;環境設定の詳細については、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)または[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

* タスクが承認に関連付けられている場合、承認設定に関連付けられた時間。詳しくは、[グローバル承認設定の指定](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)を参照してください。

自動的に設定された場合、予定完了日は次の計算に基づいて決定されます。

```
Planned Completion Date = Planned Start Date + Duration
```

例えば、タスクの開始日が 9月16日で期間が 10 日間の場合、予定完了日は 9月26日になります。

>[!NOTE]
>
>予定時間数と期間を自動的に調整するには、プロジェクトの「更新タイプ」を「自動・変更時」または「自動」に設定する必要があります。\
>更新タイプについて詳しくは、[プロジェクトの更新タイプの選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)の記事を参照してください。
