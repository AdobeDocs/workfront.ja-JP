---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: グループの非アクティブ化または再アクティブ化
description: 管理対象のグループを非アクティブ化して、使用しなくなったグループを削除できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# グループの非アクティブ化または再アクティブ化

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

管理対象のグループを非アクティブ化して、使用しなくなったグループを削除できます。

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

## グループの非アクティブ化または再アクティブ化

>[!IMPORTANT]
>
>グループを非アクティブ化すると、そのグループの下にあるサブグループも非アクティブ化されます。
>
>いずれかのイベントを再アクティブ化する必要がある場合は、次のいずれかの操作を行った後に再アクティブ化できます。
>
>* 親グループから削除します。 詳しくは、 [親グループからサブグループを削除し、最上位グループにする](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 記事内 [サブグループの管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* アクティブなグループの下に移動します。 詳しくは、 [サブグループの作成、移動、表示、編集、コピー、名前変更、書き出し、削除](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) 記事内 [サブグループの管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左のパネルで、「 」を選択します。 **グループ**.

   表示されるリストで、管理しているグループと、そのグループに含まれているサブグループを確認できます。 Adobe Workfront管理者は、すべてのグループを表示できます。

1. グループの名前をクリックして、そのページを開きます。

1. その他メニューをクリックします。 ![](assets/more-icon.png) グループ名の横にあるをクリックし、 **無効化** または **再開**.

   >[!NOTE]
   >
   >グループが非アクティブなグループのサブグループである場合、「アクティブである」オプション（「プレビュー」の「再開」オプション）は使用できません。 再アクティブ化する前に、親グループから削除するか、上記の重要事項の説明に従って、アクティブなグループの下に移動する必要があります。

1. （条件付き）グループを非アクティブ化する場合、 **無効化** 内 **グループを非アクティブ化** ボックスが表示されます。

## 非アクティブなグループに関する考慮事項

「アクティブ」オプションを無効にして非アクティブにしたグループについては、の節で説明する点に注意してください。 [グループの非アクティブ化または再アクティブ化](#View) 」を参照してください。

* グループを非アクティブ化すると、そのグループの下にあるすべてのサブグループも非アクティブ化されます。 非アクティブ化した後に追加するサブグループも含まれます。

   この状況でのサブグループの再アクティブ化については、 [非アクティブな親グループの下のサブグループの再アクティブ化について](#about-reactivating-a-subgroup-below-an-inactive-parent-group) 」を参照してください。

* [ セットアップ ] の [ グループ ] 領域に移動すると、[ アクティブ ] が既定のフィルタなので、リストにはアクティブなグループのみが表示されます ![](assets/filter-nwepng.png) それに対して 非アクティブなグループも含め、管理しているすべてのグループを表示する場合は、すべてフィルターを使用できます。 または、非アクティブフィルターを使用して、非アクティブなフィルターのみをリストします。

   リスト内のフィルターについて詳しくは、 [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* グループを非アクティブ化しても、以下は変更されません。

   * グループのオブジェクトへの関連付け。 関連オブジェクトは、変更を加えることなく、以前と同様に機能し続けます。

      例えば、非アクティブ化したグループにプロジェクトが関連付けられている場合、そのプロジェクトは変更を加えることなく、グループの環境設定とステータスを引き続き使用します。

   * 設定のグループのページ内から、承認、チーム、会社などの新しいオブジェクトを作成する機能。 デフォルトでは、新しいオブジェクトは非アクティブなグループに関連付けられます。
   * 管理者がフィルターとレポートでグループを検索する機能。

      また、[ 設定 ] 領域でグループの設定を管理するグループの先行入力フィールドにも表示されます。 これには、「環境設定」、「イベント通知」、「システムライセンス」の各領域が含まれます。

      例えば、設定/プロジェクト環境設定/プロジェクトに移動して、上のオプションの先行入力フィールドをクリアした場合、非アクティブなグループを見つけて、そのプロジェクト環境設定を設定できます。

## 非アクティブな親グループの下のサブグループの再アクティブ化について {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

グループを非アクティブ化すると、そのグループの下にあるすべてのサブグループも非アクティブ化されます。 非アクティブなグループの下のサブグループの 1 つを再アクティブ化する必要がある場合は、次の 2 つの操作のいずれかを実行できます。

* アクティブなグループの下にサブグループを移動します。 次に、移動したグループの「アクティブ」オプションを有効にします。詳しくは、 [グループの非アクティブ化または再アクティブ化](#View) 」を参照してください。

   グループの移動手順については、 [グループの移動](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* 親グループからサブグループを削除します（サブグループを最上位グループにします）。 次に、移動したグループの「アクティブ」オプションを有効にします。詳しくは、 [グループの非アクティブ化または再アクティブ化](#View) 」を参照してください。

   親グループからサブグループを削除する手順については、 [親グループからサブグループを削除し、最上位グループにする](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) 記事内 [サブグループの管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
