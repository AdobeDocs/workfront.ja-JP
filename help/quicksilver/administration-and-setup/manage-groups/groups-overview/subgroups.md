---
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
title: サブグループの概要
description: 1 つのグループの下に、最大 14 レベルのサブグループを作成できます。 これらのレベルのいずれかで、並列サブグループを無制限に作成できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a4280498-6719-4911-a69a-b715a5438eed
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# サブグループの概要

1 つのグループの下に、最大 14 レベルのサブグループを作成できます。 これらのレベルのいずれかで、並列サブグループを無制限に作成できます。 手順については、 [サブグループの作成](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

グループについて詳しくは、 [グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## サブグループは何を継承しますか？

サブグループは親グループのメンバーシップを継承します。 したがって、サブグループ内のユーザーとグループは、共有する親グループに属するユーザーとグループと同じ可視性、権限、およびすべてのオブジェクトへのアクセス権を持ちます。

また、サブグループは最上位グループのグループ管理者を自動的に継承しますが、グループ管理者としての役割を果たすために、サブグループのメンバーを割り当てることもできます。

>[!TIP]
>
>サブグループを使用して既存のグループに複数のユーザーを追加し、必要なオブジェクトへのアクセス権を付与する場合もあります。
>
>たとえば、ヘルプデスクの技術者グループと IT ディレクターグループが別々にいるとします。 ヘルプデスクグループは、特定のリクエストキューに対する権限を持っています。 IT ディレクターをヘルプデスクグループに追加し、リクエストキューに対する権限も持たせたい。 サブグループ機能がない場合は、IT ディレクターをヘルプデスクグループに手動で追加する必要があり、非効率で管理が困難な可能性があります。 IT ディレクターグループをサブグループとしてヘルプデスクグループに追加すると、1 回の変更でこのタスクをより迅速に実行できます。

>[!NOTE]
>
>ユーザがサブグループと親グループの両方に個別に追加された場合、一方からユーザを削除しても、他方からはユーザを削除しません。 ユーザーが親グループに対するアクセスを許可されないようにするには、サブグループと親グループの両方からユーザーを削除する必要があります。

## パブリックおよびプライベートサブグループ

公開グループの場合、編集ユーザーアクセス権を持つ（グループ内またはグループ外の）ユーザーは、他のユーザーのプロファイルにグループを追加できます。 これは、プライベートグループに対しては実行できません。

このオプションは、複数のレベルを持つグループの階層の上位の親グループでのみ編集できます。 親グループのすべてのサブグループが設定を継承します。

パブリックなグループの下にサブグループを作成した場合、そのサブグループもデフォルトでパブリックになります。 グループの作成と公開について詳しくは、 [グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). ユーザーの編集に必要なアクセスについて詳しくは、 [ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

既存のグループに追加したグループは、自動的にサブグループになり、メイングループになりません。 ただし、サブグループは、既存のユーザーと、新しい親グループに属するすべてのプロジェクト、タスクおよび問題ステータスに加えて、プロジェクト、問題、タスクに関連付けられたすべてのユーザーを保持します。

## サブグループのグループ管理者

<!--
Group Admins of a subgroup can't manage statuses or project preferences of the subgroup YET (Sprint 22/Oct 28, 2020)</p>
-->

サブグループの作成時や編集時に、サブグループのメンバーをグループ管理者としてサブグループに割り当てることができます。 手順については、 [](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create) 記事内 [グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

または、サブグループの管理を、その上のグループに割り当てられているグループ管理者に任せることもできます。 サブグループを作成すると、上のグループの管理者は、そのサブグループを自動的に管理する権限を持ちます。

>[!NOTE]
>
>ユーザをサブグループに追加し、そのユーザがサブグループの上の任意のグループのグループ管理者である場合、そのユーザは、そのサブグループのグループ管理者として割り当てられていなくても、そのサブグループを管理する管理権限を持ちます。

Workfrontシステムを管理するAdobe Workfront管理者、トップレベルグループを管理するグループ管理者、サブグループを管理するグループ管理者が使用できるアクションについては、 [様々なタイプの管理者に許可されるアクション](../../../administration-and-setup/manage-groups/group-roles/group-actions-allowed-different-types-admins.md).
