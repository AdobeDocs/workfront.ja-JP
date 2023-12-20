---
title: グループ管理者
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: 多くの部門を持つ大規模な組織のAdobe Workfront管理者は、組織のすべての部門とグループをそれらの部門内で管理したくない場合があります。 代わりに、グループ管理者が管理する各部門とグループのグループを作成できます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 850e0801511177efc5189258acd9b88234cf59c9
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# グループ管理者

<!-- Audited: 12/2023 -->

多くの部門を持つ大規模な組織のAdobe Workfront管理者は、組織のすべての部門とグループをそれらの部門内で管理したくない場合があります。 代わりに、グループ管理者が管理する各部門とグループのグループを作成できます。

グループ管理者は、ユーザーのメンバーシップ、レイアウトテンプレート、カスタムデータ、ステータス、環境設定など、グループのニーズを管理できます。

1 つのグループの下に、最大 14 レベルのサブグループを配置できます。

>[!NOTE]
>
>サブグループの上の階層のグループ管理者は、すべて、そのサブグループを管理する管理権限を持っています。

グループの作成と管理について詳しくは、 [グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) および [グループの管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). また、 [サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## グループ管理者の指定

すべての最上位グループには、少なくとも 1 人のグループ管理者が必要です。 グループのWorkfront管理者または管理者は、グループのサブグループにグループ管理者を割り当てることができますが、これは必須ではありません。 詳しくは、 [グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Workfront管理者の場合は、ユーザーをグループ管理者に指定する前に、次の操作をおこなうことをお勧めします。

* システム内のWorkfront管理者の現在の数をメモしておきます。
* システム内に存在するグループの数をメモしておきます。
* 一部のWorkfront管理者のアクセスレベルを変更できるかどうかを決定し、代わりにグループ管理者として指定します。

  グループ管理者の機能について詳しくは、 [グループ管理者がおこなったタスク](#tasks-done-by-group-administrators) 」を参照してください。

* グループ管理者が他のユーザーとしてログインできるようにするか、管理しているグループ内のユーザーのパスワードをリセットするかを指定します。 これらのタスクを実行するには、次に示すように、追加のアクセス権が必要です。 [グループ管理者に必要なアクセス](#access-needed-for-group-administrators).
* ユーザー管理を改善するには、次のオブジェクトにユーザーではなくグループまたはサブグループを割り当てることを検討します。

   * レイアウトテンプレート
   * スケジュール
   * 定期タイムシート

## グループ管理者に必要なアクセス {#access-needed-for-group-administrators}

グループ管理者は全員、

* 現在の価格とパッケージングモデルのプランライセンス
* 新しい価格とパッケージモデルの標準ライセンス

グループ管理者は、次のタスクを実行できるように、ユーザーに対して編集アクセス権を持つことをお勧めします。

* 管理するグループとサブグループの他のユーザーとしてログインします。
* 管理対象のグループ内の別のユーザーのパスワードをリセットします。

>[!IMPORTANT]
>
>グループ管理者は、管理しているグループ管理者より高いアクセス権を持つ必要があります。そうしないと、低いアクセスレベルを表示または変更できなくなります。
>このアクセス権の付与手順については、 [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

グループとサブグループ内のユーザーにタイムシートプロファイルを割り当てる必要があるグループ管理者の場合は、タイムシートと時間に対する管理アクセス権もお勧めします。 このアクセス権の付与手順については、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## グループ管理者がおこなったタスク {#tasks-done-by-group-administrators}

グループ管理者は、以下に説明するタスクを実行して、管理対象のグループを管理できます。 これらの中には、Workfront管理者が提供する機能と同じものもあります。

>[!NOTE]
>
>新しい価格とパッケージのモデルでは、次の操作を実行するには、Prime プラン以上が必要です。
>
> * グループイベント通知の作成
> * グループプロジェクトの環境設定
> * グループタスクと問題の環境設定を設定
> * サブグループ環境設定の設定をロック解除
> * タイムシートと時間の基本設定をグループ化
> * タイムシートと時間の優先設定をロック解除

### グループメンバーの管理 {#manage-group-members}

* 管理するグループとサブグループ内のサブグループを作成、編集、削除します。 手順については、 [サブグループの作成](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* 編集アクセス権を持つユーザーをグループとサブグループに追加します。 また、ユーザーのプロファイルを編集して、グループとサブグループにユーザーを追加することもできます。

  また、アクセスレベルでユーザー管理者（グループユーザー）権限が有効になっている場合は、グループメンバーのプロファイルのフィールドを更新することもできます。

  詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Workfront管理者は、グループ管理者がおこなったグループメンバーシップの変更を上書きできます。

* 管理するグループのメンバーであるユーザーのパスワードをリセットします。 詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* 管理するグループのメンバーであるユーザーとしてログインします。 詳しくは、 [別のユーザーとしてログイン](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* グループとその下のサブグループで使用可能なライセンスの数を表示します。 詳しくは、 [システムで使用可能なライセンスを管理](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### グループオブジェクトの管理 {#manage-group-objects}

* グループレベルのレイアウトテンプレートを作成し、管理するグループとサブグループに関連付けます。 詳しくは、 [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* グループレベルのタイムシートプロファイルを作成し、管理するユーザーとグループに関連付け、タイムシートを手動で生成します。 詳しくは、 [タイムシートプロファイルの作成、編集、割り当て](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* 承認プロセスに対する管理アクセス権がない場合は、管理するグループとサブグループの承認プロセスを作成および編集します。 詳しくは、 [作業項目の承認プロセスの作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  承認プロセスへの管理者アクセスについて詳しくは、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* スケジュールを作成し、管理するグループに関連付けます。 詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* 管理するグループに割り当てられているチームを、チームのメンバーではなく管理します。 また、「グループ」フィールドに基づいてチームレポートを作成し、特定のチームが割り当てられているグループを特定します。 詳しくは、 [チームの作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* 管理するグループに関連付けられたプロジェクトを、そのプロジェクトに関連付けられたタスク、問題、ドキュメントと共に復元します。 詳しくは、 [削除した項目を復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### グループの環境設定とツールの管理 {#manage-group-preferences-and-tools}

* システム全体のグループに対して、プロジェクトの優先順位、タスクの優先順位、またはタイムシートと時間の優先順位がロック解除されている場合は、管理するグループの優先順位を編集します。 これらの環境設定は、プロジェクト、タスクおよび問題の動作に影響を与えます。 詳しくは、次を参照してください。

   * [グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [グループのタスクと問題の環境設定を設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* 管理するグループのグループステータスを作成および編集します。 詳しくは、 [グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* 管理するグループに対してイベント通知を設定します。 これをおこなうには、Workfront管理者が、システムを介してグループのイベント通知を設定する機能をロック解除した後に限り、おこなえます。 詳しくは、 [グループのイベント通知を表示および設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
