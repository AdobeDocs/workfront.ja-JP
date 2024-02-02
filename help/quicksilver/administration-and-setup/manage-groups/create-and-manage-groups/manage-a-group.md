---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理, グループ化, 編集,
navigation-topic: create-and-manage-groups
title: グループの管理
description: グループ管理者は、「設定」の「グループ」エリアで、管理対象のグループを管理できます。管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: ht
source-wordcount: '1321'
ht-degree: 100%

---

# グループの管理

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

グループ管理者は、「設定」の「グループ」エリアで、管理対象のグループを管理できます。管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>グループの管理者として割り当てられた場合、そのグループの下にあるすべてのサブグループのグループ管理者の役割を継承します。サブグループを管理できるユーザーは、その上位グループのグループ管理者と、そのサブグループに割り当てられているグループ管理者のみです。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプランまたはライセンスタイプを確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## グループのメンバーシップの管理

管理しているグループに対して、ユーザーや他のグループを追加したり、削除したりできます。また、グループメンバーをグループの管理者として割り当てたり、グループメンバーのユーザープロファイル情報を管理したりすることもできます。

手順については、[グループのメンバーシップの表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md)を参照してください。

## グループの詳細の管理

管理対象のグループまたはサブグループについて、グループの詳細ページを表示して編集することができます。このページには、グループの説明、ビジネスリーダーとグループ管理者の名前、およびグループとそのすべてのサブグループを公開または非公開にするオプションが含まれます。また、カスタムフォームを管理できるアクセスレベルの場合は、カスタムフォームをグループに添付できます。

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

手順については、[グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)を参照してください。

## グループの編集、コピー、削除

表示しているグループのメインページから離れずに、グループをすばやく編集、コピー、削除できます

<!--
DRAFTED IN FLARE:
or deactivate

-->

。

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. 「**グループ**」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. グループを選択し、編集 ![](assets/edit-icon.png)、コピー ![](assets/copy-icon.png)、または削除 ![](assets/delete.png) のアイコンをクリックします。

   表示されるボックスの使用に関する情報が必要な場合は、次のいずれかを参照してください。

   * **編集**：[グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **コピー**：[グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)記事の[既存のグループまたはサブグループをコピーしてトップレベルグループを作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group)を参照してください。

   * **削除**：[グループの削除](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## グループのプロジェクト、タスクおよびイシューの環境設定の指定

システムレベルで設定された設定とは異なるプロジェクト、タスク、イシューの環境設定が必要なグループのグループ管理者は、Workfront 管理者に問い合わせて、組織全体のすべてのグループの環境設定のロックを解除するよう依頼できます。ロックを解除した後、管理者（および他のすべてのグループのグループ管理者）は、管理しているグループに対して設定できます。

手順については、[グループのプロジェクト環境設定を行う](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)および[グループのタスクとイシューの環境設定を行う](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)を参照してください。

## サブグループのリスト、追加、設定

管理対象のグループの下でサブグループを作成、表示、編集、コピー、名前変更、書き出し、削除できます。

## グループのイベント通知の設定

Workfront 管理者が、組織内のグループのイベント通知の設定機能のロックを解除した場合は、管理しているグループに対してイベント通知を設定できます。手順については、[グループのイベント通知を表示および設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)を参照してください。

## グループのステータスの作成とカスタマイズ

グループ管理者は、管理する最上位グループに対してカスタムステータスを作成できます。これにより、グループが自立し、会社全体で多くのカスタムステータスを使用する必要がなくなります。（Workfront 管理者は、任意のグループに対してこの操作を実行することもできます）。

Workfront 管理者がカスタマイズを許可するように設定している場合は、トップレベルグループのシステムステータスをカスタマイズすることもできます。

手順については、[グループステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。

## グループのプロジェクトの操作

「設定」の「グループ」エリアで、管理するグループのメインページを表示しているときに、プロジェクトで次の操作を実行できます。

* グループとそのサブグループに関連付けられ、自分と共有されているプロジェクトのリストと操作（編集、コピー、削除、書き出し）
* グループの新しいプロジェクトの作成

手順については、[グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md)を参照してください。

## グループの承認プロセスの表示と管理

グループエリアで管理するグループを表示している場合、そのグループの管理者またはそのサブグループの 1 人が管理アクセス権を持つ承認プロセスを表示および操作できます。

手順については、[グループレベルの承認プロセス](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md)を参照してください。

## グループのレイアウトテンプレートの表示と管理

グループエリアで管理するグループを表示している場合、そのグループの管理者またはそのサブグループの 1 人が管理アクセス権を持つレイアウトテンプレートを表示および操作できます。

手順については、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

## グループメンバーのスケジュールの表示と管理

グループのスケジュールを作成するグループ管理者は、管理者がスケジュールを管理するグループを指定する必要があります。通常、これはスケジュールが作成されるグループですが、グループ管理者が複数のグループを管理し、他のグループを代わりに指定する場合は、別のグループになる可能性があります。

管理するグループのメインページを表示しているときに、管理者がスケジュールを編集できるグループとして指定されている場合は、そのグループのページからスケジュールを表示および管理できます。

手順については、[グループのスケジュールを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md)を参照してください。

## グループメンバーのタイムシートプロファイルを表示および管理

管理しているグループのメインページを表示している場合は、自分とグループ（またはそのサブグループのうちの 1 つ）の他の管理者が編集権限を持つタイムシートプロファイルを管理できます。手順については、[グループのタイムシートプロファイルを作成および管理](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)を参照してください。

## グループのサブグループメンバーを表示および管理する

管理しているグループのメインページを表示しているときに、グループのサブグループ内のすべてのユーザーを表示および管理できます。手順については、[サブグループメンバーを表示および管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)を参照してください。

## グループのチームを表示および管理

グループエリアで管理するグループを表示している場合、グループまたはその任意のサブグループに関連付けられたチームを表示し、共同作業ができます。

手順については [グループのチームを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)を参照してください。

## グループの会社を表示および管理

グループエリアで管理するグループを表示している場合、グループまたは任意のそのサブグループに関連付けられた会社を表示し、共同作業ができます。手順については、[グループの会社を作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md)を参照してください。

## グループのポートフォリオとプログラムを表示および管理

グループエリアで管理するグループを表示している場合、以下の両方に該当する場合に、ポートフォリオとプログラムを表示し、操作できます。

* 表示中のグループまたはその任意のサブグループに関連付けられている
* 自分が作成したか、自分と共有されていたため、それらを表示する権限がある

手順については、[グループのプロジェクトを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md)と[グループのプログラムを作成、変更、表示](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md)を参照してください。

## グループの非アクティブ化または再アクティブ化

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

グループは、デフォルトのアクティブ状態のままにすることも、非アクティブにすることもできます。

グループを非アクティブ化すると、ユーザーが別のオブジェクトに関連付けるグループを検索するときに先行入力フィールドにそのグループが表示されなくなるため、そのグループが現在使用されていない場合に便利です。

グループを非アクティブ化またはアクティブ化する手順については、[グループの非アクティブ化や再アクティブ化](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md)を参照してください。
