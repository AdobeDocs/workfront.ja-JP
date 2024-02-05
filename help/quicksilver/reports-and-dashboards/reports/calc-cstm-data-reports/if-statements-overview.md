---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF ステートメントの概要
description: 「IF」ステートメントは、一般的なプログラミング言語で使用できます。Adobe Workfront では、「IF」ステートメントを使用すると、レポートおよびカスタムデータの両方の目的で、データのフィールドを比較、書式設定、および文字列化できます。また、「IF」ステートメントに関する数学的な考え方は、式の変数が一般的に使用されるので、概念的な理解を深めます。
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 23b5ba9564b514e11c1ca9d5cca276238ef11066
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 87%

---

# 「IF」ステートメントの概要

<!-- Audited: 1/2024 -->

「IF」ステートメントは、一般的なプログラミング言語で使用できます。Adobe Workfront では、「IF」ステートメントを使用すると、レポートおよびカスタムデータの両方の目的で、データのフィールドを比較、書式設定、および文字列化できます。また、「IF」ステートメントに関する数学的な考え方は、式の変数が一般的に使用されるので、概念的な理解を深めます。

## 「IF」ステートメントの推奨事項

「IF」ステートメントを作成する前に、次の点を考慮してください。

* 一般的なプログラミング言語に関する基礎知識を身に付けることをお勧めしますが、このガイドでは必要としません。
* Workfront テキストモードの構文について、詳しく理解しておく必要があります。これは、Workfront API の用語を把握し、これらの特定の形式のカスタムデータの構文を理解するのに役立ちます。

  Workfront API について詳しくは、[API の基本](../../../wf-api/general/api-basics.md)を参照してください。

  テキストモードの使用について詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)を参照してください。

* 次の Workfront 要素に対して「IF」ステートメントを作成できます。

   * ビュー
   * グループ化
   * 計算済みカスタムフィールド

* フィルターに対して「IF」ステートメントを作成することはできません。その結果、Workfrontで「Whoops」エラーが発生します。
* サポートチームは、カスタムデータの作成を支援しません。カスタムフィールドまたは列を作成した後で、希望する結果が表示されない場合は、サポートチームに連絡してください。式の作成に関するヘルプが必要な場合は、アカウント担当者にお問い合わせいただき、当社のコンサルティングオプションをご確認ください。
* これらの式は、Sublime や Visual Studio Code などのテキストエディターで最初に記述することをお勧めします。これは、Workfront で表示されるよりもデータをより明確に表示するのに役立つからです。

## 「IF」ステートメントの構成要素

次の形式を使用して、Workfront で「IF」ステートメントを作成できます。
<pre>IF(Condition,True Expression,False Expression)</pre>「IF」ステートメントの構成要素は次のとおりです。

* **IF** =これは、Workfrontの「関数」の計算データ式です。 SUM 式や PROD 式と同様に、この式は最初に、関数を「IF」ステートメントとして理解するようにシステムに指示します。このステートメントの「IF」には必ず大文字を使用してください。\
  すべての計算データ式のリストについては、 [計算データ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **条件** =これはWorkfront変数が満たす必要がある条件で、この式の基礎です。 式で後から指定できるものはすべて、条件によって異なります。いくつかの参照、比較、数式を使用して、数式を開始できます。条件の例を次に示します。

   * 指定したオブジェクトの日付が別の日付よりも大きくなっています。
   * ステータスは、指定したオブジェクトで使用可能なステータスの 1 つに等しくなります。
   * タスクの完了率が、特定の割合よりも小さいか大きいです。

* **Condition Operator** = これは、「IF」ステートメントの条件の作成に役立つ演算子です。例えば、「is equal to」または「is greater than」は条件演算子です。ステートメントで使用できる条件演算子のリストについては、[計算されたカスタム式の条件演算子](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md)を参照してください。

* **True****Expression** =これは「True」変数で、条件の条件が満たされた場合にどの指標を表示するか（真の指標）を数式に示します。

* **False 式** =これは「False」変数で、条件の条件が満たされない場合にどの指標を表示するかを式に示します（偽の指標）。

次の例では、元のステートメントの形式を使用して、「IF」ステートメントの単純なデータ式を記述します。この式は、Workfront の 2 つの異なる日付フィールドを比較し、その後に True/False の結果をデータ文字列として返します。

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

日常会話では、このステートメントは次のことを意味します。自分のオブジェクトの予定完了日が同じオブジェクトの予定完了日よりも「大きい」場合、このフィールドに「予定外」という単語を表示します。そうでない場合は、「順調」という単語を表示します。

## 「IF」ステートメントを使用してカスタムフォームまたはカスタム列の計算フィールドを作成する

カスタムフォームまたはカスタム列の計算フィールドに「IF」ステートメントを作成できます。

計算カスタムフォームと計算カスタム列で使用する構文には違いがあります。次の例を参照してください。

* [単一「IF」文](#single-if-statements)
* [多重「IF」文](#multiple-if-statements)

### 単一「IF」文 {#single-if-statements}

次に示すのは、1 つの「IF」文を使用した計算カスタムフィールドとそれに対応する列の例です。

* 計算カスタムフィールド：

カスタムフィールドを作成する場合は、次の構文の「IF」文を使用します。

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* 計算カスタム列：

カスタム列を作成する場合は、値式行の「IF」文に次の構文を使用してください。

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### 多重「IF」文 {#multiple-if-statements}

より複雑で動的な式を作成するには、次の文を使用して複数の「IF」文を組み合わせます。

<pre>IF (条件 1，True 式，IF (条件 2，True 式，False 式))</pre>最初の「IF」の false 文がなくなったことに注意してください。その代わりに、2 番目の「IF」の開始に置き換わりました。

次に示すのは、多重「IF」文を使用した計算カスタムフィールドとそれに対応するカスタム列の例です。

* 計算カスタムフィールド：

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* 計算カスタム列：

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

この例では、2 つの異なる条件変数を組み合わせることで、同じことが実現されています。\
これらのオプションについては、お使いの環境でこれらの例を再作成することで、さらに詳しく調べることができます。

これを習得する最善の方法は、様々なフィールドやシナリオを試すことです。また、API エクスプローラーに慣れれば、使用可能なフィールド名が簡単にわかるようになります。API エクスプローラーについては、[API エクスプローラー](../../../wf-api/general/api-explorer.md)を参照してください。

計算データ式のWorkfront構文について詳しくは、 [計算データ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
