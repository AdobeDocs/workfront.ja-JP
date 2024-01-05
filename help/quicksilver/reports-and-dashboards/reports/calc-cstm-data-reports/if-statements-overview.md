---
content-type: overview
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: IF 文の概要
description: 「IF」文は、一般的なプログラミング言語で使用できます。 Adobe Workfrontでは、「IF」ステートメントを使用すると、レポートおよびカスタムデータの両方の目的で、データのフィールドを比較、書式設定および文字列化できます。 また、「IF」文に関する数学的な考え方は、式の変数が一般的に使用されるので、概念的な理解を深めます。
author: Nolan
feature: Reports and Dashboards
exl-id: 090a85fd-fdbe-4507-8bad-ce8c29bf8fc9
source-git-commit: 23b5ba9564b514e11c1ca9d5cca276238ef11066
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# 「IF」文の概要

<!-- Audited: 1/2024 -->

「IF」文は、一般的なプログラミング言語で使用できます。 Adobe Workfrontでは、「IF」ステートメントを使用すると、レポートおよびカスタムデータの両方の目的で、データのフィールドを比較、書式設定および文字列化できます。 また、「IF」文に関する数学的な考え方は、式の変数が一般的に使用されるので、概念的な理解を深めます。

## Recommendations （「IF」文用）

「IF」文を作成する前に、次の点を考慮してください。

* 一般的なプログラミング言語に関する基礎知識を身に付けることをお勧めしますが、このガイドでは必要としません。
* Workfrontテキストモードの構文について、詳しく理解しておく必要があります。 これは、Workfront API の用語を把握し、これらの特定の形式のカスタムデータの構文を理解するのに役立ちます。

  Workfront API について詳しくは、 [API の基本](../../../wf-api/general/api-basics.md).

  テキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

* 次のWorkfront要素に対して「IF」文を作成できます。

   * ビュー
   * グループ化
   * 計算済みカスタムフィールド

* フィルターに対して「IF」ステートメントを作成することはできません。 その結果、Workfrontで「Whoops」エラーが発生します。
* サポートチームは、カスタムデータの作成に役立ちません。 カスタムフィールドまたは列を作成した後で、希望する結果が表示されない場合は、サポートチームに連絡してください。 式の作成に関するヘルプが必要な場合は、アカウント担当者にお問い合わせいただき、当社のコンサルティングオプションをご確認ください。
* これらの式は、Sublime や Visual Studio Code などのテキストエディターで最初に記述することをお勧めします。これは、Workfrontで表示されるよりもデータをより明確に表示するのに役立つからです。

## 「IF」文の構成要素

次の形式を使用して、Workfrontで「IF」文を作成できます。
<pre>IF(Condition,True Expression,False Expression)</pre>「IF」文の構成要素は次のとおりです。

* **IF** =これは、Workfrontの「関数」の計算データ式です。 SUM 式や PROD 式と同様に、この式は最初に、関数を「IF」文として理解するようにシステムに指示します。 この文の「IF」には必ず大文字を使用してください。\
  すべての計算データ式のリストについては、 [計算データ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

* **条件** =これはWorkfront変数が満たす必要がある条件で、この式の基礎です。 式で後から指定できるものはすべて、条件によって異なります。 数の参照、比較、数式を使用して、数式を開始できます。 条件の例を次に示します。

   * 指定したオブジェクトの日付が別の日付よりも大きくなっています。
   * ステータスは、指定したオブジェクトで使用可能なステータスの 1 つに等しくなります。
   * タスクの完了率が、特定の割合よりも小さいか大きいです。

* **条件演算子** =これは、「IF」文の条件の作成に役立つ演算子です。 例えば、「次と等しい」または「次よりも大きい」は条件演算子です。 ステートメントで使用できる条件演算子のリストについては、 [計算されたカスタム式の条件演算子](../../../reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

* **True****Expression** =これは「True」変数で、条件の条件が満たされた場合にどの指標を表示するか（真の指標）を数式に示します。

* **False 式** =これは「False」変数で、条件の条件が満たされない場合にどの指標を表示するかを式に示します（偽の指標）。

次の例では、元の文の形式を使用して、「IF」文の単純なデータ式を記述します。 この式は、Workfrontの 2 つの異なる日付フィールドの後に、True/False の結果がデータ文字列として比較します。

```
IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

毎日の音声で、このステートメントは、「オブジェクトの完了予定日が同じオブジェクトの完了予定日が計画日より大きい」の場合、このフィールドに「トラック外」と表示します。 そうでない場合は、「追跡中」という単語を表示します。

## 「IF」ステートメントを使用してカスタムフォームまたはカスタム列の計算フィールドを作成する

計算フィールドのカスタムフォームまたはカスタム列のいずれかで、「IF」ステートメントを作成できます。

計算カスタムフォームと計算カスタム列で使用する構文には違いがあります。 次の例を参照してください。

* [単一の「IF」文](#single-if-statements)
* [複数の「IF」文](#multiple-if-statements)

### 単一の「IF」文 {#single-if-statements}

次に、「IF」ステートメントを使用した計算済みカスタムフィールドとその対応する列の例を示します。

* 計算済みカスタムフィールド：

カスタムフィールドを作成する場合、「IF」ステートメントに次の構文を使用します。

```
IF({Projected Completion Date}>{Planned Completion Date},"Off Track","On Track")
```

* 計算されたカスタム列：

カスタム列を作成する場合、値式行の「IF」ステートメントには次の構文を使用する必要があります。

```
valueexpression=IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track","On Track")
```

### 複数の「IF」文 {#multiple-if-statements}

より複雑で動的な式を作成するには、次のステートメントを使用して複数の「IF」ステートメントを組み合わせます。

<pre>IF( 条件 1，真の式，IF（条件 2，真の式，偽の式）)</pre>最初の「IF」に対して偽の文が存在しなくなりました。 代わりに、2 つ目の「IF」の先頭に置き換えました。

次に、複数の「IF」ステートメントを使用した計算済みカスタムフィールドと対応するカスタム列の例を示します。

* 計算済みカスタムフィールド：

  ```
  IF({projectedCompletionDate}>{plannedCompletionDate},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
  ```

* 計算されたカスタム列：

```
valueexpression=IF({"projectedCompletionDate"}>{"plannedCompletionDate"},"Off Track",IF({plannedCompletionDate}>{projectedCompletionDate},"Off Track","On Track"))
```

この例では、2 つの異なる条件変数を組み合わせることで、同じことが実行されています。\
これらのオプションは、独自の環境で再構築することでさらに詳しく調べることができます。

これを学ぶ最善の方法は、様々なフィールドとシナリオを試すことです。 また、API エクスプローラーにも慣れて、使用可能なフィールド名を確認します。 API エクスプローラーについて詳しくは、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

計算データ式のWorkfront構文について詳しくは、 [計算データ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
