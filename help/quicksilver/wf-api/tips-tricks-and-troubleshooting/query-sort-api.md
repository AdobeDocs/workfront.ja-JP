---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API でのクエリ結果の並べ替え
description: API でのクエリ結果の並べ替え
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '60'
ht-degree: 100%

---


# API でのクエリ結果の並べ替え

API 呼び出しに以下を追加すると、任意のフィールド別に結果を並べ替えることができます。

```
&entryDate_Sort=asc
```

例えば、タスクの予定開始日で並べ替える場合は、`entryDate` を削除し、`plannedCompletionDate` に置き換えます。

これは、Adobe Workfront のほとんどのフィールドで使用できます。
