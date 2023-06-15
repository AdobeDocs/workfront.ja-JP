---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Adobe Workfront Fusion で組織にユーザーを追加する
description: Adobe Workfront Fusion で組織にユーザーを追加できます。
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

# Adobe Workfront Fusion で組織にユーザーを追加する

>[!IMPORTANT]
>
>このページで説明する手順は、まだ [!DNL Adobe Admin Console]. 組織が [!DNL Adobe Admin Console]を使用する場合は、 [!DNL Adobe Admin Console].
>
>ユーザーを[!DNL  Adobe Admin Console]詳しくは、この記事の「ユーザーの詳細を編集する」の節を参照してください。 [ユーザーを個別に管理](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) または、 [!UICONTROL Adobe Admin Console] 管理者。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront Fusion/Adobeビジネスプラットフォーム )](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

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

## 組織へのユーザーの追加

<p>ユーザーを Fusion 組織に追加する手順は、組織がAdobeビジネスプラットフォームにオンボーディングされているかどうかによって異なります。 </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Adobeビジネスプラットフォームにオンボーディングされた組織にユーザーを追加する</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Adobe・ビジネス・コンソールにオンボーディングされていない組織にユーザーを追加</a> </p> </li>
</ul>
<div>
<p><strong>Adobeビジネスプラットフォームにオンボーディングされた組織にユーザーを追加する</strong></p>
<p>組織がAdobeビジネスプラットフォームにオンボーディングされている場合は、Adobe Admin Consoleを通じてこの操作を実行する必要があります。</p>
<p>Adobe Admin Consoleでユーザーを追加する手順については、次の手順を実行します。</p>
<ul>
<li> <p>詳しくは、 <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Adobe Admin Consoleを使用したWorkfrontでのユーザー作成</a></p> </li>
<li> <p>この記事の「ユーザーの追加」の節を参照してください <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">ユーザーを個別に管理</a></p> </li>
<li> <p>Adobe Admin Console管理者に問い合わせてください。</p> </li>
</ul>
<p>組織がAdobeビジネスプラットフォームにオンボーディングされているかどうかに応じて異なる手順のリストについては、 <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )</a>.</p>
</div>
<p><strong>Adobe・ビジネス・コンソールにオンボーディングされていない組織にユーザーを追加</strong></p>

ユーザーを組織に追加するには、ユーザーを追加する組織の管理者である必要があります。 役割について詳しくは、 [の組織の役割 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

組織にユーザーを追加する手順は、次のとおりです。

1. に移動します。 **[!UICONTROL 組織]** メニューで、ユーザーを追加する組織を選択します。
1. を開きます。 **[!UICONTROL ユーザー]** 」タブをクリックします。
1. クリック **[!UICONTROL 新しいユーザーの招待]**&#x200B;をクリックして、フォーム（電子メール、メッセージ、役割）に入力し、招待状を送信します。 **[!UICONTROL 送信]**.

>[!NOTE]
>
>   
><p>[!UICONTROL 新しいユーザーを招待 ] ボタンが表示されない場合、組織は [!DNL Adobe Business Platform.] </p>
>
>   <p>を参照してください。 [!DNL Adobe Business Platform]を参照してください。 <a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">に転送されたユーザーを [!DNL Adobe Business Platform]</a></p>

ユーザーが招待メールを受け取り、ユーザーが [!UICONTROL 役割の承認] 」ボタンをクリックします。
