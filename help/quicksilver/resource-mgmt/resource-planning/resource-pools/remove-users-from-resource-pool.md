---
product-area: resource-management
navigation-topic: resource-pools
title: リソースプールからのユーザーの削除
description: リソースプールに含めることのできるユーザー数に制限はありませんが、ユーザーのリストには最初の 2000 ユーザーのみが、アルファベット順に表示されます。
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 88%

---

# リソースプールからのユーザーの削除

{{preview-and-fast-release-Q424}}

リソースプールに含めることのできるユーザー数に制限はありませんが、ユーザーのリストには最初の 2000 ユーザーのみが、アルファベット順に表示されます。

すべてのリソースプールで常に正確なユーザーのリストを確保できるように、非アクティブ化されたユーザー、役割や部門を移動したユーザーを削除することをお勧めします。

リソースプールについて詳しくは、[ リソースプールの概要](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：任意</p>
       <p>または</p>
       <p>現在：Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>リソース プール管理へのアクセスを含むリソース管理へのアクセスを編集します</p> <p>ユーザーに対する表示以上のアクセス権</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リソースプールからユーザーを削除

ユーザーがリソースプールで不要になった場合は、そのユーザーをリソースプールから削除できます。

リソースプールからユーザーを削除するには、次の手順に従います。

{{step1-to-resourcing}}

1. 左側のパネルで「**リソースプール**」をクリックします。
1. リソースプールを選択し、「**編集**」をクリックします。
または\
   リソースプールの名前をクリックします。

1. 削除するユーザーの名前を「**このリソースプール内を検索**」フィールドに入力します。\
   または\
   エンティティに関連付けられているすべてのユーザーを削除する場合は、会社、担当業務、チーム、またはグループの名前を入力します。

   <span class="preview"> プレビュー環境のサンプル画像：<span>

   ![ リソース プールからユーザーを削除 ](assets/remove-users-from-resource-pool.png)

   実稼動環境のサンプル画像：
   ![ リソース プール内の検索 ](assets/search-inside-new-resource-pool-350x314.png)

1. ユーザーレベルで「x」アイコンをクリックして、リソースプールからユーザーを削除します。 それらは、表示されるすべてのリストから削除されます。\
   または\
   担当業務、グループ、チーム、または会社に関連付けられているすべてのユーザーを削除するには、担当業務、グループ、チームレベル、または会社レベルで「**削除**」をクリックします。これにより、その担当業務、グループ、チーム、または会社に関連付けられているすべてのユーザーが、リソースプールから削除されます。

1. 「**保存**」をクリックします。
