---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfrontユーザー資格情報と [!DNL SAML] ユーザーの資格情報
description: ユーザーの作成後、ユーザーを編集し、「Only Allow SAML 2.0 Authentication」を有効にして、ユーザーとパスワードを SAML システムで制御できます。 このオプションを有効にすると、ユーザーは SAML 経由でのログインのみ許可されます。 ユーザーが [!DNL Workfront] URL を指定すると、SAML システムに自動的にリダイレクトされ、SAML ユーザー名とパスワードの入力を求められます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Adobe Workfrontユーザー資格情報と SAML ユーザー資格情報の比較

この記事では、特に以下に焦点を当てます。 [!DNL Adobe Workfront] SAML およびは他の SSO 認証方法を扱いません。

データベースで、 [!DNL Workfront] 各ユーザーの電子メールアドレスをそのユーザーの [!DNL Workfront] ユーザー名とユーザー名 [!DNL Workfront] パスワード。 これらの資格情報は、プレビューおよびカスタム更新サンドボックスにレプリケートされます。

ユーザーの作成中に、 [!DNL Workfront] SAML 2.0 が設定されたことを検出します。ユーザーのデフォルト値は「Only Allow SAML 2.0 Authentication」です。 [ この人に招待メールを送信する ] ボックスが有効になっている場合、 [!DNL Workfront] 「SAML 2.0 認証のみを許可」を無効にし、このオプションを非表示にします。 「この人に招待メールを送信」が有効になると、ユーザーは SAML 以外のユーザーになります [!DNL Workfront] ユーザー。

ユーザーの作成後、ユーザーを編集し、 **[!UICONTROL SAML 2.0 認証のみを許可]** ユーザーとパスワードを SAML システムで制御できるようにします。

これにより、ユーザーは SAML 経由でのみログインできます。 ユーザーが [!DNL Workfront] URL を指定すると、SAML システムに自動的にリダイレクトされ、SAML ユーザー名とパスワードの入力を求められます。

SAML 資格情報は、Workfrontではなく、Microsoftの ADFS などの外部 SAML システムに保存されます。
