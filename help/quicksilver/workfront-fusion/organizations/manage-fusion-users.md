---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 管理 [!DNL Adobe Workfront Fusion] 組織内のユーザー
description: 管理 [!DNL Adobe Workfront Fusion] 組織内のユーザー
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# 管理 [!DNL Adobe Workfront Fusion] 組織内のユーザー

[!DNL Adobe Workfront Fusion] 管理者は、内でユーザーの役割を管理できます [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
    <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> 
     <p>次の条件を満たす必要があります。 [!DNL Workfront Fusion] 組織の管理者。</p>
     <p>次の条件を満たす必要があります。 [!DNL Workfront Fusion] チームの管理者。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## ユーザーの役割の表示または編集 {#view}

[!DNL Adobe Workfront Fusion] 管理者は、ユーザーの役割を表示および更新できます。

1. While loggin as a [!DNL Workfront Fusion] 管理者、選択 **[!UICONTROL ユーザー]** をクリックします。
1. クリック **[!UICONTROL 詳細]** を選択します。
1. （オプション）ユーザーの役割を更新するには、 **[!DNL Role]** ユーザーの役割を変更する組織の行の列で、新しい役割を選択します。

## ユーザーの詳細の表示または編集 {#view2}

[!DNL Adobe Workfront Fusion] 管理者は、ユーザーの詳細を表示および更新できます。

1. While loggin as a [!DNL Workfront Fusion] 管理者、選択 **[!UICONTROL ユーザー]** をクリックします。
1. クリック **[!UICONTROL 詳細]** を選択します。
1. （オプション）ユーザーの詳細を更新するには、 **[!UICONTROL オプション]** 画面の右上隅で、「 **[!UICONTROL 変更の詳細]**.

## ユーザーの削除 {#delete}

[!DNL Adobe Workfront Fusion] 管理者はユーザーを削除できます。

1. While loggin as a [!DNL Workfront Fusion] 管理者、選択 [!UICONTROL ユーザー] をクリックします。
1. クリック **[!UICONTROL 詳細]** を選択します。
1. （オプション）ユーザーの詳細を更新するには、 **[!UICONTROL オプション]** 画面の右上隅で、「 **[!UICONTROL 削除]**.

### Workfront Fusion でユーザーを削除する際の考慮事項

* ユーザーを削除すると、そのユーザーの接続、キー、Web フックは削除されます。 ユーザーに属するシナリオは、組織の所有者に転送されます。 ユーザーに属する接続が無効になったので、これらのシナリオの接続を更新する必要があります。
* 削除されたユーザーがアプリケーションまたはパブリックテンプレートを所有している場合、そのアプリケーションまたはパブリックテンプレートは組織の所有者に転送されます。 組織の所有者がいない場合、アプリケーションまたはパブリックテンプレートは別のユーザーに転送されます。
