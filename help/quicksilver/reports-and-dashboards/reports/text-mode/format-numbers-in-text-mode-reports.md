---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードのレポートでの数値、通貨、割合の値の形式設定
description: Adobe Workfront では、レポートやリストに様々な形式で表示されるように、通貨を含む数値を設定できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 99%

---

# テキストモードのレポートでの数値、通貨、割合の値の形式設定

<!-- Audited: 1/2025 -->

Adobe Workfront では、レポートやリストに様々な形式で表示されるように、通貨を含む数値を設定できます。

数値のフォーマットを変更するには、列の **valueformat** 行を編集する必要があります。

例えば、予算の列を 1000 ドルと表示する場合、値の形式行は次のようになります。

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

テキストモードを使用した Workfront のレポートおよびリストでの条件付き形式の適用について詳しくは、[テキストモードでの条件付き形式の使用](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)を参照してください。

次の値を列の `valueformat` 行に使用して、数値の書式を設定できます。

| 例 | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br> または <br>`int` |
| 1,234 | `doubleAsInt` |
| $1,234 | `currencyStringCurrencyRounded` |
| 1234.56 | `doubleAsDouble` |
| $1,234.56 | `currencyStringCurrency` |
| 12% | `doubleAsPercentRounded` |
| 12.34% | `doubleAsPercent` |
| (1,234.56) | `doubleAsFinancial` |
| (1,234) | `doubleAsFinancialRounded` |

