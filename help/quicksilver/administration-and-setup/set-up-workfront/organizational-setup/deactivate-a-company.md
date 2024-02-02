---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 会社を非アクティブ化または再アクティブ化
description: 関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されていたのと同じように機能し続けます。削除もブロックもされません。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: ht
source-wordcount: '410'
ht-degree: 100%

---

# 会社を非アクティブ化または再アクティブ化

関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されていたのと同じように機能し続けます。削除もブロックもされません。

## アクセス要件

[!DNL Workfront] で会社を管理するには、以下のものが必要です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] プラン*</p> </td> 
   <td>[!UICONTROL Team] 以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] ライセンス*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>次のうちのいずれか：</p> 
    <ul> 
     <li> <p>システム内の任意の会社を編集できる、[!UICONTROL System Administrator]のアクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。 </p> </li> 
     <li> <p>システム内の任意の会社を編集できる、会社を管理するための管理者アクセス。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>を参照してください。</p> </li> 
    </ul> <p><b>メモ</b>：  
     <ul> 
      <li> <p>また、自分がグループ管理者として割り当てられている任意のグループに関連する会社を管理することもできます。</p> </li> 
      <li> <p>[!DNL Workfront] システムからユーザーを追加あるいは削除するには、以下のいずれかが必要です。</p> 
       <ul> 
        <li> <p>[!UICONTROL System Administrator] アクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。 </p> </li> 
        <li> <p>アクセスレベルの [!UICONTROL Users] 設定で、[!UICONTROL Edit] が選択されている必要があります。また、[!UICONTROL Users] 設定には、[!UICONTROL Fine-tune your settings]<img src="assets/gear-icon-in-access-levels.png">の下で、[!UICONTROL Create] オプション、ならびに 2 つの [!UICONTROL User Admin] オプションのうち 1 つ以上を有効にする必要があります。 </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>[!UICONTROL User Admin (Group Users)] オプションを使用している場合は、ユーザーがメンバーとなっているグループのグループ管理者である必要があります。</p> </li> 
       </ul> <p>アクセスレベルでのユーザー設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセスレベル設定を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 会社を非アクティブ化または再アクティブ化

1. [!DNL Adobe]Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 左側のパネルで、**[!UICONTROL 会社]** ![](assets/companies-icon-left-panel.png) をクリックします。

1. 非アクティブ化または再アクティブ化する会社を 1 つ以上選択します。
1. 「**[!UICONTROL 編集]**」をクリックします。
1. 会社が 1 つの場合、「**[!UICONTROL アクティブ]**」オプションを無効にして非アクティブ化するか、オプションを有効にしてアクティブ化します。

   または

   複数の会社の場合、**[!UICONTROL アクティブ]**&#x200B;ドロップダウンメニューから「**[!UICONTROL いいえ]**」を選択して、非アクティブ化するか、「**[!UICONTROL はい]**」を選択してアクティブ化します。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
