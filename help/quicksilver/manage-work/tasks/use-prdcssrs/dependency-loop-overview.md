---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: タスク依存ループの概要
description: タスクに先行タスク関係を追加すると、依存関係ループが発生する場合があります。 先行タスクの詳細については、先行タスクの概要を参照してください。
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
TQID: https://experienceleague.adobe.com/cQbPOUES-tmSgZTpXrft8lQby-ubPmI-TZ1PjdGURMc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 68%

---

# タスク依存関係ループの概要

タスクに先行タスク関係を追加すると、依存関係ループが発生する場合があります。 先行タスクについて詳しくは、[タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

## 依存関係ループの概要

依存関係ループは、相互に依存して完了する2つ以上のタスクがある場合に発生します。 Adobe Workfrontでは、依存関係ループを作成する場合、タスク間に先行タスク関係を作成できません。

**例：**&#x200B;タスク 2 はタスク 1 の先行タスクで、タスク 1 の作業を開始する前にタスク 2 を完了する必要があります。

タスク 1 をタスク 2 の先行タスクにしようとすると、タスク 1 はタスク 2 が完了するまで開始できないけれど、タスク 2 はタスク 1 が終了するまで開始できないので、依存関係ループエラーが発生します。

![依存関係ループエラーメッセージ &#x200B;](assets/dependency-loop-error-message-350x209.png)

![&#x200B; タスクリストの依存関係ループ &#x200B;](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 依存関係ループに関する考慮事項

* 依存関係ループには、2 つ以上のタスクを含めることができます。 先行タスク関係に接続するタスクの親の数は、依存関係ループを作成する親の数になる場合があります。
* また、親を子の先行タスクにしようとすると、依存関係のループが発生する場合もあります。
* 依存関係ループの場合、タスクまたはプロジェクトを保存することはできません。 依存関係ループを修正するには、エラーメッセージにリストされているタスク間の先行タスク関係を再評価し、タスクまたはプロジェクトを保存する前に競合を削除する必要があります。


