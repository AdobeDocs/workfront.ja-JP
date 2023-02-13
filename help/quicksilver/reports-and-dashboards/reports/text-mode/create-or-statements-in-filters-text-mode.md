---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードフィルターでの「OR」ステートメントの作成
description: リストおよびレポートでフィルターを作成する際に、複数のステートメントを含めることができます。
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# テキストモードフィルターでの「OR」ステートメントの作成

リストおよびレポートでフィルターを作成する際に、複数のステートメントを含めることができます。

フィルターの作成について詳しくは、次の記事を参照してください。

* [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [テキストモードを使用したフィルターの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## テキストモードのフィルター演算子

標準フィルターインターフェイスのAdobe Workfrontフィルター演算子について詳しくは、 [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfrontには、各フィルター文を結び付ける 2 つのフィルター演算子があります。

* **および**:AND 演算子で 2 つのフィルター文を結合する場合、両方のフィルター文を同時に満たす必要があることを示します。

   デフォルトでは、フィルター内のステートメントは AND 演算子で結合されます。

   テキストモードインターフェイスで AND フィルターを作成する場合、AND 演算子を使用する必要はありません。 想定されています。

   **例：** 「計画完了日」が「今日」で、「完了率」が 100%未満のタスクをフィルタするには、次のテキスト・モード・コードを使用します。

   <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **または**:OR 演算子で 2 つのフィルター文を結合する場合は、いずれかの文を満たす必要があることを示します。

   >[!TIP]
   >
   >AND 文を OR 文に変更すると、レポートの項目数が増えます。

   テキストモードインターフェイスを使用して OR フィルターを作成する場合は、OR 演算子を使用する必要があります。

   **例：** 「計画完了日」が「今日」または「完了率」が 100%未満のタスクをフィルタするには、次のテキスト・モード・コードを使用します。

   <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>または:1:percentComplete=100</pre><pre>または:1:percentComplete_Mod=lt</pre>

## OR フィルターのテキストモード構文

OR フィルターのテキストモード構文には、次の内容が含まれている必要があります。

* OR 文内のオブジェクトを参照する各フィルタ行の先頭にコロン、数値、および別のコロンが続く OR 演算子。 これには、フィルタフィールドまたは属性を参照する行と、フィルタ修飾子を参照する行が含まれます。

   OR フィルターを作成する場合は、次のパターンに従います。

   <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>OR:1:<field name in camel case>=<value></pre><pre>OR:1:<field name in camel case>_Mod=<modifier value></pre>

   >[!TIP]
   >
   >OR 演算子は大文字と小文字が区別され、常に大文字になります。

   1 つのフィルターに複数の OR ステートメントを含めることができます。 この場合、各 OR ステートメントは、ステートメントを適用する順序で数値を受け取ります。

   **例：**  「計画完了日」が「今日」、「完了率」が 100%未満のタスクまたは「新規」ステータスを持つタスクをフィルタするには、次のテキスト・モード・コードを使用します。

   <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>または:1:status=NEW</pre><pre>または:1:status_Mod=in</pre><pre>または:2:percentComplete=100</pre><pre>または:2:percentComplete_Mod=lt</pre>

* フィールドの名前やフィルターで参照する属性は、キャメルケースで記述する必要があります。 キャメルケースについて詳しくは、 [テキストモード構文の概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md).
* OR フィルタでカスタムフィールドを参照する場合は、DE を挿入する必要があります。OR 修飾子の構文とカスタムフィールドの名前の間に挿入されます。 Workfrontインターフェイスに表示されるカスタムフィールドの名前は、スペルする必要があります。

   **例：** ステータスが「新規」または「完了率」が 100%未満のタスク、または値が「次と等しい」のカスタムフィールドをフィルターするには、次のテキストモードコードを使用します。

   <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>または:1:percentComplete=100</pre><pre>または:1:percentComplete_Mod=lt</pre><pre>または:2:DE:Account Type=Capital</pre><pre>または:2:DE:Account Type_Mod=in</pre>
