---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算データ式
description: データ式を使用して、Adobe Workfrontで計算済みのカスタムデータフィールドを定義できます。 新しいフィールドを生成するステートメントで、既存のWorkfrontフィールドを接続します。
author: Nolan
feature: Reports and Dashboards
exl-id: cfb3ace9-76c3-4006-878f-e2ad25ffa03b
source-git-commit: 18f26f976a47af003817f2f82f8550bdfbc0ab90
workflow-type: tm+mt
source-wordcount: '2368'
ht-degree: 7%

---

# 計算データ式

データ式を使用して、Adobe Workfrontで計算済みのカスタムデータフィールドを定義できます。 新しいフィールドを生成するステートメントで、既存のWorkfrontフィールドを接続します。

計算データ式は、次の場所で使用できます。

* カスタムフォーム

   Workfrontのカスタムフォームで計算済みカスタムデータフィールドを作成する方法について詳しくは、 [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* テキストモードを使用する場合の、レポートまたはリストの計算済みカスタム列

   レポートおよびビューでのテキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 計算カスタムフィールドと計算カスタム列の構文

使用する関数は同じですが、計算カスタムフィールドで式を作成する場合の構文は、計算カスタム列を作成する場合の構文とは異なる場合があります。

例：

* カスタムフィールドのタスクのカスタムフォームでは、次の情報を使用して、カスタムフォームが添付されているタスクの親プロジェクトの名前を生成します。

   ```
   {project}.{name}
   ```

* レポートのカスタム列では、次の手順を使用して、タスクレポートにプロジェクト名のカスタム列を追加します。

   ```
   valuefield=project:name
   ```

   または

   ```
   valueexpression={project}.{name}
   ```

   >[!TIP]
   >
   >同じ構文が、計算式が使用されるすべてのテキストモードレポート要素に適用されます。ビュー、フィルタ、グループ化、プロンプト。

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
   <td>フィールド名を <code>valuefield </code>行 <p>フィールド名を <code>valueexpression</code> 行</p> </td> 
  </tr> 
  <tr> 
   <td>フィールドはピリオドで区切ります。</td> 
   <td> <p>フィールドを <code>valuefield </code>行</p> <p>フィールドを <code>valueexpression </code>行 </p> </td> 
  </tr> 
 </tbody> 
</table>

計算カスタム列で使用する必要がある構文について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 使用できるデータ式

以下のリストは、Workfrontで 3 種類の計算カスタムフィールドのいずれかを作成する際に使用できる式を定義します。

* [日付と時刻の計算されたカスタムフィールド](#date-time-calculated-custom-fields)
* [数学計算カスタムフィールド](#mathematical-calculated-custom-fields)
* [テキスト計算カスタムフィールド](#text-calculated-custom-fields)

### 日付と時刻の計算されたカスタムフィールド {#date-time-calculated-custom-fields}

>[!NOTE]
>
>時間部分を含まない日付と時間の計算を作成した場合、または$$TODAY や$$NOW の日付ワイルドカードを使用する場合、ローカルタイムゾーンではなく協定世界時 (UTC) ゾーンに従って日付が使用されます。 これは予期しない日付の結果を引き起こす可能性があります。

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
   <td> <p>この式は、日付に日数を追加します。 数値には日の一部を含めることができます（例： 1.5 は日付に 1 日半を追加します）。</p> <p>式の形式は次のとおりです。</p><pre>ADDDAYS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>平日の追加</strong> </td> 
   <td> <p>この式は、日付に平日数を追加します。 この式は、整数値を切り捨てて日付に加算します。 </p> <p>式の形式は次のとおりです。</p><pre>平日の追加 (日、数値)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDMONTHS</strong> </td> 
   <td> <p>この式は、日付に月数を追加し、次の形式で記述します。</p><pre>ADDMONTHS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ADDYEARS</strong> </td> 
   <td> <p>この式は、日付に年数を追加し、次の形式で記述します。</p><pre>ADDYEARS(date, number)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>CLEARTIME</strong> </td> 
   <td> <p>この式は、日付の時間部分をクリアし、次の形式に設定されます。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>CLEARTIME({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATE</strong> </td> 
   <td> <p>この式は、文字列を日付に変換し、次の形式で表されます。</p><pre>DATE(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DATEDIFF</strong> </td> 
   <td> <p>この式は、選択した期間の開始日と終了日、およびその日のタイムスタンプを考慮して、2 つの日付の間の日数を返します。 例えば、開始日の開始時刻が午後 3 時の場合、開始日は 1 日としてカウントされません。</p> <p>式の形式は次のとおりです。</p><pre>DATEDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFMONTH</strong> </td> 
   <td> <p>この式は、日付の月の日を 1 ～ 31 の数値で返します。</p> <p>式の形式は次のとおりです。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>DAYOFMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYOFWEEK</strong> </td> 
   <td> <p>この式は、1（日曜日）から 7（土曜日）の間の日付を数値で返します。</p> <p>式の形式は次のとおりです。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>DAYOFWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINMONTH</strong> </td> 
   <td> <p>この式は、月の合計日数を数値で返し、次の形式になります。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>DAYSINMONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINSPLITWEEK</strong> </td> 
   <td> <p>この式は、日付から週の終わりまでの合計平日、または月の終わりのいずれか最初の日を返します。 この例では、日付は作業オブジェクトのエントリ日です。</p> <p>式の形式は次のとおりです。</p><pre>DAYSINSPLITWEEK({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DAYSINYEAR</strong> </td> 
   <td> <p>この式は、日付の年の合計日数を数値で返し、次の形式で指定します。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>DAYSINYEAR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMAX</strong> </td> 
   <td> <p>この式は、リストの最新の日付を返し、次の形式で設定されます。</p><pre>DMAX(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>DMIN</strong> </td> 
   <td> <p>この式は、リストの最も古い日付を返し、次の形式で表されます。</p><pre>DMIN(date1, date2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>HOUR</strong> </td> 
   <td> <p>この式は、日付の時間を 0 ～ 23 の数値で返します。</p> <p>式の形式は次のとおりです。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>HOUR({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MINUTE</strong> </td> 
   <td> <p>この式は、日付の分を 0 ～ 60 の数値で返し、次の形式で記述します。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>MINUTE({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>MONTH</strong> </td> 
   <td> <p>この式は、月を 1 ～ 12 の数値で返し、次の形式で記述します。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>MONTH({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SECOND</strong> </td> 
   <td> <p>この式は、2 番目の日付を 0 ～ 60 の数値で返し、次の形式で記述します。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>SECOND({entryDate})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WEEKDAYDIFF</strong> </td> 
   <td> <p>この式は、選択した期間の開始日と終了日、およびその日のタイムスタンプを考慮して、2 つの日付の間の平日数を返します。 例えば、開始日の開始時刻が午後 3 時の場合、開始日は 1 日としてカウントされません。</p> <p>式の形式は次のとおりです。</p><pre>WEEKDAYDIFF(date2, date1)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>WORKMINUTESDIFF</strong> </td> 
   <td> <p>この式は、デフォルトのスケジュールに従って、日付間の予定分数を返します。</p> <p>式の形式は次のとおりです。</p><pre>WORKMINUTESDIFF(date1, date2)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>YEAR</strong> </td> 
   <td> <p>この式は、日付の年を次の形式の 4 桁の数値で返します。 この例では、日付は作業オブジェクトのエントリ日です。</p><pre>YEAR({entryDate})</pre> </td> 
  </tr> 
 </tbody> 
</table>

### 数学計算カスタムフィールド {#mathematical-calculated-custom-fields}

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
   <td>この式は、数値の絶対値を返し、次の形式で指定します。 この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。<pre>ABS({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>AVERAGE</strong> </td> 
   <td>この式は、数の平均を返し、次の形式で設定されます。<pre>AVERAGE(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>CEIL</strong> </td> 
   <td>この式は、数値を最も近い整数に丸め、次の形式にします。 この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。<pre>CEIL({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>DIV</strong> </td> 
   <td>この式では、すべての数値を指定された順序で除算し、次のように書式設定します。<pre>DIV(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>FLOOR</strong> </td> 
   <td>この式は、数値を最も近い整数に切り捨て、次の形式にします。 この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。<pre>FLOOR({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LN</strong> </td> 
   <td>この式は、数の自然対数値を返し、次の形式で指定します。<pre>LN({numberOfChildren})</pre></td> 
  </tr> 
  <tr> 
   <td><strong>LOG</strong> </td> 
   <td>この式は、数値 1 の底となる数値 2 の対数値を返し、次の形式で指定します。<pre>LOG(number1, number2)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>最大</strong> </td> 
   <td>この式は、リスト内の最大の項目を返し、次のように書式設定されます。<pre>MAX(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>最小</strong> </td> 
   <td>この式は、リスト内の最小の項目を返し、次のように書式設定されます。<pre>MIN(item1, item2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>NUMBER</strong> </td> 
   <td>この式は、文字列を数値に変換し、次の形式で設定します。<pre>NUMBER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>POWER</strong> </td> 
   <td>この式は、指数を返します。次の形式で指定します。<pre>POWER(number, power)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>PROD</strong> </td> 
   <td>この式は、すべての数値を乗算し、次のように書式設定されます。<pre>PROD(number1, number2, ....)</pre>
   <b>メモ</b>

時間を含むフィールドに乗算する場合は、選択したフィールドの時間がデータベースに保存される時間（分、時間、秒）を必ず把握してください。 時間が分または秒単位で保存され、Workfrontインターフェイスに時間単位で表示される場合、この計算を使用して式を書き込む際に、分または秒から時間への変換を考慮する必要が生じる場合があります。
</td> 
  </tr> 
  <tr> 
   <td><strong>ROUND</strong> </td> 
   <td>この式は、数値を指定された精度の桁数に丸めます。次の形式で指定します。<p>ROUND（数値，精度）</p></td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCNUM</strong> </td> 
   <td> <p> この式は、昇順で数値を並べ替え、次のように書式設定されます。</p><pre>SORTASCNUM(number1, number2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCNUM</strong> </td> 
   <td>この式は、数値を降順で並べ替え、次の形式で記述します。<pre>SORTDESCNUM(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>SQRT</strong> </td> 
   <td> <p>この式は、数の平方根を返し、次の形式で指定します。 この例では、カスタムフォームが添付されるオブジェクトの下のオブジェクト数を使用します。</p><pre>SQRT({numberOfChildren})</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUB</strong> </td> 
   <td>この式は、指定された順序ですべての数値を引き、次の形式で指定します。<pre>SUB(number1, number2, ...)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>合計</strong> </td> 
   <td>この式は、すべての数値を追加し、次の形式で記述します。<pre>SUM(number1, number2, ...)</pre></td> 
  </tr> 
 </tbody> 
</table>

### テキスト計算カスタムフィールド {#text-calculated-custom-fields}

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
   <td> <p>この式は、他の式と共に使用され、インデックス番号に基づいてリストから値を選択します。 インデックス番号は、数値（通常は既知の範囲）を返すフィールドまたは関数です。</p> <p>式の形式は次のとおりです。</p><pre>CASE(indexNumber, value1, value2, ...)</pre> <p>例えば、次の式は、集計列で曜日の名前を返します。ここで、1=日曜日、2=月曜日などです。</p><pre>CASE(DAYOFWEEK({entryDate}),"日曜日","月曜日","火曜日","水曜日","木曜日","金曜日","土曜日")</pre> <p>この式は、DAYOFWEEK、DAYOFMONTH、MONTH など、数値を返す他の式に最適です。</p> </td> 
  </tr> 
  <tr> 
   <td><strong>CONCAT</strong> </td> 
   <td> <p>この式は、文字列を連結し、次の形式で表されます。</p><pre>CONCAT(string1,"separator", string2)</pre> <p>次に、含めることができる区切り文字の例を示します。</p> 
    <ul> 
     <li>スペース：" "</li> 
     <li>ダッシュ："-"</li> 
     <li>スラッシュ："/"</li> 
     <li>コンマ：","</li> 
     <li>単語："or"、"and"</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>次を含む</strong> </td> 
   <td>この式は、findText 文字列が withinText 文字列内で見つかり、次の形式である場合、true を返します。<pre>CONTAINS(findText, withinText)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>ENCODEURL</strong> </td> 
   <td>この式は、URL 引数に含めることができるように、文字列内の特殊文字をエスケープします。<p>式の形式は次のとおりです。</p><pre>ENCODEURL(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>IF</strong> </td> 
   <td> <p>この式は、指定した条件を評価し、true の場合は trueExpression の値を返します。false の場合は falseExpression の値を返します。</p> <p>式の形式は次のとおりです。</p><pre>IF(condition, trueExpression, falseExpression)</pre> <p>例えば、2 つの異なる日付フィールドの後に True/False の結果が続くデータ文字列を比較できます。</p><pre>IF（{projectedCompletionDate}&gt;{plannedCompletionDate},"トラック外","トラック上"）</pre> <p>毎日の話し方では、この文は次のことを意味します。「オブジェクトの予想完了日が、同じオブジェクトの計画完了日より「大きい」の場合は、このフィールドに「未達成」と表示します。それ以外の場合は、「追跡中」という単語を表示します。</p> <p>true または false の式にラベルを付けたくない場合は、ステートメントに次のような空白のラベルを挿入する必要があります。</p><pre>IF（{projectedCompletionDate}&gt;{plannedCompletionDate},"","追跡中"）</pre> <p>または</p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Off Track","")</pre> <p>「IF」文の作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md" class="MCXref xref">「IF」文の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>IFIN</strong> </td> 
   <td> <p>この式を使用すると、指定可能な値の文字列内の特定の値を検索できます。 検索する値が指定された値のいずれかと等しい場合、式は trueExpression を返します。それ以外の場合は、 falseExpression を返します。</p> <p>式の形式は次のとおりです。</p><pre>IFIN（値，値 1，値 2,..., trueExpression, falseExpression）</pre> <p>例えば、特定のプロジェクト所有者を検索し、プロジェクトビューで指定したタグを使用して、これらのプロジェクトにマークを付けることができます。 <br><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team","Other Teams")</code></p> <p> 毎日の話し方では、この文は次のことを意味します。「プロジェクト所有者が Jennifer Campbell または Rick Kuvec の場合、このプロジェクトを「マーケティングチーム」とマークします。それ以外の場合は、「その他のチーム」とマークします。」</p> <p> true または false の式にラベルを付けたくない場合は、ステートメントに次のような空白のラベルを挿入する必要があります。 </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","","Other Teams")</code></p> <p>または </p> <p><code>IFIN({owner}.{name},"Jennifer Campbell","Rick Kuvec","Marketing Team",""</code> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>IN</strong> </td> 
   <td> <p>この式は、値が指定された値のいずれかと等しい場合に true を返します。それ以外の場合、式は false を返します。</p> <p>式の形式は次のとおりです。</p><pre>IN(value, value1[, value2...])</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>ISBLANK</strong> </td> 
   <td> <p>この式は、値が null または空の場合に true を返します。それ以外の場合、式は false を返します。</p> <p>式の形式は次のとおりです。</p><pre>ISBLANK(value)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEFT</strong> </td> 
   <td> <p>この式は、文字列の左側から指定された数の文字を返し、次のように書式設定されます。</p><pre>LEFT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LEN</strong> </td> 
   <td> <p>この式は、文字列の長さを返し、次の形式で設定されます。</p><pre>LEN(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>LOWER</strong> </td> 
   <td>この式は、小文字の文字列を返し、次のように書式設定されます。<pre>LOWER(string)</pre></td> 
  </tr> 
  <tr> 
   <td><strong>置き換え</strong> </td> 
   <td> <p>この式は、string1 内の文字列 2 のすべての箇所を文字列 3 に置き換えます。</p> <p>式の形式は次のとおりです。</p><pre>REPLACE(string1, string2, string3)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>RIGHT</strong> </td> 
   <td> <p>この式は、文字列の右側から指定された数の文字を返し、次のように書式設定されます。</p><pre>RIGHT(string, length)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SEARCH</strong> </td> 
   <td> <p>この式は、Text 内の文字列で、指定された開始位置から始まる findText の最初の値のインデックスを返します。テキストが見つからない場合は、-1 を返します。</p> <p>式の形式は次のとおりです。</p><pre>SEARCH(findText, withinText, start)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>STRING</strong> </td> 
   <td> <p>この式は、数値を文字列に変換し、次の形式で設定します。</p><pre>STRING（数値）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTASCSTRING</strong> </td> 
   <td> <p>この式は、文字列のリストを昇順に並べ替え、次のように書式設定します。</p><pre>SORTASCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SORTDESCSTRING</strong> </td> 
   <td> <p> この式は、文字列のリストを降順に並べ替え、次のように書式設定します。</p><pre>SORTDESCSTRING(string1, string2, ...)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>SUBSTR</strong> </td> 
   <td> <p>この式は、指定された開始インデックスと終了インデックスに基づいて、文字列の文字を返します。次のような形式で指定します。</p><pre>SUBSTR（{string}，開始位置の数，終了位置の数）</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>TRIM</strong> </td> 
   <td> <p>この式は、文字列の先頭と末尾から空白を削除し、次のように書式設定されます。</p><pre>TRIM(string)</pre> </td> 
  </tr> 
  <tr> 
   <td><strong>UPPER</strong> </td> 
   <td> <p>この式は、大文字の文字列を返し、次のように書式設定されます。</p><pre>UPPER(string)</pre> </td> 
  </tr> 
 </tbody> 
</table>
