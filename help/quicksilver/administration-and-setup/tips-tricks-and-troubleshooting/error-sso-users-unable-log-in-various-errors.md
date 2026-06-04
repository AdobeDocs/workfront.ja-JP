---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: エラー：SSO ユーザーは、様々なエラーにより [!DNL Adobe Workfront] にログインできません
description: フェデレーションシングルサインオン、ユーザー名とパスワードの組み合わせ、または [!DNL Workfront], the problem might be that your [!DNL Workfront]  インスタンスへのアクセスでSSOが使用され、不正なURLを使用してログインしようとすると、ログインエラーが発生します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
TQID: https://experienceleague.adobe.com/8L78zoOjC2KgtVKTorhvWDd8MvaficRL2pZKOfrlGSs
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
source-wordcount: 166
ht-degree: 58%

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
