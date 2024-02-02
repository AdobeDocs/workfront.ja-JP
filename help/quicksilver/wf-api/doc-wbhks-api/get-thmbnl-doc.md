---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントのサムネールの取得
description: ドキュメントのサムネールの取得
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '50'
ht-degree: 100%

---


# ドキュメントのサムネールの取得

ドキュメントのサムネールの未加工バイトデータを返します。

**URL**

GET /thumbnail

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| id  | ドキュメント ID |
| size  | サムネールの幅。 |


## 応答

サムネールの未加工のバイトデータです。

**例**：https://www.acme.com/api/thumbnail?id=123456
