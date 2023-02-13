---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: サブグループの作成
description: 管理対象のグループの下にサブグループを作成して、ユーザーやプロジェクトを整理し、Adobe Workfront内でアクセス権を割り当てることができます。 通常、グループ管理者はグループとサブグループを管理します。 グループページを使用して、グループとサブグループを 1 か所で管理できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 3%

---

# サブグループの作成

管理対象のグループの下にサブグループを作成して、ユーザーやプロジェクトを整理し、Adobe Workfront内でアクセス権を割り当てることができます。

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

ただし、グループ管理者はグループとサブグループを管理します。 グループページを使用して、グループとサブグループを 1 か所で管理できます。 グループとサブグループがWorkfront内でどのように機能するかについては、 [グループの概要](../../../administration-and-setup/manage-groups/groups-overview/groups.md) および [サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## サブグループを追加

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **グループ**.

   表示されるリストで、管理しているグループと、そのグループに含まれているサブグループを確認できます。 Adobe Workfront管理者は、すべてのグループを表示できます。

1. 新しいサブグループを追加する既存のグループまたはサブグループを選択します。
1. クリック **新規サブグループ**.
1. 内 **新規サブグループ** 表示されるボックスに、 **グループ名** サブグループに対して。
1. （オプション）次の情報を指定します。

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
      <td>サブグループの説明を入力します。 512 文字まで入力できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">アクティブ</td> 
      <td> <p>（デフォルトで有効）Workfrontインスタンスでグループをアクティブにします。</p> <p>以下に示すような先行入力フィールドでは、通常のユーザーがグループを検索してオブジェクトに関連付けたり、オブジェクトと共有したりすると、アクティブなグループのみがリストに表示されます。</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>これをユーザーに対して合理化するには、現在使用中でないグループの「アクティブである」オプションを無効にします。</p> <p>このフィールドを使用すると、アクティブなステータスや非アクティブなステータスに基づいて、グループリストを簡単に表示、フィルタリングおよびグループ化できます。 リストでのビュー、フィルター、グループ化の使用について詳しくは、 <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">レポート要素：フィルター、ビュー、グループ化</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">このグループとそのサブグループを公開</td> 
      <td> <p>（サブグループではなく、最上位グループの詳細を表示している場合にのみ使用可能です）。 このオプションを有効にすると、編集ユーザーアクセス（グループの管理者ではないユーザー）を持つサブグループ内のユーザーが、このグループとそのサブグループを他のユーザーのユーザープロファイルに追加できます。</p> <p>公開グループの場合、編集ユーザーアクセス権を持つ（グループ内またはグループ外の）ユーザーは、他のユーザーのプロファイルにグループを追加できます。 これは、プライベートグループに対しては実行できません。</p> <p>このオプションは、複数のレベルを持つグループの階層の上位の親グループでのみ編集できます。 親グループのすべてのサブグループが設定を継承します。</p> <p><b>メモ</b>:  
        <ul> 
         <li>サブグループを単独で公開することはできませんが、最上位の親グループを公開にして、親のサブグループをすべて公開にすることができます。</li> 
         <li>パブリックグループに属するサブグループは、デフォルトでパブリックになっているので、編集ユーザーアクセス権を持つユーザーは、そのサブグループを他のユーザーにも追加できます。</li> 
        </ul> </p> <p>ユーザーの編集に必要なアクセスに関する情報が必要な場合は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">ユーザーへのアクセス権の付与</a>. ユーザーの編集について詳しくは、 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">ユーザーのプロファイルの編集</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ビジネスリーダー </td> 
      <td> <p>管理するサブグループに対して、1 人のユーザーをビジネスリーダーとして割り当てることができます。 ビジネスリーダーとは、サブグループに関するビジネス上の意思決定を行う人です。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">ビジネスリーダーの概要</a><span>.</span></p> <p>人物がまだサブグループのメンバーでない場合は、このフィールドに名前を追加すると、グループにも追加されます。</p> <p><b>メモ</b>:  
        <ul> 
         <li>サブグループからビジネスリーダーを削除する前に、「ビジネスリーダー」フィールドから名前を削除する必要があります。</li> 
         <li>「ビジネス・リーダー」フィールドから名前を削除した場合、そのユーザーは、削除しない限り、サブグループのメンバーのままです。 グループからユーザーを削除する手順については、 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">グループのメンバーシップを管理する</a> 記事内 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">グループの管理</a>.</li> 
        </ul> </p> <p>詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">ビジネスリーダーの概要</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">グループのメンバーおよびグループ管理者</td> 
      <td> 
       <ul> 
        <li> <p>グループメンバー：サブグループにユーザーとグループを追加するには、追加する既存のユーザーまたはグループの名前を入力し、表示されたら名前を選択します。</p> <p>追加したユーザーとグループは、そのグループと共有されるすべてのオブジェクトにアクセスできます。</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">グループ管理者：サブグループは、その上のグループのグループ管理者を継承するので、サブグループのグループ管理者としてのユーザーの指定は任意です。 ユーザー名の右にあるドロップダウンメニューを使用して、グループメンバーをグループの管理者として割り当てることができます。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リスト内でユーザーとグループを検索する</td> 
      <td> このサブグループに既に割り当てられているユーザーまたはグループを検索する必要がある場合は、ここに名前を入力し、表示されたときに選択できます。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **保存します。**
