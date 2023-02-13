---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの「開始可能」の概要
description: タスクを開始する準備が整ったら、Adobe Workfrontはタスクに開始可能インジケーターを追加して、タスクの作業を開始しても安全であることを簡単に識別できます。 この指標は、タスクリストまたはレポートのビューで表示できます。
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# タスクの「開始可能」の概要

タスクを開始する準備が整ったら、Adobe Workfrontはタスクに開始可能インジケーターを追加して、タスクの作業を開始しても安全であることを簡単に識別できます。 この指標は、タスクリストまたはレポートのビューで表示できます。

タスクを実行する準備が整ったら、タスクの [ 開始可能 ] フィールドを True に設定します。

## Workfrontがタスクを「開始可能」としてマークする仕組み

Workfrontは、タスクを「開始可能」フィールドに「True」とマークする前に、次の項目を確認します。

* タスクに親がある場合は、True に設定された親の Can Start の値を確認します。 親の値が False の場合、すべてのサブタスクの値は Can Start に False に設定されます。 
* また、タスクの先行タスクと、その親の先行タスクが完了したかどうかも確認します。 タスクが完了した場合、タスクの Can Start 値は True に設定されます。 タスクの先行タスクまたはその親の先行タスクのいずれかが完了していない場合、またはステータスが [ 承認待ち ] の場合、タスクの [ 開始可能 ] の値は False に設定されます。 

   タスクの先行タスクの詳細については、 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 開始する準備が整ったタスクの識別に関する考慮事項

* タスクと先行タスクの [ 依存関係の種類 ] が [ 開始 — 開始 ] の場合は、先行タスクの関係が解決され、後続タスクを開始できるように、先行タスクを開始する必要があります。 依存関係タイプについて詳しくは、 [タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* タスクにプロジェクト間の先行タスクがある場合、先行タスクの完了によって、後続タスクに自動的に適用する [ 開始可能 ] インジケータがトリガーされません。 後続のタスクが [ 開始可能 ] タスクとして表示される前に、後続のプロジェクトのタイムラインを手動で再計算するか、Workfrontで自動的に再計算する必要があります。 プロジェクトタイムラインの再計算の詳細については、 [プロジェクトタイムラインを再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   プロジェクト間の先行タスクの詳細については、 [プロジェクト間の先行タスクの作成](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
