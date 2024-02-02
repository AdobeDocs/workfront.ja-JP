---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: ' [!DNL Workfront Proof] へのシングルサインオン'
description: シングルサインオン（SSO）を使用すると、ユーザーは組織の既存のユーザー名とパスワードを使用して  [!DNL Workfront Proof]  へログインできます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: ht
source-wordcount: '166'
ht-degree: 100%

---

# [!DNL Workfront Proof] へのシングルサインオン

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の [!DNL Workfront Proof] の機能について説明します。[!DNL Adobe Workfront] 内のプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

この機能を使用するには、[!UICONTROL Enterprise] [!DNL Workfront] プランが必要です。利用可能な様々なプランについて詳しくは、[Workfront プラン](https://www.workfront.com/plans)を参照してください。

シングルサインオン（SSO）を使用すると、ユーザーは組織の既存のユーザー名とパスワードを使用して [!DNL Workfront Proof] へログインできます。

この機能を提供するために、XML ベースの [!DNL Security Assertion Markup Language]（SAML）2.0 プロトコルで、ID プロバイダーと web サービスの間でデータの認可と認証の交換をできるようにします。

つまり、[!DNL Workfront Proof] のログインページではなく、自組織のログインシステムに対して認証を行います。

SAML を有効にするには、[!DNL Workfront] Proof アカウントにカスタムのサブドメインまたはドメインを設定する必要があります。

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* 完全にカスタマイズされたドメインについて詳しくは、[ [!DNL Workfront Proof]  サイトのブランド化 - 詳細](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md)を参照してください。

ご利用のアカウントでの SSO の設定について詳しくは、[ [!DNL Workfront Proof]  ユーザーのシングルサインオンを設定する](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md)を参照してください。
