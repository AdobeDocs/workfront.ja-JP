---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードフィルターでの「OR」ステートメントの作成
description: リストおよびレポートでフィルターを作成する際には、複数のステートメントを含められます。
author: Nolan
feature: Reports and Dashboards
exl-id: be145e22-d66c-4a74-af0e-8bb0598b4d67
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 91%

---

# テキストモードフィルターでの「OR」ステートメントの作成

リストおよびレポートでフィルターを作成する際には、複数のステートメントを含められます。

フィルターの作成について詳しくは、次の記事を参照してください。

* [フィルターの概要](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [テキストモードを使用したフィルターの編集](/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)

## テキストモードのフィルター演算子

標準フィルターインターフェイスの Adobe Workfront フィルター演算子について詳しくは、[フィルターの概要](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)を参照してください。

Workfront には、それぞれのフィルターステートメントを結び付ける 2 つのフィルター演算子があります。

* **AND**:2 つのフィルターステートメントを AND 演算子で結合する場合、両方のフィルターステートメントを同時に満たすことを指定します。

  デフォルトでは、フィルター内のステートメントは AND 演算子で結合されます。

  テキストモードインターフェイス内に AND フィルターを作成する場合、AND 演算子を使用する必要はありません。想定済みです。

  **例：**&#x200B;予定完了日が今日のタスク、および完了率が 100％未満であるタスクをフィルタリングするには、次のテキストモードコードを使用します。

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq 
  percentComplete=100 percent
  Complete_Mod=lt
  ```

* **OR**：OR 演算子で 2 つのフィルターステートメントを結合する場合は、どちらかのステートメントを満たす必要があることを示します。

  >[!TIP]
  >
  >AND ステートメントを OR ステートメントに変更すると、レポートの項目数が増えます。

  テキストモードインターフェイスを使用して OR フィルターを作成する場合は、OR 演算子を使用する必要があります。

  **例：**&#x200B;予定完了日が今日のタスク、または完了率が 100％未満のタスクをフィルタリングするには、次のテキストモードコードを使用します。

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  ```

## OR フィルターのテキストモード構文

OR フィルターのテキストモード構文には、次の内容が含まれている必要があります。

* OR ステートメント内のオブジェクトを参照するそれぞれのフィルター行の先頭にコロン、数値、および別のコロンが続く OR 演算子。これには、フィルターフィールドまたは属性を参照する行と、フィルター修飾子を参照する行が含まれます。

  OR フィルターを作成する場合は、次のパターンに従います。

  ```
  <field name in camel case>=<value>
  <field name in camel case>_Mod=<modifier value>
  OR:1:<field name in camel case>=<value>
  OR:1:<field name in camel case>_Mod=<modifier value>
  ```

  >[!TIP]
  >
  >OR 演算子では大文字と小文字が区別され、常に大文字です。

  1 つのフィルターに複数の OR ステートメントを含められます。この場合、すべての OR ステートメントは、ステートメントを適用する順序で数値が付けられます。

  **例：**&#x200B;予定完了日が今日のタスク、または完了率が 100％未満のタスクまたは新規ステータスを持つタスクをフィルタリングするには、次のテキストモードコードを使用します。

  ```
  plannedCompletionDate=$$TODAY
  plannedCompletionDate_Mod=eq
  OR:1:status=NEW
  OR:1:status_Mod=in
  OR:2:percentComplete=100
  OR:2:percentComplete_Mod=lt
  ```

* フィールドの名前やフィルターで参照する属性は、キャメルケースで記述する必要があります。キャメルケースについて詳しくは、[テキストモードの構文の概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)を参照してください。
* OR フィルターでカスタムフィールドを参照する場合は、OR 修飾子の構文とカスタムフィールドの名前の間に DE: を挿入する必要があります。カスタムフィールドの名前は、Workfront インターフェイスに表示されるとおりにスペルする必要があります。

  **例：**&#x200B;ステータスが新規のタスク、または完了率が 100％未満のタスク、または「アカウントタイプ」という名前のカスタムフィールドの値が「等しい」タスクをフィルタリングするには、次のテキストモードコードを使用します。

  ```
  status=NEW
  status_Mod=in
  OR:1:percentComplete=100
  OR:1:percentComplete_Mod=lt
  OR:2:DE:Account Type=Capital
  OR:2:DE:Account Type_Mod=in
  ```
