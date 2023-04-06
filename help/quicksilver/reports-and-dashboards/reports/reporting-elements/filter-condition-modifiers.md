---
product-area: reporting
navigation-topic: reporting-elements
title: フィルターおよび条件修飾子
description: フィルターおよび条件修飾子を使用すると、フィルターを作成し、レポート結果を書式設定するための条件を設定できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 13e9d926-8a89-490e-aa7a-e6e8baf2a36b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# フィルターおよび条件修飾子

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: This is temporary - Lilit is fixing this in a future story: NOTE If the field you are filtering for has multiple options, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. See this document and search for "not equal" for the link to the req doc: https://docs.google.com/document/d/1WA0zZ_wws-2qb908i53BFQ8zDwL3nPJHyIybtJvvnqU/edit) </p>
-->

フィルターおよび条件修飾子を使用すると、フィルターを作成し、レポート結果を書式設定するための条件を設定できます。

フィルターの作成について詳しくは、「 [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

ビューで条件付き書式を使用する方法について詳しくは、「 [ビューでの条件付き書式の使用](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

## フィルターおよび条件修飾子

組み込みの時間枠修飾子のリストについては、「 [時間枠でレポートをフィルタリングする](../../../reports-and-dashboards/reports/creating-and-managing-reports/filter-reports-time-frames.md).

一部の修飾子は組み込みで、フィルター内のドロップダウンメニューまたは条件付き書式ステートメントから選択できます。 その他の修飾子は、テキストモードのフィルターでのみ使用できます。 テキストモードについて詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

フィルターおよび条件付き書式設定ステートメントでは、次の条件修飾子を使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>ビルトイン修飾子</strong> </p> </th> 
   <th> <p><strong>テキストモード修飾子</strong> </p> </th> 
   <th> <p><strong>説明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td> <p><strong>ブランク</strong> </p> </td> 
   <td> <p><strong>ブランク</strong> </p> </td> 
   <td> <p>オブジェクトに対してフィールドが存在しますが、フィールドに値がまだ指定されていません。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>ブランクでない</strong> </p> </td> 
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
   <td> <p>（大文字と小文字を区別しない）これは、 <strong>次を含む</strong>. 例："cicontains inf"は"Inf"または"inf"を含む値をキャプチャします。</p> <p> <p>注意：Adobe Workfrontは、各フィルター文に指定した語句を検索します。 例えば、名前に「new project」という語句を含むプロジェクトを検索すると、Workfrontでは、名前に「new」、「project」、「new main project」のいずれかが含まれるプロジェクトは表示されません。 フィルターは、名前に「new project」と完全に一致するフレーズを持つプロジェクトのみを検索します。</p> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cieq</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別しない）これは、 <strong>eq</strong>. 検索された値の完全一致のみが返されます。</p> <p>例えば、特定の名前のタスクを検索する場合、「task name cieq test」は、名前が「Test」、「TEST」、または「Test」のタスクを検索しますが、「test 123」という名前のタスクは見つかりません。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>cin</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別しない）これは、 <strong>in</strong>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>線毛</strong> </p> </td> 
   <td> <p>これは、大文字と小文字を区別しないバージョンの <strong>いいね！</strong>. 例："cilike %Current% %Dead%"は、"Current to Dead"または"current to dead"を含む注記を返します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>シノチン</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別しない）これは、 <strong>notin</strong>.</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 テキストモードを使用したフィルターの作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>含む</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別）テキスト文字列全体で指定したテキストを検索します。</p> <p>例えば、「Infinity」という単語など、「Infi」を含むすべての情報を取り込みます。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>含まない (大文字と小文字を区別しない)</strong> </p> </td> 
   <td> <p><strong>cinotains</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別しない）指定した値を持たない項目をフィルタリングします。</p> <p>例えば、「次を含まない」と指定すると、名前に「Inf」または「inf」が含まれていないすべての情報が取り込まれます。</p> <p>注意： <span>フィルターを適用するフィールドに複数のオプションが含まれる場合、指定した選択肢と指定した選択肢の両方を含む結果が除外されます。</span> </p> </td> 
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
   <td> <p> </p> <p> </p> <p> </p> <p><strong>等しい (大文字と小文字を区別しない)</strong> </p> </td> 
   <td> <p></strong>の<strong> </strong></p> </td> 
   <td> <p>（大文字と小文字を区別）この修飾子を使用すると、変数のコンマ区切りリストを作成して、フィルターで評価された単一の属性と比較できます。 リスト全体は OR ステートメントとして扱われ、1 つ以上の変数の条件を満たす結果が返されます。</p> <p>たとえば、プロジェクトを検索する場合、「CUR、PLN、CPL」を使用すると、「現在」、「計画」、「完了」のステータスのすべてのプロジェクトが戻されます。</p> <p>組み込みの修飾子 <strong>次と等しい</strong> は、 <strong>in</strong>. つまり、「次と等しい」をフィールドに複数の値を指定して選択できます。</p> <p>例えば、プロジェクトレポートで「ステータス=現在、計画、デッド」を選択し、これらのステータスのプロジェクトを表示できます。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td> <p><strong>eq</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別）検索された値に完全に一致するもののみを返します。</p> <p>例えば、完全なプロジェクトを検索する場合、「eq CPL」は完全なステータスのすべてのプロジェクトを返します。 「eq CPL, CUR」は、プロジェクトを完了し、同時に現在の状態にすることができないため、結果を返しません。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 テキストモードを使用してフィルターを作成する方法について詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>より大きい</strong> </p> </td> 
   <td> <p><strong>gt</strong> </p> </td> 
   <td> <p>入力された値より大きい値（入力された値を除く）を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>いいね！</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別） <strong>次を含む</strong>. しかし、 <strong>いいね！</strong> には、ワイルドカード文字を挿入してテキストを分割する機能があります。</p> <p>例えば、メモを検索する際に「like %Current% %Dead%」を使用すると、「Current to Dead」というフレーズを含むメモが返されます。 「Dead to Current」を含むメモは含まれません。 各値は、リストに表示されている順序で検索されます。 %は、テキストの文字やセグメントを置き換えるワイルドカードを表します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>より小さい</strong> </p> </td> 
   <td> <p><strong>lt</strong> </p> </td> 
   <td> <p>入力された値を含まず、入力された値より小さい値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>以上</strong> </p> </td> 
   <td> <p><strong>gte</strong> </p> </td> 
   <td> <p>入力された値以上の値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>以下</strong> </p> </td> 
   <td> <p><strong>lte</strong> </p> </td> 
   <td> <p>入力された値以下の値を持つすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>間</strong> </p> </td> 
   <td> <p><strong>間</strong> </p> </td> 
   <td> <p>2 つの必須フィールド値を提供し、入力された値を含む両方のフィールドの範囲内にあるすべての結果を検索します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notcontains</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別）指定した値を持たない項目をフィルタリングします。</p> <p>例えば、「notcontains inf」は「inf」を含まないすべてのを取り込みますが、「Inf」を含む値が表示されます。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p> </p> </td> 
   <td> <p><strong>notbetween</strong> </p> </td> 
   <td> <p>これは、 <strong>間</strong>. 2 つの必須の値フィールドを提供し、入力された値を含む両方のフィールドの範囲外にあるすべての結果を検索します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>等しくない (大文字と小文字を区別しない)</strong> </p> </td> 
   <td> <p><strong>notin</strong> </p> </td> 
   <td> <p>（大文字と小文字を区別）これは、 <strong>in</strong>. 指定したリストにない結果のみを返します。</p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> <p>注意： <span>フィルターを適用するフィールドに複数のオプションが含まれる場合、指定した選択肢と指定した選択肢の両方を含む結果が除外されます。</span> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>ne</strong> </td> 
   <td> <p>（大文字と小文字を区別）これは、 <strong>eq</strong>. 検索された値と完全に一致しない結果のみが返され、また、値と大文字と小文字が一致します。</p> <p>例： <b>ne</b> は、「現在」に等しくない値を返しますが、「現在」に等しくない値は返しません。 </p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.<br></p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> </td> 
   <td><strong>シネ</strong> </td> 
   <td> <p>（大文字と小文字を区別しない）これは、 <strong>ne</strong> そしてそれは <b>cieq</b> 修飾子。 検索された値と完全に一致しない結果のみが返され、値の場合は考慮されません。</p> <p>例： <b>シネ</b> 「current」または「Current」に等しくない値を返します。 </p> <p>この修飾子は、テキストモードのフィルターでのみ使用できます。 フィルターのテキストモードについて詳しくは、 <a href="../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">テキストモードを使用したフィルターの編集</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
