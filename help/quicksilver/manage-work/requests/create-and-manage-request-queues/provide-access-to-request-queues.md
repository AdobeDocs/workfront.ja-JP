---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: リクエストキューへのアクセスの提供
description: リクエストキューへのアクセスを提供する際に、組織内の誰が Adobe Workfront のリクエスト領域にリクエストキューを表示できるかを決定します。
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/FG-KGqoEVFkHh6-n2h77HMfSfncJmWznEvViz1Zl-Uk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 474
ht-degree: 54%

---

# リクエストキューへのアクセスを提供する

<!-- Audited: 6/2025 -->

リクエストキューへのアクセスを提供する際に、組織内の誰が Adobe Workfront のリクエスト領域にリクエストキューを表示できるかを決定します。

プロジェクト チーム、プロジェクト グループ、プロジェクト会社のいずれに属しているかに応じて、さまざまなユーザーにリクエストキューへのアクセス権を付与できます。 また、システム内のすべてのユーザーにリクエストキューのアクセス権を提供することもできます。

これは、外部の関係者をWorkfrontに招待し、ユーザーのアクセスを特定の領域に制限したい組織で便利です。 この場合、プロジェクトの会社またはグループに関連付けられているユーザーに対してのみ開かれているリクエストキューは、外部の関係者に対する表示を制限します。 誰にでもアクセスできるようにすると、内部および外部の関係者にリクエストが表示されるようになります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>標準 </p>
   <p>プラン </p> </td> 
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

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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

1. 左側のパネルで「**キューの詳細**」をクリックします。
1. 「**ヘルプリクエストキューとして公開**」を選択して、プロジェクトをリクエストキューとして指定します。
1. 表示される次のオプションから選択します。

   * **全員**：任意のユーザーがリクエストキューを表示し、リクエストを追加できます。
   * **このプロジェクトへの表示アクセス権を持つユーザー**: プロジェクトに対する表示権限を持つユーザーは、リクエスト キューにリクエストを表示および追加できます。
   * **このプロジェクトの会社のユーザー**: プロジェクトの会社に関連付けられているユーザーは、リクエストを表示および追加できます。 プロジェクトに関連付けられている会社は、このオプションの横に括弧で囲まれています。
   * **このプロジェクトのグループのユーザー**: プロジェクトのグループに関連付けられているユーザーは、リクエストを表示および追加できます。 プロジェクトに関連付けられているグループは、このオプションの横にある括弧で囲まれています。

     グループキューは、複数の部門が Workfront アカウントを共有して一意の組織目標を達成する場合に役立ちます。 各部門は、他のグループのメンバーが見ることのできない、独自のキューを持っている場合があります。

     プロジェクトに対する権限を持つユーザーについて詳しくは、[Adobe Workfront でのプロジェクトの共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。

     グループと会社は、プロジェクトの編集時にプロジェクトに関連付けることができます。 詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

1. 「**保存**」をクリックします。
