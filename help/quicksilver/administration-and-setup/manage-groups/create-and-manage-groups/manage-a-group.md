---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理、グループ、編集、
navigation-topic: create-and-manage-groups
title: グループの管理
description: グループ管理者は、「設定」の「グループ」領域で、管理するグループを管理できます。 管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 0%

---

# グループの管理

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

グループ管理者は、「設定」の「グループ」領域で、管理するグループを管理できます。 管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>グループの管理者として割り当てられた場合、そのグループの下にあるすべてのサブグループのグループ管理者の役割を継承します。 サブグループを管理できるユーザーは、その上位グループのグループ管理者と、そのサブグループに割り当てられているグループ管理者のみです。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループのメンバーシップを管理する

管理しているグループに対して、ユーザーや他のグループを追加したり、削除したりできます。 また、グループメンバーをグループの管理者として割り当てたり、グループメンバーのユーザープロファイル情報を管理したりすることもできます。

手順については、 [グループのメンバーシップを表示および管理する](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## グループの詳細の管理

管理対象のグループまたはサブグループの [ グループの詳細 ] ページを表示および編集できます。 このページには、グループの説明、ビジネス・リーダーとグループ管理者の名前、およびグループとそのすべてのサブグループを公開または非公開にするオプションが含まれます。 また、アクセスレベルでカスタムフォームを管理できる場合は、カスタムフォームをグループに添付できます。

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

手順については、 [グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## グループの編集、コピー、削除

表示しているグループのメインページから離れずに、すばやく編集、コピー、削除できます

<!--
DRAFTED IN FLARE:
or deactivate

-->

グループ。

<!--
DRAFTED IN FLARE:
Make this change when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **グループ**.

   表示されるリストで、管理しているグループと、そのグループに含まれているサブグループを確認できます。 Adobe Workfront管理者は、すべてのグループを表示できます。

1. グループを選択し、「編集」タブをクリックします。 ![](assets/edit-icon.png)，コピー ![](assets/copy-icon.png)、または削除 ![](assets/delete.png) アイコン

   表示されるボックスの使用に関する情報が必要な場合は、次のいずれかを参照してください。

   * **編集**: [グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **コピー**: [既存のグループまたはサブグループをコピーして最上位グループを作成する](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) 記事内 [グループの作成](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **削除**: [グループの削除](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## グループのプロジェクト、タスクおよび問題の環境設定を設定する

グループ管理者で、システムレベルで設定された設定とは異なるプロジェクト、タスク、問題の環境設定が必要な場合は、Workfront管理者に問い合わせて、組織全体のすべてのグループの環境設定のロックを解除してもらうことができます。 ロックを解除した後、管理者（および他のすべてのグループのグループ管理者）は、管理しているグループに対して設定できます。

手順については、 [グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) および  [グループのタスクと問題の環境設定を設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## サブグループのリスト、追加、設定

管理グループの下にサブグループを作成、表示、編集、コピー、名前変更、エクスポート、削除できます。

## グループのイベント通知の設定

Workfrontの管理者が、組織内のグループのイベント通知の設定機能のロックを解除した場合は、管理しているグループに対してイベント通知を設定できます。 手順については、 [グループのイベント通知を表示および設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## グループのステータスの作成とカスタマイズ

グループ管理者は、管理する最上位グループに対してカスタムステータスを作成できます。 これにより、グループが自立し、会社全体で多くのカスタムステータスを使用する必要がなくなります。 (Workfrontの管理者は、任意のグループに対してこの操作を実行することもできます )。

また、Workfrontの管理者がカスタマイズを許可するように設定している場合は、トップレベルグループのシステムステータスをカスタマイズすることもできます。

手順については、 [グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## グループのプロジェクトの操作

「設定」の「グループ」領域で、管理するグループのメインページを表示しているときに、プロジェクトで次の操作を実行できます。

* グループとそのサブグループに関連付けられ、自分と共有されているプロジェクトのリストと操作（編集、コピー、削除、エクスポート）
* グループの新しいプロジェクトを作成します

手順については、 [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## グループの承認プロセスの表示と管理

[ グループ ] 領域で管理するグループを表示している場合、そのグループの管理者またはそのサブグループの 1 人が管理アクセス権を持つ承認プロセスを表示し、操作できます。

手順については、 [グループレベルの承認プロセス](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## グループのレイアウトテンプレートの表示と管理

[ グループ ] 領域で管理するグループを表示している場合は、そのグループの管理者またはそのサブグループの 1 人が管理アクセス権を持つレイアウトテンプレートを表示し、操作できます。

手順については、 [グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## グループメンバーのスケジュールの表示と管理

グループのスケジュールを作成するグループ管理者は、管理者がスケジュールを管理するグループを指定する必要があります。 通常、これはスケジュールが作成されるグループですが、グループ管理者が複数のグループを管理し、他のグループを代わりに指定する場合は、別のグループになる可能性があります。

管理するグループのメインページを表示しているときに、管理者がスケジュールを編集できるグループに指定されている場合は、そのグループのページでスケジュールを表示および管理できます。

手順については、 [グループのスケジュールの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## グループメンバーのタイムシートプロファイルを表示および管理します

管理しているグループのメインページを表示している場合は、自分とグループの他の管理者（またはそのサブグループの 1 つ）が編集権限を持っているタイムシートプロファイルを管理できます。 手順については、 [グループのタイムシートプロファイルを作成および管理する](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## グループのサブグループメンバーの表示と管理

管理するグループのメイン・ページを表示している場合は、グループのサブグループ内のすべてのユーザーを表示および管理できます。 手順については、 [サブグループメンバーの表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## グループのチームの表示と管理

[ グループ ] 領域で管理するグループを表示している場合、グループまたはそのサブグループに関連付けられたチームを表示し、操作できます。

手順については、 [グループのチームの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## グループの会社の表示と管理

[ グループ ] 領域で管理するグループを表示している場合、グループまたはそのサブグループに関連付けられた会社を表示し、操作できます。 手順については、 [グループの会社の作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## グループのポートフォリオおよびプログラムの表示と管理

[ グループ ] 領域で管理するグループを表示している場合、次の両方に該当する場合に、ポートフォリオとプログラムを表示し、操作できます。

* 表示中のグループまたはそのサブグループに関連付けられています
* 自分が作成したか、自分と共有されていたため、自分にはそれらを表示する権限があります

手順については、 [グループのプロジェクトの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) および [グループのプログラムの作成、変更、表示](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## グループの非アクティブ化または再アクティブ化

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

グループは、デフォルトのアクティブ状態のままにすることも、非アクティブにすることもできます。

グループの非アクティブ化は、他のオブジェクトに関連付けるグループを検索する際に、先行入力フィールドに表示されなくなったので、現在使用されていない場合に便利です。

グループを非アクティブまたはアクティブにする手順については、 [グループの非アクティブ化または再アクティブ化](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
