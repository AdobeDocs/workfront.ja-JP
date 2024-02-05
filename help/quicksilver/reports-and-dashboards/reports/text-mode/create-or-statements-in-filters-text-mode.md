---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードフィルターでの「OR」ステートメントの作成
description: リストおよびレポートでフィルターを作成する際には、複数のステートメントを含められます。
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 96%

---

# テキストモードフィルターでの「OR」ステートメントの作成

リストおよびレポートでフィルターを作成する際には、複数のステートメントを含められます。

フィルターの作成について詳しくは、次の記事を参照してください。

* [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [テキストモードを使用したフィルターの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## テキストモードのフィルター演算子

標準フィルターインターフェイスのAdobe Workfrontフィルター演算子について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Workfront には、それぞれのフィルターステートメントを結び付ける 2 つのフィルター演算子があります。

* **AND**：AND 演算子で 2 つのフィルターステートメントを結合する場合は、両方のフィルターステートメントを同時に満たすように指定します。

  デフォルトでは、フィルター内のステートメントは AND 演算子で結合されます。

  テキストモードインターフェイス内に AND フィルターを作成する場合、AND 演算子を使用する必要はありません。想定済みです。

  **例：**&#x200B;予定完了日が今日のタスク、および完了率が 100％未満であるタスクをフィルタリングするには、次のテキストモードコードを使用します。

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>percentComplete=100</pre><pre>percentComplete_Mod=lt</pre>

* **OR**：OR 演算子で 2 つのフィルターステートメントを結合する場合は、どちらかのステートメントを満たす必要があることを示します。

  >[!TIP]
  >
  >AND ステートメントを OR ステートメントに変更すると、レポートの項目数が増えます。

  テキストモードインターフェイスを使用して OR フィルターを作成する場合は、OR 演算子を使用する必要があります。

  **例：**&#x200B;予定完了日が今日のタスク、または完了率が 100％未満のタスクをフィルタリングするには、次のテキストモードコードを使用します。

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OR:1:percentComplete=100</pre><pre>OR:1:percentComplete_Mod=lt</pre>

## OR フィルターのテキストモード構文

OR フィルターのテキストモード構文には、次の内容が含まれている必要があります。

* OR ステートメント内のオブジェクトを参照するそれぞれのフィルター行の先頭にコロン、数値、および別のコロンが続く OR 演算子。これには、フィルターフィールドまたは属性を参照する行と、フィルター修飾子を参照する行が含まれます。

  OR フィルターを作成する場合は、次のパターンに従います。

  <pre><field name in camel case>=<value></pre><pre><field name in camel case>_Mod=<modifier value></pre><pre>または:1:<field name in camel case>=<value></pre><pre>または:1:<field name in camel case>_Mod=<modifier value></pre>

  >[!TIP]
  >
  >OR 演算子では大文字と小文字が区別され、常に大文字です。

  1 つのフィルターに複数の OR ステートメントを含められます。この場合、すべての OR ステートメントは、ステートメントを適用する順序で数値が付けられます。

  **例：**&#x200B;予定完了日が今日のタスク、または完了率が 100％未満のタスクまたは新規ステータスを持つタスクをフィルタリングするには、次のテキストモードコードを使用します。

  <pre>plannedCompletionDate=$$TODAY</pre><pre>plannedCompletionDate_Mod=eq</pre><pre>OR:1:status=NEW</pre><pre>OR:1:status_Mod=in</pre><pre>OR:2:percentComplete=100</pre><pre>OR:2:percentComplete_Mod=lt</pre>

* フィールドの名前やフィルターで参照する属性は、キャメルケースで記述する必要があります。キャメルケースについて詳しくは、[テキストモードの構文の概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)を参照してください。
* OR フィルターでカスタムフィールドを参照する場合は、OR 修飾子の構文とカスタムフィールドの名前の間に DE: を挿入する必要があります。カスタムフィールドの名前は、Workfront インターフェイスに表示されるとおりにスペルする必要があります。

  **例：**&#x200B;ステータスが新規のタスク、または完了率が 100％未満のタスク、または「アカウントタイプ」という名前のカスタムフィールドの値が「等しい」タスクをフィルタリングするには、次のテキストモードコードを使用します。

  <pre>status=NEW</pre><pre>status_Mod=in</pre><pre>OR:1:percentComplete=100</pre><pre>OR:1:percentComplete_Mod=lt</pre><pre>OR:2:DE:Account Type=Capital</pre><pre>OR:2:DE:Account Type_Mod=in</pre>
