---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: かんばんの概要
description: かんばんボードの機能をより深く理解するには、この記事を参照してください。
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: fa499d74df891441e729c32188e9b2f74e4ef5c0
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 91%

---

# かんばんの概要

<!-- Audited: 01/2024 -->

以下の節を参照すると、[!UICONTROL かんばん]ボードがどのように機能するかをより詳しく理解できます。

K の説明[!UICONTROL 禁止する] 方法については、 [アジャイルチームの作成](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

アジャイルチームの[!UICONTROL かんばん]ボードから[!DNL Workfront] [!UICONTROL ボード]への移行に関心がある場合は、「[アジャイルチームの[!UICONTROL かんばん]カードから  [!DNL Workfront]  ボード](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md)への移行」を参照してください。

## [!UICONTROL かんばん]ボードのレイアウトと機能

[!UICONTROL かんばん]ボードは、次の要素で構成されます。

**バックログ列**：現在バックログに残っているすべてのタスクを表示します。この列は、デフォルトでは表示されません。[!UICONTROL かんばん]ボードにバックログを表示する方法など、バックログについて詳しくは、[アジャイルバックログの管理](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)を参照してください。

**ストーリーのステータス**：ストーリーがどのステータス列にあるかに基づいて、ストーリーの進行状況を示します。

詳しくは、[[!UICONTROL カンバン]ボードのストーリーのステータスの更新](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)を参照してください。

「 」セクションで説明しているように、アジャイルビューを変更して、プロジェクトに合わせてストーリーステータスをカスタマイズできます [[!UICONTROL アジャイルビューの作成またはカスタマイズ]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [でビューを作成または編集 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>デフォルトでは、かんばんボードには最大 50 枚のカードが表示されますが、「**[!UICONTROL さらに表示]**」をクリックすると、追加のカードを表示できます。

## サブタスクとストーリー間の関係

ストーリーにサブタスクが含まれている場合、親ストーリー自体の情報（ポイントや時間、完了率など）を更新することはできません。さらに、[!UICONTROL かんばん]ボード上でストーリーを移動してステータスを更新することはできません。ストーリーのサブタスクに加えた変更がストーリーに反映されます。すべてのサブタスクのストーリーポイントまたは時間を合計したものが、親ストーリーのポイントまたは時間になります。

例えば、ストーリーに 4 ポイントのサブタスクが 1 つだけある場合、ストーリー自体も 4 ポイントとなります。サブタスクポイントの値を 3 に変更すると、親ストーリーのポイントの値が 3 に変わります。同じストーリーに別のサブタスクを作成し、そのサブタスクのポイント値を 4 に設定した場合、両方のサブタスクの合計ポイント値を反映して、ストーリーのポイント値は 7 に変わります。

この同じロジックは、第 2 レベルのサブタスク（サブタスクのサブタスク）にも適用されます。サブタスクに第 2 レベルのサブタスクが 1 つ以上ある場合、サブタスクは第 2 レベルのサブタスクに基づいて計算されます。

## サポート機能

かんばんボードを使用する際には、次のアクションを実行できます。

* [[!UICONTROL かんばん]ボードの既存のストーリーにサブタスクを追加する](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [既存のタスクまたはイシューを[!UICONTROL かんばん]ボードに追加する](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [ユーザーを[!UICONTROL かんばん]ボード上のストーリーに割り当てる](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [[!UICONTROL かんばん]ボードからストーリーとイシューを追加する](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [[!UICONTROL かんばん]ボードからストーリーやイシューを削除する](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [ストーリー情報の編集](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [[!UICONTROL かんばん]ボード上でユーザーによってフィルタリングする](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [[!UICONTROL かんばん]ボード上で進行中の作業（WIP）の制限を管理する](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [[!UICONTROL かんばん]ボードでストーリーを並べ替える](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [[!UICONTROL かんばん]ボードでストーリーのステータスを更新する](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [[!UICONTROL かんばん]ボードでストーリーにフラグを使用する](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [[!UICONTROL かんばん]ボードにバックログを追加する](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
