---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 大きなページ分割検索中に返される重複
description: 大きなページ分割検索中に返される重複
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---


# 大きなページ分割検索中に返される重複

## 問題

API でオブジェクトに対して大きなページ分割検索を実行すると、重複したエントリと見つからないレコードを受け取る問題を修正しました。

## 解決策

順序が正式に定義されていない場合、Oracleデータベースから返される行の順序に依存しますが、決定論的な順序は保証されません。 例えば、同じクエリで連続した 2 回の呼び出しを実行すると、異なる順序で行が返される場合があります。 同様に、ページングを実行すると、行が異なる「ページ」にランダムに割り当てられ、重複が発生する場合があります。 最も簡単な解決策は、ID で並べ替えを追加することです。

```
&ID_Sort=asc
```

