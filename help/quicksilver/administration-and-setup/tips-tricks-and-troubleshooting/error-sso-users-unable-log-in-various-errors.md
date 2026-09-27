---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: エラー：様々なエラーのため、SSO ユーザーは [!DNL Adobe Workfront] にログインできません
description: フェデレーションシングルサインオン、ユーザー名とパスワードの組み合わせ、または[!DNL Workfront]へのアクセスに関するログインエラーが発生した場合、問題は[!DNL Workfront] インスタンスがSSOを使用しており、誤ったURLを使用してログインしようとしていることである可能性があります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
TQID: 'https://experienceleague.adobe.com/8L78zoOjC2KgtVKTorhvWDd8MvaficRL2pZKOfrlGSs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 63%
---
# エラー：様々なエラーのため、SSO ユーザーは [!DNL Adobe Workfront] にログインできません

## 問題

[!DNL Workfront] にログインできず、次のいずれかのエラーが表示されます。

* 申し訳ありませんが、このログイン画面から [!DNL Workfront] にアクセスすることはできません。 [!DNL Workfront]は、SAML 2.0を使用したフェデレーテッド シングル サインオン用に設定されています。 [!DNL Workfront]管理者にお問い合わせください。
* ユーザー名とパスワードの組み合わせが不適切でした。 キャップ ロックがオンになっていないことを確認して、もう一度試してください。
* 申し訳ありませんが、[!DNL Workfront] にアクセスできません。 [!DNL Workfront] 管理者に連絡して、ユーザー名とパスワードを取得してください。

## ソリューション

[!DNL Workfront] インスタンスは SSO を使用しており、間違った URL からログインしようとしています。 「.com」の後に何も付けずに正しい URL を使用してログインしていることを確認してください

>[!TIP]
>
>無効な URL を持つ既存のブックマークを削除します。
