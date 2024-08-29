---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Workfront Goals での目標の共有
description: 目標を共有する場合、目標を作成していないユーザーに対して、目標に対する管理権限を付与します。
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 90%

---

# Adobe Workfront Goals での目標の共有

目標を共有する場合、目標を作成していないユーザーに対して、目標に対する管理権限を付与します。

## アクセス要件

次のものが必要です。

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
   <p>新しいプランとライセンス構造の場合：
  <ul><li>究極の計画 </li></ul>
   </p>
<p>現在のプランおよびライセンス構造の場合： 
<ul><li> プロまたはそれ以上 </li>
  <li>Workfront ライセンスに加えて、Adobe Workfront Goals ライセンス。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront プラン*</td>
 <td>
 <p>新規ライセンス：コントリビューター以上</p>
 または
 <p>現在のライセンス：リクエスト以上</p> </td>
 </tr>
 <tr>
 <td role="rowheader">製品*</td>
 <td>
 <p> 新製品の要件は、次のいずれかです。 </p>
<ul>
<li>Select または Prime Adobe Workfront プランと、追加のAdobe Workfront Goals ライセンス。</li>
<li>Workfront Goals をデフォルトで含む究極のWorkfront プラン。 </li></ul>
 <p>または</p>
 <p>現在の必要な製品：Workfront プランとAdobe Workfront Goals の追加ライセンス。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">アクセスレベル</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">オブジェクト権限</td>
 <td>
  <div>
  <p>目標の表示には表示権限以上が必要</p>
  <p>目標に対する編集権限を管理</p>
  <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者を含むすべてのユーザーには、メインメニューに「目標」エリアが含まれるレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 目標の共有に関する考慮事項

* ユーザーは、目標に対して次の権限を持つことができます。

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>目標の権限</b></p></td> 
      <td>
      <p><b>説明</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>表示</p></td> 
      <td>
      <p>ユーザーには目標を表示する権限がありますが、目標の情報を編集することはできません。また、結果やアクティビティに関する情報の追加や編集、ステータスの更新、目標の削除を行うことはできません。</p>      
      <p>デフォルトでは、目標へのアクセス権を持つすべてのユーザーが、システム内のすべての目標を表示できます。アクセスレベルで目標に対する編集アクセス権を持っている場合、ユーザーは目標をコピーできます。</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>管理</p></td> 
      <td> <p>ユーザーは、結果やアクティビティを含む、目標に関するすべての情報を編集できます。これには削除も含まれます。</p> 
      <p>目標の作成者、または特に目標に対する管理権限を付与されたユーザーのみが、目標を管理できます。</p> 
      目標に対する管理権限を持つユーザーのみが、目標を他のユーザーと共有して、目標に対する管理権限を付与できます。 </p> </td> 
   </tr> 
   </tbody> 
   </table>

* 以下のタイプの目標を他のユーザーと共有できます。

   * 自身が作成した目標
   * 他のユーザーが作成し、管理権限を付与されている目標。

* 目標に対する管理権限を持っている場合は、目標の作成者が持つ目標に対する権限を変更できます。デフォルトでは、目標の作成時に管理権限を持っていますが、権限を表示に変更することができます。

## 目標を共有する

1. 右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)／**目標**&#x200B;をクリックします。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   目標リストが表示されます。

1. リストで目標の名前をクリックします。目標ページが開きます。

1. 目標名の横の&#x200B;**詳細アイコン**&#x200B;をクリックし、「**共有**」をクリックします。

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   目標アクセスボックスが表示されます。

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. 次のいずれかの操作を行います。

   * **システム全体の管理**&#x200B;設定を選択して、アクセスレベルで目標への編集アクセス権を持つシステム内の全員に、管理権限を付与します。これは、すべての新しい目標に対してデフォルトでは選択されていません。
   * 管理権限を付与するユーザーの名前を「**管理権限を与える**」ボックスに入力し始めます。名前がリストに表示されたら、選択します。

     >[!TIP]
     >
     >他のユーザーとのみ目標を共有できます。目標をグループや、チーム、会社と共有することはできません。

1. 「**共有**」をクリックします。

   目標は指定したユーザーと共有されます。目標の詳細パネルの「管理アクセス権」フィールドに、「システム全体」のラベルまたは目標に対する管理権限を持つユーザーの名前が表示されます。

## 目標の権限オプション

次の表に、目標を共有する際に付与できる権限を示します。ユーザーがライセンスに基づいて取得するアクセスについて詳しくは、[Adobe Workfront Goals へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)を参照してください。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>アクション</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>ビュー</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>目標を表示</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>結果やアクティビティを表示</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>目標をコピー* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>結果やアクティビティを他の目標に変換*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>アクティビティとして追加されたプロジェクトを表示** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>目標を編集</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>結果やアクティビティを編集</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>目標の結果やアクティビティを追加</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>プロジェクトをアクティビティとして目標に関連付け**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>目標を削除</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>結果やアクティビティを削除</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>目標からプロジェクトを切断</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*結果やアクティビティを目標に変換するには、アクセスレベルで目標に対する編集アクセス権が必要です。

**プロジェクトを表示するアクセス権と、追加されたプロジェクトまたは目標に追加して表示するプロジェクトに対する表示権限を持っている必要があります。

プロジェクトのアクセスレベルについては、[プロジェクトへのアクセス権を付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)を参照してください。

プロジェクト権限については、[Adobe Workfront でプロジェクトを共有](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。

 
