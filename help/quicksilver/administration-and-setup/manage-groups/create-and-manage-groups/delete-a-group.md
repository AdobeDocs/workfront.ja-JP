---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: グループの削除
description: 管理対象のグループを削除できます。 管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f92eb1f5-fe98-4c7e-8ef7-8ed7134db8d4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---

# グループの削除

管理対象のグループを削除できます。 管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

サブグループの削除について詳しくは、 [グループの管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md).

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

## グループの削除

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. 削除するグループを選択し、削除アイコン ![](assets/delete.png).

   >[!IMPORTANT]
   >
   >グループまたはサブグループを削除する場合は、現在割り当てられているユーザー、作業項目、およびサブグループを保持する必要があります。 保持されていることを確認するために、次の手順で、グループのオブジェクトを別のグループに再割り当てするプロンプトが表示されます。

1. 内 **グループを削除** ボックスが表示され、入力を開始し、削除するグループのメンバ、作業項目、およびサブグループを移動するグループの名前を選択します。

   適切なグループを選択していることを確認するには、グループにカーソルを移動して、情報アイコンをクリックします ![](assets/info-icon.png) その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。

1. クリック **削除**.
