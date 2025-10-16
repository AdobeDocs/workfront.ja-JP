---
user-type: administrator
product-area: system-administration;user-management
keywords: 作成,グループ,サブグループ,新規
navigation-topic: create-and-manage-groups
title: グループの作成
description: Adobe Workfront 管理者は、ユーザーやプロジェクトを整理し、Workfront 内でアクセス権を割り当てるためのグループを作成できます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '1633'
ht-degree: 87%

---

# グループの作成

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Adobe Workfront 管理者は、ユーザーやプロジェクトを整理し、Workfront 内でアクセス権を割り当てるためのグループを作成できます。詳しくは、[グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md)を参照してください。

各サブグループには 1 人以上のグループ管理者が必要です。グループ管理者は、グループページを使用して、自分のグループを 1 か所で管理できます。

グループ管理者または Workfront 管理者の場合は、グループの下にサブグループを作成することもできます。手順について詳しくは、[サブグループの作成](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md)を参照してください。

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

## トップレベルのグループを最初から作成

次の手順では、新しいグループを最初から作成する方法を説明します。既存のグループまたはサブグループをコピーして作成する方法については、[既存のグループまたはサブグループをコピーしてトップレベルグループを作成](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup)を参照してください。

トップレベルグループを作成するには、Workfront 管理者である必要があります。

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**![&#x200B; グループ &#x200B;](assets/groups-icon.png)」をクリックします。

1. グループのリストの上の&#x200B;**新しいグループ**&#x200B;をクリックします。

   >[!TIP]
   >
   >グループのリストの下部で、「**さらにグループを追加**」をクリックして、インラインでグループを追加して、グループ情報の追加が終了したら、「**入力**」をクリックします。

1. 表示される「**新規グループ**」ボックスに、グループの名前を入力します。
1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">グループ名</td> 
      <td>グループの名前を変更します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>グループの説明を入力します。512 文字まで入力できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>（デフォルトで有効）Workfront インスタンスでグループをアクティブ化します。</p> <p>下図のような先行入力フィールドでは、オブジェクトの関連付けやオブジェクトの共有のために、標準ユーザーがグループを検索しようとすると、アクティブなグループのみがリストに表示されます。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>これをユーザーが効率的に利用できるようにするには、現在使用していないグループの「アクティブ」オプションを無効にします。</p> <p>このフィールドを使用すると、ステータスがアクティブか非アクティブかに基づいて、グループリストを簡単に表示、フィルタリング、グループ化できます。リストでのビュー、フィルターおよびグループ化の使用については、<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">レポート要素：フィルター、ビューおよびグループ化</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このグループとそのサブグループを公開</td> 
      <td> <p>（サブグループではなく、最上位グループの詳細を表示している場合にのみ使用できます）。 このオプションを有効にすると、編集ユーザーアクセス権を持つグループのユーザー（グループの管理者でない）が、このグループとそのサブグループを他のユーザーのユーザープロファイルに追加できるようになります。</p> <p>パブリックグループの場合、編集ユーザー権限のあるユーザー（グループの内外を問わない）は、他のユーザーのプロファイルにグループを追加できます。これは、プライベートグループに対しては実行できません。</p> <p>このオプションは、複数のレベルを持つグループの最上位階層の親グループでのみ編集できます。すべてのサブグループは親グループの設定を継承します。</p> <p><b>メモ</b>:  
        <ul> 
         <li>サブグループ自体を公開することはできませんが、最上位の親グループを公開することはできます。これにより、親のすべてのサブグループも公開されます。</li> 
         <li>パブリックグループに属するサブグループは、デフォルトで公開になっているので、編集ユーザーアクセス権を持つユーザーは、そのサブグループを他のユーザーにも追加できます。</li> 
        </ul> </p> <p>ユーザーの編集に必要なアクセスに関する情報が必要な場合は、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。ユーザーの編集について詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ビジネスリーダー </td> 
      <td> <p>管理するグループに対して、1 人のユーザーをビジネスリーダーに割り当てることができます。ビジネスリーダーとは、グループのビジネス上の決定を行う人物のことです。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">ビジネスリーダーの概要</a>を参照してください<span>。</span></p> <p>ユーザーがまだグループのメンバーでない場合は、このフィールドに名前を追加すると、そのユーザーもグループに追加されます。</p> <p><b>メモ</b>：  
        <ul> 
         <li>グループからビジネスリーダーを削除する前に、「ビジネスリーダー」フィールドから名前を削除する必要があります。</li> 
         <li>ビジネスリーダーフィールドから名前を削除した場合、そのユーザーはグループから削除されない限り、グループのメンバーのままでいます。グループからユーザーを削除する手順については、<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">グループの管理</a>の記事にある<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">グループのメンバーシップの管理</a>の節を参照してください。</li> 
        </ul> </p> <p>詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">ビジネスリーダーの概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループのメンバーおよびグループ管理者</td> 
      <td>
        <p>グループメンバーを追加するには、追加する既存のユーザーまたはグループの名前を入力し、表示されたら名前を選択します。</p> 
        <p>追加したユーザーとグループは、そのグループと共有されるすべてのオブジェクトにアクセスできます。</p>
        <p>最上位のグループには、1 人以上のグループ管理者が必要です。 </p>
     </tr> 
     <tr> 
      <td role="rowheader">リスト内でユーザーとグループを検索する</td> 
      <td> 既にこのグループに割り当てられているユーザーまたはグループを検索する必要がある場合は、ここに名前を入力し、表示されたときに選択できます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**グループを作成**」をクリックします。

## 既存のグループまたはサブグループをコピーして最上位グループを作成 {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Workfront 管理者は、既存のグループまたはサブグループをコピーして、新しい最上位グループを作成できます。

これを行う場合は、以下の点に注意してください。

* 既存のグループに属するすべてのメンバーとサブグループが、新しい最上位グループにコピーされます。
* コピーされたグループのメンバーは、元のグループでの割り当てを保持します。したがって、元のグループのグループ管理者は、コピーされたグループのグループ管理者にも指定されます。

グループまたはサブグループをコピーして新しい最上位グループを作成するには、以下のようにします。

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**![&#x200B; グループ &#x200B;](assets/groups-icon.png)」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. コピーするグループを選択し、コピーアイコン ![&#x200B; コピーアイコン &#x200B;](assets/copy-icon.png) をクリックします。
1. 表示される&#x200B;**グループのコピー**&#x200B;ボックスに、コピーしたグループの&#x200B;**グループ名**&#x200B;を入力します。

1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">グループ名</td> 
      <td>グループの名前を変更します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>グループの説明を入力します。512 文字まで入力できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>（デフォルトで有効）Workfront インスタンスでグループをアクティブ化します。</p> <p>下図のような先行入力フィールドでは、オブジェクトの関連付けやオブジェクトの共有のために、標準ユーザーがグループを検索しようとすると、アクティブなグループのみがリストに表示されます。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>これをユーザーが効率的に利用できるようにするには、現在使用していないグループの「アクティブ」オプションを無効にします。</p> <p>このフィールドを使用すると、ステータスがアクティブか非アクティブかに基づいて、グループリストを簡単に表示、フィルタリング、グループ化できます。リストでのビュー、フィルターおよびグループ化の使用については、<a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">レポート要素：フィルター、ビューおよびグループ化</a>を参照してください。</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このグループとそのサブグループを公開</td> 
      <td> <p>（サブグループではなく、最上位グループの詳細を表示している場合にのみ使用できます）。 このオプションを有効にすると、編集ユーザーアクセス権を持つグループのユーザー（グループの管理者でない）が、このグループとそのサブグループを他のユーザーのユーザープロファイルに追加できるようになります。</p> <p>パブリックグループの場合、編集ユーザー権限のあるユーザー（グループの内外を問わない）は、他のユーザーのプロファイルにグループを追加できます。これは、プライベートグループに対しては実行できません。</p> <p>このオプションは、複数のレベルを持つグループの最上位階層の親グループでのみ編集できます。すべてのサブグループは親グループの設定を継承します。</p> <p><b>メモ</b>:  
        <ul> 
         <li>サブグループを単独での公開はできませんが、トップレベルの親グループを公開することは可能で、これにより親のサブグループもすべて公開できます。</li> 
         <li>パブリックグループに属するサブグループは、デフォルトで公開になっているので、編集ユーザーアクセス権を持つユーザーは、そのサブグループを他のユーザーにも追加できます。</li> 
        </ul> </p> <p>ユーザーの編集に必要なアクセスに関する情報が必要な場合は、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">ユーザーへのアクセス権の付与</a>を参照してください。ユーザーの編集について詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">ユーザーのプロファイルの編集</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ビジネスリーダー </td> 
      <td> <p>管理するグループに対して、1 人のユーザーをビジネスリーダーに割り当てることができます。ビジネスリーダーとは、グループのビジネス上の決定を行う人物のことです。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">ビジネスリーダーの概要</a>を参照してください<span>。</span></p> <p>ユーザーがまだグループのメンバーでない場合は、このフィールドに名前を追加すると、そのユーザーもグループに追加されます。</p> <p><b>メモ</b>：  
        <ul> 
         <li>グループからビジネスリーダーを削除する前に、「ビジネスリーダー」フィールドから名前を削除する必要があります。</li> 
         <li>ビジネスリーダーフィールドから名前を削除した場合、そのユーザーはグループから削除されない限り、グループのメンバーのままでいます。グループからユーザーを削除する手順については、<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">グループの管理</a>の記事にある<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">グループのメンバーシップの管理</a>の節を参照してください。</li> 
        </ul> </p> <p>詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">ビジネスリーダーの概要</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループのメンバーおよびグループ管理者</td> 
      <td> 
       <ul> 
        <li> <p>グループメンバー：グループにユーザーとグループを追加するには、追加する既存のユーザーまたはグループの名前を入力し、表示されたら名前を選択します。</p> <p>追加したユーザーとグループは、そのグループと共有されるすべてのオブジェクトにアクセスできます。</p> </li> 
        <li> <p>グループ管理者：元のグループのグループ管理者は、コピーしたグループのグループ管理者にも指定されます。ユーザー名の右にあるドロップダウンメニューを使用して、グループメンバーをグループの管理者として割り当てることができます。</p> <p>最上位のグループには、1 人以上のグループ管理者が必要です。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リスト内でユーザーとグループを検索する</td> 
      <td> 既にこのグループに割り当てられているユーザーまたはグループを検索する必要がある場合は、ここに名前を入力し、表示されたときに選択できます。</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* 元のグループにサブグループがある場合、サブグループは新しいグループに追加され、サブグループの名前はデフォルトで「元のサブグループ名（コピー）」になります。
   >* ユーザーまたはサブグループの名前の右側にある X をクリックすると、元のグループからユーザーまたはサブグループを削除できます。

1. 「**グループを作成**」をクリックします。
