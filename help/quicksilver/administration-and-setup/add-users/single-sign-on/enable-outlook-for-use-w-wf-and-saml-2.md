---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Outlook をWorkfrontおよび SAML 2.0 で使用できるようにする
description: SAML 2.0 Authentication を有効にし、ユーザーが SAML 2.0 資格情報を使用して Microsoft Outlook から Workfront にログインできるようにする場合は、Office アドインで SAML 2.0 を有効にして認証を行う必要があります。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 63%

---

# Workfront と SAML 2.0 での Outlook の使用を有効化

>[!IMPORTANT]
>
>[Microsoftでは、従来の Exchange オンライン トークン &#x200B;](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。
>
>* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**
>
>この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**

SAML 2.0 Authentication を有効にし、ユーザーが SAML 2.0 資格情報を使用して Microsoft Outlook から Workfront にログインできるようにする場合は、Office アドインで SAML 2.0 を有効にして認証を行う必要があります。

>[!NOTE]
>
>組織の Workfront インスタンスがカスタム SSO Portal を使用している場合は使用できません。>
><!--
>or is enabled with Adobe IMS>
>-->
>詳細情報が必要な場合は、ネットワークまたは IT 管理者にお問い合わせください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p><p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront と SAML 2.0 での Outlook の使用を有効化

{{step-1-to-setup}}

1. **システム**／**環境設定**&#x200B;をクリックします。

1. 「**セキュリティ**」セクションで、「**Office 365 アドインで SAML 2.0 Authentication を許可**」が有効になっていることを確認します。

   このオプションを使用すると、Office 365 アドインの Iframe でのみ Workfront の埋め込みを有効にすることができます。クリック可能なコンテンツが含まれていないので、クリックジャッキング侵害を起こしません。

   このオプションは、デフォルトで有効になっています。

   >[!NOTE]
   >
   >「**iframe への Workfront の埋め込みを許可**」オプションを有効にする場合、「**Office 365 アドインで SAML 2.0 Authentication を許可**」オプションはグレー表示になり、有効になります。
   >
   >![&#x200B; 埋め込みを許可オプション &#x200B;](assets/if-you-enable.png)
   >

1. 「**保存**」をクリックします。

   ここで保存した変更内容は、Workfront のすべてのユーザーのエクスペリエンスに影響します。
