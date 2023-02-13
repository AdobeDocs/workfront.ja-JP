---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードのレポートで日付を書式設定する
description: Adobe Workfrontでは、レポートやリストに様々な形式で表示されるように日付を設定できます。 日付形式を設定するには、列のテキストモードコードの valueformat 行を変更する必要があります。
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 2%

---

# テキストモードのレポートで日付を書式設定する

Adobe Workfrontでは、レポートやリストに様々な形式で表示されるように日付を設定できます。 日付形式を設定するには、 `valueformat` 列内のテキストモードコードの行。

`valueformat= [new date format]` 例えば、「完了予定日」を「MM/DD/YY」と表示する場合、コードは次のようになります。

```
valueformat=atDate
valuefield=projectedCompletionDate
```

「計画完了日」を「 *月、日、年*&#x200B;の場合、コードは次のようになります。

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

テキストモードを使用したWorkfrontのレポートおよびリストでの条件付き書式の適用について詳しくは、 [テキストモードでの条件付き書式の使用](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

次のように日付をフォーマットできます。

```
valueformat
```

 テキストモード値：

| **形式** | 例  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY 時間 | 10/11/18 12:00pm | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| 月、日、年 | 2018 年 10 月 12 日 | `mediumAtDate` |
| DW、月、日、年 | 2018 年 10 月 11 日 (PT) | `partialAtDate` |
| DW、月、日、年 | 2018 年 10 月 11 日 (PT) 午後 12:00 | `fullAtDate` |
