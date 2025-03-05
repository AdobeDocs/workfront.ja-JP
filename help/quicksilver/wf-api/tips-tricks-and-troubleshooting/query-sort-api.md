---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API でのクエリ結果の並べ替え
description: API でのクエリ結果の並べ替え
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
source-git-commit: 5936982217adc6cfcaf9e400bfff67a1496d3a78
workflow-type: tm+mt
source-wordcount: '60'
ht-degree: 71%

---


# API でのクエリ結果の並べ替え

API 呼び出しに以下を追加すると、任意のフィールド別に結果を並べ替えることができます。

```
&entryDate_Sort=asc
```

例えば、予定完了日でタスクを並べ替える場合は、`entryDate` を削除して `plannedCompletionDate` に置き換えます。

```
&plannedCompletionDate_Sort=asc
```

これは、Adobe Workfront のほとんどのフィールドで使用できます。
