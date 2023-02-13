---
content-type: api
navigation-topic: wf-api
title: ユーザーに利用可能な時間 API を取得する
description: ユーザーに利用可能な時間 API を取得する
author: John
feature: Workfront API
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: aea37c1d200dfadf9ccbb7b36145eb04d5ab4b6d
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 7%

---

# ユーザーが利用できる時間 API

**URI:attask/api/v15.0/user/getUsersAvailableTime**

ユーザーが利用可能な時間エンドポイントは、ユーザーの利用可能な時間に関するデータを取得します。 これにより、ユーザー属性と時間間隔に従ってデータを集計するための統合が可能になります。

## リクエストの例

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## リクエストパラメーター

* **userIDs**:文字列の配列。 必須. 例: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**:datetime. 文字列。 必須. 例:  `"2022-07-10T00:00:00"`.

* **toDate**:datetime. 文字列。 必須. 例 `"2022-07-20T23:59:59"`.

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

* **AVL**:実際の使用可能時間。 数値の配列。
* **パブル**:非営業日やユーザーのタイムオフを含まないスケジュールに使用できる純粋な時間。 String.
