---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 期間タイプの概要：シンプル
description: シンプル期間タイプは、Adobe Workfrontでタスクに設定できる期間タイプです。
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 46%

---

# 期間タイプの概要：シンプル

<!-- Audited: 5/2025 -->

シンプル期間タイプは、Adobe Workfrontでタスクに設定できる期間タイプです。 Workfrontの期間タイプについて詳しくは、[ タスク期間と期間タイプの概要 ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) を参照してください。

## シンプル期間タイプの概要

Workfrontまたはグループの管理者は、システムまたはグループのデフォルトの期間タイプをシンプルに設定できます。 この場合、すべての新しいタスクはこの期間タイプで作成されます。

システムレベルまたはグループレベルのプロジェクト環境設定の一部として、タスクやイシューの環境設定を変更する方法については、[システム全体のタスクとイシュー環境を設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

タスクの期間タイプが [ シンプル ] の場合、次のことが発生します。

* プロジェクトマネージャーは、担当者間での時間の配分方法を変更する際に、タスクの期間と予定時間数の両方を変更できます。

  詳しくは、[シンプル期間タイプを使用したタスクの予定時間数と期間の更新](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md)を参照してください。

  >[!IMPORTANT]
  >
  >最初にタスクを作成し、それに「シンプル」期間タイプを割り当てたが、期間を指定しなかった場合、Workfrontはそのタスクに指定された予定時間数に基づいてタスクの期間を計算します。 シンプル期間タスクの期間を手動で変更すると、Workfrontは、予定時間数を期間に合わせるのを停止します。これは、予定時間数を手動で定義すると想定されるからです。
  >
  >Workfrontは、次の数式を使用して、手動で期間が変更されていないタスクの期間を計算します。
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Workfront 管理者は、インスタンスの設定のプロジェクト環境設定エリアで `Typical hours per work day` を定義します。

* 配分率は非表示になっていますが、配分の時間は編集できます。
* 新規顧客の場合、システムレベルの期間タイプはシンプルに設定されます。

## タスクの期間タイプをシンプルに変更

タスクの期間タイプの変更については、[タスクの期間タイプの更新](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
