---
filename: configure-if-proofs-autogenerate
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: プルーフを自動的に生成するかどうかの設定
description: 指定したユーザーが Workfront にドキュメントを追加する場合、システムが自動的にプルーフを生成するかどうかを設定できます。この設定は、デフォルトで無効になっています。
author: Courtney
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 82%

---


# プルーフを自動的に生成するかどうかの設定

指定したユーザーが Workfront にドキュメントを追加する場合、システムが自動的にプルーフを生成するかどうかを設定できます。この設定は、デフォルトで無効になっています。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Adobe Workfront プラン</a> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">ライセンスの概要</a>*</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセス設定</td> 
   <td> <p>Workfront 管理者である必要があります。Workfront 管理者について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 1 人のユーザーに対してプルーフを自動的に生成するかどうかを設定

1. Adobe Workfrontの右上隅にある **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**ユーザー** ![ ユーザー ](assets/users-icon-in-main-menu.png) をクリックします。
1. プルーフアクセス権を持つユーザーを選択し、「**編集**」をクリックします。
1. 「**環境設定**」セクションで、**ドキュメントのアップロード時にプルーフを自動生成**&#x200B;チェックボックスを有効または無効にします。

   ![ 自動生成プルーフ ](assets/autogenerate-proofs-350x216.png)

1. 「**変更を保存**」をクリックします。

## 複数のユーザーに対してプルーフを自動的に生成するかどうかを設定

1. Adobe Workfrontの右上隅にある **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**ユーザー** ![ ユーザーアイコン ](assets/users-icon-in-main-menu.png) をクリックします。
1. プルーフアクセス権を持つユーザーを選択し、「**編集**」をクリックします。

   >[!IMPORTANT]
   >
   >すべてのユーザーがプルーフアクセス権を持っていない場合、「ドキュメントのアップロード中に自動的にプルーフを作成する」オプションは表示されません。

1. 「**環境設定**」セクションで、**ドキュメントのアップロード中に自動的にプルーフを作成する**&#x200B;チェックボックスをオンにして、「**はい**」または「**いいえ**」を選択します。

   ![ 自動生成プルーフの一括 ](assets/autogenerate-proofs-bulk-350x285.png)

1. 「**変更を保存**」をクリックします。

