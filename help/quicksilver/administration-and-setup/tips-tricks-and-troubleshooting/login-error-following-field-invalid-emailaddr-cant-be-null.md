---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 「ログインエラー：次のフィールドが無効です：emailAddr を null にすることはできません」
description: ドメインの URLで  [!DNL Adobe Workfront]  にログインしようとすると、SAML ログインポータルにリダイレクトされ、 [!DNL Workfront]  にリダイレクトされて、emailAddr フィールドを null にすることはできないというエラーが表示されます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 92%

---

# ログインエラー：次のフィールドは無効です：emailAddr を null にすることはできません

## 問題

URL（https://customerdomain.my.workfront.com）で [!DNL Adobe Workfront] にログインしようとすると、SAML ログインポータルにリダイレクトされ、次のエラーが表示されて [!DNL Workfront] にリダイレクトされます。

「もう一度試してください。次のフィールドは無効です：emailAddr を null にすることはできません。」

## 原因

このエラーは、SAML 2.0 設定におけるユーザー属性のマッピングエリアの誤った項目が原因で発生します。SAML 2.0 のユーザー属性のマッピングについて詳しくは、[SAML 2.0 で Adobe Workfront を設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)を参照してください。

## ソリューション

メールアドレスの属性マッピングを更新し、「**[!UICONTROL 保存]**」をクリックします。
