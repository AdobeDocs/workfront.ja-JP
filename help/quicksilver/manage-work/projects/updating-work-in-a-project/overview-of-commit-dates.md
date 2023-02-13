---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: コミット日の概要
description: 「コミット日」は、タスクに割り当てられたユーザーまたはイシューがタスクまたはイシューを完了するためにコミットする日付です。 これは、作業を担当するユーザーのみが提供する完了日をより現実的に見積もるため、「計画完了日」とは異なります。 計画完了日の詳細は、タスクの概要計画完了日を参照してください。
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# コミット日の概要

「コミット日」は、タスクに割り当てられたユーザーまたはイシューがタスクまたはイシューを完了するためにコミットする日付です。 これは、作業を担当するユーザーのみが提供する完了日をより現実的に見積もるため、「計画完了日」とは異なります。 計画完了日については、 [タスクの概要計画完了日](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

## コミット日の概要

コミット日を使用する際は、次の点に注意してください。

* コミット日を持つのはタスクと問題のみです。
* コミット日は、Adobe Workfrontでは自動的に設定されません。\
   タスクまたはイシューを作成する場合、タスクまたはイシューにコミット日は割り当てられません。
* タスクまたはイシューに割り当てられている場合は、次のいずれかの操作を行ってコミット日を設定できます。

   * Workfrontは、タスクまたはタスクの [ 作業 ]、[ タスクの開始 ]、または [ タスクの開始 ] をクリックして、タスクまたはタスクの既存の計画完了日に一致するようにコミット日を設定します。 「Work On It」ボタンを「Start」ボタンに置き換える方法については、  [「作業対象」ボタンを「開始」ボタンに置き換えます](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * タスクまたは問題が完了したと思われるタイミングに応じて、自分でコミット日を手動で設定します。 これは、タスクまたは問題を特定の日までに完了させる、担当者としてのプロジェクトマネージャーに対する推定とコミットメントです。

>[!NOTE]
>
>コミット日を変更するには、タスクのタスク所有者である必要があります。 次のユーザーは、タスクのコミット日を変更できません：
>
>* プロジェクト所有者
>* プロジェクト スポンサー
>* リソース管理者
>* システム管理者
>* タスクのその他の担当者
>* タスクに対する権限を持つその他のユーザー。
>
>タスク所有者の詳細については、 [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) 記事内 [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## コミット日の変更によってトリガーされる通知と更新 {#notifications-and-updates-triggered-by-changing-the-commit-date}

タスクまたは担当者がプロジェクト所有者が設定した計画完了日とは異なるコミット日を選択すると、プロジェクト所有者およびこの変更に関する他のユーザーに通知と更新がいくつか表示されます。

>[!NOTE]
>
>コミット日を変更しても、計画日は自動的に変更されず、計画日に加えた変更でも、コミット日は自動的に変更されません。 

タスクまたはイシューのコミット日を設定すると、次の変更がトリガーされます。

* 「コミット日」は、タスクまたはイシューの「ストリームを更新」に入力されます。

   ![](assets/update-stream-confirmation-that-commit-date-changed-nwe-350x73.png)

   Workfront管理者がセットアップの「フィードを更新」領域でこの更新を有効にした場合、コミット日の変更がタスクまたは問題の更新領域に表示されます。 詳しくは、 [システムで追跡された更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

* タスクまたはタスクの「予想完了日」が同じ日付に設定されます。これは、タスクが完了する可能性が高い時期をより正確に示すようになったためです。

   完了予定日の詳細は、 [プロジェクト、タスクおよび問題に関する予定完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

   ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* プロジェクト所有者には、タスクの通知領域と「更新」タブで、この変更がプロジェクトタイムラインに影響を与えるかどうかが通知されます。

   ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

   >[!TIP]
   コミット日が変更された通知は、Workfront管理者が設定の「更新フィード」領域にコミット日を表示できるようにした場合にのみ、プロジェクト所有者に送信されます。 詳しくは、 [システムで追跡された更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

   プロジェクト所有者が変更を受け入れたくない場合は、新しい日付を提案するユーザーにコメントを返して、コミット日を元の計画日に戻すか、新しい日付を選択するように求めることをお勧めします。 プロジェクト所有者が変更を受け入れた場合は、手動で計画完了日を調整して、アイテムに割り当てられたユーザーが提供するコミット日に一致させることができます。

   プロジェクト所有者は、「コミット日」を使用して、計画完了日をリセットできます。 それには、タスクの「更新日」タブで「予定日の設定先」オプションを選択します。 この変更を受け入れるには、タスクとプロジェクトを管理するアクセス権が必要です。

   >[!NOTE]
   タスクの完了予定日の変更を承認して、プロジェクトのタイムラインがどのように影響を受けるかを確認するには、 **プロジェクトタイムライン**. これにより、ガントチャートが開き、日付の変更を評価できます。
   ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >

作業項目の更新時に使用できる追加機能について詳しくは、  [作業を更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

タスクと問題のコミット日の更新の詳細については、 [タスクと問題に関するコミット日の更新](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE:&nbsp;moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On&nbsp;It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click&nbsp;<strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
