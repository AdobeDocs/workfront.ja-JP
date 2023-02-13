---
user-type: administrator
product-area: system-administration;user-management
keywords: 作成，グループ，サブグループ，新規
navigation-topic: create-and-manage-groups
title: グループの作成
description: Adobe Workfront管理者は、ユーザーやプロジェクトを整理し、Workfront内でアクセス権を割り当てるためのグループを作成できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 3%

---

# グループの作成

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Adobe Workfront管理者は、ユーザーやプロジェクトを整理し、Workfront内でアクセス権を割り当てるためのグループを作成できます。 詳しくは、 [グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

各サブグループには少なくとも 1 人のグループ管理者が必要です。 グループ管理者は、グループページを使用して、自分のグループを 1 か所で管理できます。

グループ管理者またはWorkfront管理者の場合は、グループの下にサブグループを作成することもできます。 手順については、 [サブグループの作成](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

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

## 最上位グループを最初から作成する

以下の手順では、新しいグループを最初から作成する方法を説明します。 既存のグループまたはサブグループをコピーして作成する方法については、 [既存のグループまたはサブグループをコピーして最上位グループを作成する](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) 」を参照してください。

トップレベルグループを作成するには、Workfrontの管理者である必要があります。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. グループのリストの上の **新しいグループ**.

   >[!TIP]
   >
   >グループのリストの下部で、 **グループをさらに追加** インラインでグループを追加するには、 **入力** グループ情報の追加が終了したら、次の手順に従います。

1. 内 **新しいグループ** 表示されるボックスに、グループの名前を入力します。
1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">グループ名</td> 
      <td>グループ名を変更します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>グループの説明を入力します。 512 文字まで入力できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>（デフォルトで有効）Workfrontインスタンスでグループをアクティブにします。</p> <p>以下に示すような先行入力フィールドでは、通常のユーザーがグループを検索してオブジェクトに関連付けたり、オブジェクトと共有したりすると、アクティブなグループのみがリストに表示されます。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>これをユーザーに対して合理化するには、現在使用中でないグループの「アクティブである」オプションを無効にします。</p> <p>このフィールドを使用すると、アクティブなステータスや非アクティブなステータスに基づいて、グループリストを簡単に表示、フィルタリングおよびグループ化できます。 リストでのビュー、フィルター、グループ化の使用について詳しくは、 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">レポート要素：フィルター、ビュー、グループ化</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このグループとそのサブグループを公開</td> 
      <td> <p>（サブグループではなく、最上位グループの詳細を表示している場合にのみ使用可能です）。 このオプションを有効にすると、編集ユーザーのアクセス権を持つグループ（グループの管理者ではないユーザー）内のユーザーが、このグループとそのサブグループを他のユーザーのユーザープロファイルに追加できます。</p> <p>公開グループの場合、編集ユーザーアクセス権を持つ（グループ内またはグループ外の）ユーザーは、他のユーザーのプロファイルにグループを追加できます。 これは、プライベートグループに対しては実行できません。</p> <p>このオプションは、複数のレベルを持つグループの階層の上位の親グループでのみ編集できます。 親グループのすべてのサブグループが設定を継承します。</p> <p><b>メモ</b>:  
        <ul> 
         <li>サブグループを単独で公開することはできませんが、最上位の親グループを公開にして、親のサブグループをすべて公開にすることができます。</li> 
         <li>パブリックグループに属するサブグループは、デフォルトでパブリックになっているので、編集ユーザーアクセス権を持つユーザーは、そのサブグループを他のユーザーにも追加できます。</li> 
        </ul> </p> <p>ユーザーの編集に必要なアクセスに関する情報が必要な場合は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>. ユーザーの編集について詳しくは、 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ビジネスリーダー </td> 
      <td> <p>管理するグループに対して、1 人のユーザーをビジネスリーダーに割り当てることができます。 ビジネスリーダーとは、グループのビジネス上の意思決定を行う人のことです。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">ビジネスリーダーの概要</a><span>.</span></p> <p>ユーザーがまだグループのメンバーでない場合は、このフィールドに名前を追加すると、そのユーザーもグループに追加されます。</p> <p><b>メモ</b>:  
        <ul> 
         <li>グループからビジネスリーダーを削除する前に、「ビジネスリーダー」フィールドから名前を削除する必要があります。</li> 
         <li>[ ビジネスリーダー ] フィールドから名前を削除した場合、そのユーザーはグループから削除しない限り、グループのメンバーのままです。 グループからユーザーを削除する手順については、 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">グループのメンバーシップを管理する</a> 記事内 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">グループの管理</a>.</li> 
        </ul> </p> <p>詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">ビジネスリーダーの概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループのメンバーおよびグループ管理者</td> 
      <td> 
       <ul> 
        <p>グループメンバーを追加するには、追加する既存のユーザーまたはグループの名前を入力し、表示されたら名前を選択します。</p> 
        <p>追加したユーザーとグループは、そのグループと共有されるすべてのオブジェクトにアクセスできます。</p>
        <p>最上位のグループには、少なくとも 1 人のグループ管理者が必要です。 </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リスト内でユーザーとグループを検索する</td> 
      <td> 既にこのグループに割り当てられているユーザーまたはグループを検索する必要がある場合は、ここに名前を入力し、表示されたときに選択できます。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **グループを作成**.

## 既存のグループまたはサブグループをコピーして最上位グループを作成する {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Workfrontの管理者は、既存のグループまたはサブグループをコピーして、新しい最上位グループを作成できます。

これをおこなう場合は、次の点に注意してください。

* 既存のグループに属するすべてのメンバーとサブグループが、新しい最上位グループにコピーされます。
* コピーされたグループのメンバーは、元のグループに割り当てられた割り当てを保持します。 したがって、元のグループのグループ管理者も、コピーされたグループのグループ管理者に指定されます。

グループまたはサブグループをコピーして新しい最上位グループを作成するには、次の手順に従います。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

   表示されるリストで、管理しているグループと、そのグループに含まれているサブグループを確認できます。 Adobe Workfront管理者は、すべてのグループを表示できます。

1. コピーするグループを選択し、コピーアイコンをクリックします。 ![](assets/copy-icon.png).
1. 内 **グループをコピー** 表示されるボックスに、 **グループ名** コピーしたグループの

1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">グループ名</td> 
      <td>グループ名を変更します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>グループの説明を入力します。 512 文字まで入力できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>（デフォルトで有効）Workfrontインスタンスでグループをアクティブにします。</p> <p>以下に示すような先行入力フィールドでは、通常のユーザーがグループを検索してオブジェクトに関連付けたり、オブジェクトと共有したりすると、アクティブなグループのみがリストに表示されます。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>これをユーザーに対して合理化するには、現在使用中でないグループの「アクティブである」オプションを無効にします。</p> <p>このフィールドを使用すると、アクティブなステータスや非アクティブなステータスに基づいて、グループリストを簡単に表示、フィルタリングおよびグループ化できます。 リストでのビュー、フィルター、グループ化の使用について詳しくは、 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">レポート要素：フィルター、ビュー、グループ化</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このグループとそのサブグループを公開</td> 
      <td> <p>（サブグループではなく、最上位グループの詳細を表示している場合にのみ使用可能です）。 このオプションを有効にすると、編集ユーザーのアクセス権を持つグループ（グループの管理者ではないユーザー）内のユーザーが、このグループとそのサブグループを他のユーザーのユーザープロファイルに追加できます。</p> <p>公開グループの場合、編集ユーザーアクセス権を持つ（グループ内またはグループ外の）ユーザーは、他のユーザーのプロファイルにグループを追加できます。 これは、プライベートグループに対しては実行できません。</p> <p>このオプションは、複数のレベルを持つグループの階層の上位の親グループでのみ編集できます。 親グループのすべてのサブグループが設定を継承します。</p> <p><b>メモ</b>:  
        <ul> 
         <li>サブグループを単独で公開することはできませんが、最上位の親グループを公開にして、親のサブグループをすべて公開にすることができます。</li> 
         <li>パブリックグループに属するサブグループは、デフォルトでパブリックになっているので、編集ユーザーアクセス権を持つユーザーは、そのサブグループを他のユーザーにも追加できます。</li> 
        </ul> </p> <p>ユーザーの編集に必要なアクセスに関する情報が必要な場合は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">ユーザーへのアクセス権の付与</a>. ユーザーの編集について詳しくは、 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">ユーザーのプロファイルの編集</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ビジネスリーダー </td> 
      <td> <p>管理するグループに対して、1 人のユーザーをビジネスリーダーに割り当てることができます。 ビジネスリーダーとは、グループのビジネス上の意思決定を行う人のことです。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">ビジネスリーダーの概要</a><span>.</span></p> <p>ユーザーがまだグループのメンバーでない場合は、このフィールドに名前を追加すると、そのユーザーもグループに追加されます。</p> <p><b>メモ</b>:  
        <ul> 
         <li>グループからビジネスリーダーを削除する前に、「ビジネスリーダー」フィールドから名前を削除する必要があります。</li> 
         <li>[ ビジネスリーダー ] フィールドから名前を削除した場合、そのユーザーはグループから削除しない限り、グループのメンバーのままです。 グループからユーザーを削除する手順については、 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">グループのメンバーシップを管理する</a> 記事内 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">グループの管理</a>.</li> 
        </ul> </p> <p>詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">ビジネスリーダーの概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループのメンバーおよびグループ管理者</td> 
      <td> 
       <ul> 
        <li> <p>グループメンバー：グループにユーザーとグループを追加するには、追加する既存のユーザーまたはグループの名前を入力し、表示されたら名前を選択します。</p> <p>追加したユーザーとグループは、そのグループと共有されるすべてのオブジェクトにアクセスできます。</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.copied groups">グループ管理者：元のグループのグループ管理者は、コピーしたグループのグループ管理者にも指定されます。 ユーザー名の右にあるドロップダウンメニューを使用して、グループメンバーをグループの管理者として割り当てることができます。</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">トップレベルのグループには、少なくとも 1 人のグループ管理者が必要です。</p> </li> 
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
   >* 元のグループにサブグループが含まれている場合、サブグループは新しいグループに追加され、その名前はデフォルトでは「元のサブグループ名（コピー）」になります。
   >* ユーザーまたはサブグループの名前の右側にある X をクリックすると、元のグループからユーザーまたはサブグループを削除できます。


1. クリック **グループを作成**.
