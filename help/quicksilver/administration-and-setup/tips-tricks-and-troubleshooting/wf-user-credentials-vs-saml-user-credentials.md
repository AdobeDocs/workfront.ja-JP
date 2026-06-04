---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Adobe Workfront ユーザー認証情報とSAML ユーザー認証情報の比較
description: ユーザーの作成後、ユーザーを編集し、「SAML 2.0 認証のみを許可」を有効にすると、ユーザーとパスワードを SAML システムで制御することができます。 このオプションを有効にすると、ユーザーはSAML経由でのみログインできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: faa55b09-10c3-48e6-8b39-33f9feb0a335
TQID: https://experienceleague.adobe.com/8paS2GIumamOltxTC8Gw2mBZ4bKB6TOgbly7IBPKhDw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 235
ht-degree: 90%

---

# Adobe Workfront ユーザー資格情報と SAML ユーザー資格情報

この記事では、特に [!DNL Adobe Workfront] と SAML に焦点を当てており、他の SSO 認証方法については説明しません。

[!DNL Workfront] は各ユーザーのメールアドレスを[!DNL Workfront] ユーザー名として、[!DNL Workfront] パスワードとともにデータベースに保存します。 これらの資格情報は、プレビューおよびカスタム更新サンドボックスに複製されます。

ユーザーの作成中に、SAML 2.0 が設定されていることを[!DNL Workfront]が検出した場合、そのユーザーに対してデフォルトで「SAML 2.0 認証のみを許可」が設定されます。 「このユーザーに招待メールを送信」ボックスが有効になっている場合は、[!DNL Workfront] は「SAML 2.0 認証のみを許可」を無効にし、このオプションを非表示にします。 「このユーザーに招待メールを送信」が有効になると、ユーザーは、非 SAML [!DNL Workfront] ユーザーになります。

ユーザーの作成後、ユーザーを編集し、**[!UICONTROL SAML 2.0 認証のみを許可]**&#x200B;を有効にすると、ユーザーとパスワードを SAML システムで制御することができます。

これが完了すると、ユーザーは SAML 経由でのみログインできます。 [!DNL Workfront]URL にアクセスすると、自動的に SAML システムにリダイレクトされ、SAML ユーザー名とパスワードの入力を求められます。

SAML 資格情報は、Workfront ではなく、Microsoft の ADFS などの外部 SAML システムに保存されます。
