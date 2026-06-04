---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: ログインエラー：次のフィールドは無効です：emailAddr を null にすることはできません
description: ドメインの URLで  [!DNL Adobe Workfront]  にログインしようとすると、SAML ログインポータルにリダイレクトされ、 [!DNL Workfront]  にリダイレクトされて、emailAddr フィールドを null にすることはできないというエラーが表示されます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 15b702cf-61b8-41dc-8253-77cadc69bd80
TQID: https://experienceleague.adobe.com/MfWVOYcQAVjlbxwiqVaPwipyq5ulv0toajH-2tX7c9k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 100%

---

# ログインエラー：次のフィールドは無効です：emailAddr を null にすることはできません

## 問題

URL（https://customerdomain.my.workfront.com）で [!DNL Adobe Workfront] にログインしようとすると、SAML ログインポータルにリダイレクトされ、次のエラーが表示されて [!DNL Workfront] にリダイレクトされます。

「もう一度試してください。 次のフィールドは無効です：emailAddr を null にすることはできません。」

## 原因

このエラーは、SAML 2.0 設定におけるユーザー属性のマッピングエリアの誤った項目が原因で発生します。 SAML 2.0 のユーザー属性のマッピングについて詳しくは、[SAML 2.0 で Adobe Workfront を設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)を参照してください。

## ソリューション

メールアドレスの属性マッピングを更新し、「**[!UICONTROL 保存]**」をクリックします。
