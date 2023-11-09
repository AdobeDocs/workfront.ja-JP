---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 計算カスタムフィールドと計算列の比較
description: レポートとダッシュボードのカスタムデータについて説明します
author: Nolan
feature: Reports and Dashboards
exl-id: 17ac554d-0c90-4592-946e-a89f1784571d
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 計算カスタムフィールドと計算列の比較

Adobe Workfrontで複数のフィールドを集計し、その集計値を新しいフィールドに表示するには、次の操作を実行します。

* カスタムフォームの計算済みカスタムフィールド\
  計算カスタムフィールドをカスタムフォームに追加する方法について詳しくは、 [カスタムフォームに計算フィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#creating-calculated-custom-fields) 記事内 [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

* ビューの計算列\
  ビューでの計算の使用の詳細については、「 [ビューでのテキストモードの使用](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md#using-text-mode-in-views) 記事内 [テキストモードの一般的な使用例の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

テキストモードを使用して計算フィールドと計算列の両方を作成できますが、それらを作成する構文は異なります。 計算フィールドと計算列を作成する方法については、上記の記事を参照してください。 計算カスタムフィールドや計算列など、計算データの式で使用される様々な構文について詳しくは、「 [計算カスタムフィールドと計算カスタム列の構文](#syntax-of-calculated-custom-fields-vs-calculated-custom-columns-syntax) 」を参照してください。

計算列と計算フィールドの両方で同じ計算を使用できます。 ただし、これらの計算の目的に応じて、どちらか一方を作成することを検討する必要があります。

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
  >同じ構文は、計算式が使用されるすべてのテキストモードレポート要素（ビュー、フィルタ、グループ化、プロンプト）に適用されます。

2 つの構文の違いは次のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>計算済みカスタムフィールド</td> 
   <td>計算済みカスタムレポート要素</td> 
  </tr> 
  <tr> 
   <td> <p>フィールドの名前は、Workfrontインターフェイスに表示されるとおりに使用します。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span>計算カスタムフィールドで使用されるフィールド名の例： <code>Planned Completion Date</code>.</p> </td> 
   <td> <p>オブジェクトまたはフィールドの名前は、Workfrontデータベースに表示されるとおりに使用します。 オブジェクトとフィールドの名前は、小文字またはキャメル文字（複合名の場合）で入力されます。 </p> <p>データベースに表示されるすべてのWorkfrontオブジェクトとフィールドの在庫については、 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラ</a>. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span>計算カスタムレポート要素で使用されるフィールド名の例： <code>plannedCompletionDate</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>フィールド名を括弧または中括弧で囲みます。</td> 
   <td> <p>フィールド名を <code>valuefield </code>行。</p> <p>フィールド名を <code>valueexpression</code> 行。</p> </td> 
  </tr> 
  <tr> 
   <td>フィールドをピリオドで区切ります</td> 
   <td> <p>フィールドを <code>valuefield </code>行</p> <p>フィールドをピリオドで区切ります ( <code>valueexpression </code>行。 </p> </td> 
  </tr> 
 </tbody> 
</table>

計算カスタム列で使用する必要がある構文について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## 計算カスタムフィールドを使用するタイミング

* 集計した結果をレポートでグループ化する場合や、この情報をグラフに表示する場合
* フィールドで計算される集計以外にデータを集計する場合
* データは更新されず、時間の経過と共に変化する可能性があるので、データの適時性を気にしない場合

## 計算済みカスタムフィールドの更新をトリガーにするアクション

* オブジェクトのメインページで、「その他」アイコンをクリックします。 ![](assets/more-icon.png)をクリックし、 **式を再計算**

* 複数のオブジェクトの一括編集 ( **カスタム式の再計算** が有効になっている
* 次の場合にカスタムフォームを編集する **以前の計算を更新** は計算済みカスタムフィールドに対して有効です。

## ビューで計算列を使用する場合

* リアルタイムデータをレポートで使用できるようにする場合。

  計算されたビューは常に新鮮です。これは、レポートの実行時やビューの適用時に計算が行われるからです。

* 集計した結果でグループ化する予定がなく、この情報をグラフで使用する予定がない場合。
* 列で計算される集計を超えてデータを集計する予定がない場合（データは 1 回のみ集計できます）。
* $$TODAY ワイルドカードまたは$$NOW ワイルドカードを使用して、現在の日付への参照を計算に含める場合。

  >[!TIP]
  >
  >この参照は、アタッチされたオブジェクトが編集されたときにのみ再計算されるので、計算済みのカスタムフィールドでは使用しないでください。 このタイプの計算は古くなります。

## 計算済みカスタムフィールドと列の例

計算カスタムフィールドの例については、 [レポート内の計算済みカスタムデータ](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-data-reports.md).

ビューの計算済みカスタム列の例については、次の記事を参照してください。

* [テキストモードの一般的な使用例の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)
* [カスタム・ビュー、フィルタ、グループ化のサンプル](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)
