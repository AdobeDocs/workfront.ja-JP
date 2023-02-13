---
title: リソース管理へのアクセス権の付与
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Adobe Workfront管理者は、アクセスレベルを使用して、Workfrontでのリソース管理に対するユーザーのアクセスを定義できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 3%

---

# リソース管理へのアクセス権の付与

Adobe Workfront管理者は、アクセスレベルを使用して、リソース管理に対するユーザーのアクセスを定義できます。詳しくは、 [アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタムアクセスレベルを使用して、リソース管理ツールへのユーザーアクセスを設定する

1. アクセスレベルの作成または編集を開始します ( [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 歯車アイコンをクリックします。 ![](assets/gear-icon-settings.png) の **表示** または **編集** 「リソース管理」の右にあるボタンをクリックし、許可するアビリティを **設定を微調整する**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">プランナー内の優先度と予算計上時間数を編集します</td> 
      <td> <p>このライセンスを持つユーザーに対し、次の操作を許可します。</p> <p>リソースプランナーのプロジェクトに優先順位を付けます。</p> <p>生産資源計画ツール（プロジェクトのビジネス・ケースの「生産資源計画担当」および「生産資源予算編成」セクション）の生産資源に対する予算割当。</p> <p>このオプションは、デフォルトで有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">リソース プールの管理</td> 
      <td> <p>このライセンスを持つユーザーがリソースプールを作成、編集、削除できるようにします。 このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>ワークロード バランサーの予定時間数を更新する</span> </td> 
      <td> <p>このライセンスを持つユーザーが、ワークロードバランサーでのユーザー割り当てを更新する際に、予定時間の作業項目を更新できるようにします。 割り当てられた時間の合計数は、作業項目の計画時間になります。</p> <p>このオプションはデフォルトでは無効になっています。</p> <p> 詳しくは、 <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）作業中のアクセスレベルの他のオブジェクトや領域のアクセス設定を構成するには、 [Adobe Workfrontへのアクセスの設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)例： [タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) および [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完了したら、「 **保存**.

   アクセスレベルを作成したら、そのレベルをユーザーに割り当てることができます。 詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## ライセンスタイプ別のリソース管理へのアクセス

各アクセスレベルのユーザーがリソース管理で実行できる操作について詳しくは、「 [リソース管理](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) 記事内 [各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 共有された問題へのアクセス

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

別のユーザーとオブジェクトを共有する場合、そのオブジェクトに対する予算または表示リソースの割り当てに関する受信者の権限は、次の 3 つの組み合わせによって決まります。

* リソース管理に関する受信者のアクセスレベル設定
* 財務データへのユーザーのアクセス。詳しくは、 [財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* 共有者がオブジェクトに対して付与した財務データに対する権限

ユーザーがオブジェクトを共有する際にオブジェクトの財務データに付与できる権限の詳細については、 [オブジェクトに対する財務権限の共有](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
