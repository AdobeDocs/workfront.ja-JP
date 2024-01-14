---
title: グループの概要
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Workfront管理者は、部門の構造と一致するユーザーのグループを作成できます。 グループは、チームや会社に似ていますが、異なります。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: 9c4aa8d1f812299ba6cdcb664b990c1119e3cb31
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 0%

---

# グループの概要

Workfront管理者は、部門の構造と一致するユーザーのグループを作成できます。 グループは、チームや会社に似ていますが、異なります。

Workfrontの管理者は、作業および通信が必要なWorkfront領域へのアクセス権をグループに付与します。 その後、各グループは、ユーザー、テンプレート、カスタムフォームなどのWorkfrontの情報や、プロジェクトを他の部門の情報とは別に保持できます。

グループごとに少なくとも 1 人のグループ管理者が必要です。 グループ管理者は、グループページを使用して、自分のグループを 1 か所で管理できます。 詳しくは、 [グループ管理者](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

1 つのグループの下に、最大 14 レベルのサブグループを作成できます。 詳しくは、 [サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) および [サブグループの作成](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## グループを使用したユーザーの整理

Workfrontの管理者またはグループ管理者は、ユーザーをグループおよびサブグループに関連付けることができます。 グループを公開する場合、Planner ライセンスを持つユーザーは、そのグループにユーザーを関連付けることができます。 グループ管理者とパブリックグループについて詳しくは、 [グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

ユーザーを作成する場合は、そのユーザーを適切なホームグループと、そのユーザーが作業する必要のあるその他のグループに追加することをお勧めします。 1 人のユーザーが持つことのできるホームグループは 1 つだけですが、他の複数のグループに属することもできます。

グループの一部であれば、グループとサブグループと共有されるオブジェクトにユーザーがアクセスできます。 たとえば、プロジェクトをグループと共有する場合、グループ内のユーザーとグループ内のサブグループにアクセスできます。

>[!TIP]
>
>組織内の部門が共同でプロジェクトとそれらのプロジェクト上のリソースを管理する場合は、部門を多数の小さなグループに分ける必要がない場合があります。 いくつかの高レベルグループが最も効果的な場合があります。

1 つのグループに設定できるユーザーの数に制限はありません。

新しいユーザーの作成について詳しくは、 [ユーザーを追加](../../../administration-and-setup/add-users/add-users.md).

## オブジェクトに対するグループアクセスの許可

オブジェクトをグループと共有すると、そのグループのすべてのメンバー（サブグループのメンバーを含む）がそのオブジェクトにアクセスできます。 Workfrontでの共有について詳しくは、 [オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## グループとオブジェクトの関連付け

次のWorkfrontオブジェクトの 1 つを作成または編集する際に、そのオブジェクトをグループに関連付けることができます。

* **プロジェクト**：プロジェクトの所有権を示すために、1 つのグループをプロジェクトに関連付けることができます。

  これにより、グループの各メンバーに対する権限が暗黙的に付与されるわけではありません。 プロジェクトユーザーに対する権限を付与するには、プロジェクトがユーザーと共有されている必要があります。

  ユーザーは複数のグループのメンバーになることができますが、プロジェクトには 1 つのグループを関連付けることができます。 プロジェクトが他のグループと共有されている場合でも、他のグループのユーザーは同じプロジェクトで作業できます。 通常、プロジェクトに関連付けられるグループは、プロジェクトの完了を担当するグループか、プロジェクトが配信されるグループのどちらかです。

  プロジェクトをグループに関連付ける手順については、 [プロジェクトの概要領域で情報を管理します。](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio、プログラムまたは会社**：ポートフォリオ、プログラムまたは会社を作成または編集する際に、ポートフォリオに 1 つのグループを割り当てて、そのグループがそのポートフォリオを所有しているか、そのグループが責任を持っていることを示すことができます。 この関連付けを行うと、管理者やユーザーは、どのポートフォリオ、プログラム、会社が作業しているかを簡単に識別できます。

  例えば、グループ管理者は、リストまたはレポートを使用して組織内のすべてのポートフォリオをリストし、「グループ」列にそのポートフォリオに割り当てられたポートフォリオをメモすることができます。

  >[!NOTE]
  >
  >グループを持つポートフォリオ、プログラム、または会社にグループを割り当てても、そのグループ内の情報が自動的にそのデータにアクセスできるとは限りません。 データへのアクセスを表示する前に、手動でグループとデータへのアクセスを共有する必要があります。

  手順については、 [ポートフォリオの作成](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [プログラムの作成](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)、および [会社の作成と編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **承認プロセス**：承認プロセスを、特定のグループに属するプロジェクト、タスクおよび問題で使用できるようにします。 詳しくは、 [作業項目の承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **マイルストーンのパス**：特定のグループのユーザーが、プロジェクトでマイルストーンパスを使用できるようにします。 詳しくは、 [マイルストーンパスを作成する](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **レイアウトテンプレート**：グループの管理者に、レイアウトテンプレートを変更する権限を付与できます。 手順については、 [レイアウトテンプレートの管理アクセス権の付与](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **タイムシートプロファイル**：タイムシートプロファイルを変更するグループの管理者権限を付与できます。 詳しくは、 [タイムシートプロファイルの作成、編集、割り当て](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **スケジュール**：グループの管理者に、スケジュールを変更する権限を付与できます。 詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **チーム**：グループとチームを関連付けて、グループおよびそのサブグループの管理者がグループ領域でこれらのチームを表示および操作できるようにします。 詳しくは、 [チームの作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) または [チーム設定を編集](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **テンプレート**：プロジェクトテンプレートにグループを割り当てることができます。 これにより、プロジェクト作成プロセスを合理化し、どのグループがどのプロジェクトテンプレートを所有しているかをより簡単に特定してレポートできるようになります。 詳しくは、 [概要](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) 記事内 [プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **最近削除および復元された項目**：最近削除されたグループの項目を表示および管理できます。 詳しくは、 [グループの最近削除された項目の表示と管理](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) および [グループの最近復元された項目の表示と管理](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
