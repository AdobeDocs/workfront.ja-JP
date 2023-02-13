---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移動またはコピーされたタスクまたは問題に対するカスタムステータス
description: タスクまたはイシューを別のプロジェクトに移動またはコピーすると、タスクまたはイシューの一部のステータスが、移動先のプロジェクトのグループで使用されているステータスに合わせて更新される場合があります。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 移動またはコピーされたタスクまたは問題に対するカスタムステータス

タスクまたはイシューを別のプロジェクトに移動またはコピーすると、タスクまたはイシューの一部のステータスが、移動先のプロジェクトのグループで使用されているステータスに合わせて更新される場合があります。 これは、そのグループに同じキーを持つステータスが存在するかどうかによって異なります。

* タスクまたはイシューのステータスが、タスクまたはイシューのステータスと同じキーを持つ場合、タスクまたはイシューのステータスは同じままです。

   これら 2 つのステータスのラベルが一致しない場合、タスクまたは問題のステータスは、宛先プロジェクトのグループで使用されているステータスのラベルを継承します。

* タスクまたはイシューのステータスが、ターゲットプロジェクトのグループの同等のステータスと同じキーを持たない場合、タスクまたはイシューのステータスは、ターゲットプロジェクトのグループの同等の既定のステータスに変わります。

ステータスキーについて詳しくは、 [グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
