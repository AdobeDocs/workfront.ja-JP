---
title: フィルター、ビュー、グループ化へのアクセス権を付与する
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、アクセスレベルを使用して、リストおよびレポートのフィルター、ビュー、グループ化コントロールに対するユーザーのアクセス権を定義できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: 14b3bfaf16a4ab8749538b32100ce6363a3a9335
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 75%

---

# フィルター、ビュー、グループ化に対するアクセス権を付与

[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)の説明に従って、Adobe Workfront 管理者は、アクセスレベルを使用して、リストおよびレポートのフィルター、ビュー、グループ化コントロールに対するユーザーのアクセス権を定義できます。

フィルター、ビュー、グループ化コントロールについて詳しくは、[レポート要素：フィルター、ビューおよびグループ化](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタムアクセスレベルを使用して、フィルター、ビュー、グループ化に対するユーザーアクセスを設定

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. 「フィルター」の右にある「**表示**」ボタンまたは「**編集**」ボタン上の歯車アイコン ![](assets/gear-icon-settings.png) をクリックし、付与する機能を「**設定を微調整**」の下で選択します。

   ![](assets/gear-icon-filters-dashboards-groupings.png)

   デフォルトでは、Standard、Plan、Work、Light、Reviewer、Contributor、またはRequest ライセンスを持つユーザーは、完全な表示および編集機能を持ちます。 外部ユーザーライセンスを持つユーザーは、フィルター、ビュー、グループ化にアクセスできません。

   <!--
   If this changes, undraft section with table below
   -->

1. （オプション）作業中のアクセスレベルで他のオブジェクトや他の領域のアクセス権を設定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)のリストに記載されている、[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)や[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)などの記事を参照してください。
1. 完了したら「**保存**」をクリックします。

   作成したアクセスレベルは、ユーザーに割り当てることができます。 詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## ライセンスタイプ別のフィルター、ビュー、グループへのアクセス

各アクセスレベルのユーザーがフィルター、ビュー、グループ化で実行できる操作について詳しくは、「[&#x200B; フィルター、ビュー、グループ化](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md#filters-views-and-groupings)」の各オブジェクトタイプで利用できる機能[を参照してください](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md)。

<!--

Drafting out this section for now because the table is redundant since all four license types can do everything.


This table lists what a Workfront administrator can allow users with each license type to do with filter, views, and groupings. For information about the Workfront license types, see [Adobe Workfront licenses overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> Action </th>
<th> Planner </th>
<th> Worker </th>
<th> Reviewer </th>
<th> Requester </th>
</tr>
</thead>
<tbody>
<tr>
<td>Edit filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Create filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>View filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Delete filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Share filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Share filters, views, and groupings system-wide</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>

-->