---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算済みカスタムフィールドと計算済み列の比較
description: Adobe Workfront で複数のフィールドを集計し、その集計値を新しいフィールドに表示するには、カスタムフォームで計算済みカスタムフィールドを作成するか、ビューで計算列を作成します。
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: c49b545938a78716084296ef1b4e7c0fc075ef95
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 100%

---

# 計算済みカスタムフィールドと計算済み列の比較

Adobe Workfront で複数のフィールドを集計し、その集計値を新しいフィールドに表示するには、次のように作成します。

* カスタムフォームの計算済みカスタムフィールド\
  計算済みカスタムフィールドをカスタムフォームに追加する方法について詳しくは、[計算済みデータをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)の記事の[計算済みフィールドをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#add-a-calculated-field-to-a-custom-form)の節を参照してください。

* ビューの計算済み列\
  ビューで計算を使用する方法について詳しくは、[テキストモードの一般的な使用例の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)の記事の[ビューでテキストモードを使用](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#use-text-mode-in-views)の節を参照してください。

計算済みフィールドと計算済み列は、どちらもテキストモードを使用して作成できますが、作成する構文が異なります。計算済みフィールドと計算済み列を作成する方法について詳しくは、上記の記事を参照してください。計算済みカスタムフィールドや計算済み列など、計算済みのデータ式で使用される様々な構文について詳しくは、この記事の[計算済みカスタムフィールドと計算済みカスタム列の構文の比較](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md#syntax-of-calculated-custom-fields-vs-calculated-custom-columns)を参照してください。

計算済みフィールドと計算済み列の両方で、同じ計算を使用できます。ただし、その計算の目的によって、どちらを作成するのかを検討する必要があります。

## 計算済みカスタムフィールドと計算済みカスタム列の構文の比較

使用する関数は同じですが、計算済みカスタムフィールドで式を作成する場合の構文は、計算済みカスタム列を作成する場合の構文とは異なる場合があります。

例：

* タスクのカスタムフォームのカスタムフィールドでは、以下を使用して、カスタムフォームが添付されているタスクの親プロジェクトの名前を生成します。

  `{project}.{name}`

* レポートのカスタム列では、以下を使用して、タスクレポートにプロジェクト名のカスタム列を追加します。

  `valuefield=project:name`

  または

  `valueexpression={project}.{name}`

  >[!TIP]
  >
  >同じ構文が、計算式を使用するすべてのテキストモードレポート要素（ビュー、フィルター、グループ化、プロンプト）に適用されます。

2 つの構文の違いは次のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>計算済みカスタムフィールド</strong></td>
   <td><strong>計算済みカスタムレポート要素</strong></td> 
  </tr> 
  <tr> 
   <td> <p>フィールドの名前は、Workfront インターフェイスに表示されるとおりに使用します。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span>計算済みのカスタムフィールドで使用されるフィールド名の例：<code>Planned Completion Date</code></p> </td> 
   <td> <p>オブジェクトまたはフィールドの名前は、Workfront データベースに表示されるとおりに使用します。オブジェクトとフィールドの名前は、小文字またはキャメルケース（複合名の場合）で入力します。 </p> <p>データベースに表示されるすべての Workfront オブジェクトとフィールドのインベントリについて詳しくは、<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラー</a>を参照してください。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span>計算済みカスタムレポート要素で使用されるフィールド名の例：<code>plannedCompletionDate</code></p> </td> 
  </tr> 
  <tr> 
   <td>フィールド名を丸括弧または中括弧で囲みます。</td> 
   <td> <p>フィールド名は、<code>valuefield </code> 行で使用する場合、角括弧または丸括弧内で囲まないでください。</p> <p>フィールド名は、<code>valueexpression</code> 行で使用する場合、中括弧で囲みます。</p> </td> 
  </tr> 
  <tr> 
   <td>フィールドはピリオドで区切ります。</td> 
   <td> <p><code>valuefield</code> 行でフィールドを使用する場合は、コロンで区切ります。</p> <p>フィールドは、<code>valueexpression</code> 行で使用する場合、ピリオドで区切ります。</p> </td> 
  </tr> 
 </tbody> 
</table>

計算済みカスタム列で使用する必要がある構文について詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)を参照してください。

## 計算済みカスタムフィールドを使用する場合

* 集計結果をレポートでグループ化する場合や、その情報をグラフに表示する場合
* フィールドで計算した集計以外のデータを集計する場合
* データは更新されず、時間が経つと変わる可能性があるので、データの適時性を気にしない場合

## 計算済みカスタムフィールドの更新をトリガーするアクション

* オブジェクトのメインページでその他アイコン ![](assets/more-icon.png) をクリックし、「**式を再計算**」をクリック

* 「**カスタム式を再計算**」が有効になっている場合に複数のオブジェクトを一括編集
* 計算済みカスタムフィールドに対して「**前の計算を更新**」が有効になっている場合にカスタムフォームを編集

## ビューで計算済み列を使用する場合

* リアルタイムデータをレポートで使用できるようにする場合。

  計算済みビューは常に最新の状態です。計算が行われるのは、レポートが実行されたときやビューが適用されたときであるためです。

* 集計した結果でグループ化する予定がなく、この情報をグラフで使用する予定もない場合。
* 列で計算される集計を超えてデータを集計する予定がない場合（データを集計できるのは 1 回のみです）。
* $$TODAY ワイルドカードまたは $$NOW ワイルドカードを使用して、現在の日付への参照を計算に含める場合。

  >[!TIP]
  >
  >この参照は、添付されたオブジェクトが編集されたときにのみ再計算されるので、計算済みカスタムフィールドでは使用しないでください。このタイプの計算は古くなります。

## 計算カスタムフィールドと列の例

計算カスタムフィールドの例については、[レポート内の計算カスタムデータ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md)を参照してください。

ビュー内の計算カスタム列の例については、次の記事を参照してください。

* [テキストモードの一般的な使用例の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [カスタムビュー、フィルター、グループ化の例：記事インデックス](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
