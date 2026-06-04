---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスク予定開始日の概要
description: タスクの予定開始日とは、タスク作成者が、その日にタスクの作業を開始する必要があると決定する日付です。 タスクの予定日は、プロジェクトの日付とタイムラインに影響します。 プロジェクトの予定開始日について詳しくは、プロジェクトの予定開始日の概要を参照してください。
author: Alina
feature: Work Management
exl-id: 2ac6327f-4a13-4fb8-ad8e-03d032221483
TQID: https://experienceleague.adobe.com/5VM6UTgVLYBRMGtwWXQ6LbXqwQiYI1EuIPl7GbQSAwk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 619
ht-degree: 45%

---

# タスクの予定開始日の概要

<!-- Audited: 6/2025 -->

タスクの予定開始日とは、タスク作成者が、その日にタスクの作業を開始する必要があると決定する日付です。 タスクの予定日は、プロジェクトの日付とタイムラインに影響します。 プロジェクトの予定開始日について詳しくは、[プロジェクトの予定開始日の概要](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)を参照してください。

## タスクの予定開始日

タスクの予定開始日を指定するか、特定の条件に応じてAdobe Workfrontに任せて計算できます。

* [タスクの予定開始日の手動設定](#manually-set-the-planned-start-date-of-a-task)
* [タスクの予定開始日の計算方法](#how-the-planned-start-date-is-calculated-for-a-task)

### タスクの予定開始日の手動設定 {#manually-set-the-planned-start-date-of-a-task}

タスクの予定開始日の設定は、タスクに割り当てるタスク制約のタイプによって異なります。

タスクの作成時に、予定開始日を手動で設定できます。 詳しくは、[ プロジェクトでのタスクの作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)を参照してください。

次のいずれかのタスク制約を選択すると、予定開始日を手動で指定できます。

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

* 設定の「タスクと問題」領域の「開始日」環境設定

  Workfrontまたはグループ管理者は、新しいタスクがプロジェクトの予定開始日と同じ日に開始するか、タスクを作成する日に開始するかを判断できます。

  タスクとイシューの環境設定について詳しくは、[ システム全体のタスクとイシューの環境設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

* タスクの制約

  タスクの制約について詳しくは、[ タスクの制約の概要](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)を参照してください。

* タスクの先行関係

  先行タスクについて詳しくは、[タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

* プロジェクトが開始日からスケジュールされている場合、プロジェクト開始日。
* タスクのプライマリ担当者の休暇スケジュール。

  プライマリ担当者がタスク期間中に休暇をスケジュールしている場合、「ユーザーの休暇を考慮」設定が「ユーザーの休暇」フィールドに選択されている場合、タスクの予定日はそれに応じて調整されます。 新しいプロジェクトでは、プロジェクト環境設定エリアからこの設定を継承しますが、この設定はプロジェクトレベルで編集できます。

  例えば、「できるだけ早く」という制約を持つタスクが6月1日から6月3日に開始され、プライマリ担当者が6月1日に休暇をマークしている場合、タスク予定開始日は6月2日になります。

  ユーザーの休暇の設定について詳しくは、[ システム全体のプロジェクトの環境設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)または[ プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

自動的に設定すると、予定開始日は次の計算に基づいて決定されます。

```
Planned Start Date = Planned Completion Date - Task Duration
```

例えば、タスクの完了日が 9月16日で期間が 10 日の場合、予定開始日は 9月6日になります。

>[!NOTE]
>
> また、プロジェクトの更新タイプを「自動」および「変更時」または「自動」に設定して、予定時間と期間を自動的に調整する必要があります。\
>更新タイプについて詳しくは、[ プロジェクト更新タイプの選択](../../../manage-work/projects/manage-projects/select-project-update-type.md)を参照してください。
