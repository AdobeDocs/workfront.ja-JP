---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: ページ分割された大規模な検索で重複する結果が返される
description: ページ分割された大規模な検索で重複する結果が返される
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 100%

---


# ページ分割された大規模な検索で重複する結果が返される

## 問題

あるオブジェクトに対して API でページ分割された大規模な検索を実行すると、重複したエントリを受け取ったり、レコードが欠落したりします。

## ソリューション

順序が形式的に定義されていない場合は、Oracle データベースから返される行の順序に依存するので、確定的な順序は保証されません。例えば、同じクエリで呼び出しを 2 回続けて実行すると、違う順序で行が返される可能性があります。同様に、ページングを実行すると、異なる「ページ」に行がランダムに割り当てられ、重複が発生する場合があります。最も簡単な解決策は、ID での並べ替えを追加することです。

```
&ID_Sort=asc
```

