---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: グループの移動
description: 管理対象の別のグループの下にグループを移動できます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 80%

---

# グループの移動

管理対象の別のグループの下にグループを移動できます。

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

## グループを別のグループの下に移動する

>[!NOTE]
>
>移動したグループのステータスがロックされている場合は、新しい親グループのステータスを継承します。
>
>移動したグループのステータスがロック解除されている場合、新しい親グループのステータスは継承されず、新しい親グループのステータスも継承されません。
>
>グループのステータスについて詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)および[グループのステータスの作成または編集](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)を参照してください。

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**![ グループ ](assets/groups-icon.png)」をクリックします。

1. グループを移動する宛先グループを選択し、編集アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。
1. 表示される&#x200B;**グループの編集**&#x200B;ボックスの&#x200B;**グループメンバーとグループ管理者**&#x200B;で、移動したいグループの名前を入力し始め、名前が表示されたらクリックします。
1. 「**保存**」をクリックします。

>[!TIP]
>
>サブグループを最上位グループにすることもできます。詳しくは、[サブグループの管理](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)の記事で[親グループからサブグループを削除し、最上位グループにする](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make)を参照してください。
