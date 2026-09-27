---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: '[!DNL Workfront Proof] へのシングルサインオン'
description: シングルサインオン（SSO）を使用すると、ユーザーは組織の既存のユーザー名とパスワードを使用して [!DNL Workfront Proof] へログインできます。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb1f6883-6209-4a55-b181-67af4b496ca0
TQID: 'https://experienceleague.adobe.com/rQkypJthOpKg1gQBH0tUjtwkbaxLn1k-lrpZj9hCQ5o'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 100%
---
# [!DNL Workfront Proof] へのシングルサインオン

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の [!DNL Workfront Proof] の機能について説明します。 [!DNL Adobe Workfront] 内のプルーフについて詳しくは、[プルーフ](../../../review-and-approve-work/proofing/proofing.md)を参照してください。

この機能を使用するには、[!UICONTROL Enterprise] [!DNL Workfront] プランが必要です。 利用可能な様々なプランについて詳しくは、[Workfront プラン](https://business.adobe.com/products/workfront/pricing.html)を参照してください。

シングルサインオン（SSO）を使用すると、ユーザーは組織の既存のユーザー名とパスワードを使用して [!DNL Workfront Proof] へログインできます。

この機能を提供するために、XML ベースの [!DNL Security Assertion Markup Language]（SAML）2.0 プロトコルで、ID プロバイダーと web サービスの間でデータの認可と認証の交換をできるようにします。

つまり、[!DNL Workfront Proof] のログインページではなく、自組織のログインシステムに対して認証を行います。

SAML を有効にするには、[!DNL Workfront] Proof アカウントにカスタムのサブドメインまたはドメインを設定する必要があります。

<!--* Custom sub-domains are free to set up. See our [Configure a branded domain in Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/configure-branded-domain-in-wp.md) for more information.-->
* 完全にカスタマイズされたドメインについて詳しくは、[ [!DNL Workfront Proof]  サイトのブランド化 - 詳細](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site-advanced.md)を参照してください。

ご利用のアカウントでの SSO の設定について詳しくは、[ [!DNL Workfront Proof]  ユーザーのシングルサインオンを設定する](../../../workfront-proof/wp-acct-admin/account-settings/configure-sso-for-wp-users.md)を参照してください。
