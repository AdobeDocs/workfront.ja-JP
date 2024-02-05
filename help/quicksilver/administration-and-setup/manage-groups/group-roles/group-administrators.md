---
title: グループ管理者
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: 多くの部門がある大規模な組織の Adobe Workfront 管理者は、組織のすべての部門と部門内のすべてのグループを管理するのが困難な場合があります。そのような場合は、すべての部門とグループを管理する代わりに部門ごとのグループを作成し、そのグループ内にサブグループを作成し、それぞれをグループ管理者が管理できるようにします。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 850e0801511177efc5189258acd9b88234cf59c9
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 90%

---

# グループ管理者

<!-- Audited: 12/2023 -->

多くの部門がある大規模な組織の Adobe Workfront 管理者は、組織のすべての部門と部門内のすべてのグループを管理するのが困難な場合があります。そのような場合は、すべての部門とグループを管理する代わりに部門ごとのグループを作成し、そのグループ内にサブグループを作成し、それぞれをグループ管理者が管理できるようにします。

グループ管理者は、ユーザーのメンバーシップ、レイアウトテンプレート、カスタムデータ、ステータス、環境設定などのグループのニーズを管理できます。

1 つのグループの下に、最大 14 レベルのサブグループを作成できます。

>[!NOTE]
>
>サブグループより上の階層にあるすべてのグループ管理者は、そのサブグループを管理する管理者権限を持ちます。

グループの作成と管理について詳しくは、[グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)および[グループの管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md)を参照してください。また、[サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)も参照してください。

## グループ管理者の指定

すべての最上位のグループには、少なくとも 1 人のグループ管理者が必要です。Workfront 管理者またはグループの管理者は、グループのサブグループにグループ管理者を割り当てることができますが、これは必須ではありません。詳しくは、[グループを作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)を参照してください。

Workfront 管理者の場合は、ユーザーをグループ管理者に指定する前に、次の操作を行うことをお勧めします。

* システム内の現在の Workfront 管理者の数をメモしておきます。
* システム内に存在するグループの数をメモしておきます。
* 一部の Workfront 管理者のアクセスレベルを変更し、代わりにグループ管理者として指定できるかどうかを判断します。

  グループ管理者の機能について詳しくは、 [グループ管理者がおこなったタスク](#tasks-done-by-group-administrators) 」を参照してください。

* グループ管理者が他のユーザーとしてログインできるようにするか、管理するグループ内のユーザーのパスワードをリセットできるようにするかを指定します。これらのタスクを実行するには、次に示すように、追加のアクセス権が必要です。 [グループ管理者に必要なアクセス](#access-needed-for-group-administrators).
* ユーザー管理を改善するには、ユーザーの代わりにグループまたはサブグループを次のオブジェクトに割り当てることを検討してください。

   * レイアウトテンプレート
   * スケジュール
   * 定期タイムシート

## グループ管理者に必要なアクセス {#access-needed-for-group-administrators}

グループ管理者は全員、

* 現在の価格とパッケージングモデルのプランライセンス
* 新しい価格とパッケージモデルの標準ライセンス

ユーザーが次のタスクを実行できるように、グループ管理者にはユーザーに対する編集アクセス権を付与することをお勧めします。

* 管理対象のグループおよびサブグループの他のユーザーとしてログインします。
* 管理対象のグループ内の別のユーザーのパスワードをリセットします。

>[!IMPORTANT]
>
>グループ管理者は、管理対象のグループ管理者より高いアクセス権を持つ必要があります。そうでない場合、下位のアクセスレベルを表示または変更できなくなります。
>このアクセス権を付与する手順については、[カスタムアクセスレベルを作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

グループおよびサブグループのユーザーに定期タイムシートを割り当てる必要があるグループ管理者には、タイムシートと時間に対する管理アクセス権も付与しておくことをお勧めします。このアクセス権を付与する手順については、[特定のエリアに対する管理者アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

## グループ管理者が実行するタスク {#tasks-done-by-group-administrators}

グループ管理者は、以下に説明するタスクを実行して、管理対象のグループを管理できます。 タスクの一部は、Workfront 管理者に提供されている機能と同じです。

>[!NOTE]
>
>新しい価格とパッケージのモデルでは、次の操作を実行するには、Prime プラン以上が必要です。
>
> * グループイベント通知の作成
> * グループプロジェクトの環境設定の指定
> * グループタスクとイシューの環境設定の指定
> * サブグループ環境設定のロック解除
> * グループのタイムシートおよび時間環境設定
> * タイムシートと時間の環境設定のロック解除

### グループメンバーを管理 {#manage-group-members}

* 管理対象のグループおよびサブグループでサブグループを作成、編集、削除します。手順については、[サブグループを作成](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)を参照してください。
* 編集アクセス権を持つユーザーをグループおよびサブグループに追加します。または、ユーザーのプロファイルを編集して、グループおよびサブグループにユーザーを追加します。

  アクセスレベルでユーザー管理者（グループユーザー）権限が有効になっている場合は、グループメンバーのプロファイルのフィールドを更新することもできます。

  詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

  >[!NOTE]
  >
  >Workfront 管理者は、グループ管理者が行ったグループメンバーシップの変更を上書きできます。

* 管理対象のグループのメンバーであるユーザーのパスワードをリセットします。詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。
* 管理対象のグループのメンバーであるユーザーとしてログインします。詳しくは、[別のユーザーとしてログイン](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md)を参照してください。
* グループとその下のサブグループで使用可能なライセンス数を表示します。詳しくは、[システムで使用可能なライセンスを管理](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)を参照してください。

### グループオブジェクトを管理 {#manage-group-objects}

* グループレベルのレイアウトテンプレートを作成し、管理するグループとサブグループに関連付けます。詳しくは、[レイアウトテンプレートを作成および管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。
* グループレベルのタイムシートプロファイルを作成し、管理するユーザーおよびグループに関連付けて、タイムシートを手動で生成します。詳しくは、[タイムシートプロファイルを作成、編集および割り当て](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。
* 承認プロセスに対する管理アクセス権がない場合は、管理するグループとサブグループの承認プロセスを作成および編集します。詳しくは、[作業アイテムの承認プロセスを作成](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)を参照してください。

  承認プロセスへの管理者アクセス権について詳しくは、[特定のエリアに対する管理者アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

* スケジュールを作成し、管理するグループに関連付けます。詳しくは、[スケジュールを作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。
* 自分が管理するグループに割り当てられたチームを、そのチームのメンバーにはならずに、管理します。また、グループフィールドに基づいてチームレポートを作成し、特定のチームが割り当てられているグループを識別します。詳しくは、[チームを作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)を参照してください。
* 管理するグループに関連付けられているプロジェクトを、プロジェクトに関連付けられているタスク、イシューまたはドキュメントと共に復元します。詳しくは、[削除された項目を復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。

### グループの環境設定とツールを管理 {#manage-group-preferences-and-tools}

* プロジェクトの環境設定、タスクまたはイシューの環境設定、またはタイムシートと時間の環境設定がシステム全体のグループに対してロック解除されている場合は、管理するグループに対してその環境設定を編集します。これらの環境設定は、プロジェクト、タスクおよびイシューの動作に影響を与えます。詳しくは、以下を参照してください。

   * [グループのプロジェクト環境設定を指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [グループのタスクとイシューの環境設定を行う](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* 管理するグループのグループステータスを作成および編集します。詳しくは、[グループステータスを作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。
* 管理するグループに対してイベント通知を設定します。これは、Workfront 管理者がシステム全体でグループのイベント通知を設定する機能のロックを解除した後のみに、実行できます。詳しくは、[グループのイベント通知を表示および設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)を参照してください。
