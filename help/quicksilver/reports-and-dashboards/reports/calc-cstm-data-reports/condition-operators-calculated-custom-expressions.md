---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算されたカスタム式の条件演算子
description: テキストモードの使用時に、Adobe Workfrontで計算済みのカスタムデータを作成する際に、条件演算子または修飾子を使用できます。
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 1%

---

# 計算カスタムフィールドの条件演算子

テキストモードの使用時に、Adobe Workfrontで計算済みのカスタムデータを作成する際に、条件演算子または修飾子を使用できます。

Workfrontでのテキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

条件演算子または修飾子は、ステートメント内の既存のWorkfrontフィールドを結合し、新しいフィールドを生成することで、条件ステートメントを作成するのに役立ちます。 条件演算子の最も一般的な使用法は、「IF」文の条件を作成することです。

Workfrontの「IF」ステートメントを使用して、レポートおよびカスタムデータの両方の目的で、データのフィールドを比較、書式設定および文字列化できます。

次のWorkfront要素に対して「IF」文を作成できます。

* ビュー
* グループ化
* 計算済みカスタムフィールド

「IF」文の作成について詳しくは、 [「IF」文の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md).

このガイドの例では、計算カスタムフィールドでの条件演算子の使用方法を説明します。 レポートの計算カスタムフィールドの正しい構文に従う場合は、計算カスタム列やグループでも使用できます。

レポート内の計算カスタムフィールドと計算カスタムデータの構文の違いについて詳しくは、 [計算カスタムフィールドと計算列](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

API エクスプローラーを参照して、計算カスタム式で参照するフィールドを見つけます。 API エクスプローラーについて詳しくは、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

Workfrontでは、次の条件修飾子を使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>条件演算子</th> 
   <th>条件演算子の構文</th> 
   <th>条件演算子の定義</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>等しい (大文字と小文字を区別しない)</td> 
   <td>= </td> 
   <td> <p>ステートメントの最初のフィールドが 2 番目のフィールドと等しい場合に条件が満たされることを示すには、この演算子を使用します。</p> <p>例えば、次の文を計算カスタムフィールドで使用して、計画完了日とタスクの予定完了日を比較する「IF」文を作成します。 </p><pre>IF（{projectedCompletionDate}={plannedCompletionDate},"追跡中","追跡外"）</pre> </td> 
  </tr> 
  <tr> 
   <td>より大きい </td> 
   <td>&gt; </td> 
   <td>ステートメントの最初のフィールドが 2 番目のフィールドより大きい場合に条件が満たされることを示すには、この演算子を使用します。 <p>例えば、次の文を計算カスタムフィールドで使用して、計画完了日とタスクの予定完了日を比較する「IF」文を作成します。 </p><pre>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</pre></td> 
  </tr> 
  <tr> 
   <td>次よりも大きいか等しい </td> 
   <td>&gt;= </td> 
   <td>ステートメントの最初のフィールドが 2 番目のフィールド以上の場合に条件が満たされることを示すには、この演算子を使用します。 <p>例えば、次の文を計算カスタムフィールドで使用して、計画完了日とタスクの予定完了日を比較する「IF」文を作成します。 </p><pre>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</pre></td> 
  </tr> 
  <tr> 
   <td>より小さい </td> 
   <td>&lt; </td> 
   <td>ステートメントの最初のフィールドが 2 番目のフィールドより小さい場合に条件が満たされることを示すには、この演算子を使用します。 <p>例えば、次の文を計算カスタムフィールドで使用して、計画完了日とタスクの予定完了日を比較する「IF」文を作成します。 </p><pre>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</pre></td> 
  </tr> 
  <tr> 
   <td>次よりも小さいか等しい </td> 
   <td>&lt;= </td> 
   <td>ステートメントの最初のフィールドが 2 番目のフィールド以下の場合に条件が満たされることを示すには、この演算子を使用します。 <p>例えば、次の文を計算カスタムフィールドで使用して、計画完了日とタスクの予定完了日を比較する「IF」文を作成します。 </p><pre>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</pre></td> 
  </tr> 
  <tr> 
   <td>次の値と等しくない </td> 
   <td>! </td> 
   <td> <p>上記の演算子の前にこの演算子を追加して、演算子を無効にします。 </p> <p>例： </p> 
    <ul> 
     <li>が次と等しい: = </li> 
     <li>が次と等しくない: != </li> 
    </ul> <p>次のデータ式の前にこの演算子を追加すると、式に負の文が追加されます。 </p> 
    <ul> 
     <li>含む </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>これらのデータ式について、および完全なリストについては、 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">計算データ式</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>または </td> 
   <td>|| </td> 
   <td> <p>この演算子は、式がステートメントの最初または 2 番目の値を見つけたときに条件が満たされることを示す場合に使用します。 </p> <p>たとえば、次の文を計算カスタム・フィールドで使用して、現在または計画ステータスのプロジェクトを「アクティブ」としてマークする「IF」文を作成します。 </p><pre>IF({status}="PLN"||{status}="CUR","Active","Not Active")</pre> </td> 
  </tr> 
  <tr> 
   <td> および </td> 
   <td>&amp;&amp; </td> 
   <td> <p>式が、同時に 2 つの条件を満たす項目を見つけた場合に、条件が満たされることを示すには、この演算子を使用します。 </p> <p>たとえば、計算されたカスタムフィールドで次の文を使用して、現在のステータスのプロジェクトを検索し、リスク条件を持ち、それらを「調停が必要」とマークする「IF」文を作成します。 </p><pre>IF（{status}="CUR"&amp;&amp;{condition}="AR","調停が必要",""）</pre> </td> 
  </tr> 
 </tbody> 
</table>
