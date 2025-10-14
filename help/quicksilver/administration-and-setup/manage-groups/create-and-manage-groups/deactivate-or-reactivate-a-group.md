---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: グループのディアクティベートまたは再アクティベート
description: 管理対象の使用しなくなったグループを非アクティブ化できます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 90%

---

# グループの非アクティブ化または再アクティブ化

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

管理対象の使用しなくなったグループを非アクティブ化できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>グループのグループ管理者またはシステム管理者である必要があります。</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループの非アクティブ化または再アクティブ化

>[!IMPORTANT]
>
>グループを非アクティブ化すると、そのグループの下にあるサブグループも非アクティブ化されます。
>
>いずれかのイベントを再アクティブ化する必要がある場合は、次のいずれかの操作を行った後に再アクティブ化できます。
>
>* 親グループから削除します。詳しくは、[サブグループの管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)の記事にある[親グループからサブグループを削除し、最上位グループにする](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make)を参照してください。
>
>* アクティブなグループの下に移動します。詳しくは、[サブグループを管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)の記事にある[サブグループの作成、移動、表示、編集、コピー、名前変更、書き出しまたは削除](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create)を参照してください。

{{step-1-to-setup}}

1. 左のパネルで、「**グループ**」を選択します。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. グループの名前をクリックして、そのページを開きます。

1. グループ名の横にある「詳細 ![&#x200B; メニュー &#x200B;](assets/more-icon.png) 「詳細」アイコン）をクリックし、「**アクティベートを解除**」または **アクティベートを再アクティベート** をクリックします。

   >[!NOTE]
   >
   >グループが非アクティブ化されたグループのサブグループである場合、「アクティブ」オプション（プレビューの「再アクティブ化」オプション）は使用できません。再アクティブ化する前に、親グループから削除するか、上記の重要事項の説明に従って、アクティブなグループの下に移動する必要があります。

1. （条件付き）グループを非アクティブ化する場合、表示される「**グループを非アクティブ化**」ボックスの「**非アクティブ化**」をクリックします。

## 非アクティブなグループに関する考慮事項

「アクティブ」オプションを無効にして非アクティブ化にしたグループに関して、[グループの非アクティブ化または再アクティブ化](#View)の節で説明する点に注意してください。

* グループを非アクティブ化すると、そのグループの下にあるすべてのサブグループも非アクティブ化されます。これには、非アクティブ化した後に追加するサブグループが含まれます。

  この状況でのサブグループの再アクティブ化について詳しくは、[非アクティブな親グループの下のサブグループの再アクティブ化について](#about-reactivating-a-subgroup-below-an-inactive-parent-group)を参照してください。

* 「設定」の「グループ」領域に移動すると、リスト内のアクティブなグループのみが表示されます。これは、そのデフォルトのフィルター ![&#x200B; フィルターアイコン &#x200B;](assets/filter-nwepng.png) がアクティブであるためです。 非アクティブなグループも含め、管理するすべてのグループを表示する場合は、すべてのフィルターを使用できます。または、非アクティブフィルターを使用して、非アクティブなフィルターのみをリストします。

  リスト内のフィルターについて詳しくは、[フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)を参照してください。

* グループを非アクティブ化しても、次は変更されません。

   * オブジェクトへのグループの関連付け。関連オブジェクトは、変更を加えることなく、以前と同様に機能し続けます。

     例えば、非アクティブ化したグループにプロジェクトが関連付けられている場合、そのプロジェクトは変更されることはなく、グループの環境設定とステータスを引き続き使用します。

   * 設定のグループのページ内から、承認、チーム、会社などの新しいオブジェクトを作成する機能。デフォルトでは、新しいオブジェクトは非アクティブなグループに関連付けられます。
   * 管理者としてフィルターとレポートでグループを検索する機能。

     また、設定領域でグループの設定を管理するグループの先行入力フィールドにも表示されます。これには、環境設定、イベント通知、システムライセンスの各エリアが含まれます。

     例えば、設定／プロジェクト環境設定／プロジェクトに移動して、上のオプションの先行入力フィールドをクリアした場合、非アクティブなグループを見つけて、そのプロジェクト環境設定を設定できます。

## 非アクティブな親グループの下のサブグループの再アクティブ化について {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

グループを非アクティブ化すると、そのグループの下にあるすべてのサブグループも非アクティブ化されます。非アクティブなグループの下のサブグループの 1 つを再アクティブ化する必要がある場合は、次の 2 つの操作のいずれかを実行できます。

* そのサブグループをアクティブなグループの下に移動します。次に、移動したグループの「アクティブ」オプションを有効にします。詳しい手順は、この記事の[グループの非アクティブ化と再アクティブ化](#View)セクションで説明されています。

  グループの移動について詳しくは、[グループの移動](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md)を参照してください。

* そのサブグループを親グループから削除します（これにより、サブグループが最上位グループになります）。次に、移動したグループの「アクティブ」オプションを有効にします。詳しい手順は、この記事の[グループの非アクティブ化と再アクティブ化](#View)セクションで説明されています。

  親グループからのサブグループの削除について詳しくは、[サブグループの管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)の記事にある[サブグループを親グループから削除し、それを最上位グループにする](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make)の節を参照してください。
