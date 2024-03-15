---
product-area: reporting
navigation-topic: reporting-elements
title: フィルターおよび条件修飾子
description: フィルターおよび条件修飾子を使用すると、フィルターを作成し、レポート結果を形式設定するための条件を指定できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: d2268e50080ddbe306731d034d88fd29b712b86d
workflow-type: tm+mt
source-wordcount: '1516'
ht-degree: 71%

---

# フィルターおよび条件修飾子

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

フィルターおよび条件修飾子を使用すると、フィルターを作成し、レポート結果を形式設定するための条件を指定できます。

フィルターの作成について詳しくは、「 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

ビューで条件付き形式を使用する方法について詳しくは、[ビューでの条件付き形式の使用](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)を参照してください。

## フィルターおよび条件修飾子

一部の修飾子は組み込みで、フィルター内のドロップダウンメニューまたは条件付き形式ステートメントから選択できます。その他の修飾子は、テキストモードのフィルターでのみ使用できます。

テキストモードについて詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)を参照してください。

組み込みの時間枠修飾子のリストについて詳しくは、[時間枠でレポートをフィルタリング](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md)の記事を参照してください。

フィルターおよび条件付き形式設定ステートメントでは、次の条件修飾子を使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>組み込み修飾子</strong> </p> </th> 
   <th> <p><strong>テキストモード修飾子</strong> </p> </th> 
   <th> <p><strong>説明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>が空白である</strong> </p> </td> 
   <td> <p><strong>blank</strong> </p> </td> 
   <td> <p>オブジェクトに対してフィールドが存在しますが、フィールドには現在値がありません。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>が空白でない</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>フィルターしようとするフィールドが存在し、値が指定されています。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>NULL</strong> </p> </td> 
   <td> <p>フィールドが空白か、存在しません。例えば、親タスク ID のない項目を検索するとします。つまり、スタンドアロンタスクのみを表示することを意味します。ID のないタスク（この場合は親）は存在しないので、「親タスク ID」の修飾子は <strong>NULL</strong> となります。 </p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>フィルターを適用するフィールドが存在し、NULL 以外の値が含まれています。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>次を含む</strong> </p> </td> 
   <td> <p><strong>cicontains</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> のバージョン <strong>次を含む</strong>. 例： <code>cicontains inf</code> は、次のいずれかを含む値を取り込みます。 <code>Inf</code> または <code>inf</code>.</p> <p> <p>メモ：Adobe Workfront は、各フィルターステートメントに指定したそのままの語句を検索します。例えば、次のフレーズを含むプロジェクトを検索する場合、 <code>new project</code> 「 」という名前で、Workfrontには <code>new</code> または <code>project</code>または <code>new main project</code> 」と入力します。 フィルターは、完全に一致するフレーズを持つプロジェクトのみを検索します <code>new project</code> 」と入力します。</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>が次を含まない</strong> </p> </td> 
   <td> <p><strong>cinotcontains</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> のバージョン <strong>notcontains</strong>.</p><p>この修飾子は、指定された値を持たない項目をフィルタ処理します。</p> <p>例： <code>does not contain inf</code> を使用して何もキャプチャしません <code>Inf</code> または <code>inf</code> 」と入力します。</p> <p>メモ：<span>フィルターを適用するフィールドに複数のオプションが含まれる場合、指定した選択肢、指定した選択肢と追加の選択肢の両方を含む結果をフィルタリングします。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>contains</strong> </p> </td> 
   <td> <p> 指定した <i>大文字と小文字を区別</i> テキスト文字列全体のテキスト。</p> <p>例えば、 <code>contains Inf</code> 次のものをキャプチャ： <code>Inf</code> その中で、例えば、 <code>Infinity.</code></p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用してフィルターを編集</a>を参照してください。</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>このフィルターは、 <i>大文字と小文字を区別</i> 値を指定します。</p> <p>例： <code>notcontains inf</code> を使用して何もキャプチャしません <code>inf</code>を含む値が表示されますが、 <code>Inf</code>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>を参照してください。</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> 選択肢 <strong>eq</strong>. 完全一致する検索された値のみが返されます。</p> <p>例えば、特定の名前のタスクを検索する場合、 <code>task name cieq test</code> 名前が次の場所にあるタスクを検索します <code>Test</code>, <code>TEST</code>または <code>Test</code>が見つかりませんが、 <code>test 123.</code></p> <p>ステータスを検索する場合、 <strong>cieq</strong> 修飾子はサポートされていません。 大文字と小文字を区別する修飾子を使用してください。 <strong>eq</strong>、をクリックしてステータスを検索します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用してフィルターを編集</a>を参照してください。</p> </td>
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>cine</strong> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> 選択肢 <strong>ne</strong>そして、これは <b>cieq</b> 修飾子 検索された値と完全に一致しない結果のみが返され、値の大文字小文字の区別は考慮されません。</p> <p>例えば、<b>cine</b>は、「current」または「Current」に等しくない値を返します。 </p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>を参照してください。</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>この修飾子は正確なのみを返します。 <i>大文字と小文字を区別</i> 検索された値の一致。</p> <p>例えば、完全なプロジェクトを検索する場合、 <code>eq CPL</code> 「完了」ステータスのすべてのプロジェクトを返します。 <code>eq CPL, CUR</code> は結果を返しません。これは、プロジェクトを完了し、同時に現在にすることができないからです。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用してフィルターを編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>これが <i>大文字と小文字を区別</i> ～とは反対の <strong>eq</strong>. 検索された値と完全に一致しない結果のみが返され、また、値の大文字と小文字も照合します。</p> <p>例えば、<b>ne</b> は、「Current」に等しくない値を返しますが、「current」に等しくない値は返しません。 </p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用してフィルターを編集</a>を参照してください。<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> これが <i>大文字と小文字を区別しない</i> のバージョン <strong>in</strong>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用してフィルターを編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cinotin</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> のバージョン <strong>notin</strong>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>次と等しい</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>この修飾子を使用すると、 <i>大文字と小文字を区別</i> 変数を使用して、フィルターで評価された単一の属性と比較できます。 リスト全体は OR ステートメントとして扱われ、1 つ以上の変数の条件を満たす結果が返されます。</p> <p>例えば、プロジェクトを検索する場合、 <code>in CUR, PLN, CPL</code> 「現在」、「計画」、「完了」のステータスのすべてのプロジェクトが戻されます。</p> <p>組み込み修飾子の<strong>次と等しい</strong>は、テキストモード修飾子 <strong>in</strong> に対応します。つまり、「次と等しい」をフィールドに複数の値を指定して選択できます。</p> <p>例えば、プロジェクトレポートでは、「ステータスは進行中、計画中、停止と等しい」のいずれかを選択して、これらのステータスのプロジェクトを表示できます。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>等しくない</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別</i> ～とは反対の <strong>in</strong>. 指定したリストにない結果のみを返します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用してフィルターを編集</a>を参照してください。</p> <p>メモ：<span>フィルターを適用するフィールドに複数のオプションが含まれる場合、指定した選択肢、指定した選択肢と追加の選択肢の両方を含む結果をフィルタリングします。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cilike</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> のバージョン <strong>いいね！</strong>. 例： <code>cilike %Current% %Dead%</code> を含むすべてのメモを返します。 <code>Current to Dead</code> または <code>current to dead</code>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>like</strong> </p> </td> 
   <td> <p>この修飾子は、 <i>大文字と小文字を区別</i> と似た方法でのテキスト文字列 <strong>次を含む</strong>. しかし、<strong>like</strong> には、ワイルドカード文字を挿入してテキストを分割する機能があります。</p> <p>例えば、メモを検索する場合、 <code>like %Current% %Dead%</code> 「Current to Dead」というフレーズを含むメモを返します。 「Dead to Current」を含むメモは含まれません。各値は、リストに表示されている順序で検索されます。％ は、テキストの文字やセグメントを置き換えるワイルドカードを表します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>を参照してください。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>が存在しない</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>この修飾子は、EXISTS 文内の複雑なフィルターでのみ使用します。これらのフィルターは、次のオブジェクトのみを参照します。 </p> 
    <ul> 
     <li>オブジェクト階層内の複数のレベルにまたがるオブジェクト </li> 
     <li>欠落しているオブジェクト </li> 
    </ul> <p>EXISTS ステートメントを使用した複雑なフィルターの作成について詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">EXISTS ステートメントを使用した複雑なテキストモードフィルターの作成</a>を参照してください。これは、EXISTS 文で使用される唯一の修飾子です。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>が次より大きい</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>入力された値より大きい値（入力された値を含まない）を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>より小さい</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>入力された値を含まず、入力された値より小さい値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>が次よりも大きいか等しい</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>入力された値と等しいか、それ以上の値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>が次よりも小さいか等しい</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>入力された値と等しいか、それ以下の値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>間</strong> </p> </td> 
   <td> <p><strong>間</strong> </p> </td> 
   <td> <p>2 つの必須フィールド値を提供し、入力された値を含む、両方のフィールドの範囲内にあるすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>これは、<strong>between</strong> の逆です。2 つの必須の値フィールドを提供し、入力された値を含む両方のフィールドの範囲外にあるすべての結果を検索します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、<a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用してフィルターを編集</a>を参照してください。</p> </td> 
  </tr>

</tbody> 
</table>
