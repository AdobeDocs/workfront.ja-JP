---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: トラブルシューティング：Outlook 用Workfrontを使用する際の outlookIdentityToken エラー
description: Workfront for Outlook の使用時に outlookIdentityToken エラーが発生した場合は、Microsoft 365 の従来のトークンを有効にする必要があります。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 31%

---

# トラブルシューティング：Outlook 用Workfrontを使用する際の outlookIdentityToken エラー

>[!IMPORTANT]
>
>[Microsoftでは、従来の Exchange オンライン トークン ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) のサポートを無効にする処理を行っています。現在、このトークンは、Workfront Outlook アドインで認証に使用されています。 Microsoftによるこの変更は、既にお客様に影響を与え始めており、2025 年 10 月まで段階的に展開し続けます。
>
>* **Microsoftがこれらのトークンを完全に無効にすると、Microsoft Outlook 用Workfront統合は機能しなくなります。**
>
>この変更の一環として、Microsoftは、トークンを再度有効にする方法を変更することを決定しました。 **2025 年 6 月 30 日（PT）** 以降、管理者はトークン自体を再度有効にすることができなくなります。例外を付与できるのは、Microsoft サポートのみです。 **2025 年 10 月 1 日に、すべてのテナントに対してレガシートークンがオフになります。 例外は許可されません。**


Workfront for Outlook を使用すると、次のエラーが発生する場合があります。

```
Unexpected error
Unable to get the outlookIdentityToken
```

このエラーを解決するには、組織に対して Microsoft 365 レガシートークンを有効にする必要があります。これは Microsoft 365 で実行する必要があるので、Workfront では組織に対してこれらのトークンを有効にできません。

Microsoft 365 のレガシートークンを有効にする手順について詳しくは、Microsoft ドキュメントの[レガシー Exchange Online トークンのオンとオフを切り替える](https://learn.microsoft.com/ja-jp/office/dev/add-ins/outlook/turn-exchange-tokens-on-off)を参照してください。

レガシートークンについて詳しくは、Microsoft ドキュメントの [Exchange Online レガシートークンを再びオンにできますか？](https://learn.microsoft.com/ja-jp/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on)を参照してください。
