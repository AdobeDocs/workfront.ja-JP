---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移動またはコピーされたタスクまたはイシューのカスタムステータス
description: タスクまたはイシューを別のプロジェクトに移動またはコピーすると、タスクまたはイシューの一部のステータスが、移動先のプロジェクトのグループで使用されているステータスに合わせて更新される場合があります。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
TQID: 'https://experienceleague.adobe.com/GzG3KBfUw05edjA0DVRtODyGprG2mKVjOuUV2L5eWto'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 94%
---
# 移動またはコピーされたタスクまたはイシューに対するカスタムステータス

タスクまたはイシューを別のプロジェクトに移動またはコピーすると、タスクまたはイシューの一部のステータスが、移動先のプロジェクトのグループで使用されているステータスに合わせて更新される場合があります。 これは、そのグループに同じキーを持つステータスが存在するかどうかによって異なります。

* タスクまたはイシューのステータスが、移動先プロジェクトのグループで使用されるステータスと同じキーを持つ場合、タスクまたはイシューのステータスは同じままになります。

  これら 2 つのステータスのラベルが一致しない場合、タスクまたはイシューのステータスは、移動先のプロジェクトのグループで使用されているステータスのラベルを継承します。

* タスクまたはイシューのステータスが、移動先のプロジェクトのグループと同等のステータスと同じキーを持たない場合、タスクまたはイシューのステータスは、移動先のプロジェクトのグループのデフォルトステータスに変わります。

ステータスキーについて詳しくは、[グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。
