---
content-type: api
navigation-topic: wf-api
title: ユーザーに利用可能な時間 API を取得する
description: ユーザーに利用可能な時間 API を取得する
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
TQID: https://experienceleague.adobe.com/JPvalH2RQRfMeqbYyWXyjyXCx-bdaZwRoR6WDRerZ5U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 95
ht-degree: 100%

---

# ユーザーが利用できる時間 API

**URI: attask/api/v15.0/user/getUsersAvailableTime**

ユーザーが利用可能な時間エンドポイントは、ユーザーの利用可能な時間に関するデータを取得します。 これにより、ユーザー属性と時間間隔に従ってデータを集計するための統合が可能になります。

## リクエストの例

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## パラメーターのリクエスト

* **userIDs**：文字列の配列。 必須。 例：`"61a9cc0500002f9fdaa7a6f824f557e1"`

* **fromDate**：datetime。 文字列。 必須。 例：`"2022-07-10T00:00:00"`

* **toDate**：datetime。 文字列。 必須。 例：`"2022-07-20T23:59:59"`

## 応答の例：

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## 応答パラメーター

* **AVL**：実際の使用可能時間。 数値の配列。
* **PAVL**：非稼働日やユーザー休暇を含まないスケジュールに使用できる純粋な時間。 文字列。
