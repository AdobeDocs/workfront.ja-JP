---
title: レートカードへのアクセス権の付与
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Adobe Workfront 管理者は、Workfront の財務データへのユーザーのアクセス権を、ユーザーのアクセスレベルによって定義できます。
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
exl-id: b21e65d3-3c9f-4f3d-95d3-de4c09199622
source-git-commit: 85399542ce8e92de6da5a1de0960194e72958987
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 49%

---

# レートカードへのアクセス権の付与

Adobe Workfront管理者は、[ アクセスレベルの概要](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)で説明されているように、ユーザーのアクセスレベルを通じてレートカードへのユーザーのアクセス権を定義できます。

レートカードについて詳しくは、[ レートカードの管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>ワークフロー Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レートカードへのアクセス権を付与するための考慮事項

Workfrontでレートカードへのアクセスを許可する場合は、次の点を考慮してください。

* プロジェクトにレートカードを添付するには、ユーザーがレートカード、プロジェクト、財務データに対する編集アクセス権を持っている必要があります。
* レートカードへのアクセス権がなく、財務データへのアクセス権を編集できないユーザーは、レートカードをプロジェクトに添付することはできませんが、プロジェクト上の他のソースから取得した他の請求レートを編集することはできます。

## カスタムアクセスレベルを使用したレートカードへのユーザーアクセスの設定

1. [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)の説明に従って、アクセスレベルの作成または編集を開始します。
1. レートカードの右側にある![](assets/gear-icon-settings.png)表示&#x200B;**または**&#x200B;編集&#x200B;**ボタンの歯車アイコン**&#x200B;をクリックし、**設定を微調整**&#x200B;の下で付与する機能を選択します。

   ![ レート カード アクセスの微調整](assets/rate-card-access-fine-tune.png)

1. （オプション）作業中のアクセスレベルの他のオブジェクトやエリアのアクセス権を設定するには、[タスクへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)などの、[Adobe Workfront へのアクセス権を設定](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)にある記事に従って、作業を続けます。
1. 完了したら「**保存**」をクリックします。

   作成したアクセスレベルは、ユーザーに割り当てることができます。詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

## 共有レートカードへのアクセス

[ レートカードの共有](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md)で説明しているように、レートカードを他のユーザーに権限を付与することで、レートカードを他のユーザーと共有できます。

別のユーザーとオブジェクトを共有する場合、そのオブジェクトに対する受信者の権限は次の 2 つ項目の組み合わせによって決まります。

* オブジェクトについて受信者に付与する権限
* オブジェクトのタイプについての受信者のアクセスレベル設定
