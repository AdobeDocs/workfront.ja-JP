---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ドメインのDMARC ポリシーにより、未認証の電子メールは受け入れられません
description: ' [!DNL Workfront] システムから送信されたメールがドメインの DMARC ポリシーにより受け入れられない場合、メール管理者は workfront.com からのすべてのメールを許可するようにメールシステムを設定することで、問題を修正できます。'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2443267a-dcc0-485b-be29-17539fb54188
TQID: https://experienceleague.adobe.com/f44Wkid-gwfXgHKmSKa6oevhN5jA6720JTlOcH8kJKY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 177
ht-degree: 94%

---

# ドメインの DMARC ポリシーにより、認証されていないメールが受け入れられない

## イシュー

[テスト] 次のバウンスバックメールを受け取りました。

550-5.7.1 「customer domain.com」からの未承認のメールは、ドメインの DMARC ポリシーにより\
550-5.7.1 受け入れられません。 これが正当なメールである場合は、\
550-5.7.1 「customer domain.com」ドメインの管理者にお問い合わせください。 DMARC のイニシアチブについて確認するには、\
550-5.7.1 [*https://support.google.com/mail/answer/2451690*](https://support.google.com/mail/answer/2451690) に\
550 5.7.1 アクセスしてください。

## ソリューション

DMARC がお客様の会社のメールシステムで設定されており、これは [!DNL Adobe Workfront] の一部ではありません。 このメールを受け取った場合は、メール管理者に問い合わせる必要があります。

メール管理者は、noreply@workfront.com から送信されるメール（できれば workfront.com から送信されるすべてのメール）を許可／信頼するようにメールシステムを設定する必要があります。

DMARC について詳しくは、[https://support.google.com/mail/answer/2451690.](https://support.google.com/mail/answer/2451690) を参照してください。
