---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: ジョブの役割を削除
description: 組織で使用されなくなったジョブの役割を削除できます。 過去に作業項目に関連付けられている場合は、ジョブの役割を削除しないことをお勧めします。 作業の割り当てに関する履歴情報をすべて保持するには、役割を無効にするのではなく、役割を無効にすることをお勧めします。 ロールの非アクティブ化について詳しくは、ジョブロールの非アクティブ化を参照してください。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# ジョブの役割を削除

組織で使用されなくなったジョブの役割を削除できます。 過去に作業項目に関連付けられている場合は、ジョブの役割を削除しないことをお勧めします。

作業の割り当てに関する履歴情報をすべて保持するには、役割を無効にするのではなく、役割を無効にすることをお勧めします。 ロールの非アクティブ化について詳しくは、 [ジョブの役割の非アクティブ化](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ジョブロールへの管理者アクセス</p> <p><b>注意</b>:まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## ジョブロールを削除

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL ジョブの役割].**
1. 削除するジョブの役割を選択し、 **[!UICONTROL 削除].**
1. ジョブの役割に割り当てられているオブジェクト（ユーザー、タスク、タスク）がある場合は、次のいずれかの操作を行います。

   * **ジョブの役割を別のジョブの役割で置き換えます。** ドロップダウンリストから新しいジョブの役割を選択します。

      削除されたジョブロールに関連付けられている現在および過去のリソース割り当ては、選択したジョブロールに転送されます。

      1 つのジョブロールのみが割り当てられているユーザーは、選択したジョブロールに再割り当てされます。セカンダリジョブの役割が割り当てられているユーザーは、選択したジョブの役割に再割り当てされません。

   * **ジョブの役割とそのリソース割り当てを削除します。** 選択 **[!UICONTROL なし]** 」を選択します。

      >[!IMPORTANT]
      >
      >ジョブロールを削除すると、そのジョブロールに関連する現在および過去のリソース割り当てがすべてのプロジェクトに対して削除されます。

      &#x200B;例えば、タスクまたはイシューがそのジョブの役割にのみ割り当てられている場合は、ジョブの役割が削除された後で、タスクまたはイシューの割り当てが解除されます。

1. クリック  **[!UICONTROL はい、削除します]**.
