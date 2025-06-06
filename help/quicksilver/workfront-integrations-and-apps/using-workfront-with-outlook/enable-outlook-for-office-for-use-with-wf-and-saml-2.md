---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Outlook for Office を  [!DNL Adobe Workfront]  および SAML 2.0 で使用できるようにする
description: ' [!DNL Adobe Workfront]  システムが SAML 2.0 と統合されている場合、ユーザーが SAML 2.0 資格情報を使用して認証できるようにするには、Office アドインの SAML 2.0 認証を有効にする必要があります。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 72ffceb3-50f0-486e-92b5-0bea4c9a99c8
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 52%

---

# [!DNL Outlook for Office] を [!DNL Adobe Workfront] および SAML 2.0 で使用できるようにする

>[!IMPORTANT]
>
>[Microsoftでは、従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。
>
>* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**
>
>この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**


[!DNL Adobe Workfront] システムが SAML 2.0 と統合されている場合、ユーザーが SAML 2.0 資格情報を使用して認証できるようにするには、[!DNL Office] アドインの SAML 2.0 認証を有効にする必要があります。

SAML を使用して [!DNL Workfront] にログインする際に問題が発生した場合、[!DNL Workfront] 管理者に問い合わせて、SAML が正しく設定されていることを確認します。

SAML 2.0 ソリューションを使用して Office アドインでの認証を有効にする方法について詳しくは、[SAML 2.0 との Adobe Workfront の設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)の記事の節を参照してください。
