---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ドメインの DMARC ポリシーが原因で認証済みの電子メールが受け入れられない場合
description: 電子メールが [!DNL Workfront] ドメインの DMARC ポリシーによりシステムが受け入れられないので、電子メール管理者は、workfront.com からのすべての電子メールを許可するように電子メールシステムを設定することで、問題を修正できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 0%

---

# ドメインの DMARC ポリシーにより、未認証の電子メールが受け入れられません

## 問題

[テスト] 次のバウンスバックメールを受け取りました。

550-5.7.1 「customer domain.com」からの未認証メールは、\
550～5.7.1 ドメインの DMARC ポリシー。 「customer domain.com」の管理者にお問い合わせください\
550-5.7.1 ドメイン（これが正当なメールの場合）。 次を参照してください：\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) DMARC を学ぶには\
550 5.7.1 イニシアチブ。

## 解決策

DMARC は会社の電子メールシステムで設定され、 [!DNL Adobe Workfront]. この電子メールを受け取った場合は、電子メール管理者に問い合わせる必要があります。

電子メール管理者は、 noreply@workfront.comからの電子メールを許可/信頼するか、できれば workfront.com からのすべての電子メールを許可/信頼するように電子メールシステムを設定する必要があります。

DMARC の詳細については、 [https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690)
