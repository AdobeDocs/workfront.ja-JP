---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScalar の設定により、パフォーマンスが低下する場合があります
description: ユーザーの作成後、ユーザーを編集し、「SAML 2.0 認証のみを許可」を有効にすると、ユーザーとパスワードを SAML システムで制御することができます。このオプションを有効にすると、ユーザーは SAML 経由でのみログインできます。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 806a4c4835e47da4fbbdb28ec0c35c990f70239e
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 25%

---

# Workfront:ZScalar 設定を使用すると、パフォーマンスが低下する場合があります

>[!NOTE]
>
>これは ZScalar の問題であり、Workfrontでは修正されません。

ZScalar の web サービスでは、デフォルトで `http/1.1` を使用しているので、Workfrontのパフォーマンスが低下する可能性があります。

この問題を確認して解決するには、`http/2` を使用するように ZScalar ソフトウェアを設定します。 これはWorkfrontでは設定できません。

`http/2` について詳しくは、ZScalar のドキュメントを参照してください。
