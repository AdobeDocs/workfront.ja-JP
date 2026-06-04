---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: ページ分割された大規模な検索で重複する結果が返される
description: ページ分割された大規模な検索で重複する結果が返される
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 111
ht-degree: 100%

---

# ページ分割された大規模な検索で重複する結果が返される

## 問題

あるオブジェクトに対して API でページ分割された大規模な検索を実行すると、重複したエントリを受け取ったり、レコードが欠落したりします。

## ソリューション

順序が形式的に定義されていない場合は、Oracle データベースから返される行の順序に依存するので、確定的な順序は保証されません。 例えば、同じクエリで呼び出しを 2 回続けて実行すると、違う順序で行が返される可能性があります。 同様に、ページングを実行すると、異なる「ページ」に行がランダムに割り当てられ、重複が発生する場合があります。 最も簡単な解決策は、ID での並べ替えを追加することです。

```
&ID_Sort=asc
```

