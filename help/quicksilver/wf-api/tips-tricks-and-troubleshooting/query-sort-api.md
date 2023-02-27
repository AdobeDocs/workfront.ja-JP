---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API でのクエリ結果の並べ替え
description: API でのクエリ結果の並べ替え
author: Becky
feature: Workfront API
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 0%

---


# API でのクエリ結果の並べ替え

API 呼び出しに以下を追加すると、任意のフィールドで結果を並べ替えることができます。

```
&entryDate_Sort=asc
```

たとえば、タスク「計画開始日」で並べ替える場合は、 `entryDate` で置き換えます。 `plannedCompletionDate`.

これは、Adobe Workfrontのほとんどのフィールドで機能します。
