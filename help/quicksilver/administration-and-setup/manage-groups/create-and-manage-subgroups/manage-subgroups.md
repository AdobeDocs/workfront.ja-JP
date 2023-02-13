---
user-type: administrator
product-area: system-administration;user-management
keywords: 管理、サブグループ、編集
navigation-topic: create-and-manage-subgroups
title: サブグループの管理
description: サブグループのグループ管理者は、サブグループの作成、移動、表示、編集、コピー、名前変更、書き出し、削除を行うことができます。 また、親グループからサブグループを削除して、サブグループを最上位グループにすることもできます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 1%

---

# サブグループの管理

サブグループのグループ管理者は、サブグループの作成、移動、表示、編集、コピー、名前変更、書き出し、削除を行うことができます。

また、親グループからサブグループを削除して、サブグループを最上位グループにすることもできます。

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。 Workfront管理者（すべてのグループ）も同様です。

サブグループの詳細については、 [サブグループの概要](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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

## サブグループの作成、移動、表示、編集、コピー、名前変更、書き出し、削除

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

   表示されるリストで、管理しているグループと、そのグループに含まれているサブグループを確認できます。 Adobe Workfront管理者は、すべてのグループを表示できます。

1. 作業対象のサブグループを含むグループの名前をクリックします。

   または

   1 つ以上のサブグループを移動する場合は、移動先グループの名前をクリックします（後の手順で移動するサブグループを指定します）。

1. 左側のメニューで、 **サブグループ**.

1. 次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">新しいサブグループを作成</td> 
      <td> <p>新しいサブグループを表示しているグループから 1 レベル下に作成する場合は、 <strong>サブグループを追加</strong>.</p> <p>または、リスト内の別のサブグループの下に新しいサブグループを作成する場合は、そのサブグループを選択し、 <strong>を追加</strong><strong>ubgroup</strong>.</p> <p>サブグループの設定に使用できるオプションについて詳しくは、 <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">サブグループの作成</a>.</p> <p>グループ階層は 15 レベルを超えることはできませんが、1 つのレベルに対して、複数の並列グループを無制限に設定できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブグループを移動 </td> 
      <td> <p>既存のサブグループは、管理している別のグループの下に移動できます。</p> <p>グループ階層は 15 レベルを超えることはできませんが、1 つのレベルに対して、複数の並列グループを無制限に設定できます。</p> 
       <ol> 
        <li value="1"> <p>（オプション）サブグループを選択して、宛先グループにします。</p> <p>この手順をスキップした場合、手順 3 で選択したグループが宛先グループになります。</p> </li> 
        <li value="2">クリック <strong>サブグループを追加</strong> &gt; <strong>既存のグループ</strong>.</li> 
        <li value="3"> <p>内 <strong>既存のグループ</strong> 表示されるボックスに、移動するサブグループの名前を入力します。</p> <p>表示される結果には、宛先グループより上のグループは含まれません。</p> <p>適切なグループを選択していることを確認するには、グループにカーソルを移動して、情報アイコンをクリックします <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> </li> 
        <li value="4"> <p>移動するサブグループの名前をクリックし、リストに表示されるようにします。</p> </li> 
        <li value="5"> <p>宛先グループに移動する他のサブグループに対して、手順 c～d を繰り返します。</p> </li> 
        <li value="6">「<strong>保存</strong>」をクリックします。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブグループを編集</td> 
      <td> <p>編集するサブグループを選択し、編集アイコンをクリックします。 <img src="assets/edit-icon.png">.</p> <p>サブグループの設定に使用できるオプションについて詳しくは、 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">グループの作成</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">1 つ以上のサブグループのエクスポート</td> 
      <td> 
       <ol> 
        <li value="1">エクスポートするサブグループを選択します。</li> 
        <li value="2">書き出しアイコンをクリックします。 <img src="assets/export.png">をクリックし、目的のファイル形式を選択します。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブグループをコピーして新しいトップレベルグループを作成する</td> 
      <td> <p>(Workfront管理者のみ使用できます ) サブグループをコピーすると、そのサブグループは親グループになります。 すべてのグループメンバーとサブグループが、それと共にコピーされます。 グループメンバーは、元のグループ内での割り当てをすべて保持します。</p> <p>サブグループのコピーについて詳しくは、 <a href="#about-copying-a-subgroup" class="MCXref xref">サブグループのコピーについて</a> 」を参照してください。</p> 
       <ol> 
        <li value="1">サブグループを選択し、コピーアイコンをクリックします。 <img src="assets/copy-icon.png"> をクリックし、選択したグループに基づいて新しいトップレベルグループを作成します。</li> 
        <li value="2"> <p>新しいグループの設定を行います。</p> <p>これらの設定に関するヘルプについては、の表を参照してください。 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">既存のグループまたはサブグループをコピーして最上位グループを作成する</a> 記事内 <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">既存のグループまたはサブグループをコピーして最上位グループを作成する</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">サブグループの削除</td> 
      <td> <p><b>重要</b>:グループまたはサブグループを削除する場合は、現在割り当てられているユーザー、作業項目、およびサブグループを保持する必要があります。 保持されていることを確認するために、次の手順で、グループのオブジェクトを別のグループに再割り当てするプロンプトが表示されます。</p> 
       <ol> 
        <li value="1">サブグループを選択し、削除アイコンをクリックします。 <img src="assets/delete.png">.</li> 
        <li value="2">内 <strong>グループを削除</strong> ボックスが表示され、入力を開始し、削除するグループのメンバ、作業項目、およびサブグループを移動するグループの名前を選択します。</li> 
        <li value="3">クリック <strong>削除</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>サブグループを含むグループを管理する場合、グループ全体とそのサブグループ全体に関するデータを特定し、フィルタリングできると便利です。 これをおこなうには、レポートまたはリストの上位の親 ID フィールドを使用します。
>
>例えば、大規模なマーケティング部門を管理し、部門全体が取り組んでいるすべてのプロジェクトのリストが必要な場合を考えてみましょう。
>
>Workfrontでは、このマーケティング部門はマーケティングと呼ばれるグループに属し、フィールドマーケティング、製品マーケティング、デジタルマーケティングと呼ばれる 3 つのサブグループが存在します。 マーケティング部門全体（4 つのグループすべて）に属するプロジェクトをリストするには、次のフィルタールールを使用して「プロジェクト」領域のフィルターを作成します。
>
>
```
>Group: Top Parent ID > Equal > Marketing
>```
>
>また、「上位の親名」フィールドを使用して、最上位のグループに関連付けられているデータを識別できます。ただし、ビューでのみ識別でき、フィルターまたはグループでは識別できません。

## 親グループからサブグループを削除し、最上位グループにする

親グループからサブグループを削除することで、サブグループを最上位グループにすることができます。

>[!TIP]
>
>その下にサブグループを持つグループを非アクティブ化すると、それらのサブグループも非アクティブになります。 いずれかをアクティブにする場合は、これらの手順を使用して親グループから削除し、再アクティブ化できます。
>
>グループの非アクティブ化と再アクティブ化の手順については、 [グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) および [グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) 記事内 [グループの詳細の表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. トップレベルグループにするグループの親グループを選択し、編集アイコンをクリックします。 ![](assets/edit-icon.png).
1. 内 **グループを編集** 下に表示されるボックス **グループメンバーとグループ管理者**&#x200B;をクリックし、最上位グループにするサブグループの名前を入力し、名前の右側にある X をクリックします。
1. 「**保存**」をクリックします。

## グループのサブグループメンバーの表示と管理

管理するグループのメイン・ページを表示している場合は、グループのサブグループ内のすべてのユーザーを表示および管理できます。 手順については、 [サブグループメンバーの表示と管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## サブグループのコピーについて {#about-copying-a-subgroup}

サブグループをコピーする際は、次の点に注意してください。

* コピーするサブグループに独自のサブグループがある場合、それらはコピーに含まれ、名前は次のようにフォーマットされます。

   ```
   Original subgroup name (Copy)
   ```

* パブリックグループに属するサブグループもパブリックなので、編集ユーザーアクセス権を持つユーザーは誰でも、グループ内またはグループ外のユーザーでも、サブグループにユーザーを追加できます。
