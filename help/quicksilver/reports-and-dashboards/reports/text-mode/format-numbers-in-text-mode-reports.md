---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードのレポートでの数値、通貨、割合の値の形式設定
description: Adobe Workfront では、レポートやリストに様々な形式で表示されるように、通貨を含む数値を設定できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: e1411ce49d8668ba50bcb9b80d4a4b47d0dd00fc
workflow-type: ht
source-wordcount: '154'
ht-degree: 100%

---

# テキストモードのレポートでの数値、通貨、割合の値の形式設定

Adobe Workfront では、レポートやリストに様々な形式で表示されるように、通貨を含む数値を設定できます。

数値のフォーマットを変更するには、**valueformat** 列の行を編集する必要があります。

例えば、予算の列を 1000 ドルと表示する場合、値の形式行は次のようになります。

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

テキストモードを使用した Workfront のレポートおよびリストでの条件付き形式の適用について詳しくは、[テキストモードでの条件付き形式の使用](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)を参照してください。

次の値を `valueformat` 列の行に使用して、数値の形式を設定できます。

| 例 | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br> または <br><pre>int</pre> |
| 1,234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

