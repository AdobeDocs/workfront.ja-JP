---
title: オブジェクトに対する財務権限の共有
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーに財務データの表示や編集のアクセス権を付与できます。詳しくは、「財務データに対するアクセスを許可」を参照してください。
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e974adc053a076a4370aa0c4ec41fea700d836be
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 56%

---

# オブジェクトに対する財務権限の共有

Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーに財務データの表示や編集のアクセス権を付与できます。詳しくは、[財務データへのアクセスを許可](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。

ユーザーに付与されるアクセスレベルに加えて、自分が共有のアクセス権を持つ特定のプロジェクトや、タスク、イシューの財務データを表示または管理する権限をユーザーに付与することもできます。

各アクセスレベルのユーザーが財務データに対して実行できる操作について詳しくは、[各オブジェクトタイプで使用できる機能](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)の記事にある[財務データ](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia)の節を参照してください。

## アクセス要件

<!--
drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>プラン</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクト、タスク、イシューおよび財務データへの表示以上のアクセス</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 少なくとも請求率の表示、コスト率の表示、一般的な財務権限の表示を含むプロジェクト、タスク、および問題に対する権限以上を表示します</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## オブジェクトの共有と財務権限の付与

オブジェクトに財務権限を付与する場合は、次の点を考慮してください。

* プロジェクト、タスク、イシューに財務権限を付与できます。
* 権限は継承できます。プロジェクトに対して一般財務を表示の権限がある場合、プロジェクトのタスクと問題に対して一般財務を表示の権限を自動的に継承します。
* 請求レートとコストレートに権限を付与すると、ユーザーはそのオブジェクトのレートを表示または編集できます。 一般財務の権限を持つユーザーは、オブジェクトの一般財務フィールド（請求または原価率に関連しない）を表示または編集できます。

オブジェクトに財務権限を付与するには、次の手順に従います。

1. 他のユーザーと共有するタスク、プロジェクト、またはイシューに移動します。
1. オブジェクトの名前の近くにある「**共有**」をクリックします。

1. 「**`<Object name>`に**&#x200B;へのアクセス権を付与」フィールドで、オブジェクトを共有するユーザー、チーム、役割、グループ、または会社の名前を入力し始めます。

   >[!TIP]
   >
   >オブジェクトを共有できるのは、アクティブなユーザー、チーム、役割、または会社のみです。

1. ユーザー名の右側にあるドロップダウンをクリックし、次のいずれかのオプションを選択します。

   * **表示**
   * **参加**
   * **管理**

1. 同じドロップダウンメニューで、権限レベルの横にある詳細オプションアイコンをクリックし、次のいずれかの操作を行います。

   * 任意の権限レベルに対して、**請求率を表示**、**コスト率を表示**&#x200B;および&#x200B;**必要に応じて一般財務を表示**&#x200B;を選択します。
   * **管理**&#x200B;権限のみを使用する場合は、**請求率の編集**、**コスト率の編集**、**一般財務の編集**&#x200B;を必要に応じて選択します。

1. 「**保存**」をクリックします。

## すべての共有レベルに対する財務の権限

次の表に、オブジェクトに対する表示、属性、または管理の権限を付与した場合にユーザーが取得する財務権限を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>アクション</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>参加</strong> </th> 
   <th><strong>ビュー</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>請求記録の管理</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>請求レートを編集</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>コスト率を編集</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>  
  <tr> 
   <td>一般財務を編集</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>
  <tr> 
   <td>請求料率を表示</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>コスト率を表示</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>  
  <tr> 
   <td>一般財務を表示</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>リソース計画ツールでコスト別に情報を表示する</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>リソース計画ツールでリソース予算計上*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>リソース計画ツールでのリソースの表示*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;追加のリソース管理アクセス権が必要です。

リソース管理アクセスについて詳しくは、[リソース管理へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)を参照してください。

<!--
These rows removed from last table.

  <tr> 
   <td>Manage/ View Role Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Manage/ View User Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 

-->
