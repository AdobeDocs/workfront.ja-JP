---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: タスク依存関係ループの概要
description: タスクに先行タスク関係を追加すると、依存関係のループが発生する場合があります。 先行タスクの詳細については、「先行タスクの概要」を参照してください。
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# タスク依存関係ループの概要

タスクに先行タスク関係を追加すると、依存関係のループが発生する場合があります。 先行タスクの詳細については、 [タスクの先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 依存関係ループの概要

互いに依存して完了するタスクが 2 つ以上ある場合に、依存関係ループが発生します。 Adobe Workfrontでは、依存関係ループが作成された場合、タスク間に先行タスク関係を作成することはできません。

**例：** タスク 2 はタスク 1 の先行タスクで、タスク 1 の作業を開始する前にタスク 2 を完了する必要があります。

Task 1 を Task 2 の先行タスクにしようとすると、Task 1 を Task 2 が完了するまで開始できず、Task 1 が完了するまで開始できないので、依存ループエラーが発生します。

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 依存関係ループに関する考慮事項

* 依存関係ループには、2 つ以上のタスクを含めることができます。 先行関係に接続するタスクの親の数は、依存関係のループを作成する親の数になる場合があります。
* また、親を子の前身にしようとすると、依存関係のループが発生する場合もあります。
* 依存関係ループの場合、タスクやプロジェクトを保存することはできません。 依存関係のループを修正するには、エラーメッセージに表示されているタスク間の先行関係を再評価し、競合を解除してから、タスクまたはプロジェクトを保存する必要があります。

 
