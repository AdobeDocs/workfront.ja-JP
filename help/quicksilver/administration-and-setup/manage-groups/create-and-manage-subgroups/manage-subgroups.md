---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理、サブグループ、編集
navigation-topic: create-and-manage-subgroups
title: サブグループの管理
description: サブグループのグループ管理者は、サブグループの作成、移動、表示、編集、コピー、名前変更、書き出し、削除を行うことができます。また、親グループからサブグループを削除して、そのサブグループを最上位グループにすることもできます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: ht
source-wordcount: '1269'
ht-degree: 100%

---

# サブグループの管理

サブグループのグループ管理者は、サブグループの作成、移動、表示、編集、コピー、名前変更、書き出し、削除を行うことができます。

また、親グループからサブグループを削除して、そのサブグループを最上位グループにすることもできます。

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。Workfront 管理者（すべてのグループ）も同様です。

サブグループについて詳しくは、[サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md)を参照してください。

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

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## サブグループの作成、移動、表示、編集、コピー、名前変更、書き出し、削除

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**グループ** ![](assets/groups-icon.png)」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. 作業対象のサブグループを含むグループの名前をクリックします。

   または

   1 つ以上のサブグループを移動する場合は、移動先グループの名前をクリックします（後の手順で移動するサブグループを指定します）。

1. 左側のメニューで、「**サブグループ**」をクリックします。

1. 次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新しいサブグループの作成</td> 
      <td> <p>新しいサブグループを表示しているグループから 1 レベル下に作成する場合は、「<strong>サブグループを追加</strong>」をクリックします。</p> <p>または、リスト内の別のサブグループの下に新しいサブグループを作成する場合は、そのサブグループを選択し、「<strong>サブグループに</strong><strong>追加</strong>」をクリックします。</p> <p>サブグループの設定に使用できるオプションについて詳しくは、<a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">サブグループを作成</a>の表を参照してください。</p> <p>グループ階層は 15 レベルを超えることはできませんが、1 つのレベルに対して、複数の並列グループを無制限に設定できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブグループを移動 </td> 
      <td> <p>既存のサブグループは、管理している別のグループの下に移動できます。</p> <p>グループ階層は 15 レベルを超えることはできませんが、1 つのレベルに対して、複数の並列グループを無制限に設定できます。</p> 
       <ol> 
        <li value="1"> <p>（オプション）サブグループを選択して、宛先グループにします。</p> <p>この手順をスキップした場合、手順 3 で選択したグループが宛先グループになります。</p> </li> 
        <li value="2"><strong>サブグループを追加</strong>／<strong>既存のグループ</strong>をクリックします。</li> 
        <li value="3"> <p>表示される<strong>既存のグループ</strong>ボックスに、移動するサブグループの名前を入力します。</p> <p>表示される結果には、宛先グループより上のグループは含まれません。</p> <p>適切なグループを選択していることを確認するには、グループにカーソルを移動して、その横に表示される、情報アイコン <img src="assets/info-icon.png"> をクリックします。グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> </li> 
        <li value="4"> <p>移動するサブグループの名前をクリックし、リストに表示されるようにします。</p> </li> 
        <li value="5"> <p>宛先グループに移動する他のサブグループに対して、手順 c～d を繰り返します。</p> </li> 
        <li value="6">「<strong>保存</strong>」をクリックします。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブグループを編集</td> 
      <td> <p>編集するサブグループを選択し、編集アイコン <img src="assets/edit-icon.png"> をクリックします。</p> <p>サブグループの設定に使用できるオプションについて詳しくは、<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">グループの作成</a>の表をご参照ください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つ以上のサブグループを書き出し</td> 
      <td> 
       <ol> 
        <li value="1">書き出すサブグループを選択します。</li> 
        <li value="2">書き出しアイコン <img src="assets/export.png"> をクリックし、目的のファイル形式を選択します。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブグループをコピーして新しいトップレベルグループを作成する</td> 
      <td> <p>（Workfront 管理者のみが使用できます。）サブグループをコピーすると、それが親グループになります。すべてのグループメンバーとサブグループが一緒にコピーされます。グループのメンバーは、元のグループでの割り当てをすべて保持します。</p> <p>サブグループのコピーについて詳しくは、この記事の<a href="#about-copying-a-subgroup" class="MCXref xref">サブグループのコピーについて</a>を参照してください。</p> 
       <ol> 
        <li value="1">サブグループを選択し、コピーアイコン <img src="assets/copy-icon.png"> をクリックして、選択したグループに基づいて新しいトップレベルグループを作成します。</li> 
        <li value="2"> <p>新しいグループの設定を構成します。</p> <p>これらの設定のヘルプについては、記事<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">既存のグループまたはサブグループをコピーして最上位グループを作成</a>の記事の、<a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">既存のグループまたはサブグループをコピーして最上位グループを作成</a>の節の表を参照してください。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブグループの削除</td> 
      <td> <p><b>重要</b>：グループまたはサブグループを削除する場合は、現在そのグループに割り当てられているユーザー、作業アイテム、およびサブグループを保存する必要があります。それらが確実に保持されるように、次の手順でグループのオブジェクトを別のグループに再割り当てするように求めるプロンプトが表示されます。</p> 
       <ol> 
        <li value="1">サブグループを選択し、削除アイコン <img src="assets/delete.png"> をクリックします。</li> 
        <li value="2">表示される<strong>グループの削除</strong>ボックスで入力を開始し、削除するグループのメンバー、作業アイテム、およびサブグループを移動するグループの名前を選択します。</li> 
        <li value="3">「<strong>削除</strong>」をクリックします。</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>サブグループを含むグループを管理する場合、グループ全体とそのすべてのサブグループに関するデータを識別してフィルターできると便利です。これを行うには、レポートまたはリストの「上位の親 ID」フィールドを使用します。
>
>例えば、大規模なマーケティング部門を管理しており、部門全体が取り組んでいるすべてのプロジェクトのリストが必要だと想像してください。
>
>Workfront では、このマーケティング部門はマーケティングというグループで表され、フィールドマーケティング、プロダクト マーケティング、デジタルマーケティングという 3 つのサブグループがあります。マーケティング部門全体（4 つのグループすべて）に属するプロジェクトをリストするには、次のフィルタールールを使用してプロジェクト領域のフィルターを作成できます。
>
>```
>Group: Top Parent ID > Equal > Marketing
>```
>
>「上位の親名」フィールドを使用して、最上位のグループに関連付けられたデータを識別することもできますが、ビューのみで使用され、フィルターやグループ化では使用できません。

## サブグループを親グループから削除し、それを最上位グループにします

親グループからサブグループを削除して、そのサブグループを最上位グループにすることもできます。

>[!TIP]
>
>その下にサブグループがあるグループを非アクティブ化すると、それらのサブグループも非アクティブになります。いずれかをアクティブ化したい場合は、次の手順を使用してその親グループから削除し、再度アクティブ化することができます。
>
>グループを非アクティブ化および再アクティブ化する手順については、[グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)の記事の、[グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view)および[グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive)を参照してください。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 左側のパネルで、**グループ** ![](assets/groups-icon.png)をクリックします。

1. 最上位グループにしたいグループの親グループを選択し、編集アイコン ![](assets/edit-icon.png) をクリックします。
1. 表示される&#x200B;**グループの編集**&#x200B;ボックスの&#x200B;**グループメンバーとグループ管理者**&#x200B;で、最上位グループにしたいサブグループの名前を入力し始め、次に名前が表示されたら、その名前の右側にある「X」をクリックします。
1. 「**保存**」をクリックします。

## グループのサブグループメンバーを表示および管理する

管理しているグループのメインページを表示しているときに、グループのサブグループ内のすべてのユーザーを表示および管理できます。手順については、[サブグループメンバーの表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md)を参照してください。

## サブグループのコピーについて {#about-copying-a-subgroup}

サブグループをコピーするときは、次の点を考慮してください。

* コピーするサブグループに独自のサブグループがある場合、それらもコピーに含まれ、その名前の形式は次のようになります。

  ```
  Original subgroup name (Copy)
  ```

* 公開グループに属するサブグループもパブリックであるため、グループ内外にかかわらず、ユーザー編集アクセス権を持つユーザーは誰でもサブグループにユーザーを追加できます。
