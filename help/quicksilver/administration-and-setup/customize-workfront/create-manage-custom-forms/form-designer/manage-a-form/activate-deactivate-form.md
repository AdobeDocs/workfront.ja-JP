---
title: カスタムフォームの非アクティブ化または再アクティブ化
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: カスタムフォームを再アクティブ化または非アクティブ化できます。 履歴データの保持に使用しなくなったフォームは削除せず、カスタムフォームの非アクティブ化をお勧めします。
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# カスタムフォームの非アクティブ化または再アクティブ化

カスタムフォームを再アクティブ化または非アクティブ化できます。 履歴データの保持に使用しなくなったフォームは削除せず、カスタムフォームの非アクティブ化をお勧めします。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。

## カスタムフォームの非アクティブ化

使用しなくなったカスタムフォームは、関連する履歴データを失わずに非アクティブ化できます。 非アクティブなカスタムフォームをオブジェクトに追加することはできませんが、既に添付されているオブジェクト上のフィールドには、データを表示して追加することはできます。

非アクティブなカスタムフォーム上のフィールドは、引き続きビューでインライン編集できます。 インライン編集中に非アクティブなカスタムフォームからフィールドを追加した場合、カスタムフォームが非アクティブになっていても、フォームが自動的にオブジェクトに添付されます。

カスタムフォームを非アクティブ化するには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).
1. 左側のパネルで、を選択します。 **カスタムForms**.
1. 次の日： **Forms** 」タブで、非アクティブ化するカスタムフォームを選択します。
1. 「アクティブ」列で、を選択します。 **False** 列の外をクリックします。 フォームがアクティブではなくなりました。

## カスタムフォームの再アクティブ化

カスタムフォームを再アクティブ化しても、以前の設定が保持され、ユーザーは、非アクティブ化されなかったかのように操作できます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).
1. 左側のパネルで、を選択します。 **カスタムForms**.
1. 次の日： **Forms** 」タブで、再アクティブ化するカスタムフォームを選択します。
1. 「アクティブ」列で、を選択します。 **True** 列の外をクリックします。 これで、フォームがアクティブになります。
