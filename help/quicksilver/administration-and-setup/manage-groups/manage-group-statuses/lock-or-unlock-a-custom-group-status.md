---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: ロック済みおよびロック解除されたグループステータス
description: グループのカスタムステータスをロックすると、グループ内のユーザーとそのサブグループが作業のフローで同じプロセスを使用できます。 グループステータスがロックされると、グループ内および下位グループのすべてのユーザーがそのステータスを使用できます。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
TQID: https://experienceleague.adobe.com/WmHq8Aycq-cMfOt6ZnLF0MpNbtLPM5NhVylrsw9hHKE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 286
ht-degree: 98%

---

# ロックおよびロック解除されたグループステータス

グループのカスタムステータスをロックすると、グループ内のユーザーとそのサブグループが作業のフローで同じプロセスを使用できます。 グループステータスがロックされると、グループ内および下位グループのすべてのユーザーがそのステータスを使用できます。 ユーザー（または Workfront 管理者）は、ロックしたステータスを編集または削除できますが、下のサブグループの管理者は、それらのグループに対して編集または削除を行うことができません。変更できるのは、ステータスリスト内の表示順序のみです。

逆に、グループのカスタムステータスをロック解除すると、下位サブグループの管理者は、グループで使用する固有のワークフローをより柔軟に管理できます。 グループのステータスがロック解除されると、下位のサブグループの管理者は、そのサブグループの属性を変更したり削除したりできます。

>[!IMPORTANT]
>
>一定期間ロックを解除した後でカスタムステータスをロックすると、ステータスの設定は、下位のサブグループのグループ管理者が行った設定を置き換えます。 ステータスがロックされている間、管理者は自分のグループのステータスを変更または削除できません。

グループステータスのロックまたはロック解除の手順については、[グループのステータスを作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。

グループ承認プロセスでは、ロック済みステータスとロック解除済みステータスの両方を使用できます。 ロックが解除されたグループステータスでグループ承認プロセスを作成すると、ユーザーはグループに関連付けられている任意のプロジェクト、タスク、またはイシューに承認プロセスを添付できます。

