---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 通貨が null の場合に、プロジェクトの通貨情報を取得する
description: 通貨が null の場合に、プロジェクトの通貨情報を取得する
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '121'
ht-degree: 100%

---

# 通貨が null（割り当てられていない）の場合に、プロジェクトの通貨情報を取得する

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

プロジェクトに通貨が設定されていない場合、この応答には `null` の値の通貨が含まれます。

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

この応答には、ユーザーがデフォルトとして設定した通貨が含まれ、その通貨が設定されていない顧客のプロジェクトで使用されます。

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
