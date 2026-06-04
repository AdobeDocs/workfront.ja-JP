---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードのレポートで日付を書式設定する
description: Adobe Workfront では、レポートやリストに様々な形式で表示されるように日付を設定できます。 日付形式を設定するには、列のテキストモードコードの valueformat 行を変更する必要があります。
author: Courtney
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-8gB8XDwLQTBCUsrex-PIAyxcF-rSPsoM2Gvw2EhTaU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 204
ht-degree: 92%

---

# テキストモードのレポートで日付を書式設定する

<!-- Audited: 1/2025 -->

Adobe Workfront では、レポートやリストに様々な形式で表示されるように日付を設定できます。 日付形式を設定するには、列のテキストモードコードの `valueformat` 行を変更する必要があります。

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

日付は、次の`valueformat` テキストモード値を使用して書式設定できます。

| **形式** | 例  | ***valueformat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY Time | 10/11/18 12:00pm | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| 月、日、年 | 2018年10月11日（PT） | `mediumAtDate` |
| DW, Mth, Day, YR | 2018年10月11日(PT) | `partialAtDate` |
| DW, Mth, Day, YR Time | 2018年10月11日（月）午後12:00 | `fullAtDate` |
