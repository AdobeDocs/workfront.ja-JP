---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: カスタムフォームの削除または非アクティブ化
description: カスタムフォームは、システムから削除または非アクティブ化できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# カスタムフォームの削除または非アクティブ化

カスタムフォームは、システムから削除または非アクティブ化できます。

>[!CAUTION]
>
>カスタムフォームを削除すると、フォームに関連付けられたオブジェクト上のすべてのカスタムデータも削除されます。 削除したデータは復元できません。 代わりに、カスタムフォームの非アクティブ化を検討してください。使用しなくなったカスタムフォームを非アクティブ化すると、関連するすべての履歴データが保持されます。

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
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。

## カスタムフォームの削除

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **カスタムForms。**
1. カスタムフォームを選択し、「 **削除**.
1. カスタムフォームと、そのカスタムフォームが添付されたオブジェクト上のすべての関連データを完全に削除する場合は、 **はい、削除します**.

## カスタムフォームの非アクティブ化

使用しなくなったカスタムフォームは、関連する履歴データを失わずに非アクティブ化できます。 非アクティブなカスタムフォームをオブジェクトに追加することはできませんが、既に添付されているオブジェクト上のフィールドには、データを表示して追加することはできます。

非アクティブなカスタムフォーム上のフィールドは、引き続きビューでインライン編集できます。 インライン編集中に非アクティブなカスタムフォームからフィールドを追加した場合、カスタムフォームが非アクティブになっていても、フォームが自動的にオブジェクトに添付されます。

カスタムフォームを再度アクティブ化しても、以前の設定が保持され、ユーザーは、非アクティブ化されなかったかのように操作できます。

カスタムフォームを非アクティブ化するには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 非アクティブ化するカスタムフォームの名前をクリックします。
1. 次をクリック： **フォーム設定** タブをクリックします。
1. を無効にします。 **アクティブ** オプション。
1. クリック **保存して閉じる**.
