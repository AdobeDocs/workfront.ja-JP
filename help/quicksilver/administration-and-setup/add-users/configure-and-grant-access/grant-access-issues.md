---
title: イシューへのアクセスの許可
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、アクセスレベルを使用して、Workfront でユーザーのイシューへのアクセスを定義できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3c15f90f-ce87-484d-93a7-9eeb2963a798
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 94%

---

# イシューへのアクセスを許可

Adobe Workfront 管理者は、[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)で説明されるように、イシューに対するユーザーのアクセスを定義するために、アクセスレベルを使用できます。

カスタムアクセスレベルを使用して、Workfront の他のオブジェクトタイプへのユーザーのアクセスを管理する方法について詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

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
   <td>  <p>標準</p>
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

## カスタムアクセスレベルを使用して、ユーザーにイシューへのアクセス権を付与

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. **ビュー**&#x200B;の歯車アイコン ![](assets/gear-icon-settings.png) またはイシューの右側の「**編集**」ボタンをクリックして、**設定を微調整**&#x200B;の下で付与する機能を選択します。

   ![ 問題設定の微調整 ](assets/fine-tune-issues.png)

1. （オプション）上位のオブジェクトからのタスクに継承された権限を制限するには、「**追加制限を設定**」をクリックし、「**プロジェクト、タスク、イシューなどからドキュメントへのアクセス権を継承しない**」を選択します。

1. （オプション）作業中のアクセスレベルの他のオブジェクトやエリアのアクセス設定を指定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)にある記事のうちの 1 つ（[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)、[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)など）に従って、作業を続けます。
1. 完了したら「**保存**」をクリックします。

   作成したアクセスレベルは、ユーザーに割り当てることができます。詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## ライセンスタイプ別のイシューへのアクセス

各アクセスレベルのユーザーがイシューに対して実行できる内容については、[各オブジェクトタイプで利用可能な機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)の記事の[イシュー](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#issues)の節を参照してください。

## 共有されたイシューへアクセス

イシューの所有者または作成者として、イシューに対する権限を付与することで、[イシューを共有](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)で説明されているように、他のユーザーとイシューを共有できます。

<!--
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
-->

別のユーザーとオブジェクトを共有する場合、そのオブジェクトに対する受信者の権限は次の 2 つ項目の組み合わせによって決まります。

* オブジェクトについて受信者に付与する権限
* オブジェクトのタイプについての受信者のアクセスレベル設定

また、アクセスレベルで許可されている場合は、ユーザーはオブジェクト階層を通じてイシューへのアクセス権を取得できます。ユーザーがすでにイシューの親プロジェクトまたはタスクに対する権限を持っている場合、そのイシューに対する権限も持ちます（上記の手順 3 を参照）。イシューを共有すると、そのイシューに対する権限を継承したユーザーのリストが表示されます。

![](assets/inherited-permissions.png)
