---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算データ式の概要
description: データ式を使用して、Adobe Workfrontで計算済みのカスタムデータフィールドを定義できます。 計算式は、新しいフィールドを生成するステートメント内で、既存のWorkfrontフィールドを結び付けます。
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 3e1e651662f9ff695d475ffcbdc77f0802d108f1
workflow-type: tm+mt
source-wordcount: '2166'
ht-degree: 0%

---

# 計算データ式の概要

データ式を使用して、Adobe Workfrontで計算カスタムフィールドを定義できます。 計算式は、新しいフィールドを生成するステートメント内で、既存のWorkfrontフィールドを結び付けます。

計算データ式は、次の場所で使用できます。

* カスタムフォームの計算済みカスタムフィールド

  Workfrontのカスタムフォームで計算カスタムフィールドを作成する方法について詳しくは、 [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* テキストモードを使用する場合の、レポートまたはリスト内の計算済みカスタム列

  レポートおよびビューでのテキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 計算カスタムフィールドと計算カスタム列の構文

使用する関数は同じですが、計算カスタムフィールドで式を作成するときの構文は、計算カスタム列を作成するときの構文とは異なる場合があります。

2 つの構文の違いは次のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>計算済みカスタムフィールド</strong></td> 
   <td><strong>計算済みカスタムレポート要素</strong></td> 
  </tr> 
   <td>フィールド名を中括弧で囲みます。</td> 
   <td>フィールド名を <p><code>valuefield </code></p>行。 <p>フィールド名を <p><code>valueexpression</code></p> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>フィールドをピリオドで区切ります</td> 
   <td> <p>フィールドを <p><code>valuefield </code></p>行</p> <p>フィールドをピリオドで区切ります ( <p><code>valueexpression </code></p>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

例：

* カスタムフィールドのタスクのカスタムフォームでは、次の情報を使用して、カスタムフォームが添付されているタスクの親プロジェクトの名前を生成します。


  ` {project}.{name}`


* レポートのカスタム列では、次の手順を使用して、タスクレポートにプロジェクト名のカスタム列を追加します。


  `valuefield=project:name`


  または

  `valueexpression={project}.{name}`


  >[!TIP]
  >
  >同じ構文は、計算式が使用されるすべてのテキストモードレポート要素（ビュー、フィルタ、グループ化、プロンプト）に適用されます。

計算カスタム列で使用する必要がある構文について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 使用できるデータ式

以下のリストは、Workfrontで 3 種類の計算カスタムフィールドのいずれかを作成する際に使用できる式を定義します。

* [日付と時刻の計算されたカスタムフィールド](#date-time-calculated-custom-fields)
* [数学計算カスタムフィールド](#mathematical-calculated-custom-fields)
* [テキスト計算カスタムフィールド](#text-calculated-custom-fields)

以下に示す式を使用して、計算済みカスタム列を作成できます。 ただし、計算カスタム列の正しい構文を使用する必要があります。詳しくは、「 」の節を参照してください。  [計算カスタムフィールドと計算カスタム列の構文](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns) 」を参照してください。

### 日付と時刻の計算されたカスタムフィールド {#date-time-calculated-custom-fields}

>[!NOTE]
>
>時間部分を含まない日付と時間の計算を作成した場合、または$$TODAY や$$NOW の日付ワイルドカードを使用する場合、ローカルタイムゾーンではなく協定世界時 (UTC) ゾーンに従って日付が使用されます。 これは予期しない日付の結果を引き起こす可能性があります。

次の式を使用して、日付または時間計算のカスタムフィールドを作成できます。

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
   <td> <p>日付に日数を追加します。 数値には、日の一部を含めることができます。 例えば、1.5 の場合、日付に 1 日半が追加されます。</p> <p>式の形式は次のとおりです。</p>

<p><code>ADDDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDWEEKDAYS</strong> </td> 
   <td> <p>日付に平日数を追加します。 この式は、整数値を切り捨てて日付に加算します。 </p> <p>式の形式は次のとおりです。</p>

<p><code>ADDWEEKDAYS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>日付に月数を追加します。形式は次のとおりです。

</p><p><code>ADDMONTHS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>日付に年数を追加します。形式は次のとおりです。</p>

<p><code>ADDYEARS(date, number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>日付の時間部分をクリアし、次の形式に設定します。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>CLEARTIME({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>日付</strong> </td> 
   <td> <p>文字列を日付に変換し、次の形式にします。</p>

<p><code>DATE(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>2 つの日付の間の日数を返します。選択した期間の開始日と終了日、およびその日のタイムスタンプが考慮されます。 例えば、開始日の開始時刻が午後 3 時の場合、開始日は 1 日としてカウントされません。</p> <p>式の形式は次のとおりです。</p>

<p><code>DATEDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>日付の月の日を 1 ～ 31 の数値で返します。</p> <p>式の形式は次のとおりです。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>DAYOFMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>日付の曜日を 1（日曜日）から 7（土曜日）の間の数値で返します。</p> <p>式の形式は次のとおりです。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>DAYOFWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>日付の月の合計日数を数値で返し、次の形式で指定します。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>DAYSINMONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>日付から週の終わりまでの合計平日、または月の終わりのどちらか早い方を返します。 この例では、日付は作業オブジェクトの入力日です。</p> <p>式の形式は次のとおりです。</p>

<p><code>DAYSINSPLITWEEK({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>日付の年の合計日数を数値で返し、次の形式で指定します。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>DAYSINYEAR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>リストの最新の日付を返します。次の形式で指定します。</p>

<p><code>DMAX(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>リスト内の最も早い日付を返し、次の形式で表されます。</p>

<p><code>DMIN(date1, date2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>時間</strong> </td> 
   <td> <p>日付の時間を 0 ～ 23 の数値で返します。</p> <p>式の形式は次のとおりです。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>HOUR({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>分</strong> </td> 
   <td> <p>日付の分を、0 ～ 60 の数値（次の形式）で返します。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>MINUTE({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>月</strong> </td> 
   <td> <p>日付の月を 1 ～ 12 の数値で、次の形式で返します。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>MONTH({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>2 番目</strong> </td> 
   <td> <p>日付の 2 番目の値を、0 ～ 60 の数値で、次の形式で返します。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>SECOND({entryDate})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>2 つの日付の間の平日数を返します。選択した期間の開始日と終了日、およびその日のタイムスタンプが考慮されます。 例えば、開始日の開始時刻が午後 3 時の場合、開始日は 1 日としてカウントされません。</p> <p>式の形式は次のとおりです。</p>

<p><code>WEEKDAYDIFF(date2, date1)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>デフォルトのスケジュールに従って、日付間の予定分数を返します。</p> <p>式の形式は次のとおりです。</p>

<p><code>WORKMINUTESDIFF(date1, date2)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>年</strong> </td> 
   <td> <p>日付の年を 4 桁の数値で返します（次の形式）。 この例では、日付は作業オブジェクトの入力日です。</p>

<p><code>YEAR({entryDate})</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### 数学計算カスタムフィールド {#mathematical-calculated-custom-fields}

次の数式を使用した計算カスタムフィールドを作成できます。

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
   <td>数値の絶対値を返し、次の形式で表されます。 この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。

<p><code>ABS({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>平均</strong> </td> 
   <td>数の平均を返します。形式は次のとおりです。

<p><code>AVERAGE(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>数値を最も近い整数に丸めます。この数値は、次の形式で表されます。 この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。

<p><code>CEIL({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>すべての数値を指定された順序で除算します。形式は次のとおりです。

<p><code>DIV(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>数値を最も近い整数に丸めます。この数値は、次の形式で表されます。 この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。

<p><code>FLOOR({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>数の自然対数値を返します。次の形式で指定します。

<p><code>LN({numberOfChildren})</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ログ</strong> </td> 
   <td>底数 1 に対する数値 2 の対数値を返します。次のような形式になります。

<p><code>LOG(number1, number2)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>MAX</strong> </td> 
   <td>リスト内の最大の項目を返し、次のように書式設定されます。

<p><code>MAX(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>最小</strong> </td> 
   <td>リスト内の最小の項目を返します。次のような形式になります。

<p><code>MIN(item1, item2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>数値</strong> </td> 
   <td>文字列を数値に変換し、次の形式に設定します。<p><code>NUMBER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>指数を返します。次の形式で指定します。

<p><code>POWER(number, power)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>すべての数値を乗算し、次の形式で表します。

<p><code>PROD(number1, number2, ....)</code></p>
   <p><b>メモ</b></p>

<p>時間を含むフィールドに乗算する場合は、選択したフィールドの時間を分単位、時間単位、秒単位で保存するかどうかを確認してください。 時間が分または秒単位で保存され、Workfrontインターフェイスに時間単位で表示される場合、この計算を使用して式を書き込む際に、分または秒から時間への変換を考慮する必要が生じる場合があります。 </p>
   </td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>数値を指定された精度の小数点以下に丸めます。次のように書式設定されます。

<p><code>ROUND(number, precision)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> 数値を昇順で並べ替え、次のように書式設定します。</p>

<p><code>SORTASCNUM(number1,number2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>数値を降順で並べ替えます。形式は次のとおりです。

<p><code>SORTDESCNUM(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>数の平方根を返します。この平方根は、次の形式で表されます。 この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。</p>

<p><code>SQRT({numberOfChildren})</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>指定された順序ですべての数値を引きます。形式は次のとおりです。

<p><code>SUB(number1, number2, ...)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>SUM</strong> </td> 
   <td>すべての数値を追加します。形式は次のとおりです。

<p><code>SUM(number1, number2, ...)</code></p></td> 
  </tr> 
 </tbody> 
</table>

### テキスト計算カスタムフィールド {#text-calculated-custom-fields}

次の式を使用してテキスト形式の値を表示する計算済みカスタムフィールドを作成できます。

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
   <td><strong>CASE</strong> </td> 
   <td> <p>他の式と共に使用し、インデックス番号に基づいてリストから値を選択します。 </p>
   <p>インデックス番号は、数値（通常は既知の範囲）を返すフィールドまたは関数です。</p> 
   <p>式の形式は次のとおりです。</p>
   <p><code>CASE(indexNumber, value1, value2, ...)</code></p>

<p>例えば、次の式は、集計列で曜日の名前を返します。ここで、1=日曜日、2=月曜日などです。</p>

<p><code>CASE(DAYOFWEEK({entryDate}),"Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday")</code></p>

<p>DAYOFWEEK、DAYOFMONTH、MONTH など、数値を返す式を使用する場合に最も適しています。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>文字列を連結し、次の形式で記述します。</p><p><code>CONCAT(string1,"separator", string2)</code></p> <p>次に、含めることができる区切り文字の例を示します。</p> 
    <ul> 
     <li>スペース： " "</li> 
     <li>a ダッシュ："-"</li> 
     <li>スラッシュ：「/」</li> 
     <li>コンマ：","</li> 
     <li>単語：「or」、「and」</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>次を含む</strong> </td> 
   <td>findText 文字列が withinText 文字列内で見つかり、次の形式である場合、true を返します。

<p><code>CONTAINS(findText, withinText)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>URL 引数に含めることができるように、文字列内の特殊文字をエスケープします。<p>式の形式は次のとおりです。</p>

<p><code>ENCODEURL(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>指定した条件を評価し、true の場合は trueExpression の値を返します。false の場合は falseExpression の値を返します。</p>

<p>式の形式は次のとおりです。</p>

<p><code>IF(condition, trueExpression, falseExpression)</code></p>

<p>例えば、2 つの異なる日付フィールドの後に True/False の結果が続くデータ文字列を比較できます。</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","On Track")</code></p>

<p>毎日の音声で、この文は、「オブジェクトの予想完了日が、同じオブジェクトの計画完了日より大きい場合、このフィールドに「未追跡」と表示し、それ以外の場合は「追跡中」と表示します。</p>

<p>true または false の式にラベルを付けたくない場合は、ステートメントに次のような空白のラベルを挿入する必要があります。</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"","On Track")</code></p> 
   <p>または</p>

<p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</code></p>

<p>「IF」文の作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">「IF」文の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>指定可能な値の文字列内の特定の値を検索できます。 検索する値が指定された値のいずれかと等しい場合、式は trueExpression を返し、それ以外の場合は falseExpression を返します。</p> 
   <p>式の形式は次のとおりです。</p>

<p><code>IFIN(value, value1, value2,..., trueExpression, falseExpression)</code></p>

<p>例えば、特定のプロジェクト所有者を検索し、プロジェクトビューで指定したタグを使用して、これらのプロジェクトにマークを付けることができます。 <br><p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")
   </code></p>
    <p> 毎日のスピーチで、この文は「プロジェクト所有者が Jennifer Campbell または Rick Kuvec の場合、このプロジェクトを「マーケティングチーム」でマークし、それ以外の場合は「他のチーム」でマークします。」という意味です。</p> 
    <p> true または false の式にラベルを付けたくない場合は、ステートメントに次のような空白のラベルを挿入する必要があります。 </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> 
    <p>または </p> 
    <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","")</code></p> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>値が指定された値のいずれかと等しい場合は true を返し、それ以外の場合は false を返します。</p> <p>式の形式は次のとおりです。

</p><p><code>IN(value, value1[, value2...])</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>値が null または空の場合は true を返し、それ以外の場合は false を返します。</p> <p>式の形式は次のとおりです。

</p><p><code>ISBLANK(value)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>左</strong> </td> 
   <td> <p>文字列の左側から指定された数の文字を返します。次のように書式設定されます。</p>

<p><code>LEFT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>文字列の長さを返し、次の形式で表します。</p>

<p><code>LEN(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>小文字で文字列を返し、次のように書式設定されます。

<p><code>LOWER(string)</code></p></td> 
  </tr> 
  <tr> 
   <td><strong>置換</strong> </td> 
   <td> <p>string1 内での文字列 2 のすべての箇所を string3 に置き換えます。</p> <p>式の形式は次のとおりです。</p>

<p><code>REPLACE(string1, string2, string3)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>右</strong> </td> 
   <td> <p>文字列の右側から指定された数の文字を返します。次のように書式設定されます。</p>

<p><code>RIGHT(string, length)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>検索</strong> </td> 
   <td> <p>Text 内の文字列で、指定された開始位置から始まる findText の最初の値のインデックスを返します。テキストが見つからない場合は、-1 を返します。</p> <p>式の形式は次のとおりです。</p>

<p><code>SEARCH(findText, withinText, start)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>文字列</strong> </td> 
   <td> <p>数値を文字列に変換し、次の形式にします。</p>

<p><code>STRING(number)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>文字列のリストを昇順に並べ替えます。次のように書式設定されます。</p>

<p><code>SORTASCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> 文字列のリストを降順に並べ替えます。次のように書式設定されます。</p>

<p><code>SORTDESCSTRING(string1, string2, ...)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>指定された開始および終了のインデックスに基づいて、文字列の文字を返します。次のような形式で指定します。</p>

<p><code>SUBSTR({string}, number of start position, number of end position)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>トリミング</strong> </td> 
   <td> <p>文字列の先頭と末尾から空白を削除し、次のように書式設定します。</p>

<p><code>TRIM(string)</code></p> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>大文字の文字列を返し、次のように書式設定されます。</p>

<p><code>UPPER(string)</code></p> </td> 
  </tr> 
 </tbody> 
</table>
