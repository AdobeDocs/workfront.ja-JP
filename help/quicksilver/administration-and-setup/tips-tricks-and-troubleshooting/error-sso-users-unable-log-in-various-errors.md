---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「エラー：「様々なエラーが原因で  [!DNL Adobe Workfront] SSO ユーザーがログインできません」
description: フェデレーテッド シングル サインオン、ユーザー名とパスワードの組み合わせ、または  [!DNL Workfront], the problem might be that your [!DNL Workfront]  インスタンスへのアクセスで SSO を使用していることについてログイン エラーが表示された場合、誤った URL を使用してログインしようとしています。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 72%

---

# エラー：様々なエラーのため、SSO ユーザーは [!DNL Adobe Workfront] にログインできません

## 問題

[!DNL Workfront] にログインできず、次のいずれかのエラーが表示されます。

* 申し訳ありませんが、このログイン画面から [!DNL Workfront] にアクセスすることはできません。[!DNL Workfront] は、SAML 2.0 を使用した連合型シングルサインオン用に設定されています。[!DNL Workfront] 管理者にお問い合わせください。
* このユーザー名とパスワードの組み合わせは不適切です。Caps Lock がオンになっていないことを確認してください。
* 申し訳ありませんが、[!DNL Workfront] にアクセスできません。[!DNL Workfront] 管理者に連絡して、ユーザー名とパスワードを取得してください。

## ソリューション

[!DNL Workfront] インスタンスは SSO を使用しており、間違った URL からログインしようとしています。「.com」の後に何も付けずに正しい URL を使用してログインしていることを確認してください

>[!TIP]
>
>無効な URL を持つ既存のブックマークを削除します。
