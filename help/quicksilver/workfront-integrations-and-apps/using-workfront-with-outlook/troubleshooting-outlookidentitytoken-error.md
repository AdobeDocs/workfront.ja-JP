---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: トラブルシューティング：Outlook 用Workfrontを使用する際の outlookIdentityToken エラー
description: Workfront for Outlook の使用時に outlookIdentityToken エラーが発生した場合は、Microsoft 365 の従来のトークンを有効にする必要があります。
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 571ed00f44322d73183323c4d4154284cd028301
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# トラブルシューティング：Outlook 用Workfrontを使用する際の outlookIdentityToken エラー

Workfront for Outlook を使用すると、次のエラーが発生する場合があります。

```
Unexpected error
Unable to get the outlookIdentityToken
```

このエラーを解決するには、組織のMicrosoft 365 レガシートークンを有効にする必要があります。 これはMicrosoft 365 で行う必要があるので、Workfrontでは組織に対してこれらのトークンを有効にできません。

Microsoft 365 の従来のトークンを有効にする手順については、Microsoft ドキュメントの [ 従来の Exchange Online トークンのオン/オフの切り替え ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) を参照してください。

レガシー・トークンの詳細については、[Exchange Online のレガシー・トークンをオンにできますか？Microsoft ドキュメントを ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) 照してください。
