---
title: レイアウトテンプレートに対する管理アクセス権の付与
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Adobe Workfront 管理者は、特定のグループのグループ管理者にレイアウトテンプレートの管理者アクセス権を付与して、テンプレートを編集できるようにすることができます。 これは、グループ内のユーザーにはテンプレートは割り当てるものではありません。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
TQID: https://experienceleague.adobe.com/hV6I8IYKJWZBeIibkJh2KMfeVlimx1i0Yd-lIVQd4tE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 430
ht-degree: 92%

---

# レイアウトテンプレートの管理アクセス権の付与

Adobe Workfront 管理者は、特定のグループのグループ管理者にレイアウトテンプレートの管理者アクセス権を付与して、テンプレートを編集できるようにすることができます。 これは、グループ内のユーザーにはテンプレートは割り当てるものではありません。

レイアウトテンプレートへのユーザーの割り当てについて詳しくは、[レイアウトテンプレートへのユーザーの割り当て](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

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
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
        <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レイアウトテンプレートの管理アクセス権の付与

1. [レイアウトテンプレートを作成および管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されているように、レイアウトテンプレートの使用を開始します。
1. ページ上部のセクションで「**アクセス権付与先**」をクリックします。
1. 表示されるボックスで、「**グループを追加**」をクリックし、グループの名前を入力していきます。表示された名前をクリックし、「**完了**」をクリックします。

   指定したグループのグループ管理者として指定されたユーザーは、レイアウトテンプレートを管理できます。 ただし、テンプレートをグループのメンバーに割り当ててメンバーが使用できるようにすることはできません。 レイアウトテンプレートをグループに割り当てる方法については、[レイアウトテンプレートのユーザーへの割り当て](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign)を参照してください。

   >[!NOTE]
   >
   >* グループ管理者がレイアウトテンプレートを作成する場合は、管理アクセス権の割り当てが必須です。 レイアウトテンプレートは、指定したグループに対して指定され、指定したグループにのみ表示されます。 詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。 グループ管理者について詳しくは、[グループ管理者](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)を参照してください。
   >   
   >* 特定のグループ内のグループ管理者に管理アクセス権を付与しない場合、ユーザーアカウントを編集できるすべてのユーザーが、レイアウトテンプレートに対する管理アクセス権を持ちます。 Workfront 管理者によっては、レイアウトテンプレートをシステムレベルのレイアウトテンプレートにするために、レイアウトテンプレートに対する管理アクセス権を付与しないことを意図的に選択している場合があります。

1. レイアウトテンプレートのカスタマイズを続行します。 「**適用**」はいつでもクリックして、進行状況を保存できます。

   または

   カスタマイズが完了したら、**保存して閉じる**&#x200B;をクリックします。
