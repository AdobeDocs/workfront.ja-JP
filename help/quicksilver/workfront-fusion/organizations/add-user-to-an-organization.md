---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion で組織にユーザーを追加する
description: Adobe Workfront Fusion で組織にユーザーを追加できます。
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 447ab70566d5f9de3bc368933c9efdb94d2b9e7e
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 90%

---

# Adobe Workfront Fusion で組織にユーザーを追加する

>[!IMPORTANT]
>
>このページで説明する手順は、[!DNL Adobe Admin Console] にまだ登録されていない組織にのみ適用されます。組織が [!DNL Adobe Admin Console] に登録されている場合は、[!DNL Adobe Admin Console] を通じてこのアクションを実行してください。
>
>[!DNL  Adobe Admin Console] にユーザーを追加する手順については、[ユーザーを個別に管理する](https://helpx.adobe.com/jp/enterprise/using/manage-users-individually.html)の記事のユーザーの詳細の編集の節を参照するか、[!UICONTROL Adobe Admin Console] の管理者にお問い合わせください。
>
>組織が Adobe Admin Console に登録されているかどうかによって手順が異なり、その手順のリストについては、[プラットフォームによる管理の違い（Adobe Workfront Fusion、Adobe Business Platform）](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md)を参照してください。

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

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 組織へのユーザーの追加


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->

ユーザーを組織に追加するには、ユーザーを追加する組織の管理者である必要があります。役割について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md) での組織の役割を参照してください。

組織にユーザーを追加する手順は、次のとおりです。

1. メニューの&#x200B;**[!UICONTROL 組織]**&#x200B;に移動し、ユーザーを追加する組織を選択します。
1. ダッシュボードの「**[!UICONTROL ユーザー]**」タブを開きます。
1. 「**[!UICONTROL 新しいユーザーを招待]**」をクリックしてフォーム（メール、メッセージ、役割）に記入し、「**[!UICONTROL 送信]**」をクリックして招待を送信します。

>[!NOTE]
>
>   
>次の項目が表示されない場合、 [!UICONTROL 新しいユーザーの招待] 」ボタンが表示された場合、組織は [!DNL Adobe Business Platform.]
>
>  を参照してください。 [!DNL Adobe Business Platform]を参照してください。 [ユーザーの追加先 [!DNL Adobe Workfront Fusion] から [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

ユーザーは招待メールを受け取り、招待を承諾することができます。
