---
content-type: reference
product-area: projects
navigation-topic: task-information
title: タスクの予定期間と予定期間の違い
description: 期間とは、作業アイテムの予定開始日から予定完了日までの時間です。 タスクの期間タイプに応じて、Adobe Workfront には期間と予定期間が表示されます。
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
TQID: https://experienceleague.adobe.com/tVh55DKoBvOUZdq9lZ6y72rxZQ1WOoAYL-Pz8nlU588
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 272
ht-degree: 87%

---

# タスクの予定期間と期間の違い

期間とは、作業アイテムの予定開始日から予定完了日までの時間です。 タスクの期間タイプに応じて、Adobe Workfront には期間と予定期間が表示されます。

イシューとプロジェクトは、期間タイプに関連付けることはできません。期間のみを持ちます。

## タスクの期間

タスクの場合、期間と計画期間には通常同じ値が表示されます。この値は、タスクの予定開始日から予定完了日までの時間です。

タスクの期間タイプが、作業優先の場合、リソースをタスクに追加するにつれて予定期間は減少します。

**例：**&#x200B;期間タイプが作業優先であるタスクの期間が 3 日で、フルタイムのスケジュールを持つ 1 つのリソースをタスクに割り当てた場合、予定期間も 3 日です。

フルタイムのスケジュールを持つ3つのリソースを同じタスクに割り当てる場合、期間は3日のままですが、予定期間は1日になります。予定期間では、タスクの予定開始日と予定完了日も変更され、新しい予定期間が反映されます。その結果、プロジェクトのタイムラインにも影響が及びます。
タスクを複数のリソースに割り当てる場合は、「労力駆動期間タイプ」を使用できます。これにより、タスクが完了するのにかかる時間を短縮できます。

作業優先の期間タイプの詳細は、[期間タイプの概要：作業優先](../../../manage-work/tasks/taskdurtn/effort-driven.md)を参照してください。

## イシューとプロジェクト期間

イシューとプロジェクトには、期間の値が 1 つのみあります。これは、イシューの予定開始日と予定完了日、プロジェクトの予定開始日と予定完了日それぞれの差です。
