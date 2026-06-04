---
content-type: api
navigation-topic: api-navigation-topic
title: イベント登録用のアウトバウンドメッセージ形式
description: イベント登録用のアウトバウンドメッセージ形式
author: Becky
feature: Workfront API
role: Developer
exl-id: addcf5bc-a101-4bb0-93a6-46b4af67c848
TQID: https://experienceleague.adobe.com/-yUOhE9OsdK5SHaObgFhMgGt7Ih-FY7XqdEJn6QI4hk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 95%

---

# イベント登録用のアウトバウンドメッセージ形式

Adobe Workfront 2017.3 のリリースでは、イベント登録のアウトバウンドメッセージの形式が変更され、パフォーマンスを向上させ、統合のためにイベント登録をより適切に使用できるようになります。

## アウトバウンドメッセージ形式の更新

アウトバウンドメッセージの形式に対して、次の変更が行われます。

* アウトバウンドメッセージには、Workfront リソースの oldState と newState が含まれます。

  これらの値は、Workfront でのイベントの結果としてオブジェクトに加えられた変更を表示します。

* eventTime メタデータフィールドが、すべての送信メッセージに追加されます。

  このフィールドは、イベントが発生した時刻をナノ秒（Nanosecond）およびエポック秒（EpochSeconds）単位で、示します。 統合で処理されるイベントを並べ替える際に、eventTime を使用します。

* NOTE リソース上の所有者:companyIDが参照しているフィールドが削除されます。
* DOCU（Document）リソースの currentVersion が参照している objectOn は削除されます。

現在 Workfront イベントの登録を使用している場合、これらの変更に対応するには、2017.3 リリースより前にWorkfront 統合を更新する必要があります。

イベント登録について詳しくは、[Event Subscription API](../../wf-api/general/event-subs-api.md) を参照してください。

## 古いメッセージ形式と新しいメッセージ形式のサンプル

次の古い形式の CREATE メッセージは、2017.3 のリリース後は使用されなくなります。

```
{
  "eventType": "CREATE",
  "subscriptionId": "8a0d839d5ef32c9a015ef33064b00001",
  "fields": {
     "ID": "59d7db3c0000014b05536251b669a3e4",
     "name": "EventSub Test 53350c27-ce58-40e9-af75-a2d45ff13046",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:36:28.722-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:36:28.785-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1891,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```

2017.3 のリリース後は、次の新しい形式の CREATE メッセージが使用されます。

```
{
   "eventType": "CREATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef32e2cde0000",
   "eventTime": {
      "nano": 414000000,
      "epochSecond": 1507318444
   },
   "newState": {
     "ID": "59d7daab0000011b8faebf0f60d25d08",
     "name": "EventSub Test 3700e224-0ef7-4571-b200-09109712152c",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:34:03.562-0600",
     "accessorIDs": ["544820df0000142362741fc0c368de19"],
     "lastUpdateDate": "2017-10-06T13:34:04.000-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1890,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   },
   "oldState": {}
```

次の古い形式の UPDATE メッセージは、2017.3 のリリース後は使用されなくなります。

```
{
     "eventType": "UPDATE",
     "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
     "fields": {
     "ID": "59d7dcde000001b2330bda8ac63fee16",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:43:26.305-0600",<
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:43:49.265-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1892,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
   }
 }
```

2017.3 のリリース後は、次の新しい形式の UPDATE メッセージが使用されます。

```
{
   "eventType": "UPDATE",
   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
   "eventTime": {
     "nano": 998000000,
     "epochSecond": 1507319336
   },
   "newState": {
     "ID": "59d7ddf7000002322d791eb08bafddfb",
     "name": "EventSub Test updated",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:48:07.776-0600",
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19",
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1894,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  },
  "oldState": {
     "ID": "59d7ddf7000002322d791eb08bafddfb",
     "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
     "objCode": "PROJ",
     "entryDate": "2017-10-06T13:48:07.776-0600",
     "accessorIDs": [
        "544820df0000142362741fc0c368de19"
     ],
     "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
     "groupID": "544820df0000140f6a9c1faa7cacadd3",
     "sponsorID": null,
     "description": null,
     "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
     "enteredByID": "544820df0000142362741fc0c368de19",
     "ownerID": "544820df0000142362741fc0c368de19"
     "templateID": null,
     "priority": 0,
     "companyID": null,
     "portfolioID": null,
     "referenceNumber": 1894,
     "lastUpdatedByID": "544820df0000142362741fc0c368de19",
     "customerID": "544820df0000135b7719dcca654391f6",
     "currency": null,
     "categoryID": null,
     "status": "CUR",
     "parameterValues": {}
  }
}
```
