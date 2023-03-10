---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: ロックおよびロック解除されたグループステータス
description: グループのカスタムステータスをロックすると、グループ内のユーザーとそのサブグループが作業の流れで同じプロセスを使用するようになります。 グループステータスがロックされると、グループ内および下位グループのすべてのユーザーがグループステータスを使用できます。 自分 ( またはWorkfrontの管理者 ) は、ロックしたステータスを編集または削除できますが、下のサブグループの管理者は、これらのグループに対しては編集できません。 逆に、グループのカスタムステータスをロック解除すると、下位サブグループの管理者は、ワークフローを柔軟に管理できます。 ロック解除済みのステータスの属性を変更したり、グループから削除したりできます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3463e4cb-7336-49b7-b81a-c2acef72f61d
source-git-commit: d67de32fcbe4706cf8a1fc6f5bb8ec9d08b07119
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# ロックおよびロック解除されたグループステータス

グループのカスタムステータスをロックすると、グループ内のユーザーとそのサブグループが作業の流れで同じプロセスを使用するようになります。 グループステータスがロックされると、グループ内および下位グループのすべてのユーザーがグループステータスを使用できます。 自分 ( またはWorkfront管理者 ) は、ロックしたステータスを編集または削除できますが、下のサブグループの管理者は、これらのグループに対しては編集できません。ステータスリストでの表示順のみを変更できます。

逆に、グループのカスタムステータスをロック解除すると、下位サブグループの管理者は、グループで使用する一意のワークフローを柔軟に管理できます。 グループのステータスがロック解除されると、下位サブグループの管理者は、その属性を変更したり、それらのサブグループの属性を削除したりできます。

>[!IMPORTANT]
>
>ロック解除後にカスタムステータスをロックすると、下位のサブグループのグループ管理者が行ったステータスの設定が置き換えられます。 ステータスがロックされている間、管理者は自分のグループのステータスを変更または削除できません。

グループステータスのロックまたはロック解除の手順については、 [グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

グループ承認プロセスでは、ロック済みステータスとロック解除済みステータスの両方を使用できます。 ロックが解除されたグループステータスでグループ承認プロセスを作成した場合、ユーザーは、そのグループに関連付けられているプロジェクト、タスクまたはイシューに承認プロセスを添付できます。

