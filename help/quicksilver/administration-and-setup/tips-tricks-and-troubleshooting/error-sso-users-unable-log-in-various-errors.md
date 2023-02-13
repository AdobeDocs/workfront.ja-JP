---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'エラー：SSO ユーザーがにログインできません [!DNL Adobe Workfront] 様々なエラーのため'
description: フェデレーテッドシングルサインオン、ユーザー名とパスワードの組み合わせ、または [!DNL Workfront], the problem might be that your [!DNL Workfront] インスタンスが SSO を使用しているので、間違った URL を使用してログインしようとしています。 「.com」の後に何も付けずに正しい URL を使用してログインしていることを確認してください。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 9%

---

# エラー：SSO ユーザーがにログインできません [!DNL Adobe Workfront] 様々なエラーによる

## 問題

にログインできません [!DNL Workfront] そして次のエラーの 1 つを受け取りました。

* 申し訳ありませんが、次にアクセスできません： [!DNL Workfront] このログイン画面を使用して、 [!DNL Workfront] は、SAML 2.0 を使用したフェデレーテッドシングルサインオン用に設定されています。 [!DNL Workfront] 管理者。
* このユーザー名とパスワードの組み合わせは不適切です。 Caps Lock がオンになっていないことを確認してください。
* 申し訳ありませんが、次へのアクセス権がありません： [!DNL Workfront]. お問い合わせください [!DNL Workfront] 管理者に問い合わせて、ユーザー名とパスワードを取得します。

## 解決策

お使いの [!DNL Workfront] インスタンスが SSO を使用しており、間違った URL を使用してログインしようとしています。 「.com」の後に何も付けずに正しい URL を使用してログインしていることを確認してください

>[!TIP]
>
>無効な URL を持つ既存のブックマークを削除します。
