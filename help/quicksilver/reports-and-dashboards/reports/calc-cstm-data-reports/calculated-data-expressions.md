---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算済みデータ式の概要
description: データ式を使用して、Adobe Workfront で計算済みのカスタムデータフィールドを定義できます。計算式は、新しいフィールドを生成するステートメントで Workfront の既存のフィールドを接続します。
author: Jenny, Lisa
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '2551'
ht-degree: 88%

---

# 計算済みデータ式の概要

<!--Audited: 12/2023-->

データ式を使用すると、Adobe Workfront で計算済みカスタムフィールドを定義できます。計算式は、新しいフィールドを生成するステートメントで Workfront の既存のフィールドを接続します。

計算済みデータ式は、次の場所で使用できます。

* カスタムフォームの計算済みカスタムフィールド

  Workfrontのカスタムフォーム上に計算カスタムフィールドを作成する方法について詳しくは、[ 計算フィールドをフォームに追加 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) を参照してください。

* テキストモードを使用する場合の、レポートまたはリスト内の計算済みカスタム列

  レポートおよびビューでのテキストモードの使用について詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)を参照してください。

## 計算済みカスタムフィールドと計算済みカスタム列の構文の比較

使用する関数は同じですが、計算済みカスタムフィールドで式を作成する場合の構文は、計算済みカスタム列を作成する場合の構文とは異なる場合があります。

2 つの構文の違いは次のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>計算済みカスタムフィールド</strong></td> 
   <td><strong>計算済みカスタムレポート要素</strong></td> 
  </tr> 
   <td>フィールド名を波括弧で囲む</td> 
   <td>フィールド名を <p><code>valuefield </code></p>行で使用する場合、角括弧または丸括弧内で囲まないでください。 <p>フィールド名を <p><code>valueexpression</code></p> 行で使用する場合、角括弧または丸括弧内で囲まないでください。</p> </td> 
  </tr> 
  <tr> 
   <td>フィールドはピリオドで区切ります。</td> 
   <td> <p>フィールドを <p><code>valuefield </code></p>行で使用する場合、コロンで区切ります。</p> <p>フィールドを <p><code>valueexpression </code></p>行で使用する場合、角括弧または丸括弧内で囲まないでください。 </p> </td> 
  </tr> 
 </tbody> 
</table>

例：

* タスクのカスタムフォームのカスタムフィールドでは、以下を使用して、カスタムフォームが添付されているタスクの親プロジェクトの名前を生成します。


  ` {project}.{name}`


* レポートのカスタム列では、以下を使用して、タスクレポートにプロジェクト名のカスタム列を追加します。


  `valuefield=project:name`


  または

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >同じ構文が、計算済みの式が使用されるすべてのテキストモードレポート要素（ビュー、フィルター、グループ化、プロンプト）に適用されます。

計算済みカスタム列で使用する必要がある構文について詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)を参照してください。

## 使用できるデータ式

以下のリストは、Workfront で 3 種類の計算済みカスタムフィールドのいずれかを作成する際に使用できる式を定義します。

* [日付と時刻の計算済みカスタムフィールド](#date-time-calculated-custom-fields)
* [数学的な計算済みカスタムフィールド](#mathematical-calculated-custom-fields)
* [テキスト計算済みカスタムフィールド](#text-calculated-custom-fields)

以下に示す式を使用すると、計算済みカスタム列を作成できます。ただし、計算済みカスタム列の正しい構文を使用する必要があります。詳しくは、この記事の[計算済みカスタムフィールドと計算済みカスタム列の構文](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns)の節を参照してください。

### 日付と時刻の計算済みカスタムフィールド {#date-time-calculated-custom-fields}

>[!NOTE]
>
>時間部分を含まない日付と時間の計算を作成した場合または $$TODAY や $$NOW の日付ワイルドカードを使用する場合、ローカルタイムゾーンではなく協定世界時（UTC）ゾーンに従って日付が使用されます。これは予期しない日付の結果を引き起こす可能性があります。

次の式を使用すると、日付または時刻の計算済みカスタムフィールドを作成できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>式</th> 
   <th>説明と例</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ADDDAYS</strong> </td> 
   <td> <p>日付に日数を追加します。数値には、日の一部を含めることができます。例えば、1.5 の場合、日付に 1 日半が追加されます。</p> <p>式の形式は次のとおりです。</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>平日の追加</strong> </td> 
   <td> <p>日付に平日の数を追加します。この式は、整数値を切り捨てて日付に加算します。 </p> <p>式の形式は次のとおりです。</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>日付に月数を追加し、次の形式に設定されます。

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>日付に年数を追加し、次の形式に設定されます。</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDHOURS</strong> </td> 
   <td> <p>日付に時間数を追加します。次のような形式です。</p>

<p><code>ADDHOUR(date, number)</code></p>
   <p>メモ：この式は、Workfront Planning ではサポートされていません。</p></td> 
  </tr>
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>日付の時間部分をクリアし、次の形式で表します。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>文字列を日付に変換し、次の形式で表します。</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>選択した期間の開始日と終了日に加え、その日のタイムスタンプを考慮して、2 つの日付の間の日数を返します。例えば、開始日の開始時刻が午後 3 時の場合、開始日は 1 日としてカウントされません。</p> <p>式の形式は次のとおりです。</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>その日付が何日であるかを 1 から 31 の数値で返します。</p> <p>式の形式は次のとおりです。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>その日付の曜日を 1（日曜日）から 7（土曜日）の数値で返します。</p> <p>式の形式は次のとおりです。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>指定日の月の合計日数を数値で返し、次の形式で表します。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>指定日から週末、あるいは月末までの合計週日数で少ない方を返します。この例では、日付は作業オブジェクトのエントリ日です。</p> <p>式の形式は次のとおりです。</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>その日付の年の合計日数を数値で返し、次の形式で表します。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>リストの最新の日付を返し、次の形式で表します。</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>リストの一番古い日付を返し、次の形式で表します。</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>その日付の時間を 0 から 23 の数値で返します。</p> <p>式の形式は次のとおりです。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>その日付の分を 0 から 60 の数値で返し、次の形式で表します。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>その日付の月を 1 から 12 の数値で、次の形式で返します。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>日付の秒を次の形式の 0 ～ 60 の数値で返します。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>選択した期間の開始日と終了日、およびそれらの日の時刻を考慮して、2 つの日付の間の平日数を返します。例えば、開始日の開始時刻が午後 3 時の場合、開始日は 1 日としてカウントされません。</p> <p>式の形式は次のとおりです。</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>既定のスケジュールに基づき、日付間のスケジュール分数を返します。</p> <p>式の形式は次のとおりです。</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>YEAR</strong> </td> 
   <td> <p>日付の年を次の形式の 4 桁の数値で返します。この例では、日付は作業オブジェクトのエントリ日です。</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### 数学計算カスタムフィールド {#mathematical-calculated-custom-fields}

次の数式を使用した計算済みカスタムフィールドを作成できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>式</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong>ABS</strong> </td> 
   <td>数値の絶対値を次の形式で返します。この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>数の平均を次の次の形式で返します。

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>数値を最も近い整数に丸め、次の形式で表します。この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>すべての数値を指定された順序で除算し、次の形式で表します。

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>数値を最も近い整数に切り捨て、次の形式で表します。この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>数値の自然対数値を次の形式で返します。

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>数値 1 を底として数値 2 の対数値を次の形式で返します。

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>最大</strong> </td> 
   <td>リスト内の最大の項目を次の形式で返します。

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>最小</strong> </td> 
   <td>リスト内の最小の項目を次の形式で返します。

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>文字列を次の形式の数値に変換します。<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>数値をべき乗した値を次の形式で返します。

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>すべての数値を乗算し、次の形式にします。

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>メモ</b></p>

<p>時間を含んだフィールドを乗算する場合は、選択したフィールドの時間をデータベースが分、時間、秒のいずれで保存するかを必ず把握してください。時間が分または秒単位で保存され、Workfront インターフェイスに時間単位で表示される場合、この計算を使用して式を書き込む際に、分または秒から時間への変換を考慮する必要が生じる場合があります。 </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>数値の端数を指定の精度に切り上げ、次の形式にします。

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 数値を昇順で並べ替え、次の形式にします。</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>数値を降順で並べ替えます。形式は次のとおりです。

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>数値の平方根を返します。形式は次のとおりです。この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>指定された順序ですべての数値を減算します。形式は次のとおりです。

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>合計</strong> </td> 
   <td>すべての数値を加算します。形式は次のとおりです。

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### テキスト計算済みカスタムフィールド {#text-calculated-custom-fields}

次の式を使用して、テキスト形式の値を表示する、計算されたカスタムフィールドを作成できます。

<table style="table-layout:auto:fixed"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>式</th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><strong> 配列 </strong> </td> 
   <td> <p>文字列を配列に変換します。区切り文字には任意の文字列を使用できます。</p> 
   <p>式の形式は次のとおりです。</p>
   <p><code>ARRAY(string1, "delimiter")</code></p> 
   </td> 
  </tr>

<tr> 
   <td><strong>ARRAYCONTAINS</strong> </td> 
   <td> <p>リストまたは配列内の特定の値を検索します。 値が見つかった場合、この関数は True を返し、それ以外の場合は False を返します。 </p> 
   <p>式の形式は次のとおりです。</p>
   <p><code>ARRAYCONTAINS(array, value)</code></p> 
   </td> 
  </tr>


<tr> 
   <td><strong>ARRAYLENGTH</strong> </td> 
   <td> <p>配列内の要素の数を返します。次のような形式になります。</p>
   <p><code>ARRAYLENGTH(array)</code></p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>ARRAYELEMENT</strong> </td> 
   <td> <p>配列内の指定された数値の要素を返します。インデックスが範囲外の場合、空が返されます。</p> 
   <p>式の形式は次のとおりです。</p>
   <p><code>ARRAYELEMENT(array, number)</code></p> 
   </td> 
  </tr>

<tr>   
   <td><strong>CASE</strong> </td> 
   <td> <p>他の式と共に使用され、インデックス番号に基づいてリストから値を選択します。 </p>
   <p>インデックス番号は、数値（通常は既知の範囲）を返すフィールドまたは関数です。</p> 
   <p>式の形式は次のとおりです。</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>例えば、次の式は、集計列に曜日の名前を返します。ここで、1=日曜日、2=月曜日などです。</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>DAYOFWEEK、DAYOFMONTH、MONTH など、数値を返す他の式に最適です。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>文字列を連結します。形式は次のとおりです。</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>使用できる区切り記号の例を示します。</p> 
    <ul> 
     <li>スペース：「 」</li> 
     <li>ダッシュ：「-」</li> 
     <li>スラッシュ：「/」</li> 
     <li>コンマ：「,」</li> 
     <li>単語：「or」、「and」</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>CONTAINS</strong> </td> 
   <td>withinText 文字列内で findText 文字列が見つかったときに true を返します。形式は次のとおりです。

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>URL 引数に含められるよう、文字列の特殊文字をエスケープします。<p>式の形式は次のとおりです。</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong> 形式 </strong> </td> 
   <td><p>書式設定されたテキストを返します。 FORMAT では、ここに示すパラメータ オプションのみを使用できます。</p>
   <p>カラーオプションは$$POSITIVE、$$INFORMATIVE、$$NEGATIVE、$$NOTICE で、その他の書式設定オプションは$$BOLD、$$ITALIC、$$UNDERLINE です。 1 つのカラーオプションと、最大 3 つの他の書式設定オプションのみが許可されます。 カラーオプションを指定しない場合、システムのデフォルトのカラーが適用されます。</p>
   <p>式の形式は次のとおりです。</p>
   <p><code>FORMAT($$POSITIVE, $$BOLD, $$ITALIC)</code></p>
   <p>メモ：この式は、Workfront Planning ではサポートされていません。</p></td> 
  </tr>   
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>指定した条件を評価し、true の場合は trueExpression の値を返します。false の場合は falseExpression の値を返します。</p>

<p>式の形式は次のとおりです。</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>例えば、2 つの異なる日付フィールドを比較し、True/False の結果をデータ文字列として出力することができます。</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>分かりやすく言えば、こステートメントは、「オブジェクトの見込み完了日が、予定完了日より大きい場合、このフィールドに「遅延」と表示し、それ以外の場合は「順調」と表示します。</p>

<p>true または false の式にラベルを付けたくない場合は、ステートメントに次のような空白のラベルを挿入する必要があります。</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>または</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>「IF」ステートメントの作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">「IF」ステートメントの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>使用可能な値の文字列内から特定の値を検索できます。検索する値が指定された値のいずれかと等しい場合、式は trueExpression を返し、それ以外の場合は falseExpression を返します。</p> 
   <p>式の形式は次のとおりです。</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>例えば、特定のプロジェクト所有者を検索し、プロジェクトビューで指定したタグを使用して、該当するプロジェクトにマークを付けることができます。 <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> 分かりやすく言えば、この文は「プロジェクト所有者が Jennifer Campbell または Rick Kuvec の場合、このプロジェクトを「マーケティングチーム」でマークし、それ以外の場合は「他のチーム」でマークします」という意味です。</p> 
    <p> true または false の式にラベルを付けたくない場合は、ステートメントに次のような空白のラベルを挿入する必要があります。 </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>または </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>指定された値のいずれかと値が等しい場合は true を返し、それ以外の場合、式は false を返します。</p> <p>式の形式は次のとおりです。

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>値が null または空の場合は true を返し、それ以外の場合、式は false を返します。</p> <p>式の形式は次のとおりです。

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>指定された数の文字を文字列の左側から返します。形式は次のとおりです。</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>文字列の長さを返します。形式は次のとおりです。</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>小文字の文字列を返します。形式は次のとおりです。

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong> パスカル </strong> </td> 
   <td> <p>入力文字列を PascalCase に変換します。変換するには、各単語の最初の文字を大文字にし、すべてのスペースを削除します。 </p>
   <p>式の形式は次のとおりです。</p>
   <p><code>PASCAL(string) </code></p>
   <p>例えば、「hello world」は「HelloWorld」になります</p> 
   </td> 
  </tr>
  <tr> 
   <td><strong>REMOVEACCENTS</strong> </td> 
   <td> <p>入力文字列内のすべてのアクセント付き文字から発音区別符号を削除します。 </p> 
   <p>式の形式は次のとおりです。</p>
   <p><code>REMOVEACCENTS(string)</code></p> 
   <p>例えば、「Héllo wörld with âccénts」は「Hello world with accentes」になります。 </p>
   </td> 
  </tr>
  <tr> 
   <td><strong>REPLACE</strong> </td> 
   <td> <p>string1 にある string2 のすべてのオカレンスを string3 に置き換えます。</p> <p>式の形式は次のとおりです。</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr>

<tr> 
   <td><strong>REPLACEPATTERN</strong> </td> 
   <td> <p>指定されたパターンの一致を置換文字列で置き換えます。 </p> 
   <p>式の形式は次のとおりです。</p>
   <p><code>REPLACEPATTERN (string, pattern, replacement string)</code></p> 
   <p>例えば、REPLACEPATTERN （"foo123bar", "\d+", "_"）は、文字列「foo_bar」を生成します。
   </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>指定された数の文字を文字列の右側から返します。式の形式は次のとおりです。</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>文字列 withinText 内で指定の開始位置から findText の最初のオカレンスのインデックスを返します。このテキストが見つからない場合は、-1 を返します。</p> <p>式の形式は次のとおりです。</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong> ソルタスカレイ </strong> </td> 
   <td> <p>配列要素を昇順に並べ、最初の要素の型に変換します。</p>
   <p>式の形式は次のとおりです。</p>
   <p><code>SORTASCARRAY(array)</code></p>
   <p>例えば、["-12.6", -13.0] は ["-12.6", "-13"] になります。</p>
   <p>メモ：この式は、Workfront Planning ではサポートされていません。</p></td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCCARRAY</strong> </td> 
   <td> <p>配列要素を降順で並べ替え、最初の要素のタイプに変換します。</p>
   <p>式の形式は次のとおりです。</p>
   <p><code>SORTDESCARRAY(array)</code></p>
   <p>例えば、["-12.6", -13.0] は ["-13", "-12.6"] になります。</p>
   <p>メモ：この式は、Workfront Planning ではサポートされていません。</p></td> 
  </tr>
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>この式は、数値を文字列に変換します。形式は次のとおりです。</p>

<p><code>STRING(number)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>文字列のリストを昇順に並べ替えます。形式は次のとおりです。</p>
   <p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr>
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 文字列のリストを降順に並べ替えます。形式は次のとおりです。</p>
   <p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>指定された開始インデックスと終了インデックスに基づいて文字列を返します。形式は次のとおりです。</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong> 切り替え </strong> </td> 
   <td> <p>値のリストに対して式を評価し、最初に一致した値に対応する結果を返します。</p>
   <p>式の形式は次のとおりです。</p>
   <p><code>SWITCH(expression, value1, result1, [value2, result2], ...)</code></p>
   <p>この式は、Workfront Planning ではサポートされていません。</p></td> 
  </tr>   
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>文字列の先頭と終わりから空白を削除します。形式は次のとおりです。</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>大文字の文字列を返します。形式は次のとおりです。</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>

