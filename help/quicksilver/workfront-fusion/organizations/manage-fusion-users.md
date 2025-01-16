---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: 組織内の  [!DNL Adobe Workfront Fusion]  ユーザーの管理
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 77%

---

# 組織内の [!DNL Adobe Workfront Fusion] ユーザーの管理

[!DNL Adobe Workfront Fusion] 管理者は、[!DNL Workfront Fusion] 内でユーザーの役割を管理できます。

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ ユーザーの役割の表示または編集 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/manage-users-and-teams/view-or-edit-user-roles.html)
>* [ ユーザーの詳細の表示または編集 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/manage-users-and-teams/view-or-edit-user-details.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

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

>[!NOTE]
>
>現在、組織がWorkfrontへの移行プロセスを行っている場合、Adobe Admin Consoleでユーザーを管理（ユーザーの追加または削除）することはできません。 移行が完了したら、Adobe Admin Consoleでこれらの操作を実行できます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
    <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> 
     <p>組織の [!DNL Workfront Fusion] 管理者である必要があります。</p>
     <p>チームの [!DNL Workfront Fusion] 管理者である必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## ユーザーの役割を表示または編集 {#view}

[!DNL Adobe Workfront Fusion] 管理者は、ユーザーの役割を表示および更新できます。

1. [!DNL Workfront Fusion] 管理者としてログインしているときに、左側のナビゲーションで&#x200B;**[!UICONTROL ユーザー]**&#x200B;を選択します。
1. 表示したいユーザーの行で&#x200B;**[!UICONTROL 詳細]**&#x200B;をクリックします。
1. （オプション）ユーザーの役割を更新するには、ユーザーの役割を変更する組織の行の **[!DNL Role]** 列のドロップダウンをクリックし、新しい役割を選択します。

## ユーザーの詳細を表示または編集 {#view2}

[!DNL Adobe Workfront Fusion] 管理者は、ユーザーの詳細を表示および更新できます。

1. [!DNL Workfront Fusion] 管理者としてログインしているときに、左側のナビゲーションで&#x200B;**[!UICONTROL ユーザー]**&#x200B;を選択します。
1. 表示したいユーザーの行で&#x200B;**[!UICONTROL 詳細]**&#x200B;をクリックします。
1. （オプション）ユーザーの詳細を更新するには、画面の右上隅にある&#x200B;**[!UICONTROL オプション]**&#x200B;をクリックし、「**[!UICONTROL 詳細を変更]**」を選択します。

## ユーザーを削除 {#delete}

[!DNL Adobe Workfront Fusion] 管理者はユーザーを削除できます。

1. [!DNL Workfront Fusion] 管理者としてログインしているときに、左側のナビゲーションで[!UICONTROL ユーザー]を選択します。
1. 表示したいユーザーの行で&#x200B;**[!UICONTROL 詳細]**&#x200B;をクリックします。
1. （オプション）ユーザーの詳細を更新するには、画面の右上隅の&#x200B;**[!UICONTROL オプション]**&#x200B;をクリックし、続いて「**[!UICONTROL 削除]**」を選択します。

### Workfront Fusion でユーザーを削除する際の考慮事項

* ユーザーを削除すると、そのユーザーの接続、キー、web フックは削除されます。ユーザーに属するシナリオは、組織の所有者に転送されます。ユーザーに属する接続が有効ではなくなったので、これらのシナリオの接続を更新する必要があります。
* 削除されたユーザーがアプリケーションや公開テンプレートを所有している場合、そのアプリケーションまたは公開テンプレートは組織の所有者に転送されます。組織の所有者がいない場合、そのアプリケーションや公開テンプレートは別のユーザーに転送されます。
