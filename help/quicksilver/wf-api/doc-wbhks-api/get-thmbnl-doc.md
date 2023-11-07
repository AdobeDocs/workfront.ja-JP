---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントのサムネールを取得する
description: ドキュメントのサムネールを取得する
author: Becky
feature: Workfront API
role: Developer
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '54'
ht-degree: 5%

---


# ドキュメントのサムネールを取得する

ドキュメントの生のサムネールのバイト数を返します。

**URL**

GET/サムネール

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| id  | ドキュメント ID。 |
| サイズ  |  サムネールの幅。 |


## 応答

生のサムネールのバイト数です。

**例：**: https://www.acme.com/api/thumbnail?id=123456
