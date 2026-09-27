---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: グループの削除
description: 管理対象のグループを削除できます。 管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront 管理者（すべてのグループ）も同様です。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f92eb1f5-fe98-4c7e-8ef7-8ed7134db8d4
TQID: 'https://experienceleague.adobe.com/TZRGyGC-yxRIq02ot7BmGHhxylkE10xyHkM0fO4y5P8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 78%
---
# グループを削除

管理対象のグループを削除できます。 管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront 管理者（すべてのグループ）も同様です。

サブグループの削除について詳しくは、[グループの管理](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md)を参照してください。

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
   <td>グループのグループ管理者またはシステム管理者でなければなりません。</td>
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループを削除

{{step-1-to-setup}}

1. 左側のパネルで、**グループ** ![ グループ ](assets/groups-icon.png)をクリックします。

1. 削除するグループを選択し、削除アイコン ![削除](assets/delete.png)をクリックします。

   >[!IMPORTANT]
   >
   >グループまたはサブグループを削除する場合は、現在割り当てられているユーザー、作業アイテムおよびサブグループを保持する必要があります。 それらが確実に保持されるように、次の手順でグループのオブジェクトを別のグループに再割り当てするように求めるプロンプトが表示されます。

1. 表示される「**グループの削除**」ボックスに入力を開始し、削除するグループのメンバー、作業アイテムおよびサブグループを移動するグループ名を選択します。

   適切なグループを選択していることを確認するには、そのグループにカーソルを合わせ、その横に表示される情報アイコン ![情報アイコン ](assets/info-icon.png)をクリックします。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。

1. 「**これらを削除します**」をクリックします。
