---
content-type: api
navigation-topic: api-navigation-topic
title: API-Internal の廃止
description: API-Internal の廃止
author: John
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# API-Internal の廃止

API-Internal は、設計と目的によりサポートされないAdobe Workfront API のバージョンです。 Workfront API の最新の更新が含まれていますが、通知なしに変更される可能性があるので、実稼動環境への統合では慎重に使用する必要があります。 Workfrontでは、すべての API-Internal 統合をバージョン管理された API に更新することを強くお勧めします。

Workfront API のサポート対象バージョンについて詳しくは、 [API のバージョン管理とサポートのスケジュール](../../wf-api/api/api-version-support-schedule.md).

**API-Unsupported を使用**

統合で、バージョン管理された API で使用できない機能が必要な場合、Workfrontでは API-Unsupported を使用することをお勧めします。 API-Internal と同様、API-Unsupported はサポートされていません。 API-Unsupported は、Workfront API に対する最新の変更も含まれており、予告なく変更される場合があります。 Workfrontでは、新しい機能を調べて API にバグがないことを確認できるテスト環境で API-Unsupported を使用することを推奨しています。

**使用している API バージョンの確認**

REST を使用して、HTTPS 経由でWorkfrontに呼び出しを送信し、JSON 応答を返す URI を構築することで、統合で使用する API のバージョンを決定できます。

次の例は、API-Internal を呼び出す URI を示しています。

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

次の例は、API-Unsupported を呼び出す URI を示しています。

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

次の例は、API のバージョン 7.0 を呼び出す URI を示しています。

```
https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c70…
```
