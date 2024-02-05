---
title: カスタムフォームの非アクティブ化または再アクティブ化
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: カスタムフォームを再アクティブ化または非アクティブ化できます。履歴データを保持するために、使用しなくなったカスタムフォームは非アクティブ化にして、削除しないことをお勧めします。
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 3319fbfad98350635b7194a434f26e8528753e7b
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 88%

---

# カスタムフォームの非アクティブ化または再アクティブ化

カスタムフォームを再アクティブ化または非アクティブ化できます。履歴データを保持するために、使用しなくなったカスタムフォームは非アクティブ化にして、削除しないことをお勧めします。

>[!NOTE]
>
>カスタムフォームが非アクティブ化されたが、まだキュートピックまたはリクエストキュー定義の一部である場合、新しいリクエストに添付されます。 フォームをリクエストに含めたくない場合は、リクエストキューから手動で削除する必要があります。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td>プラン</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> <p>Workfront 管理者がこのアクセス権を付与する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>を参照してください。</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセスレベル設定を確認するには、Workfront 管理者にお問い合わせください。

## カスタムフォームの非アクティブ化

使用しなくなったカスタムフォームは、関連する履歴データを失わずに非アクティブ化できます。非アクティブなカスタムフォームをオブジェクトに追加することはできませんが、既に添付されているオブジェクト上のフィールドには、データの表示と追加が可能です。

非アクティブなカスタムフォーム上のフィールドは、引き続きビューでインライン編集できます。インライン編集中に非アクティブなカスタムフォームからフィールドを追加した場合、カスタムフォームが非アクティブになっていても、フォームが自動的にオブジェクトに添付されます。

カスタムフォームを非アクティブ化するには：

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。
1. 左側のパネルで、「**カスタムフォーム**」を選択します。
1. 「**フォーム**」タブで、非アクティブ化するカスタムフォームを選択します。
1. アクティブ列で、**False** を選択して列の外をクリックします。フォームがアクティブではなくなりました。

## カスタムフォームの再アクティブ化

再アクティブ化したカスタムフォームでは以前の設定が保持され、ユーザーは、フォームが非アクティブ化されなかったかのように操作できます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックしたあと、**設定**&#x200B;アイコン ![](assets/gear-icon-settings.png) をクリックします。
1. 左側のパネルで、「**カスタムフォーム**」を選択します。
1. 「**フォーム**」タブで、再アクティブ化するカスタムフォームを選択します。
1. アクティブ列で、**True** を選択して列の外をクリックします。フォームがアクティブになりました。
