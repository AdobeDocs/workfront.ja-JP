---
title: グループの概要
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: Workfront 管理者は、部門の構造と一致するユーザーのグループを作成できます。グループは、チームや会社に似ていますが、異なります。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: b5e0a590d258df4510a0bb6a44b57099f32ae6b9
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 92%

---

# グループの概要

<!-- Audited: 01/2024 -->

Workfront 管理者は、部門の構造と一致するユーザーのグループを作成できます。グループは、チームや会社に似ていますが、異なります。

Workfront 管理者は、作業およびコミュニケーションが必要な Workfront エリアへのアクセス権をグループに付与します。各グループは、ユーザー、テンプレート、カスタムフォームなどの Workfront の情報やプロジェクトを他の部門のものと分けて別に管理できます。

グループごとに 1 人以上のグループ管理者が必要です。グループ管理者は、グループページを使用して、自分のグループを 1 か所で管理できます。詳しくは、[グループ管理者](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)を参照してください。

1 つのグループの下に、最大 14 レベルのサブグループを作成できます。詳しくは、[サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)および[サブグループの作成](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)を参照してください。

## グループを使用したユーザーの整理

Workfrontの管理者またはグループ管理者は、ユーザーをグループおよびサブグループに関連付けることができます。 グループを公開する場合、標準（新規）またはプラン（現在）のライセンスを持つユーザーは、そのグループにユーザーを関連付けることができます。 グループ管理者とパブリックグループについて詳しくは、[グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)を参照してください。

ユーザーを作成する場合は、そのユーザーを適切なホームグループと、そのユーザーが作業する必要のあるその他のグループに追加することをお勧めします。1 人のユーザーが持つことのできるホームグループは 1 つだけですが、他の複数のグループに属することもできます。

グループの一員であるユーザーは、そのグループおよびサブグループと共有されるオブジェクトにアクセスできます。例えば、プロジェクトをグループと共有する場合、グループ内のユーザーとグループ内のサブグループにアクセスできます。

>[!TIP]
>
>組織内の部門が共同でプロジェクトを管理し、それらのプロジェクト上のリソースを管理する場合は、部門を多数の小さなグループに分ける必要がない場合があります。少数の高レベルグループが最も効果的な場合があります。

1 つのグループに対してユーザーの数に制限はありません。

新規ユーザーの作成について詳しくは、[ユーザーを追加](../../../administration-and-setup/add-users/add-users.md)を参照してください。

## オブジェクトに対するグループアクセスの許可

オブジェクトをグループと共有する場合、そのグループのすべてのメンバー（サブグループのメンバーを含む）がそのオブジェクトにアクセスできます。Workfront での共有について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

## グループとオブジェクトの関連付け

次の Workfront オブジェクトの 1 つを作成または編集する場合、そのオブジェクトをグループに関連付けることができます。

* **プロジェクト**：プロジェクトの所有権を示すために、1 つのグループをプロジェクトに関連付けることができます。

  これにより、グループの各メンバーに対して権限が暗黙的に付与されるわけではありません。プロジェクトユーザーに対する権限を付与するには、プロジェクトがユーザーと共有されている必要があります。

  ユーザーは複数のグループのメンバーになることができますが、プロジェクトに関連付けられるグループは 1 つです。プロジェクトが他のグループと共有されている場合でも、他のグループのユーザーは同じプロジェクトで作業できます。 通常、プロジェクトに関連付けられるグループは、プロジェクト完了を担当するグループか、完了したプロジェクトを引き渡されるグループのどちらかです。

  プロジェクトをグループに関連付ける手順について詳しくは、[プロジェクトの概要エリアで情報を管理](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)を参照してください。

* **ポートフォリオ、プログラムまたは会社**：ポートフォリオ、プログラムまたは会社を作成または編集する場合、ポートフォリオに 1 つのグループを割り当てて、そのグループがそのポートフォリオを所有しているか、そのグループが担当することを示すことができます。この関連付けを行うと、管理者やユーザーは、どのポートフォリオ、プログラムおよび会社が作業しているかを簡単に識別できます。

  例えば、グループ管理者は、リストまたはレポートを使用して組織内のすべてのポートフォリオをリストし、グループ列にそのポートフォリオに割り当てられたポートフォリオをメモすることができます。

  >[!NOTE]
  >
  >グループを持つポートフォリオ、プログラムまたは会社にグループを割り当てても、そのグループ内の情報が自動的にそのデータにアクセスできるとは限りません。データの表示を許可するには、手動でグループとデータへのアクセスを共有する必要があります。

  手順については、[ポートフォリオの作成](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)、[プログラムの作成](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)および [会社の作成と編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)を参照してください。

* **承認プロセス**：承認プロセスを、特定のグループに属するプロジェクト、タスクおよびイシューで使用できるようにします。詳しくは、[作業アイテムの承認プロセスを作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)を参照してください。
* **マイルストーンパス**：特定のグループのユーザーが、プロジェクトでマイルストーンパスを使用できるようにします。詳しくは、[マイルストーンパスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md)を参照してください。
* **レイアウトテンプレート**：レイアウトテンプレートを変更するグループの管理者権限を付与できます。手順について詳しくは、[レイアウトテンプレートの管理アクセス権を付与](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)を参照してください。

* **タイムシートプロファイル**：タイムシートプロファイルを変更するグループの管理者権限を付与できます。詳しくは、[タイムシートプロファイルの作成、編集および割り当て](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

* **スケジュール**：スケジュールを変更するグループの管理者権限を付与できます。詳しくは、[スケジュールを作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。
* **チーム**：グループとチームを関連付けて、グループおよびそのサブグループの管理者がグループエリアでこれらのチームを表示および共同に作業できるようにします。詳しくは、[チームを作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)または[チーム設定を編集](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)を参照してください。
* **テンプレート**：プロジェクトテンプレートにグループを割り当てることができます。これにより、プロジェクト作成プロセスを合理化し、どのグループがどのプロジェクトテンプレートを所有しているかをより簡単に特定してレポートできるようになります。詳しくは、[プロジェクトテンプレートを編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)の記事にある、[概要](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview)の節を参照してください。

* **最近削除および復元された項目**：最近削除されたグループの項目を表示および管理できます。詳しくは、[グループの最近削除された項目の表示と管理](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md)および[グループの最近復元された項目の表示と管理](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md)を参照してください。
