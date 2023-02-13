---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: オブジェクトの継承された権限の表示
description: Adobe Workfront管理者は、アクセスレベルを割り当てる際に、オブジェクトの表示や編集のアクセス権を付与できます。 詳細については、「プロジェクトへのアクセス権の付与」を参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: 7025f097-ea99-41bf-965e-617b0f532ff7
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# オブジェクトの継承された権限の表示

Adobe Workfront管理者は、アクセスレベルを割り当てる際に、オブジェクトの表示や編集のアクセス権を付与できます。 詳しくは、 [プロジェクトへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

ユーザーに付与されるアクセスレベルに加えて、共有するアクセス権を持つ特定のオブジェクトに対してユーザーに権限を付与することもできます。 アクセスレベルと権限の詳細については、 [アクセスレベルと権限の連携](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

オブジェクトは、Adobe Workfrontの親オブジェクトから権限を継承します。

Workfrontのオブジェクトの階層について詳しくは、 [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p>
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access on the objects you want to view permissions for</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the objects you want to view permissions for</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>権限を表示するオブジェクトの表示または高いアクセス権</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>権限を表示するオブジェクトに対する権限を表示するか、それ以上に設定します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## オブジェクトの継承された権限の表示

継承された権限の表示は、すべてのオブジェクトで同じです。

プロジェクトの継承された権限を表示するには：

1. 共有権限を表示するプロジェクトに移動します。
1. 次をクリック： **詳細** メニュー ![](assets/more-icon.png)を選択し、「 **共有**.

1. を展開します。 **継承された権限** リスト。

   このリストには、プロジェクトが属するポートフォリオまたはプログラムにアクセスでき、プロジェクトに対する権限を持つユーザーの名前が表示されます。

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

1. （オプション）継承された権限をオブジェクトから削除するには、 [オブジェクトから権限を削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   >[!NOTE]
   >
   >継承された権限を削除するには、オブジェクトに対する管理権限が必要です。

 

 
