---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: コミット日の概要
description: コミット日は、ユーザーがタスクまたは問題を完了するとコミットする日付です。 これは、作業を直接担当するユーザーが与える完了日をより現実的に見積もるため、予定完了日とは異なります。
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 37%

---

# コミット日の概要

<!--Audited: 05/2025-->

<!-- <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

コミット日は、ユーザーがタスクまたは問題を完了するとコミットする日付です。 これは、タスクやイシューの予定完了日とは異なり、作業の担当者のみが指定する完了日をより現実的に見積もるためです。

予定完了日について詳しくは、[タスクの予定完了日の概要](../../../manage-work/tasks/task-information/task-planned-completion-date.md)を参照してください。

## コミット日の概要

コミット日を扱う際は、次の点を考慮してください。

* コミット日があるのはタスクとイシューのみです。
* コミット日は、Adobe Workfrontによって自動的に設定されるわけではありません。 タスクまたは問題を作成する際、コミット日は割り当てられていません。
* タスクまたはイシューに割り当てられている場合は、次のいずれかの操作を行ってコミット日を設定できます。

   * Workfront は、タスクまたはイシューの「作業」、「問題の取り組みを開始」、または「タスクを開始」をクリックして、タスクまたはイシューの既存の予定完了日に一致するようにコミット日を設定します。詳しくは、[ 「作業対象」ボタンの「開始」ボタンへの置き換え ](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) を参照してください。
   * タスクまたは問題が完了すると思われるタイミングに応じて、自分でコミット日を設定します。 これは、特定の日までにタスクまたは問題を完了するという、プロジェクト管理者への担当者としての推定とコミットメントです。 詳しくは、[タスクやイシューのコミット日の更新](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)を参照してください。

>[!NOTE]
>
>コミット日を変更するには、タスクのタスク所有者である必要があります。次のユーザーは、タスクのコミット日を変更できません。
>
>* プロジェクト所有者
>* プロジェクトスポンサー
>* リソース管理者
>* システム管理者
>* タスクのその他の担当者
>* タスクに対する権限を持つその他のユーザー
>
>タスク責任者について詳しくは、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

## タスクおよび問題のコミット日を見つける

タスクとイシューのコミット日は、Workfrontの次の領域で確認できます。

* 詳細ページ
* Workfront管理者またはグループ管理者がレイアウトテンプレートに追加した後の概要パネル。 詳しくは、[ レイアウトテンプレートを使用した概要パネルのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md) を参照してください。
* Workfront管理者またはグループ管理者がレイアウトテンプレートに追加した後のタスクまたはイシューのヘッダー。 詳しくは、[レイアウトテンプレートを使用してオブジェクトヘッダーをカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

## コミット日の変更によってトリガーされる通知と更新 {#notifications-and-updates-triggered-by-changing-the-commit-date}

タスクまたはイシューの担当者がコミット日をプロジェクト所有者が設定した予定完了日とは異なる日付に手動で変更すると、プロジェクト所有者や他のユーザーにこの変更について警告する通知や更新が多数行われます。

>[!NOTE]
>
>コミット日に加えた変更によって予定日が自動的に変更されることはありません。また、予定日に加えた変更によってコミット日が自動的に変更されることはありません。

タスクまたはイシューのコミット日を手動で設定すると、次の変更がトリガーされます。

* コミット日の変更は、タスクまたは問題の「システム」アクティビティと「更新」セクションの「すべて」タブに入力されます。

  ![ コミット日の変更通知 ](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  Workfront管理者が「設定」の「更新フィード」領域でこの更新を有効にすると、コミット日の変更がタスクまたは問題の「更新」領域に表示されます。詳しくは、[システムで追跡された更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)を参照してください。

  プロジェクト所有者が変更を受け入れない場合は、「更新」セクションの「コメント」タブを使用して、新しい日付を提案しているユーザーにコメントバックし、コミット日を元の予定日に戻すように依頼するか、新しい日付を選択することをお勧めします。

  プロジェクト所有者が変更を受け入れる場合は、タスクまたは問題を編集して、アイテムに割り当てられたユーザーが提供するコミット日に一致するように、手動で予定完了日を調整できます。

  タスクまたはイシューを編集するには、これらを管理するアクセス権が必要です。

  >[!TIP]
  >
  >システム管理者またはグループ管理者に依頼して、概要パネルまたはヘッダーに「コミット日」フィールドを追加して、更新を容易にすることができます。
  >
  >詳しくは、次の記事を参照してください。
  >
  >* [ 概要 ](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [ レイアウトテンプレートを使用した概要パネルのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [レイアウトテンプレートを使用してオブジェクトヘッダーをカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* タスクの見込み完了日が同じ日に設定されているのは、タスクが完了する可能性の高いときをより正確に示すためです。

  詳しくは、[プロジェクト、タスクおよびイシューの見込み完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* プロジェクト所有者には、「通知」領域で、タスクまたは問題のコミット日が変更されたことを通知されます。

  ![ コミット日の変更通知 ](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >コミット日の変更通知は、Workfront 管理者が設定の更新フィードエリアでコミット日を表示できるようにした場合にのみ、プロジェクト所有者に送信されます。詳しくは、[システムで追跡された更新の設定](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)を参照してください。

作業項目の更新時に使用できる追加機能について詳しくは、「[ 作業の更新 ](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)」を参照してください。

タスクとイシューのコミット日の更新について詳しくは、[タスクとイシューに関するコミット日の更新](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update Commit Dates on tasks and issues</h2>
<p>(NOTE: moved to its own article) </p>
<p>Updating the Commit Date is identical for tasks and issues.</p>
<ol>
<li value="1"> <p>Go to a task or issue that you are assigned to as the <strong>Task Owner</strong>.</p> <p>For more information about finding out who the Task Owner for an issue or task is, see the section <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments" class="MCXref xref">Edit tasks</a> in the article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks.md" class="MCXref xref">Edit tasks</a>.</p> </li>
<li value="2"> <p>Click Work on it in the task or issue header</p> <p>Or</p> <p>Click <strong>Start Task</strong> or <strong>Start Issue</strong> if the Work on it button has been customized in your environment to indicate that you are now working on the work item. </p> <p>At this time, the Commit Date and the Planned Completion Date of the task or issue are the same.</p> </li>
<li value="3"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">(Optional) If you clicked Start Task or Start Issue, click <strong>Undo</strong> in the lower-left corner of the screen. The Commit Date is removed. </p> <p>For information about replacing the Work On It button with a Start button, see <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a></span>.</p> <note type="tip">
The option to undo your selection to start your work is not available when you click
<span style="font-weight: bold;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Work on it</span>.
</note> </li>
<li value="4"> <p> Expand the <strong>This will be done by</strong> date picker, and select a new Commit Date.</p>
<div>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<p>Click <strong>Updates</strong> in the left panel, then click the <strong>Start a new update</strong>><strong>Commit Date</strong></p>
<p>Or</p>
<p>Click <strong>Task Details</strong> or <strong>Issue Details</strong> in the left panel, then double click <strong>Commit Date</strong> and select a new date from calendar. </p>
</div>
<p>The Commit Date and the Planned Completion date are no longer the same.</p>
<p>Instead, the Commit Date and the Projected Completion Date of the task or issue become the same.</p>
<p>The changes are saved automatically.</p>
<p>The Project Owner is notified that you have suggested a new Commit Date for the task or issue and can, at this time, update the Planned Completion Date of the task or issue to match the Commit Date you suggested. For information about the notifications and updates that are triggered by this change, see the section <a href="#notifications-and-updates-triggered-by-changing-the-commit-date" class="MCXref xref">Notifications and updates triggered by changing the Commit Date</a> in this article.</p>
</div> </li>
</ol>
</div>
-->
