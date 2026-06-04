---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 会社の非アクティブ化または再アクティブ化
description: 関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。 既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されていたのと同じように機能し続けます。 削除もブロックもされません。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
TQID: https://experienceleague.adobe.com/GrxcFYKSrmJsaITu6twBnTZxfkMcvsnRdfn7-qoSXI4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 335
ht-degree: 57%

---

# 会社を非アクティブ化または再アクティブ化

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

関連する履歴データをすべて保持したまま、使用しなくなった会社を非アクティブ化できます。 既にシステム内のどこかで使用されている会社を非アクティブ化しても、その会社は常に使用されていたのと同じように機能し続けます。 削除もブロックもされません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] パッケージ</p> </td> 
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
     <li> <p>[!UICONTROL システム管理者] アクセス レベル。システム内の任意の会社を編集できます。</p> </li> 
     <li> <p>会社を管理するための管理アクセス。システム内の任意の会社を編集できます。</p> </li> 
    </ul> <p><b>メモ</b>：
     <ul> 
      <li> <p>また、自分がグループ管理者として割り当てられている任意のグループに関連する会社を管理することもできます。</p> </li> 
      <li> <p>ユーザーを[!DNL Workfront] システムから追加および削除するには、次のいずれかの操作を行う必要があります。</p> 
       <ul> 
        <li> <p>[!UICONTROL System Administrator] アクセスレベル。 </p> </li> 
        <li> <p><b>[!UICONTROL Users]</b>設定をアクセスレベルで<b>[!UICONTROL Edit]</b> アクセスに設定し、<b>[!UICONTROL Create]</b>と、2つの<b>[!UICONTROL User Admin]</b> オプションのうち1つ以上を<b>[!UICONTROL Fine-tune your settings]</b><img src="assets/gear-icon-in-access-levels.png">で有効にします。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>これらの2つのオプションのうち、<b>[!UICONTROL User Admin （Group Users） ]</b>が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> </li> 
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

1. 左側のパネルで、**[!UICONTROL 会社]** ![会社アイコン ](assets/companies-icon-left-panel.png)をクリックします。

1. 非アクティブ化または再アクティブ化する会社を 1 つ以上選択します。
1. **[!UICONTROL 編集]**.<!--MAKE THIS A SEPARATE NUMBERED LINE<span class="preview">(Conditional) In the Preview environment, disable the **[!UICONTROL Is Active]** option to deactivate it, or enable the option to activate it.</span>-->をクリックします
1. 単一の会社の場合、**[!UICONTROL はアクティブです]** オプションを無効にして非アクティブにするか、オプションを有効にしてアクティブにします。<!--ADD TO THE FRONT OF THIS SENTENCE In the Production environment, -->

   または

   複数の会社の場合、**[!UICONTROL アクティブ]**&#x200B;ドロップダウンメニューから「**[!UICONTROL いいえ]**」を選択して、非アクティブ化するか、「**[!UICONTROL はい]**」を選択してアクティブ化します。

1. 「**[!UICONTROL 変更を保存]**」をクリックします。
