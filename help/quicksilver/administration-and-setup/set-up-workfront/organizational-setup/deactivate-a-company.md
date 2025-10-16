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
source-git-commit: 30b61b32add4c6d062b5b524773d309008c9563d
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 60%

---

# 会社を非アクティブ化または再アクティブ化

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されていたのと同じように機能し続けます。削除もブロックもされません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] package</p> </td> 
   <td><p>任意</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] ライセンス</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>アクセスレベル設定</td> 
  <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>[!UICONTROL システム管理者 ] アクセス レベル。システム内の任意の会社を編集できます。</p> </li> 
     <li> <p>会社を管理するための管理者アクセス。システム内の任意の会社を編集できます。</p> </li> 
    </ul> <p><b>メモ</b>：  
     <ul> 
      <li> <p>また、自分がグループ管理者として割り当てられている任意のグループに関連する会社を管理することもできます。</p> </li> 
      <li> <p>[!DNL Workfront] システムにユーザーを追加したり、システムからユーザーを削除したりするには、次のいずれかが必要です。</p> 
       <ul> 
        <li> <p>[!UICONTROL System Administrator] アクセスレベル。 </p> </li> 
        <li> <p>アクセスレベルの <b>[!UICONTROL ユーザー ]</b> 設定が <b>[!UICONTROL 編集 ]</b> アクセスに設定され、<b>[!UICONTROL 作成 ]</b> と、<b> </b>[!UICONTROL 設定 ]<b> で有効になっている 2 つの </b>[!UICONTROL ユーザー管理者 ]<img src="assets/gear-icon-in-access-levels.png"> オプションのうち少なくとも 1 つが設定されています。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>これら 2 つのオプションのうち、<b>[!UICONTROL User Admin （Group Users） ]</b> が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 会社を非アクティブ化または再アクティブ化

{{step-1-to-setup}}

1. 左側のパネルで、**[!UICONTROL 会社]**![ 会社アイコン ](assets/companies-icon-left-panel.png) をクリックします。

1. 非アクティブ化または再アクティブ化する会社を 1 つ以上選択します。
1. **[!UICONTROL 編集]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>--> をクリックします。
1. <!--In the Production environment, -->会社が 1 つの場合、「**[!UICONTROL アクティブ]**」オプションを無効にして非アクティブ化するか、オプションを有効にしてアクティブ化します。

   または

   複数の会社の場合、**[!UICONTROL アクティブ]**&#x200B;ドロップダウンメニューから「**[!UICONTROL いいえ]**」を選択して、非アクティブ化するか、「**[!UICONTROL はい]**」を選択してアクティブ化します。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
