---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードのレポートで日付を書式設定する
description: Adobe Workfront では、レポートやリストに様々な形式で表示されるように日付を設定できます。日付形式を設定するには、列のテキストモードコードの valueformat 行を変更する必要があります。
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 94%

---

# テキストモードのレポートで日付を書式設定する

<!-- Audited: 1/2025 -->

Adobe Workfront では、レポートやリストに様々な形式で表示されるように日付を設定できます。日付形式を設定するには、列のテキストモードコードの `valueformat` 行を変更する必要があります。

`valueformat= [new date format]`例えば、見込み完了日を MM/DD/YY と表示する場合、コードは次のようになります。

```
valueformat=atDate
valuefield=projectedCompletionDate
```

予定完了日を&#x200B;*月、日、年*&#x200B;として表示する場合、コードは次のようになります。

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

テキストモードを使用した Workfront レポートおよびリストでの条件付き書式の適用について詳しくは、[テキストモードでの条件付き書式の使用](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)を参照してください。

次の `valueformat` テキストモードの値を使用して、日付を書式設定できます。

| **形式** | 例  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY Time | 10/11/18 12:00pm | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| 月、日、年 | 2018年10月11日（PT） | `mediumAtDate` |
| DW, Mth, Day, YR | 2018年10月11日(PT) | `partialAtDate` |
| DW, Mth, Day, YR Time | 2018年10月11日午後12:00（PT） | `fullAtDate` |
