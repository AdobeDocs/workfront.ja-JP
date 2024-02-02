---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ドメインの DMARC ポリシーにより認証済みのメールが受け入れられない場合
description: ' [!DNL Workfront] システムから送信されたメールがドメインの DMARC ポリシーにより受け入れられない場合、メール管理者は workfront.com からのすべてのメールを許可するようにメールシステムを設定することで、問題を修正できます。'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: ht
source-wordcount: '165'
ht-degree: 100%

---

# ドメインの DMARC ポリシーにより、認証されていないメールが受け入れられない

## イシュー

[テスト] 次のバウンスバックメールを受け取りました。

550-5.7.1 「customer domain.com」からの未承認のメールは、ドメインの DMARC ポリシーにより\
550-5.7.1 受け入れられません。これが正当なメールである場合は、\
550-5.7.1 「customer domain.com」ドメインの管理者にお問い合わせください。DMARC のイニシアチブについて確認するには、\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) に\
550 5.7.1 アクセスしてください。

## ソリューション

DMARC がお客様の会社のメールシステムで設定されており、これは [!DNL Adobe Workfront] の一部ではありません。このメールを受け取った場合は、メール管理者に問い合わせる必要があります。

メール管理者は、noreply@workfront.com から送信されるメール（できれば workfront.com から送信されるすべてのメール）を許可／信頼するようにメールシステムを設定する必要があります。

DMARC について詳しくは、[https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690) を参照してください。
