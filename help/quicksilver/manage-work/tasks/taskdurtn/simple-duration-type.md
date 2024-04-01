---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 「期間タイプの概要：シンプル」
description: シンプル期間タイプは、Adobe Workfront のタスクに設定できる期間タイプです。Workfront の期間タイプに関する一般情報については、タスク期間の概要と期間タイプを参照してください。
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: 1efd7c0270fe1396345cfa6e5499e8f998297d61
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 79%

---

# 期間タイプの概要：シンプル

シンプル期間タイプは、Adobe Workfront のタスクに設定できる期間タイプです。Workfront の期間タイプに関する一般情報については、[タスク期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

## シンプル期間タイプの概要

Workfront 管理者またはグループ管理者は、システムまたはグループのデフォルトの期間タイプを「シンプル」に設定できます。この場合、すべての新しいタスクは、この期間タイプで作成されます。システムレベルまたはグループレベルのプロジェクト環境設定の一部として、タスクやイシューの環境設定を変更する方法については、[システム全体のタスクとイシュー環境を設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

タスクの期間タイプがシンプルの場合は、次のようになります。

* プロジェクトマネージャーは、担当者間での時間の配分方法を変更する際に、タスクの期間と予定時間数の両方を変更できます。

  詳しくは、[シンプル期間タイプを使用したタスクの予定時間数と期間の更新](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md)を参照してください。

  >[!IMPORTANT]
  >
  >最初にタスクを作成し、そのタスクに単純期間タイプを割り当て、期間を指定しない場合、Workfrontでは、タスクに指定した計画時間数に基づいてタスクの期間が計算されます。 シンプル期間タスクの期間を手動で変更すると、Workfront は予定時間数と期間を照合しなくなります。それらをユーザー自身が手動で定義する必要があると Workfront が見なすからです。
  >
  >Workfrontは、次の式を使用して、期間が手動で変更されていないタスクの期間を計算します。
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Workfront管理者が `Typical hours per work day` （インスタンスのセットアップの「プロジェクトの環境設定」領域）をクリックします。

* 配分率は非表示になり、代わりに時間配分を編集できます。
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
