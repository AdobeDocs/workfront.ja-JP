---
content-type: api
navigation-topic: api-navigation-topic
title: API-Internal の廃止
description: API-Internal の廃止
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: acc7414a9c6eef838147aee675603b6cc2566fb9
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 96%

---

# API-Internal の廃止

API-Internal は、設計と目的が原因でサポートされていない Adobe Workfront API バージョンです。Workfront API の最新の更新が含まれていますが、通知なしに変更される可能性があるので、実稼動環境への統合では慎重に使用する必要があります。Workfront では、すべての API-Internal 統合をバージョン管理された API に更新することを強くお勧めします。

Workfront API のサポート対象バージョンについて詳しくは、[API のバージョン管理とサポートスケジュール](../../wf-api/api/api-version-support-schedule.md)を参照してください。

**API-Unsupported の使用**

バージョン管理された API で使用できない機能が統合で必要な場合、Workfront では API-Unsupported を使用することをお勧めします。API-Internal と同様に、API-Unsupported はサポート対象外です。また、API-Unsupported も Workfront API の最新の変更を含んでおり、予告なく変更される場合があります。Workfront では、新しい機能を調べて API にバグがないことを確認できるテスト環境で API-Unsupported を使用することをお勧めします。

**使用している API バージョンの確認**

統合で使用している API のバージョンを特定するには、REST を使用して、HTTPS で Workfront に呼び出しを送信して JSON 応答を返す URI を作成します。

次の例は、API-Internal を呼び出す URI を示しています。

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

次の例は、API-Unsupported を呼び出す URI を示しています。

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>API-Unsupported 呼び出しでは、 `/api` 」セクションに含める必要があります。

次の例は、API のバージョン 15.0 を呼び出す URI を示しています。

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
