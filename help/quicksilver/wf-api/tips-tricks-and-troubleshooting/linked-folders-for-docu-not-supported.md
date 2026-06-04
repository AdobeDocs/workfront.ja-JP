---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: DOCU オブジェクトでは、リンクされたフォルダーはサポートされていません
description: DOCU オブジェクトでは、リンクされたフォルダーはサポートされていません
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
TQID: https://experienceleague.adobe.com/iPjiffn9QLDldjWRdxMyf8RTaZaB9X6axc7UVY1B3Bg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 118
ht-degree: 100%

---

# API を使用したリンクされたフォルダーの追加がサポートされていない

API を使用した Document（DOCU）オブジェクトのフォルダー配列へのリンクフォルダーの追加はサポートされていません。 リクエストは成功しますが、ドキュメントが一部の外部プロバイダーによってシステムから削除される場合があります。 これは、外部システムが真実の最終的な源として使用されるからです。 したがって、ドキュメントが外部プロバイダーから削除された場合、そのドキュメントは存在しなくなったと見なされます。 リンク（外部）フォルダーにないドキュメントは、[!DNL Workfront] から自動的に削除され、復元できません。
