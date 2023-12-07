---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: タスク依存関係タイプの概要
description: 依存タイプは、タスク間の先行タスク関係を指します。 先行タスクの開始または終了に基づいて、依存タスクを開始または終了できるタイミングを定義します。
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 45c82f659d02dca69d2a2c390b084330773d4252
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# タスク依存関係タイプの概要

依存タイプは、タスク間の先行タスク関係を指します。 先行タスクの開始または終了に基づいて、依存タスクを開始または終了できるタイミングを定義します。

>[!IMPORTANT]
>
>Adobe Workfrontは、先行関係が適用されない限り、依存関係の種類に基づいて、依存タスクの開始や終了を制限しません。 先行タスクの適用の詳細については、 [先行タスクの実行](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

タスク間でこの関係を確立する場合は、先行関係の「依存関係タイプ」を指定する必要があります。

先行タスクの詳細については、「 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

次に、 Workfront Dependency Types を示します。

* **Finish-Start (fs)**：先行タスクは、依存タスクが開始する前に完了する必要があります。 これはデフォルトの依存タイプで、他の依存タイプが指定されていない場合に使用されます。
* **完了 — 完了 (ff)**：先行タスクは、依存タスクが終了する前に終了する必要があります。
* **開始 — 開始 (ss)**：先行タスクは、依存タスクが開始できる前に開始する必要があります。 先行タスクが少なくとも開始していない場合は、依存タスクを開始できません。
* **開始 — 完了 (sf)**：先行タスクは、依存タスクが終了する前に開始する必要があります。 先行タスクの開始前に依存タスクを開始できますが、先行タスクが開始しない限り、タスクを終了することはできません。
* **Scheduled-Start (sd)**：タスクを「終了 — 開始」としてスケジュールしますが、実際の実施タイプは「終了 — 終了」になります。 これを使用すると、依存タスクは先行タスクの完了後に開始するようにスケジュールされます。 ただし、実施によって、依存タスクはいつでも開始できますが、先行タスクが終了するまで完了できません。

>[!NOTE]
>
>[ 依存関係の種類 ] の略語は、先行タスク関係を定義するタスクリストで使用されます。 詳しくは、 [タスクリスト内の先行タスクの値の例](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [タスクの先行タスクの概要](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

