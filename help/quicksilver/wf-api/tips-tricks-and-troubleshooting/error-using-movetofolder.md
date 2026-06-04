---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: ドキュメントの moveToFolder アクションが機能しない
description: Document moveToFolder アクションを使用すると、422 エラーが返されます。
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 12%

---

# ドキュメントの moveToFolder アクションが機能しない

## 問題

Document オブジェクトの`moveToFolder` アクションを使用すると、422 エラーが返されます。

または

Workfront FusionのAdobe Authenticator モジュールでこのアクションを使用すると、ドキュメントは移動されませんが、エラーの兆候はありません。 エラーは同じですが、Adobe Authenticator モジュールには表示されません。

## ソリューション

このアクションの422 エラーの原因として考えられるのは、アクションが1つのリンクされたフォルダー内のドキュメントを別のリンクされたフォルダーに移動しようとすることです。

移動するドキュメントがリンクされたフォルダーにないことを確認します。
