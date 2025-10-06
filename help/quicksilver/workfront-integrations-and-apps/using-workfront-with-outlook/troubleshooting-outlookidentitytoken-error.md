---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: トラブルシューティング：Outlook 用Workfrontを使用する際の outlookIdentityToken エラー
description: Workfront for Outlook の使用時に outlookIdentityToken エラーが発生した場合は、Microsoft 365 の従来のトークンを有効にする必要があります。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 43%

---

# トラブルシューティング：Outlook 用Workfrontを使用する際の outlookIdentityToken エラー

>[!IMPORTANT]
>
>[Microsoftでは、Workfront Outlook アドインで認証に使用されていた従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートが無効になっています。 Microsoftによるこの変更は、段階的にロールアウトされ、2025 年 10 月 1 日（PT）に完了します。
>
>**Microsoftがこれらのトークンを無効にしたため、Microsoft Outlook 用Workfront統合は機能しなくなりました。**

Workfront for Outlook を使用すると、次のエラーが発生する場合があります。

```
Unexpected error
Unable to get the outlookIdentityToken
```

このエラーを解決するには、組織に対して Microsoft 365 レガシートークンを有効にする必要があります。これは Microsoft 365 で実行する必要があるので、Workfront では組織に対してこれらのトークンを有効にできません。

Microsoft 365 のレガシートークンを有効にする手順について詳しくは、Microsoft ドキュメントの[レガシー Exchange Online トークンのオンとオフを切り替える](https://learn.microsoft.com/ja-jp/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)を参照してください。

レガシートークンについて詳しくは、Microsoft ドキュメントの [Exchange Online レガシートークンを再びオンにできますか？](https://learn.microsoft.com/ja-jp/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on)を参照してください。
