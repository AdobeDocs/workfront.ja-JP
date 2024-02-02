---
product-area: resource-management
navigation-topic: resource-pools
title: リソースプールとユーザーを関連付ける
description: リソースプールとユーザーを関連付ける
author: Alina
feature: Resource Management
exl-id: 0816a2d6-2a45-4e01-8ca2-6d0d190b2568
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '494'
ht-degree: 100%

---

# リソースプールとユーザーを関連付ける

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: The info about how to add resource pools to users, are duplicated from the articles listed in those sections (Creating Users, etc). I decided to keep the steps here because those articles are too long to rummage through for updating just this one field.)</p>
-->

リソースプールは、Adobe Workfront でのリソースの管理に役立つ、ユーザーのコレクションです。

リソースプールをユーザーに関連付ける前に、リソースプールを作成する必要があります。

リソースプールを作成すると、ユーザーをリソースプールに関連付けることができます。

ユーザーを設定せずにリソースプールを作成した場合は、後で新しいユーザーを編集または作成するときに、リソースプールにユーザーを関連付けることができます。

リソースプールについて詳しくは、[リソースプールの概要](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)を参照してください。

リソースプールの作成について詳しくは、[リソースプールの作成](../../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソースプールの管理へのアクセスを含む、リソース管理への編集アクセス権</p> <p>プロジェクト、テンプレート、ユーザーへのアクセスの編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リソースプールを関連付けるプロジェクト、テンプレート、およびユーザーの権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## リソースプールを 1 人のユーザーに関連付ける

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**ユーザー**」をクリックします。
1. リストのユーザー名の横にあるボックスをオンにし、「**編集**」をクリックします。
1. 「**リソース計画**」をクリックします。
1. ユーザーに関連付けるリソースプールの名前を「**リソースプール**」フィールドに入力し始め、表示されたらリストから選択します。\
   複数のリソースプールを 1 人のユーザーに関連付けることができます。\
   ![add_resource_pool_to_user.png](assets/add-resource-pool-to-user-350x307.png)

1. 「**変更を保存**」をクリックします。

ユーザーの編集について詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

新しいユーザーの作成について詳しくは、[ユーザーの追加](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。

## リソースプールとユーザーの一括関連付け

複数のユーザーを一括で編集し、すべてのユーザーを同じリソースプールに同時に関連付けることができます。

リソースプールを複数のユーザーに一括で関連付けるには：

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**ユーザー**」をクリックします。
1. リストから複数のユーザーを選択し、「**編集**」をクリックします。
1. 「**リソース計画**」をクリックします。
1. ユーザーに関連付けるリソースプールの名前を&#x200B;**リソースプール**&#x200B;フィールドに入力し始め、表示されたらリストから選択します。\
   複数のリソースプールを複数のユーザーに関連付けることができます。

   >[!NOTE]
   >
   >このフィールドには、選択したすべてのユーザーに共通するリソースプールのみが表示されます。選択したユーザーに共有のリソースプールがない場合、このフィールドは空になります。このフィールドが空の場合、ここで指定したリソースプールは、個々のリソースプールを上書きします。

1. 「**変更を保存**」をクリックします。

ユーザーを一括編集する方法について詳しくは、[ユーザープロファイルの一括編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)を参照してください。
