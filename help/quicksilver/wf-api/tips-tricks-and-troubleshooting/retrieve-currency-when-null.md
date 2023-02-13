---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 通貨が null の場合に、プロジェクトの通貨情報を取得します
description: 通貨が null の場合に、プロジェクトの通貨情報を取得します
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# 通貨が null（割り当てられていない）の場合に、プロジェクトの通貨情報を取得します

通貨フィールドを含むプロジェクトオブジェクトは、次のリクエストを使用して取得できます。

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

これにより、次の応答本文が返されます。

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

通貨がプロジェクトに設定されていない場合、この応答には値を持つ通貨が含まれます `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

プロジェクトの通貨が必要な場合（計算用など）、顧客のデフォルトの通貨を取得できます。

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

応答には、ユーザーがデフォルトとして設定した通貨が含まれます。通貨が設定されていない顧客のプロジェクトで使用されます。

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```
