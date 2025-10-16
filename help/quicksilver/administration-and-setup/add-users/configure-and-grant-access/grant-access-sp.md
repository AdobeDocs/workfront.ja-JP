---
title: シナリオプランナーへのアクセス権の付与
description: Adobe Workfront 管理者は、アクセスレベルを使用して、シナリオプランナーへのユーザーのアクセスを定義できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 94%

---

# シナリオプランナーへのアクセス権の付与

Adobe Workfront 管理者は、シナリオプランナーに対するユーザーのアクセスを定義するアクセスレベルを使用できます（[アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)を参照）。

シナリオプランナーへのアクセスに加えて、システム管理者以外のアクセスレベルのユーザーは、予算、コスト、担当業務のレートなど、プランに含まれる財務情報を確認するために、財務データへのアクセス権も必要です。詳しくは、[財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront パッケージ</p> </td> 
   <td>ビジネス以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>ライト以上</p>
   <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>Adobe Workfront Scenario Planner のライセンスを追加購入する必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>シナリオプランナーへの表示アクセス権またはそれ以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> <p>プランへの表示権限またはそれ以上</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタムアクセスレベルを使用して、シナリオプランナーへのユーザーアクセスを設定します。

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)で説明されるように、アクセスレベルの作成または編集を開始します。
1. **シナリオプランナー**&#x200B;の右側で、このアクセスレベルに使用するオプションをクリックします。

   >[!NOTE]
   >
   >リクエストライセンスタイプまたは外部ライセンスタイプには、シナリオプランナーへの表示または編集のアクセス権はありません。

1. （オプション）作業中のアクセスレベルで他のオブジェクトや他の領域のアクセス権を設定するには、[Adobe Workfront に対するアクセス権の設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)のリストに記載されている、[タスクへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)や[財務データへのアクセスの許可](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)などの記事を参照してください。
1. 完了したら「**保存**」をクリックします。

## ライセンスタイプ別のシナリオプランナーへのアクセス

各アクセスレベルのユーザーがシナリオプランナーで実行できる操作について詳しくは、[各オブジェクトタイプで使用できる機能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)の記事の[シナリオプランナーのエリア](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario)の節を参照してください。

## アクセスレベル設定別のシナリオプランナーへのアクセス

次の情報は、アクセスレベル設定を使用して、Workfront シナリオプランナー内の情報へのユーザーのアクセスを制御する方法を理解するのに役立ちます。

* [アクセスなし](#no-access)
* [表示アクセス権](#view-access)
* [編集アクセス権](#edit-access)

### アクセスなし {#no-access}

シナリオプランナーにアクセスできないユーザーの場合、そのユーザーがレイアウトテンプレートに追加されても、メインメニューのシナリオアイコンは表示されません。また、共有されたプランやイニシアチブも表示されません。プランへのリンクがシナリオプランナーへのアクセス権を持たないユーザーと共有されている場合、ユーザーはプランを表示または編集できません。

### 表示アクセス権 {#view-access}

シナリオプランナーへの表示アクセス権を持つユーザーは、次の操作を実行できます。

* メインメニュー ![](assets/esp-icon-in-main-menu.png) のシナリオアイコンを表示します。別のユーザーが共有するプランリンクをユーザーがクリックしない限り、プランエリアは空になります。
* 別のユーザーがリンクを共有した場合、プランを表示します。

  これには、プラン内の任意の担当業務情報が含まれます。

  また、受信者ユーザーが財務データにもアクセスできる場合は、担当業務のレートおよびコスト情報も含まれます。詳しくは、[財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。

### 編集アクセス権 {#edit-access}

シナリオプランナーの編集アクセス権を持つユーザーは、次の操作を実行できます。

* メインメニュー ![](assets/esp-icon-in-main-menu.png) のシナリオアイコンを表示して、プランデータにアクセスする場合に使用する。
* プランを作成する。
* 作成したプランを表示、編集、および削除する。
* 他のユーザーが共有リンクを使用してアクセスしたプランを表示、編集、削除ｓる。

  これには、プラン内の任意の担当業務情報が含まれます。

  また、受信者ユーザーが財務データにアクセスできる場合は、担当業務のレートおよびコスト情報も含まれます。詳しくは、[財務データへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。
