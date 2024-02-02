---
title: ホームグループの概要
user-type: administrator
product-area: system-administration;user-management
navigation-topic: groups-overview
description: ユーザーのプロファイルではホームグループが割り当てられています。すべてのユーザーにはホームグループが必要です。1 人のユーザーは複数のグループに属することができますが、ホームグループは1 つのみ持つことができます。システム内の既存のグループをユーザーのホームグループとして割り当てることもできますが、より大きな組織単位を表す新しいグループを作成して割り当てることをお勧めします。ホームグループを確立する際は、組織が Adobe Workfront ユーザーをどのように分割するかを検討します。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 89adb9ea-bfde-4c0d-9fec-b1f97e925340
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '390'
ht-degree: 100%

---

# ホームグループの概要

ユーザーのプロファイルではホームグループが割り当てられています。すべてのユーザーにはホームグループが必要です。1 人のユーザーは複数のグループに属することができますが、ホームグループは1 つのみ持つことができます。グループの詳細情報については、[グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md)を参照してください。

システム内の既存のグループをユーザーのホームグループとして割り当てることもできますが、より大きな組織単位を表す新しいグループを作成して割り当てることをお勧めします。

ホームグループを確立する際は、組織が Adobe Workfront ユーザーをどのように分割するかを検討します。ホームグループとして使用するグループのタイプを決定する際の推奨事項を次に示します。

* IT やマーケティングなどの部門を表すグループ
* 異なる予算で管理されるグループ
* 異なる地域や地域に位置するグループ
* 同じコストセンターに属する複数のチームで構成されるグループ

>[!NOTE]
>
>ホームグループを組織単位に再編成する必要がある場合は、次の手順を実行する必要があります。
>1. 新しいグループを作成します（[グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)を参照）。
>1. 新しいグループをユーザーのホームグループとして再割り当てします（[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)参照）。
>

## レイアウトテンプレート管理

レイアウトテンプレートをグループに割り当てると、そのグループをホームグループに割り当てているすべてのユーザは、レイアウトテンプレートで指定した設定を表示できます。

レイアウトテンプレートがホームグループに割り当てられている場合、そのホームグループに割り当てられているユーザーにのみ表示されます。

詳細情報については、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)の[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

## ライセンス管理

各ユーザーに割り当てられるホームグループは 1 つだけです。これにより、ライセンス数の管理が容易になります。

Workfront の管理者は、ホームグループの最大ライセンス数を設定することができます。

Workfront 管理者は、最大ライセンス数を設定することで、ビジネス部門が他のビジネス部門用に購入した Workfront ライセンスを使用するのを防ぐことができます。

詳細情報については、[システムで使用可能なライセンスの管理](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)を参照してください。
