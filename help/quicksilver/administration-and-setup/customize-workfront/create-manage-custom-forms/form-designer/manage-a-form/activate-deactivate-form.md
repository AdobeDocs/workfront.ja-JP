---
title: カスタムフォームのディアクティベートまたは再アクティベート
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: カスタムフォームを再アクティブ化または非アクティブ化できます。履歴データを保持するために、使用しなくなったカスタムフォームは非アクティブ化にして、削除しないことをお勧めします。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: a7be72f0a594a21baed2592d8a2e467118ab1b7f
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 95%

---

# カスタムフォームの非アクティブ化または再アクティブ化

カスタムフォームを再アクティブ化または非アクティブ化できます。履歴データを保持するために、使用しなくなったカスタムフォームは非アクティブ化にして、削除しないことをお勧めします。

>[!NOTE]
>
>カスタムフォームが非アクティブ化されているが、まだキュートピックまたはリクエストキュー定義の一部である場合、新しいリクエストに添付されます。フォームをリクエストに含めない場合は、リクエストキューから手動で削除する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p></td> 
  </tr>  
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタムフォームの非アクティブ化

使用しなくなったカスタムフォームは、関連する履歴データを失わずに非アクティブ化できます。非アクティブなカスタムフォームをオブジェクトに追加することはできませんが、既に添付されているオブジェクト上のフィールドには、データの表示と追加が可能です。

非アクティブなカスタムフォーム上のフィールドは、引き続きビューでインライン編集できます。インライン編集中に非アクティブなカスタムフォームからフィールドを追加した場合、カスタムフォームが非アクティブになっていても、フォームが自動的にオブジェクトに添付されます。

カスタムフォームを非アクティブ化するには：

{{step-1-to-setup}}

1. 左側のパネルで、「**カスタムフォーム**」を選択します。
1. 「**フォーム**」タブで、非アクティブ化するカスタムフォームを選択します。
1. アクティブ列で、**False** を選択して列の外をクリックします。フォームがアクティブではなくなりました。

## カスタムフォームの再アクティブ化

再アクティブ化したカスタムフォームでは以前の設定が保持され、ユーザーは、フォームが非アクティブ化されなかったかのように操作できます。

{{step-1-to-setup}}

1. 左側のパネルで、「**カスタムフォーム**」を選択します。
1. **フォーム**&#x200B;エリアで、再アクティブ化するカスタムフォームを選択します。
1. アクティブ列で、**True** を選択して列の外をクリックします。フォームがアクティブになりました。
