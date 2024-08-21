---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移動またはコピーされたタスクまたは問題のカスタム状態
description: タスクまたはイシューを別のプロジェクトに移動またはコピーすると、タスクまたはイシューの一部のステータスが、移動先のプロジェクトのグループで使用されているステータスに合わせて更新される場合があります。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 94%

---

# 移動またはコピーされたタスクまたはイシューに対するカスタムステータス

タスクまたはイシューを別のプロジェクトに移動またはコピーすると、タスクまたはイシューの一部のステータスが、移動先のプロジェクトのグループで使用されているステータスに合わせて更新される場合があります。これは、そのグループに同じキーを持つステータスが存在するかどうかによって異なります。

* タスクまたはイシューのステータスが、移動先プロジェクトのグループで使用されるステータスと同じキーを持つ場合、タスクまたはイシューのステータスは同じままになります。

  これら 2 つのステータスのラベルが一致しない場合、タスクまたはイシューのステータスは、移動先のプロジェクトのグループで使用されているステータスのラベルを継承します。

* タスクまたはイシューのステータスが、移動先のプロジェクトのグループと同等のステータスと同じキーを持たない場合、タスクまたはイシューのステータスは、移動先のプロジェクトのグループのデフォルトステータスに変わります。

ステータスキーについて詳しくは、[グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。
