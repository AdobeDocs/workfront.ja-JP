---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: リクエストキューへのアクセスを提供
description: リクエストキューへのアクセスを提供する際に、組織内の誰がAdobe Workfrontの「リクエスト」領域にリクエストキューを表示できるかを決定します。
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# リクエストキューへのアクセスを提供

リクエストキューへのアクセスを提供する際に、組織内の誰がAdobe Workfrontの「リクエスト」領域にリクエストキューを表示できるかを決定します。

要求キューに対する様々なユーザーのアクセスを、プロジェクトチーム、プロジェクトグループ、プロジェクト会社のどちらに属しているかに応じて提供できます。 また、リクエストキューにシステム内のすべてのユーザーにアクセスを提供することもできます。 

これは、外部の関係者をWorkfrontに招待し、ユーザーのアクセスを特定の領域に限定する組織で役立ちます。この場合、プロジェクトの会社またはグループに関連付けられたユーザーに対してのみリクエストキューが開き、外部の関係者の表示を制限します。 誰にでもアクセスできるようにすると、内部および外部の関係者に要求が表示されます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p> プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください

## 前提条件

要求キューを要求領域のユーザーが使用できるようにするには、次の設定でプロジェクトを作成する必要があります。

* リクエストキューとして指定します。 リクエストキューの作成について詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* プロジェクトのステータスを「現在」に更新します。

## リクエストキューへのアクセスの提供

1. リクエストキューへのアクセスを提供するプロジェクトに移動します。

   >[!NOTE]
   >
   >「リクエスト」領域には、ステータスが「現在」のプロジェクトのみが表示されます。

1. クリック **キューの詳細** をクリックします。 クリックが必要になる場合があります **さらに表示**&#x200B;を、 **キューの詳細**.
1. 選択 **ヘルプリクエストキューとして公開** プロジェクトを要求キューに指定します。
1. 次のオプションから選択します。

   * **全員**:任意のユーザーがリクエストキューを表示し、リクエストを追加できます。
   * **このプロジェクトへの表示アクセス権を持つ担当者**：プロジェクトに対する表示権限を持つユーザーは、リクエストキューを表示し、リクエストに追加できます。 
   * **このプロジェクトの会社の担当者**：プロジェクトの会社に関連付けられたユーザーは、リクエストの表示と追加が可能です。 このオプションの横の括弧内に、プロジェクトに関連する会社が表示されます。 
   * **このプロジェクトのグループの担当者**：プロジェクトのグループに関連付けられているユーザーは、リクエストの表示と追加が可能です。 プロジェクトに関連付けられたグループは、このオプションの横の括弧内に表示されます。

      グループキューは、複数の部門がWorkfrontアカウントを共有して一意の組織目標を達成する場合に役立ちます。 各部門には、他のグループのメンバーが見えない独自のキューが存在する場合があります。

      プロジェクトに対する権限を持つユーザーについて詳しくは、 [Adobe Workfrontでプロジェクトを共有する](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      グループと会社は、プロジェクトの編集時にプロジェクトに関連付けることができます。 プロジェクトの編集の詳細については、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 「**保存**」をクリックします。
