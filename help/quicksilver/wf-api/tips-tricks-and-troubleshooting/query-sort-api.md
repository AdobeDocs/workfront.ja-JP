---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API でのクエリ結果の並べ替え
description: API でのクエリ結果の並べ替え
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
TQID: https://experienceleague.adobe.com/r7PCHEpU413ajyML7-uzWdmXN11gylNHRU2q60J35Go
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 60
ht-degree: 71%

---

# API でのクエリ結果の並べ替え

API 呼び出しに以下を追加すると、任意のフィールド別に結果を並べ替えることができます。

```
&entryDate_Sort=asc
```

例えば、タスクの予定完了日で並べ替える場合は、`entryDate`を削除して`plannedCompletionDate`に置き換えます。

```
&plannedCompletionDate_Sort=asc
```

これは、Adobe Workfront のほとんどのフィールドで使用できます。
