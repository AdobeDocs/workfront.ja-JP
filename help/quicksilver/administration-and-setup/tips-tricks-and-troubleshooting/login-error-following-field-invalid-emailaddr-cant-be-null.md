---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'ログインエラー：次のフィールドは無効です。emailAddr を null にすることはできません'
description: ログインしようとしたとき [!DNL Adobe Workfront] ドメインの URL が SAML ログインポータルにリダイレクトされ、にリダイレクトされる [!DNL Workfront] emailAddr フィールドを null にすることはできないというエラーが表示されます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# ログインエラー：次のフィールドは無効です。emailAddr を null にすることはできません

## 問題

ログインしようとしたとき [!DNL Adobe Workfront] URL(https://customerdomain.my.workfront.com) が入力されている場合、SAML ログインポータルにリダイレクトされ、にリダイレクトされます。 [!DNL Workfront] を次のエラーで置き換えます。

「もう一度試してください。次のフィールドは無効です。emailAddr を null にすることはできません。」

## 原因

このエラーは、SAML 2.0 設定の「Map User Attributes」領域の誤った項目が原因で発生します。 SAML 2.0 のユーザー属性のマッピングについて詳しくは、 [SAML 2.0 でのAdobe Workfrontの設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## 解決策

E メールアドレスの属性マッピングを更新し、 **[!UICONTROL 保存]**.
