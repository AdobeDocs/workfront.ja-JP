---
title: ユーザーのアクセスレベルとライセンスを一覧表示する
user-type: administrator
content-type: reference
product-area: system-administration
keywords: アクセス，レベル，ライセンス
navigation-topic: access-levels
description: ユーザーリストまたはレポートで、各ユーザーに割り当てられているアクセスレベルとライセンスを確認できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5d85509d-276a-411e-813c-8b1fa2f512db
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# ユーザーのアクセスレベルとライセンスを一覧表示する

ユーザーリストまたはレポートで、各ユーザーに割り当てられているアクセスレベルとライセンスを確認できます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ユーザーへのアクセスを表示します。 ユーザーの表示に関する詳細は、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## ユーザーのアクセスレベルとライセンスを一覧表示する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **ユーザー**.

   デフォルトでは、「アクティブ」と設定されたすべてのユーザーがリストに表示されます。

1. 内 **表示** ドロップダウンメニューで、「 **ライセンス**.

   [ ライセンス ] 列には、各ユーザに割り当てられたライセンスの名前が表示されます。

1. 内 **グループ化** ドロップダウンメニューで、 **ライセンスの種類**.

   このビューは、同じライセンスタイプを持つユーザをグループ化します。

1. （オプション）特定のライセンスでリストをフィルタリングするには、次の手順を実行します。

   1. 次をクリック： **フィルター** ドロップダウンメニューで、 **新しいフィルター**.

   1. クリック **フィルタールールを追加**.
   1. 入力を開始 **ライセンス** リストに表示されたら、選択します。
   1. を使用 **次と等しい** 修飾子を選択した場合は、リストをフィルタするライセンスの名前を入力し始めます。

      複数のライセンスの種類を指定できます。

   1. クリック **フィルターを保存**.

      このリストには、フィルタで指定したライセンスの種類に関連付けられたユーザのみが表示されます。
   >[!TIP]
   >
   >また、ライセンスの種類別にリストをグループ化したり、特定のライセンスでフィルタリングすることもできます。

