---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 担当業務を削除
description: 組織で使用されなくなった担当業務を削除できます。担当業務が過去に作業アイテムに関連付けられていた場合は、削除しないことをお勧めします。作業の割り当てに関する履歴情報をすべて保持するには、役割が不要になった場合は、削除するのではなく、非アクティブ化することをお勧めします。役割の非アクティブ化について詳しくは、担当業務の非アクティブ化を参照してください。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 95%

---

# 担当業務の削除

組織で使用されなくなった担当業務を削除できます。担当業務が過去に作業アイテムに関連付けられていた場合は、削除しないことをお勧めします。

作業の割り当てに関する履歴情報をすべて保持するには、役割が不要になった場合は、削除するのではなく、非アクティブ化することをお勧めします。役割の非アクティブ化について詳しくは、[担当業務を非アクティブ化](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)を参照してください。

## アクセス要件

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>担当業務への管理アクセス</td>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 担当業務を削除する

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. 「**[!UICONTROL 担当業務]」をクリックします。**
1. 削除する担当業務を選択し、「**[!UICONTROL 削除]」をクリックします。**
1. 担当業務に割り当てられているオブジェクト（ユーザー、タスク、イシュー）がある場合は、次のいずれかの操作を行います。

   * **担当業務を別の担当業務で置き換える：**&#x200B;ドロップダウンリストから新しい担当業務を選択します。

     削除した担当業務に関連付けられている現在および過去のリソース割り当ては、選択した担当業務に転送されます。

     1 つの担当業務のみが割り当てられているユーザーは、選択した担当業務に再割り当てされます。2 番目の担当業務が割り当てられているユーザーは、選択した担当業務に再割り当てされません。

   * **担当業務とそのリソース割り当てを削除する：**&#x200B;ドロップダウンリストから「**[!UICONTROL なし]**」を選択します。

     >[!IMPORTANT]
     >
     >担当業務を削除すると、その担当業務に関連する現在および過去のリソース割り当てがすべてのプロジェクトに対して削除されます。

     例えば、タスクまたはイシューがその担当業務にのみ割り当てられている場合は、担当業務が削除された後で、タスクまたはイシューの割り当てが解除されます。

1. 「**[!UICONTROL はい、削除します]**」をクリックします。
