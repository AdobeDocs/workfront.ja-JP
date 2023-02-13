---
title: レイアウトテンプレートの管理アクセス権の付与
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Adobe Workfront管理者は、特定のグループのグループ管理者にレイアウトテンプレートの管理者アクセス権を付与して、テンプレートを編集できるようにすることができます。 グループ内のユーザーにはテンプレートが割り当てられません。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# レイアウトテンプレートの管理アクセス権の付与

Adobe Workfront管理者は、特定のグループのグループ管理者にレイアウトテンプレートの管理者アクセス権を付与して、テンプレートを編集できるようにすることができます。 グループ内のユーザーにはテンプレートが割り当てられません。

レイアウトテンプレートへのユーザの割り当てについて詳しくは、 [レイアウトテンプレートにユーザーを割り当てる](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

レイアウトテンプレートについて詳しくは、 [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

グループのレイアウトテンプレートについて詳しくは、 [グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td><p>システム管理者のアクセスレベル</p><p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## レイアウトテンプレートの管理アクセス権の付与

1. レイアウトテンプレートの使用を開始する ( [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. クリック **へのアクセス権の付与** 」をクリックします。
1. 表示されるボックスで、 **グループを追加**&#x200B;で、グループの名前を入力し、表示されたら名前をクリックして、 **完了**.

   指定したグループのグループ管理者として指定されたユーザは、レイアウトテンプレートを管理できます。 ただし、テンプレートはグループのメンバーに割り当てられず、使用されます。 レイアウトテンプレートをグループに割り当てる方法については、 [レイアウトテンプレートをユーザーに割り当てる](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) 」を参照してください。

   >[!NOTE]
   >
   >* グループ管理者がレイアウトテンプレートを作成する場合、管理アクセス権の割り当ては必須です。 レイアウトテンプレートは、指定されたグループに対して指定され、指定されたグループにのみ表示されます。 詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). グループ管理者の詳細については、 [グループ管理者](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* 特定のグループ内のグループ管理者に管理者アクセス権を付与しない場合、ユーザーアカウントを編集できるすべてのユーザーは、レイアウトテンプレートに管理者アクセス権を持ちます。 一部のWorkfront管理者は、レイアウトテンプレートをシステムレベルのレイアウトテンプレートにするために、レイアウトテンプレートに対する管理者アクセスを許可しないことを意図的に選択しています。


1. 「保存」はいつでもクリックして進行状況を保存でき、後でテンプレートの変更を続行できます。
