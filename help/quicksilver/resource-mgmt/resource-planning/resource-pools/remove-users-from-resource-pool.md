---
product-area: resource-management
navigation-topic: resource-pools
title: リソースプールからユーザーを削除する
description: 1 つのリソースプールに含めることのできるユーザー数に制限はありませんが、ユーザーのリストには最初の 2000 人のユーザーのみが表示され、アルファベット順に一覧表示されます。
author: Alina
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# リソースプールからユーザーを削除する

1 つのリソースプールに含めることのできるユーザー数に制限はありませんが、ユーザーのリストには最初の 2000 人のユーザーのみが表示され、アルファベット順に一覧表示されます。

すべてのリソースプールで常に正確なユーザーのリストを得るために、非アクティブ化されたユーザー、または役割や部門を移動したユーザーを削除することをお勧めします。

リソースプールの詳細については、 [リソースプールの概要](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソースプールの管理へのアクセスを含むリソース管理へのアクセスを編集</p> <p>ユーザーへのアクセス権を表示するか、それ以上に設定する</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## リソースプールからユーザーを削除する

ユーザーがリソースプールで不要になった場合は、そのユーザーをリソースプールから削除できます。

リソースプールからユーザーを削除するには、次の手順に従います。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **リソース**.
1. クリック **リソースプール** をクリックします。
1. リソースプールを選択し、「**編集」をクリックします。**または\
   リソースプールの名前をクリックします。

1. 削除するユーザーの名前を「 **このリソースプール内を検索** フィールドに入力します。\
   または\
   エンティティに関連付けられているすべてのユーザーを削除する場合は、会社、職務の役割、チーム、またはグループの名前を入力します。\
   ![search_inside_NEW_resource_pool.png](assets/search-inside-new-resource-pool-350x314.png)

1. ユーザーレベルで「x」アイコンをクリックして、リソースプールからユーザーを削除します。 それらは、それらが表示されるすべてのリストから削除されます。\
   または\
   ジョブの役割、グループ、チーム、または会社に関連付けられているすべてのユーザーを削除するには、 **削除** 職務の役割、グループ、チームレベル、または会社レベル。 これにより、そのジョブの役割、グループ、チーム、または会社に関連付けられているすべてのユーザーが、リソースプールから削除されます。

1. 「**保存**」をクリックします。
