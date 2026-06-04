---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScalerの設定によってパフォーマンスが低下する可能性があります
description: ユーザーの作成後、ユーザーを編集し、「SAML 2.0 認証のみを許可」を有効にすると、ユーザーとパスワードを SAML システムで制御することができます。 このオプションを有効にすると、ユーザーはSAML経由でのみログインできます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
TQID: https://experienceleague.adobe.com/-3-p8fzXIiV-gnjIjhRzBmLfspAEEVAuD2lpmcsVjLA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 70%

---

# Workfront：ZScaler 設定によりパフォーマンスが低下する場合がある

>[!NOTE]
>
>これは ZScalar の問題であり、Workfront では修正されません。

ZScalar の web サービスは、デフォルトで `http/1.1` を使用するので、Workfront のパフォーマンスが低下する場合があります。

この問題を確認して解決するには、`http/2`を使用するようにZScaler ソフトウェアを設定します。 これは、Workfront では設定できません。

`http/2` について詳しくは、ZScalar のドキュメントを参照してください。
