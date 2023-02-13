---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントのサムネールを取得する
description: ドキュメントのサムネールを取得する
author: John
feature: Workfront API
exl-id: 31960689-1811-4ba7-a63d-0842caedf3ea
source-git-commit: 5cb65c3a0c3ffd374c4002867c9c48985378e03c
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
