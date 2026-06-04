---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの「開始可能」の概要
description: タスクを開始する準備が整ったら、Adobe Workfront はタスクに開始可能のインジケーターを追加し、タスクの作業を開始しても安全であることを簡単に識別できます。 このインジケーターは、タスクリストまたはレポートのビューで表示できます。
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
TQID: https://experienceleague.adobe.com/jb8Vj9wMNCQj31cgjHMIm6M0RH3VusK5jBdNx233yjw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 440
ht-degree: 70%

---

# 「開始可能」なタスクの概要

タスクを開始する準備が整ったら、Adobe Workfront はタスクに開始可能のインジケーターを追加し、タスクの作業を開始しても安全であることを簡単に識別できます。 このインジケーターは、タスクリストまたはレポートのビューで表示できます。

タスクを行う準備が整ったら、タスクの「開始可能」フィールドが True に設定されます。

## Workfrontがタスクを「開始可能」とマークする方法

Workfront は、タスクの「開始可能」フィールドを True に設定する前に、次の項目を確認します。

* タスクに親がある場合、親のCan Startの値をTrueに設定するかどうか。 親の値が False の場合、すべてのサブタスクの「開始可能」値は False に設定されます。
* タスクの先行タスクと親の先行タスクが完了しているかどうか。 タスクが完了している場合、タスクの「開始可能」値は True に設定されます。 タスクの先行タスクまたはその親の先行タスクのいずれかが完了していない場合、またはステータスが「承認待ち」の場合、タスクの「開始可能」の値は False に設定されます。
* タスクの依存関係タイプがStart-StartまたはStart-Finishのどちらか。 依存関係タイプがStart-StartまたはStart-Finishの場合、依存タスクは、先行タスクが進行中の後（または先行タスクの完了率が1%を超えた後）に、「開始できる」フラグをTrueに設定します。

  先行タスクについて詳しくは、[先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

## 開始する準備が整ったタスクの識別に関する考慮事項

* タスクと先行タスクの「依存関係タイプ」が「開始 - 開始」の場合は、先行タスクの関係が解決されて後続タスクを開始できるように、先行タスクを開始する必要があります。 依存関係タイプについて詳しくは、[タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)を参照してください。
* タスクにプロジェクト間先行タスクがある場合、先行タスクの完了によって、後続タスクに自動的に適用する「開始可能」インジケーターはトリガーされません。 後継タスクが「開始可能」タスクとして表示される前に、後継タスクのプロジェクトのタイムラインを手動で再計算する必要があるか、Workfrontで自動的に再計算する必要があります。 プロジェクトタイムラインの再計算について詳しくは、[プロジェクトタイムラインの再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)を参照してください。

  プロジェクト間の先行タスクについて詳しくは、[プロジェクト間の先行タスクの作成](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)を参照してください。
