---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 会社を非アクティブ化または再アクティブ化する
description: 関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。 既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されているのと同じように機能します。 削除もブロックもされません。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 会社を非アクティブ化または再アクティブ化する

関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。 既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されているのと同じように機能します。 削除もブロックもされません。

## アクセス要件

で会社を管理するには、次が必要です。 [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 計画*</p> </td> 
   <td>[!UICONTROL チーム ] 以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] ライセンス*</p> </td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>次のいずれかを実行します。</p> 
    <ul> 
     <li> <p>[!UICONTROL システム管理者 ] のアクセスレベル。システム内の任意の会社を編集できます。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>. </p> </li> 
     <li> <p>会社を管理するための管理者アクセス。システム内の任意の会社を編集できます。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </li> 
    </ul> <p><b>メモ</b>:  
     <ul> 
      <li> <p>また、グループ管理者として割り当てられている任意のグループに関連する会社を管理することもできます。</p> </li> 
      <li> <p>ユーザーを [!DNL Workfront] システムには、次のいずれかが必要です。</p> 
       <ul> 
        <li> <p>[!UICONTROL System Administrator] アクセスレベル。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>. </p> </li> 
        <li> <p>アクセスレベルで、[!UICONTROL Users] 設定で [!UICONTROL Edit] が選択されている必要があります。 また、[!UICONTROL Users] 設定の場合は、[!UICONTROL 設定の微調整 ] <img src="assets/gear-icon-in-access-levels.png"> に設定されている場合は、[!UICONTROL 作成 ] オプションと、2 つの [!UICONTROL ユーザー管理 ] オプションのうち少なくとも 1 つを有効にする必要があります。 </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>[!UICONTROL ユーザー管理（グループユーザー）] オプションを使用している場合は、ユーザーがメンバーとなっているグループのグループ管理者である必要があります。</p> </li> 
       </ul> <p>アクセスレベルでのユーザー設定について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセスレベルの設定を確認するには、 [!DNL Workfront] 管理者。

## 会社を非アクティブ化または再アクティブ化する

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe] Workfront、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **[!UICONTROL 会社]** ![](assets/companies-icon-left-panel.png).

1. 非アクティブ化または再アクティブ化する会社を 1 つ以上選択します。
1. クリック **[!UICONTROL 編集]**.
1. 会社が 1 つの場合、 **[!UICONTROL アクティブ]** オプションを使用してアクティベートを解除するか、オプションを有効にしてアクティブ化します。

   または

   複数の会社の場合、 **[!UICONTROL いいえ]** から **[!UICONTROL アクティブ]** 非アクティブ化するドロップダウンメニュー、または **[!UICONTROL はい]** をクリックしてアクティブ化します。

1. クリック **[!UICONTROL 変更を保存]**.
