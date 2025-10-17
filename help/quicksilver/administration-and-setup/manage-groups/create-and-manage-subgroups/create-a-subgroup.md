---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: サブグループの作成
description: 管理対象のグループの下にサブグループを作成して、ユーザーやプロジェクトを整理し、Adobe Workfront 内でアクセス権を割り当てることができます。通常、グループ管理者はグループとサブグループを管理します。グループページを使用して、グループとサブグループを一元的に管理できます。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 58%

---

# サブグループの作成

管理対象のグループの下にサブグループを作成して、ユーザーやプロジェクトを整理し、Adobe Workfront 内でアクセス権を割り当てることができます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

ただし、通常、グループ管理者はグループとサブグループを管理します。グループページを使用して、グループとサブグループを一元的に管理できます。グループとサブグループが Workfront 内でどのように機能するかについては、[グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md)と[サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr>
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>グループのグループ管理者またはシステム管理者である必要があります。</td>
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## サブグループを追加

{{step-1-to-setup}}

1. 「**グループ**」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. 新しいサブグループを追加する既存のグループまたはサブグループを選択します。
1. 「**新規サブグループ**」をクリックします。
1. 表示された **新規サブグループ** ボックスに、サブグループの **グループ名** を入力します。
1. （オプション）次の情報を入力します。

   * **説明**: サブグループの説明を入力します。 512 文字まで入力できます。
   * **アクティブ**：このオプションはデフォルトで有効になっており、Workfront インスタンス内でこのグループをアクティブにします。

     次に示すような typeahead フィールドでは、通常のユーザーがグループを検索してオブジェクトに添付したり、オブジェクトを共有したりすると、アクティブなグループのみがリストに表示されます。

     ![&#x200B; グループの先行入力フィールド &#x200B;](assets/typeahead-for-group.png)

     ユーザーの作業を効率化するには、現在使用されていないグループの「**アクティブ**」オプションを無効にします。

     このフィールドを使用すると、ステータスがアクティブか非アクティブかに基づいて、グループリストを簡単に表示、フィルタリング、グループ化できます。リストでのビュー、フィルターおよびグループ化の使用については、[レポート要素：フィルター、ビューおよびグループ化](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)を参照してください。

   * **ビジネスリーダー**：管理するサブグループのビジネスリーダーとして 1 人のユーザーを割り当てることができます。 ビジネスリーダーとは、サブグループのビジネス上の決定を行う人のことです。詳しくは、[ビジネスリーダーの概要](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md)を参照してください。

     ユーザーがまだサブグループのメンバーでない場合は、このフィールドに名前を追加すると、そのユーザーもサブグループに追加されます。

     >[!NOTE]
     >
     >* サブグループからビジネスリーダーを削除する前に、「ビジネスリーダー」フィールドから名前を削除する必要があります。
     >* ビジネスリーダーフィールドから名前を削除した場合、そのユーザーはサブグループから削除されない限り、サブグループのメンバーのままでいます。グループからユーザーを削除する手順については、[&#x200B; グループのメンバーシップの表示と管理 &#x200B;](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md) を参照してください。

   * **グループメンバーとグループ管理者**：ユーザーとグループをサブグループのメンバーとして追加するには、追加する既存のユーザーまたはグループの名前の入力を開始し、表示されたら名前を選択します。

     追加したユーザーとグループは、そのグループと共有されるすべてのオブジェクトにアクセスできます。

     サブグループは、その上のグループのグループ管理者を継承するので、サブグループのグループ管理者としてのユーザーの指定はオプションです。 ユーザー名の右にあるドロップダウンメニューを使用して、グループメンバーをグループの管理者として割り当てることができます。

   * **リスト内のユーザーとグループを検索**：このサブグループに既に割り当てられているユーザーまたはグループを見つける必要がある場合は、ここに名前を入力し、表示されたら選択します。

1. 「**保存**」をクリックします。
