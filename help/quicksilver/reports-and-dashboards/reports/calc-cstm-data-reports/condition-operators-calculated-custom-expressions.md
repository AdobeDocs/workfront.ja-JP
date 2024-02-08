---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算済みカスタム式の条件演算子
description: テキストモードの使用時に、Adobe Workfront で計算済みのカスタムデータを作成する際に、条件演算子または修飾子を使用できます。
author: Nolan
feature: Reports and Dashboards
exl-id: ce98ca39-cb86-4ef7-b75c-29ceb916e885
source-git-commit: 639a696c19d79cf2415a45ccb9849ec183fb0bb8
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 93%

---

# 計算カスタムフィールドの条件演算子

<!-- Audited: 2/2024 -->

テキストモードの使用時に、Adobe Workfrontで計算済みのカスタムデータを作成する際に、条件演算子または修飾子を使用できます。 Workfrontでのテキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

条件演算子または修飾子は、ステートメント内の既存の Workfront フィールドを結合し、新しいフィールドを生成することで、条件ステートメントを作成するのに役立ちます。条件演算子の最も一般的な使用法は、「IF」ステートメントの条件を作成することです。

Workfront の「IF」ステートメントを使用して、レポートおよびカスタムデータの両方の目的で、データのフィールドを比較、フォーマットおよび文字列化できます。

次の Workfront 要素に対して「IF」ステートメントを作成できます。

* ビュー
* グループ化
* 計算済みカスタムフィールド

「IF」ステートメントの作成について詳しくは、[「IF」ステートメントの概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md)を参照してください。

このガイドの例では、計算済みカスタムフィールドでの条件演算子の使用方法について説明します。レポートの計算済みカスタムフィールドの正しい構文に従う場合は、計算済みカスタム列またはグループでも使用できます。

レポート内の計算済みカスタムフィールドおよび計算済みカスタムデータの構文の違いについて詳しくは、[計算済みカスタムフィールドと計算済み列の比較](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md)を参照してください。

API エクスプローラーを参照して、計算済みカスタム式で参照するフィールドを見つけます。API エクスプローラーについて詳しくは、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を参照してください。

Workfront では、次の条件修飾子を使用できます。

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
   <td>が次に等しい</td> 
   <td>= </td> 
   <td> <p>ステートメントの最初のフィールドが 2 番目のフィールドと等しい場合に条件が満たされることを示すには、この演算子を使用します。</p> <p>例えば、次のステートメントを計算済みカスタムフィールドで使用して、予定完了日とタスクの見込み完了日を比較する「IF」ステートメントを作成します。 </p><p><code>IF({projectedCompletionDate}={plannedCompletionDate},"On Track","Off Track")</code></p> </td> 
  </tr> 
  <tr> 
   <td>より大きい </td> 
   <td>&gt; </td> 
   <td>ステートメントの最初のフィールドが 2 番目のフィールドより大きい場合に条件が満たされることを示すには、この演算子を使用します。 <p>例えば、次のステートメントを計算済みカスタムフィールドで使用して、予定完了日とタスクの見込み完了日を比較する「IF」ステートメントを作成します。 </p><p><code>IF({projectedCompletionDate}&gt;{plannedCompletionDate},"Late","")</code></p></td> 
  </tr> 
  <tr> 
   <td>が次よりも大きいか等しい </td> 
   <td>&gt;= </td> 
   <td>ステートメントの最初のフィールドが 2 番目のフィールド以上の場合に条件が満たされることを示すには、この演算子を使用します。 <p>例えば、次のステートメントを計算済みカスタムフィールドで使用して、予定完了日とタスクの見込み完了日を比較する「IF」ステートメントを作成します。 </p><p><code>IF({projectedCompletionDate}&gt;={plannedCompletionDate},"Late","Early")</code></p></td> 
  </tr> 
  <tr> 
   <td>より小さい </td> 
   <td>&lt; </td> 
   <td>ステートメントの最初のフィールドが 2 番目のフィールドより小さい場合に条件が満たされることを示すには、この演算子を使用します。 <p>例えば、次のステートメントを計算済みカスタムフィールドで使用して、予定完了日とタスクの見込み完了日を比較する「IF」ステートメントを作成します。 </p><p><code>IF({projectedCompletionDate}&lt;{plannedCompletionDate},"Early","")</code></p></td> 
  </tr> 
  <tr> 
   <td>以下 </td> 
   <td>&lt;= </td> 
   <td>ステートメントの最初のフィールドが 2 番目のフィールド以下の場合に条件が満たされることを示すには、この演算子を使用します。 <p>例えば、次のステートメントを計算済みカスタムフィールドで使用して、予定完了日とタスクの見込み完了日を比較する「IF」ステートメントを作成します。 </p><p><code>IF({projectedCompletionDate}&lt;={plannedCompletionDate},"Early","Late")</code></p></td> 
  </tr> 
  <tr> 
   <td>次の値と等しくない </td> 
   <td>! </td> 
   <td> <p>上記の演算子の前にこの演算子を追加して、演算子を無効にします。 </p> <p>例： </p> 
    <ul> 
     <li>が次と等しい: = </li> 
     <li>が次と等しくない: != </li> 
    </ul> <p>次のデータ式の前にこの演算子を追加すると、式に負のステートメントが追加されます。 </p> 
    <ul> 
     <li>が次を含む </li> 
     <li>IN </li> 
     <li>IFIN </li> 
     <li>ISBLANK </li> 
    </ul> <p>これらのデータ式について、および完全なリストについては、 <a href="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md" class="MCXref xref">計算データ式の概要</a>. </p> </td> 
  </tr> 
  <tr> 
   <td>または </td> 
   <td>|| </td> 
   <td> <p>式がステートメントの最初または 2 番目の値を見つけたときに条件が満たされることを示す場合にこの演算子を使用します。 </p> <p>例えば、次のステートメントを計算済みカスタムフィールドで使用して、現在または予定ステータスのプロジェクトを「アクティブ」としてマークする「IF」ステートメントを作成します。 </p><p><code>IF({status}="PLN"||{status}="CUR","Active","Not Active")</code></p> </td> 
  </tr> 
  <tr> 
   <td> および </td> 
   <td>&amp;&amp; </td> 
   <td> <p>式が同時に 2 つの条件を満たす項目を見つけた際に条件が満たされることを示す場合は、この演算子を使用します。 </p> <p>例えば、計算済みカスタムフィールドで次のステートメントを使用して、現在のステータスのプロジェクトを検索し、リスク条件を持ち、それらを「調停が必要」とマークする「IF」ステートメントを作成します。 </p><p><code>IF({status}="CUR"&&{condition}="AR","Mediation Needed","")</code></p> </td> 
  </tr> 
 </tbody> 
</table>