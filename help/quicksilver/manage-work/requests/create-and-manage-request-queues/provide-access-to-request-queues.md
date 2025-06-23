---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: リクエストキューへのアクセスを提供
description: リクエストキューへのアクセスを提供する際に、組織内の誰が Adobe Workfront のリクエスト領域にリクエストキューを表示できるかを決定します。
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 52%

---

# リクエストキューへのアクセスを提供する

<!-- Audited: 6/2025 -->

リクエストキューへのアクセスを提供する際に、組織内の誰が Adobe Workfront のリクエスト領域にリクエストキューを表示できるかを決定します。

リクエストキューへの様々なユーザーのアクセスを、プロジェクトチーム、プロジェクトグループ、プロジェクト会社のどれに属しているかに応じて提供できます。 また、リクエストキューへのアクセスをシステム内の全員に提供することもできます。

これは、外部の関係者をWorkfrontに招待し、ユーザーのアクセスを特定の領域に制限したい組織で役立ちます。 この場合、リクエストキューは、プロジェクトの会社またはグループに関連付けられたユーザーにのみ開かれ、外部の関係者に対する表示が制限されます。 誰にでもアクセスできるようにすると、内部および外部の関係者にリクエストが表示されるようになります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>新規：標準 </p>
   <p>現在：プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p> プロジェクトの管理権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

リクエストキューをリクエスト領域のユーザーが使用できるようにするには、次の設定でプロジェクトを作成する必要があります。

* これをリクエストキューとして指定します。 詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。
* プロジェクトのステータスを「現在」に更新します。

## リクエストキューへのアクセスの提供

1. リクエストキューへのアクセスを提供するプロジェクトに移動します。

   >[!NOTE]
   >
   >リクエスト領域には、ステータスが「現在」のプロジェクトのみが表示されます。

1. 左側のパネルで **キューの詳細** をクリックします。
1. **ヘルプリクエストキューとして公開** を選択して、プロジェクトをリクエストキューとして指定します。
1. 表示される次のオプションから選択します。

   * **全員**：任意のユーザーがリクエストキューを表示し、リクエストを追加できます。
   * **このプロジェクトへの表示アクセス権を持つユーザー**：プロジェクトに対する表示権限を持つユーザーは、リクエストを表示し、リクエストキューに追加できます。
   * **このプロジェクトの会社のユーザー**: プロジェクトの会社に関連付けられているユーザーは、リクエストを表示および追加できます。 プロジェクトに関連付けられている会社が、このオプションの横の括弧内に表示されます。
   * **このプロジェクトのグループのユーザー**：プロジェクトのグループに関連付けられたユーザーは、リクエストを表示および追加できます。 プロジェクトに関連付けられているグループが、このオプションの横の括弧内に表示されます。

     グループキューは、複数の部門が Workfront アカウントを共有して一意の組織目標を達成する場合に役立ちます。 各部門には、他のグループのメンバーが見ることのできない独自のキューが存在する場合があります。

     プロジェクトに対する権限を持つユーザーについて詳しくは、[Adobe Workfront でのプロジェクトの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。

     グループと会社は、プロジェクトの編集時にプロジェクトに関連付けることができます。 詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

1. **保存**&#x200B;をクリックします。
