---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 会社の非アクティブ化または再アクティブ化
description: 関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されていたのと同じように機能し続けます。削除もブロックもされません。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 83%

---

# 会社を非アクティブ化または再アクティブ化

関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されていたのと同じように機能し続けます。削除もブロックもされません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] プラン*</p> </td> 
   <td><p>現在：[!UICONTROL Team] 以上</p>
   <p>または</p>
   <p>新規：任意</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] ライセンス</p> </td> 
   <td><p>現在：[!UICONTROL Plan]</p>
   <p>または</p>
   <p>新規：[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル設定</strong> </td> 
   <td> <p>次のうちのいずれか：</p> 
    <ul> 
     <li> <p>[!UICONTROL システム管理者 ] アクセス レベル。システム内の任意の会社を編集できます。</p> </li> 
     <li> <p>会社を管理するための管理者アクセス。システム内の任意の会社を編集できます。</p> </li> 
    </ul> <p><b>メモ</b>：  
     <ul> 
      <li> <p>また、自分がグループ管理者として割り当てられている任意のグループに関連する会社を管理することもできます。</p> </li> 
      <li> <p>[!DNL Workfront] システムでのユーザーの追加および削除を行うには、次のいずれかが必要です。</p> 
       <ul> 
        <li> <p>[!UICONTROL System Administrator] アクセスレベル。</p> </li> 
        <li> <p>アクセスレベルの [!UICONTROL Users] 設定で、[!UICONTROL Edit] が選択されている必要があります。また、[!UICONTROL Users] 設定の場合は、[!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> 下の [!UICONTROL Create] オプションと、2 つの [!UICONTROL User Admin] オプションのうち少なくとも 1 つを有効にする必要があります。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>[!UICONTROL User Admin (Group Users)] オプションを使用している場合は、ユーザーがメンバーとなっているグループのグループ管理者である必要があります。</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 会社を非アクティブ化または再アクティブ化

{{step-1-to-setup}}

1. 左側のパネルで、**[!UICONTROL 会社]**![ 会社アイコン ](assets/companies-icon-left-panel.png) をクリックします。

1. 非アクティブ化または再アクティブ化する会社を 1 つ以上選択します。
1. 「**[!UICONTROL 編集]**」をクリックします。
1. 会社が 1 つの場合、「**[!UICONTROL アクティブ]**」オプションを無効にして非アクティブ化するか、オプションを有効にしてアクティブ化します。

   または

   複数の会社の場合、**[!UICONTROL アクティブ]**&#x200B;ドロップダウンメニューから「**[!UICONTROL いいえ]**」を選択して、非アクティブ化するか、「**[!UICONTROL はい]**」を選択してアクティブ化します。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
