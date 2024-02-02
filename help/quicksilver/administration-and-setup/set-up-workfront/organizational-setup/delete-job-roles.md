---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 担当業務の削除
description: 組織で使用されなくなった担当業務を削除できます。担当業務が過去に作業アイテムに関連付けられていた場合は、削除しないことをお勧めします。作業の割り当てに関する履歴情報をすべて保持するには、役割が不要になった場合は、削除するのではなく、非アクティブ化することをお勧めします。役割の非アクティブ化について詳しくは、担当業務の非アクティブ化を参照してください。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: ht
source-wordcount: '398'
ht-degree: 100%

---

# 担当業務の削除

組織で使用されなくなった担当業務を削除できます。担当業務が過去に作業アイテムに関連付けられていた場合は、削除しないことをお勧めします。

作業の割り当てに関する履歴情報をすべて保持するには、役割が不要になった場合は、削除するのではなく、非アクティブ化することをお勧めします。役割の非アクティブ化について詳しくは、[担当業務を非アクティブ化](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>担当業務の管理アクセス権</p> <p><b>メモ</b>：それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 担当業務を削除する

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

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
