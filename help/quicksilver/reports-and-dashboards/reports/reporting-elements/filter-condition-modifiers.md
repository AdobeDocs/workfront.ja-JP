---
product-area: reporting
navigation-topic: reporting-elements
title: フィルターおよび条件修飾子
description: フィルターおよび条件修飾子を使用すると、フィルターを作成し、レポート結果を書式設定するための条件を設定できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 7eecc4879d1e5e760735db4de89ac1a661477be7
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 0%

---

# フィルターおよび条件修飾子

<!-- Audited: 1/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

フィルターおよび条件修飾子を使用すると、フィルターを作成し、レポート結果を書式設定するための条件を設定できます。

フィルターの作成について詳しくは、「 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

ビューで条件付き書式を使用する方法について詳しくは、「 [ビューでの条件付き書式の使用](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## フィルターおよび条件修飾子

一部の修飾子は組み込みで、フィルター内のドロップダウンメニューまたは条件付き書式ステートメントから選択できます。 その他の修飾子は、テキストモードのフィルターでのみ使用できます。

テキストモードについて詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

組み込みの時間枠修飾子のリストについては、「 [時間枠でレポートをフィルタリングする](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

フィルターおよび条件付き書式設定ステートメントでは、次の条件修飾子を使用できます。

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
   <td> <p><strong>空白である</strong> </p> </td> 
   <td> <p><strong>空白</strong> </p> </td> 
   <td> <p>オブジェクトに対してフィールドが存在しますが、フィールドには現在値がありません。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>空白でない</strong> </p> </td> 
   <td> <p><strong>notblank</strong> </p> </td> 
   <td> <p>フィルターしようとしているフィールドが存在し、値が指定されています。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>null</strong> </p> </td> 
   <td> <p>フィールドが空白か、存在しません。 例えば、親タスク ID のない項目を検索するとします。 つまり、スタンドアロンタスクのみを表示したいということです。 「親タスク ID」の修飾子は次のとおりです。 <strong>null</strong>ID のないタスク（この場合は親）は存在しないので、個別に削除できます。 </p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notnull</strong> </p> </td> 
   <td> <p>フィルターを適用するフィールドが存在し、null 以外の値が含まれています。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>次を含む</strong> </p> </td> 
   <td> <p><strong>蝉</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> のバージョン <strong>次を含む</strong>. 例： <code>cicontains inf</code> は、次のいずれかを含む値を取り込みます。 <code>Inf</code> または <code>inf</code>.</p> <p> <p>注意： Adobe Workfrontは、各フィルター文に指定した語句を検索します。 例えば、次のフレーズを含むプロジェクトを検索する場合、 <code>new project</code> 「 」という名前で、Workfrontには <code>new</code> または <code>project</code>または <code>new main project</code> 」と入力します。 フィルターは、完全に一致するフレーズを持つプロジェクトのみを検索します <code>new project</code> 」と入力します。</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>次を含まない</strong> </p> </td> 
   <td> <p><strong>cinotains</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> のバージョン <strong>notcontains</strong>.</p><p>この修飾子は、指定された値を持たない項目をフィルタ処理します。</p> <p>例： <code>does not contain inf</code> を使用して何もキャプチャしません <code>Inf</code> または <code>inf</code> 」と入力します。</p> <p>注意： <span>フィルターを適用するフィールドに複数のオプションが含まれる場合、指定した選択肢と指定した選択肢の両方を含む結果が除外され、その他の選択肢も除外されます。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>次を含む</strong> </p> </td> 
   <td> <p> 指定した <i>大文字と小文字を区別</i> テキスト文字列全体のテキスト。</p> <p>例えば、 <code>contains Inf</code> 次のものをキャプチャ： <code>Inf</code> その中で、例えば、 <code>Infinity.</code></p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>このフィルターは、 <i>大文字と小文字を区別</i> 値を指定します。</p> <p>例： <code>notcontains inf</code> を使用して何もキャプチャしません <code>inf</code>を含む値が表示されますが、 <code>Inf</code>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> 選択肢 <strong>eq</strong>. 検索された値の完全一致のみが返されます。</p> <p>例えば、特定の名前のタスクを検索する場合、 <code>task name cieq test</code> 名前が次の場所にあるタスクを検索します <code>Test</code>, <code>TEST</code>または <code>Test</code>が見つかりませんが、 <code>test 123.</code></p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>シネ</strong> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> 選択肢 <strong>ne</strong>そして、これは <b>cieq</b> 修飾子 検索された値と完全に一致しない結果のみが返され、値の場合は考慮されません。</p> <p>例： <b>シネ</b> 「current」または「Current」に等しくない値を返します。 </p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr>   <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>この修飾子は正確なのみを返します。 <i>大文字と小文字を区別</i> 検索された値の一致。</p> <p>例えば、完全なプロジェクトを検索する場合、 <code>eq CPL</code> 「完了」ステータスのすべてのプロジェクトを返します。 <code>eq CPL, CUR</code> は結果を返しません。これは、プロジェクトを完了し、同時に現在にすることができないからです。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>これが <i>大文字と小文字を区別</i> ～とは反対の <strong>eq</strong>. 検索された値と完全に一致しない結果のみが返され、また、値と大文字と小文字が一致します。</p> <p>例： <b>ne</b> は、「現在」に等しくない値を返しますが、「現在」に等しくない値は返しません。 </p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>ciin</strong> </p> </td> 
   <td> <p> これが <i>大文字と小文字を区別しない</i> のバージョン <strong>in</strong>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>シノチン</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> のバージョン <strong>notin</strong>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> <p> </p> <p> </p> <p><strong>次と等しい</strong> </p> </td> 
   <td> <p><strong>in</strong> </p> </td> 
   <td> <p>この修飾子を使用すると、 <i>大文字と小文字を区別</i> 変数を使用して、フィルターで評価された単一の属性と比較できます。 リスト全体は OR ステートメントとして扱われ、1 つ以上の変数の条件を満たす結果が返されます。</p> <p>例えば、プロジェクトを検索する場合、 <code>in CUR, PLN, CPL</code> 「現在」、「計画」、「完了」のステータスのすべてのプロジェクトが戻されます。</p> <p>組み込みの修飾子 <strong>次と等しい</strong> は、 <strong>in</strong>. つまり、「次と等しい」をフィールドに複数の値を指定して選択できます。</p> <p>例えば、プロジェクトレポートで「ステータス=現在、計画、デッド」を選択し、これらのステータスのプロジェクトを表示できます。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>等しくない</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別</i> ～とは反対の <strong>in</strong>. 指定したリストにない結果のみを返します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> <p>注意： <span>フィルターを適用するフィールドに複数のオプションが含まれる場合、指定した選択肢と指定した選択肢の両方を含む結果が除外され、その他の選択肢も除外されます。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>線毛</strong> </p> </td> 
   <td> <p>これが <i>大文字と小文字を区別しない</i> のバージョン <strong>いいね！</strong>. 例： <code>cilike %Current% %Dead%</code> を含むすべてのメモを返します。 <code>Current to Dead</code> または <code>current to dead</code>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>いいね！</strong> </p> </td> 
   <td> <p>この修飾子は、 <i>大文字と小文字を区別</i> と似た方法でのテキスト文字列 <strong>次を含む</strong>. しかし、 <strong>いいね！</strong> には、ワイルドカード文字を挿入してテキストを分割する機能があります。</p> <p>例えば、メモを検索する場合、 <code>like %Current% %Dead%</code> 「Current to Dead」というフレーズを含むメモを返します。 「Dead to Current」を含むメモは含まれません。 各値は、リストに表示されている順序で検索されます。 %は、テキストの文字やセグメントを置き換えるワイルドカードを表します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td><strong>存在しない</strong> </td> 
   <td><strong>NOTEXISTS</strong> </td> 
   <td> <p>この修飾子は、EXISTS 文内の複雑なフィルターでのみ使用します。 これらのフィルターは、次のオブジェクトのみを参照します。 </p> 
    <ul> 
     <li>オブジェクト階層内の複数のレベルにまたがるオブジェクト </li> 
     <li>見つからないオブジェクト </li> 
    </ul> <p>EXISTS ステートメントを使用した複雑なフィルターの作成について詳しくは、この記事を参照してください。 <a href="../../../reports-and-dashboards/reports/text-mode/create-complex-text-mode-filters-using-exists-statements.md">EXISTS ステートメントを使用した複雑なテキストモードフィルターの作成</a>. これは、EXISTS 文で使用される唯一の修飾子です。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>次の値より大きい</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>入力された値より大きい値（入力された値を含まない）を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>次より小さい</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>入力された値を含まず、入力された値より小さい値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>次よりも大きいか等しい</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>入力された値以上の値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>次よりも小さい</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>入力された値以下の値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>期間</strong> </p> </td> 
   <td> <p><strong>次の間</strong> </p> </td> 
   <td> <p>2 つの必須フィールド値を提供し、入力された値を含む、両方のフィールドの範囲内にあるすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>これは、 <strong>次の間</strong>. 2 つの必須の値フィールドを提供し、入力された値を含む両方のフィールドの範囲外にあるすべての結果を検索します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr>

</tbody> 
</table>
