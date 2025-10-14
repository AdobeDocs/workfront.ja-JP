---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードの一般的な使用例の概要
description: テキストモードの一般的な使用例の概要
author: Nolan
feature: Reports and Dashboards
exl-id: 81512837-1ec4-4dbc-ace4-bdf08fe667ce
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 92%

---

# テキストモードの一般的な使用例の概要

<!-- Audited: 1/2025 -->

<!--(NOTE: Alina: ***This is linked to Understanding Text Mode (article), and the TOC article for examples of various reporting elements)</p>-->

レポートおよびレポート要素でテキストモードを使用して、レポート機能を拡張できます。テキストモードのバージョンを使用して、より複雑な計算カスタムフィールドを作成することもできます。テキストモードについて詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)を参照してください。

この記事では、テキストモードを使用して Adobe Workfront のレポートや計算カスタムフィールドの機能を拡張する必要があると考えられる、いくつかの一般的な例の概要を説明します。より広範な例のリストについては、以下を参照してください。

* [カスタムビュー、フィルター、およびグループ化の例：記事インデックス](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
* [レポート内の計算カスタムデータ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)

クラス、ビデオ、チュートリアルなど、テキストモードを使用したレポートの作成について詳しくは、Adobe Experience League サイトの学習の節を参照してください。

## リストとレポートでテキストモードを使用する可能性がある場合

Report Builder と List Builder を使用して、ビュー、フィルターおよびグループ化を作成することをお勧めします。ただし、テキストモードを使用してレポートやリストの内容を強化できる場合もあります。

テキストモードは、Workfrontで以下を実現する場合に使用できます。

* カスタムフォームで計算カスタムフィールドを作成します。\
  計算カスタムフィールドについて詳しくは、この記事の[計算カスタムフィールドでテキストモードを使用](#use-text-mode-in-calculated-custom-fields)の節を参照してください。
* Report Builder で可能な機能を超えて、フィルター、ビューおよびグループ化を強化します。フィルター、ビュー、グループ化でのテキストモードの使用について詳しくは、この記事の次の節を参照してください。

   * [ビューでのテキストモードを使用](#use-text-mode-in-views)
   * [フィルターでのテキストモードを使用](#use-text-mode-in-filters)
   * [グループ化でテキストモードを使用](#use-text-mode-in-groupings)

* カスタムプロンプトを作成します。テキストモードを使用する場合のみ、カスタムプロンプトを作成できます。

  カスタムプロンプトの作成について詳しくは、[レポートへのプロンプトの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)を参照してください。

## 計算カスタムフィールドでテキストモードを使用 {#use-text-mode-in-calculated-custom-fields}

テキストモードを使用して、計算カスタムフィールドをカスタムフォームに追加できます。

計算カスタムフィールドをカスタムフォームに追加する方法について詳しくは、「[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

テキストモードで計算カスタムフィールドを作成する方法について詳しくは、[&#x200B; 計算フィールドをフォームに追加する &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) を参照してください。

例えば、項目が作業中とマークされた時点の日時スタンプを表示する計算カスタムフィールドを追加できます。この計算を他のステータスに使用できます。

詳しくは、[計算カスタムフィールドの例：カスタムフォームにステータスタイムスタンプを表示](../../../reports-and-dashboards/reports/calc-cstm-data-reports/example-status-timestamp-in-calculated-field.md)を参照してください。

## ビューでのテキストモードを使用 {#use-text-mode-in-views}

ビューでテキストモードを使用すると、ビューで表示できるフィールドやオブジェクトを展開できます。

ビューでテキストモードを使用する最も一般的な理由の例については、次の記事を参照してください。

* [表示：標準インターフェイスに含まれていないオブジェクトを表示](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-objects-not-in-standard-interface.md)
* [表示：列の 2 つのフィールド間で計算結果を表示](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculation-between-two-fields.md)
* [表示：列の幅を永続的に編集](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md)
* [表示：1 つの共有列の複数の列から情報を結合](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)
* [表示：列内のオブジェクトへのリンクを削除](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-remove-link-to-object.md)
* [レポート内のコレクションの参照](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)
* [表示：列の内容の非表示](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-hide-column-content.md)
* [表示：列に文字列ではなく画像を表示](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-image-in-view.md)
* [表示：タスクリストでのタスクのインデントの表示](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-task-identations.md)
* [表示：時間と日付の差異の計算](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-calculate-time-and-date-differences.md)

## フィルターでのテキストモードの使用 {#use-text-mode-in-filters}

フィルターを作成する際に、テキストモードを使用して、フィルターに使用できるフィールドやオブジェクトを展開できます。

フィルターでテキストモードを使用する最も一般的な理由の例については、次の記事を参照してください。

* [フィルター：同じフィールド（「AND」ステートメント）を参照する複数のフィルタールールを作成](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-refrence-the-same-field-multiple-times.md)
* [フィルター：承認ステータスの項目のみを表示](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-for-items-in-approval-status.md)
* [フィルター：ステータスが異なるグループに関連付けられている場合に、同じ名前のステータスで項目を表示](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-same-name-statuses-from-different-groups.md)
* [フィルター：2 つのフィールドを比較して、リスト内の項目を除外する](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-items-by-comparing-two-fields.md)
* [EXISTS ステートメントを使用した複雑なテキストモードフィルターの作成](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)の記事で、[オブジェクト階層の複数のレベルにまたがるテキストモードフィルターの例](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#examples)の節を参照してください。
* [EXISTS ステートメントを使用した複雑なテキストモードフィルターの作成](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md)の記事で、[欠落しているオブジェクトに対して複雑なテキストモードフィルターを作成する](../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md#missing-object-filters)の節を参照してください。

## グループ化でテキストモードを使用 {#use-text-mode-in-groupings}

グループ化を作成する際に、テキストモードを使用して、リストやレポートでグループ化できるフィールドやオブジェクトを展開できます。

グループ化でテキストモードを使用する理由で最も一般的な例については、次の記事を参照してください。

* [グループ化：グループ化されたすべてのオブジェクトに共通する計算値でリストの結果を整理します](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-by-calculated-common-values.md)
* [グループ化：リストに 4 つ目のグループ化を追加します](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-add-fourth-grouping.md)
* [グループ化：グループ化された表示名を編集します](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-rename-grouping.md)
* [グループ化：テキストモードでグループ化の結果を折りたたむか展開するかを指定します](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-collapsed-or-expanded-results.md)
