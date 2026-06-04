---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: タスク依存関係タイプの概要
description: 依存タイプは、タスク間の先行タスク関係を指します。 これらは、先行タスクの開始または終了に基づいて、依存タスクを開始または終了できるタイミングを定義します。
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
TQID: https://experienceleague.adobe.com/AioKERGt0FLv1eBE5-evwa2d35fItwknWI-ZouBECSo
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
source-wordcount: 322
ht-degree: 98%

---

# タスク依存関係タイプの概要

<!-- Audited: 12/2023 -->

依存タイプは、タスク間の先行タスク関係を指します。 これらは、先行タスクの開始または終了に基づいて、依存タスクを開始または終了できるタイミングを定義します。

>[!IMPORTANT]
>
>Adobe Workfront は、先行関係が強制されない限り、依存関係タイプに基づいて、依存タスクの開始や終了を制限しません。 先行タスクの強制について詳しくは、[先行タスクの強制](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)を参照してください。

タスク間でこの関係を確立する場合は、先行関係の依存関係タイプを指定する必要があります。

先行タスクについて詳しくは、[先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

次に、Workfront の依存関係タイプを示します。

* **終了 - 開始（fs）**：先行タスクは、依存タスクが開始する前に終了する必要があります。 これはデフォルトの依存タイプで、他の依存タイプが指定されていない場合に使用されます。
* **終了 - 終了（ff）**：先行タスクは、依存タスクが終了する前に終了する必要があります。
* **開始 - 開始（ss）**：先行タスクは、依存タスクが開始する前に開始する必要があります。 先行タスクが開始されていない限り、依存タスクを開始できません。
* **開始 - 終了（sf）**：先行タスクは、依存タスクが終了する前に開始する必要があります。 先行タスクの開始前に依存タスクを開始できますが、先行タスクが開始しない限り、タスクを終了することはできません。
* **スケジュール済み - 開始（sd）**：タスクが「終了 - 開始」としてスケジュールされますが、実際の強制タイプは「終了 - 終了」になります。 これを使用すると、依存タスクは先行タスクの終了後に開始されるようにスケジュールされます。 ただし、この強制により、依存タスクはいつでも開始できますが、先行タスクが終了するまで完了できません。

>[!NOTE]
>
>依存関係タイプの略語は、先行タスク関係を定義するタスクリストで使用されます。 詳しくは、[タスクの先行タスクの概要](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md)の[タスクリストの先行タスク値の例](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list)を参照してください。

