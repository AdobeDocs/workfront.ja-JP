---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront ユーザー資格情報と  [!DNL SAML]  ユーザーの資格情報
description: ユーザーの作成後、ユーザーを編集し、「SAML 2.0 認証のみを許可」を有効にすると、ユーザーとパスワードを SAML システムで制御することができます。このオプションを有効にすると、ユーザーには SAML 経由でのログインのみが許可されます。 [!DNL Workfront]  URL にアクセスすると、自動的に SAML システムにリダイレクトされ、SAML ユーザー名とパスワードの入力を求められます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: ht
source-wordcount: '250'
ht-degree: 100%

---

# Adobe Workfront ユーザー資格情報と SAML ユーザー資格情報

この記事では、特に [!DNL Adobe Workfront] と SAML に焦点を当てており、他の SSO 認証方法については説明しません。

[!DNL Workfront] は各ユーザーのメールアドレスを[!DNL Workfront] ユーザー名として、[!DNL Workfront] パスワードとともにデータベースに保存します。これらの資格情報は、プレビューおよびカスタム更新サンドボックスに複製されます。

ユーザーの作成中に、SAML 2.0 が設定されていることを[!DNL Workfront]が検出した場合、そのユーザーに対してデフォルトで「SAML 2.0 認証のみを許可」が設定されます。「このユーザーに招待メールを送信」ボックスが有効になっている場合は、[!DNL Workfront] は「SAML 2.0 認証のみを許可」を無効にし、このオプションを非表示にします。「このユーザーに招待メールを送信」が有効になると、ユーザーは、非 SAML [!DNL Workfront] ユーザーになります。

ユーザーの作成後、ユーザーを編集し、**[!UICONTROL SAML 2.0 認証のみを許可]**&#x200B;を有効にすると、ユーザーとパスワードを SAML システムで制御することができます。

これが完了すると、ユーザーは SAML 経由でのみログインできます。[!DNL Workfront]URL にアクセスすると、自動的に SAML システムにリダイレクトされ、SAML ユーザー名とパスワードの入力を求められます。

SAML 資格情報は、Workfront ではなく、Microsoft の ADFS などの外部 SAML システムに保存されます。
