---
content-type: overview
product-area: projects
navigation-topic: update-work-in-a-project
title: コミット日の概要
description: コミット日は、タスクまたはイシューに割り当てられたユーザーがタスクまたはイシューを完了するためにコミットする日付です。これは予定完了日とは異なり、作業を直接担当するユーザーが設定する、より現実的な予定完了日です。
author: Alina
feature: Work Management
exl-id: 47072433-bb8e-4210-947a-8bfa41ec47a9
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 81%

---

# コミット日の概要

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview"> 現在のリリースについて詳しくは、[2024 年第 3 四半期リリースの概要 ](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md) を参照してください。</span>

コミット日は、タスクまたはイシューに割り当てられたユーザーがタスクまたはイシューを完了するのにコミットする日付です。

これはタスクやイシューの予定完了日とは異なり、作業を担当するユーザーが設定する、より現実的な予定完了日です。

予定完了日について詳しくは、[タスクの予定完了日の概要](../../../manage-work/tasks/task-information/task-planned-completion-date.md)を参照してください。

## コミット日の概要

コミット日を扱う際は、次の点を考慮してください。

* コミット日があるのはタスクとイシューのみです。
* コミット日は、Adobe Workfront では自動的に設定されません。\
  タスクまたはイシューを作成する場合、タスクまたはイシューにコミット日は割り当てられません。
* タスクまたはイシューに割り当てられている場合は、次のいずれかの操作を行ってコミット日を設定できます。

   * Workfront は、タスクまたはイシューの「作業」、「問題の取り組みを開始」、または「タスクを開始」をクリックして、タスクまたはイシューの既存の予定完了日に一致するようにコミット日を設定します。「作業をする」ボタンを「開始」ボタンに置き換える方法については、[「作業をする」ボタンの「開始」ボタンへの置き換え](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)を参照してください。
   * タスクまたはイシューが完了したと思われるタイミングに応じて、自分でコミット日を手動で設定します。これは、タスクまたはイシューを特定の日までに完了させる、担当者としてのプロジェクトマネージャーに対する見込みとコミットメントです。
詳しくは、[タスクやイシューのコミット日の更新](/help/quicksilver/manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)を参照してください。

>[!NOTE]
>
>コミット日を変更するには、タスクのタスク所有者である必要があります。次のユーザーは、タスクのコミット日を変更できません。
>
>* プロジェクト所有者
>* プロジェクトスポンサー
>* リソース管理者
>* システム管理者
>* タスクのその他の担当者
>* タスクに対する権限を持つその他のユーザー。
>
>タスク責任者について詳しくは、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

## タスクおよび問題のコミット日を見つける

Workfrontの次の領域で、タスクと問題のコミット日を確認できます。

* 詳細ページ
* Workfront管理者またはグループ管理者がレイアウトテンプレートに概要パネルを追加した後。 詳しくは [ レイアウトテンプレートを使用したホームと概要のカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md) を参照してください。
* <span class="preview">Workfront管理者またはグループ管理者がレイアウトテンプレートに追加した後のタスクまたはイシューのヘッダー。 詳しくは、[ レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md) を参照してください。</span>

## コミット日の変更によってトリガーされる通知と更新 {#notifications-and-updates-triggered-by-changing-the-commit-date}

タスクまたはイシューの担当者がコミット日をプロジェクト所有者が設定した予定完了日とは異なる日付に手動で変更すると、プロジェクト所有者や他のユーザーにこの変更について警告する通知や更新が多数行われます。

>[!NOTE]
>
>コミット日を変更しても、計画日は自動的に変更されず、計画日に加えた変更でも、コミット日は自動的に変更されません。

タスクまたはイシューのコミット日を手動で設定すると、次の変更がトリガーされます。

* コミット日の変更は、タスクまたはイシューの「更新」セクションの「システムアクティビティ」タブと「すべて」タブに入力されます。

  ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)

  Workfront 管理者が設定のフィードを更新エリアでこの更新を有効にした場合、コミット日の変更がタスクまたはイシューの更新エリアに表示されます。詳しくは、[システムで追跡された更新](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)を参照してください。

  プロジェクト所有者が変更を受け入れない場合は、「更新」セクションの「コメント」タブを使用して、新しい日付を提案しているユーザーにコメントバックし、コミット日を元の予定日に戻すか、新しい日付を選択することをお勧めします。

  プロジェクト所有者が変更を承認する場合は、タスクまたはイシューを編集することで、手動で予定完了日を調整して、項目に割り当てられたユーザーが指定したコミット日に一致させることができます。

  タスクまたはイシューを編集するには、これらを管理するアクセス権が必要です。

  >[!TIP]
  >
  >システム管理者またはグループ管理者に依頼して、「コミット日」フィールドを概要パネルまたはヘッダーに追加して、更新を容易にすることができます。
  >
  >詳しくは、次の記事を参照してください。
  >
  >* [ 概要 ](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
  >* [レイアウトテンプレートを使用してホームと概要をカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
  >* [ レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

<!--this is no longer possible: 
>[!NOTE]
>
>If you want to see how the timeline of the project is affected by accepting to change the Planned Completion Date of the task, click **Project Timeline**. This opens the task list where you can evaluate the date changes and the project timeline.
>
>
>![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)  >
>
-->


* タスクまたはイシューの見込み完了日が同じ日付に設定されるのは、タスクの完了する可能性が高い時期がより正確に示されるようになったためです。

  見込み完了日について詳しくは、[プロジェクト、タスク、およびイシューに関する見込み完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。

  ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

* プロジェクト所有者に、「通知」エリアでタスクまたはイシューのコミット日が変更されたことが通知されます。

  ![](assets/in-product-notification-commit-date-changed-nwe-350x149.png)

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tip below is actually wrong and the updates feeds should not control this setting, but at this time it does, according to this issue in Hub: https://hub.workfront.com/issue/61e1aa5e0002a186fdd0a73a10db0fc3/updates?email-source=comm</p>
  -->

  >[!TIP]
  >
  >コミット日の変更通知は、Workfront 管理者が設定の更新フィードエリアでコミット日を表示できるようにした場合にのみ、プロジェクト所有者に送信されます。詳しくは、[システムで追跡された更新の設定](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)を参照してください。

作業アイテムの更新時に使用できるその他の機能については、[作業の更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

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
