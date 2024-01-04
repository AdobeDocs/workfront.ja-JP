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
ht-degree: 0%

---

# かんばんの概要

<!-- Audited: 01/2024 -->

以下の節では、 [!UICONTROL かんばん] ボードの機能。

K の説明[!UICONTROL 禁止する] 方法については、 [アジャイルチームの作成](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

アジャイルチームからの移行に関心がある場合 [!UICONTROL かんばん] ～に乗り込む [!DNL Workfront] [!UICONTROL ボード]を参照してください。 [チームのアジャイルの移行 [!UICONTROL かんばん] カード [!DNL Workfront] ボード](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL かんばん] ボードのレイアウトと機能

The [!UICONTROL かんばん] ボードは、次の要素で構成されます。

**バックログ列**：現在バックログに残っているすべてのタスクを表示します。 この列は、デフォルトでは表示されません。 バックログを [!UICONTROL かんばん] ボード、詳しくは、 [アジャイルバックログの管理](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**ストーリーのステータス**：ストーリーのステータス列に基づいて、ストーリーの進行状況を示します。

詳しくは、 [ストーリーのステータスを [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

「 」セクションで説明しているように、アジャイルビューを変更して、プロジェクトに合わせてストーリーステータスをカスタマイズできます [[!UICONTROL アジャイルビューの作成またはカスタマイズ]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [でビューを作成または編集 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>デフォルトでは、最大 50 枚のカードがかんばんボードに表示されますが、クリックできます **[!UICONTROL 表示を増やす]** 追加のカードを表示するには、をクリックします。

## サブタスクとストーリー間の関係

ストーリーにサブタスクが含まれている場合、親ストーリー自体の情報（ポイント/時間、パーセント完了など）を更新することはできません。 さらに、ストーリーを [!UICONTROL かんばん] ボードを使用して、ステータスを更新します。 その代わりに、ストーリーのサブタスクに加えた変更がストーリーに反映されます。 すべてのサブタスクのストーリーポイントまたは時間を組み合わせて、親ストーリーのポイントまたは時間を指定します。

例えば、ストーリーに 4 ポイントのサブタスクが 1 つしかない場合、ストーリー自体にも 4 ポイントが割り当てられます。 サブタスクポイントの値を 3 に変更すると、親ストーリーのポイントの値が 3 に変更されます。 同じストーリーに別のサブタスクを作成し、そのサブタスクのポイント値を 4 に設定した場合、両方のサブタスクの結合ポイント値を反映するために、ストーリーのポイント値が 7 に変更されます。

この同じロジックは、第 2 レベルのサブタスク（サブタスクのサブタスク）にも適用されます。 サブタスクに第 2 レベルのサブタスクが 1 つ以上ある場合、サブタスクは第 2 レベルのサブタスクに基づいて計算されます。

## サポートされる機能

かんばんボードを使用する際には、次の操作を実行できます。

* [サブタスクを [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [既存のタスクまたはタスクを [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [ユーザーを [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [次の場所からストーリーと問題を追加： [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [次の場所からストーリーまたはイシューを削除 [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [ストーリー情報を編集](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [次の項目でユーザーをフィルター： [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [WIP の上限に対する進行中の作業 (WIP) を管理 [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [ストーリーの並べ替え [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [ストーリーのステータスを [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [ストーリーにフラグを使用する [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [バックログを [!UICONTROL かんばん] ボード](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)
