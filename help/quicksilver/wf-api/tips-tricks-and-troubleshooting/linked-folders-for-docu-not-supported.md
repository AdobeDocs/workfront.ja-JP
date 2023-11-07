---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: DOCU オブジェクトでは、リンクされたフォルダはサポートされていません
description: DOCU オブジェクトでは、リンクされたフォルダはサポートされていません
author: Becky
feature: Workfront API
role: Developer
exl-id: 33b5a998-f3e1-42a2-852e-fb862d770d50
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '118'
ht-degree: 0%

---

# API を使用したリンクされたフォルダーの追加はサポートされていません

API を使用した Document(DOCU) オブジェクトのフォルダー配列へのリンクフォルダーの追加はサポートされていません。 リクエストは成功しますが、ドキュメントが一部の外部プロバイダーによってシステムから削除される場合があります。 これは、外的なシステムが真実の最終的な源として使用されるからです。 したがって、ドキュメントが外部プロバイダーから削除された場合、そのドキュメントは存在しなくなったと見なされます。 リンク（外部）フォルダーにないドキュメントは、次の場所から自動的に削除されます： [!DNL Workfront] それを回復する方法がなかった
