---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ZScaler 設定を使用すると、パフォーマンスが低下する場合があります
description: ユーザーの作成後、ユーザーを編集し、「SAML 2.0 認証のみを許可」を有効にすると、ユーザーとパスワードを SAML システムで制御することができます。このオプションを有効にすると、ユーザーは SAML 経由でのみログインできます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 2752a9e2-44fe-49b5-a7ab-4021d91ed37b
source-git-commit: f66b219e9fd203f108844ad397bcfa848b8f1134
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 25%

---

# Workfront:ZScaler 設定によってパフォーマンスが低下する場合があります

>[!NOTE]
>
>これは ZScaler の問題であり、Workfrontでは修正されません。

ZScaler の web サービスは、デフォルトで `http/1.1` を使用しているので、Workfrontのパフォーマンスが低下する可能性があります。

この問題を確認して解決するには、`http/2` を使用するように ZScaler ソフトウェアを設定します。 これはWorkfrontでは設定できません。

`http/2` について詳しくは、ZScaler のドキュメントを参照してください。
