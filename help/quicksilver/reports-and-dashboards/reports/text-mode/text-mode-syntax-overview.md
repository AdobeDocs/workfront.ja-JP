---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードの構文の概要
description: テキストモードインタフェースを使用して、より複雑なビュー、フィルタ、グループ化、およびリストとレポート内のカスタマイズされたプロンプトを作成できます。 テキストモードを使用すると、標準モードインターフェイスでは使用できないフィールドとその属性にアクセスできます。
author: Nolan
feature: Reports and Dashboards
role: User
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 6279106f56fa0d128e0dd03cd13b63a71d4c2952
workflow-type: tm+mt
source-wordcount: '1865'
ht-degree: 0%

---

# テキストモードの構文の概要

テキストモードインタフェースを使用して、より複雑なビュー、フィルタ、グループ化、およびリストとレポート内のカスタマイズされたプロンプトを作成できます。 テキストモードを使用すると、標準モードインターフェイスでは使用できないフィールドとその属性にアクセスできます。

テキストモードを開始する前に考慮する必要がある情報については、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

すべてのレポート可能なフィールドとその属性の完全なリストについては、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

クラス、ビデオ、チュートリアルなど、テキストモードを使用したレポートの作成について詳しくは、Adobe Experience Leagueサイトの「学習」セクションを参照してください。

## テキストモードの構文に関する考慮事項

* テキストモードでレポート要素の作成を開始する前に、Adobe Workfrontの構文を理解する必要があります。 テキストモードのWorkfront構文は、このアプリケーションに固有のもので、使い慣れた独自の特性を持ちます。
* レポートでテキストモードの使用を開始する前に、高度なレポート機能に関するクラスを受講して、テキストモードの言語をより深く理解することを強くお勧めします。 <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* 標準モードのインターフェイスを使用して、ビュー、フィルターおよびグループをカスタマイズできます。 ただし、カスタムプロンプトを作成するには、テキストモードを使用する必要があります。

## テキストモードでのレポート要素の作成に関する一般的なガイドライン

テキストモードでレポートまたはリスト要素を作成する際の一般的なガイドラインを次に示します。

* Workfrontデータベース内のオブジェクトや属性を参照する場合は、必ずキャメルケースを使用してください。
* Workfrontのオブジェクトの階層に注意してください。 ビュー、フィルターおよびグループには、次のような違いがあります。

   * レポートまたはリストオブジェクトから 3 つ離れたオブジェクトをビューに表示できます。
   * グループ化、フィルタ、またはカスタムプロンプトで、メインオブジェクトから 2 つ以上離れたオブジェクトを参照することはできません。

  **例：** タスクビューにPortfolio所有者の名前または GUID を表示できます。


  `valuefield=project:portfolio:ownerID`

  タスクビューでは、Portfolio所有者のグループ化、フィルタ、プロンプトの表示はできません。

  `project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa`


  次の例では、Portfolio所有者 ID は、リストのオブジェクトから離れた 3 つのオブジェクトです。

  Workfrontでのオブジェクトの階層について詳しくは、次を参照してください。

   * [Adobe Workfrontのオブジェクトについて](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API エクスプローラー](../../../wf-api/general/api-explorer.md)

* 可能な限り、ワイルドカードを使用してレポートやリストをより動的にし、異なるユーザーや同様のタイムラインに重複しないようにします。

## キャメルケースの概要

Workfrontフィールドまたはその属性をテキストモードで参照する場合、Workfrontでは、キャメルケースで名前を入力する必要があります。 この場合、単一名フィールドのスペルは小文字になります。 複合フィールドのスペルは、次のパターンに従います。

`camelCaseSyntax`

>[!IMPORTANT]
>
>すべてのレポート要素は、この大文字と小文字のパターンに従います。

キャメルケースの特徴は次のとおりです。

* 最初の単語は、常に小文字で始まります。
* 次の単語は、常に大文字で始まります。
* 単語の間にスペースはありません。

**例：** プロジェクトの実際の完了日を参照する場合、テキストモードのレポート要素の作成時に使用するフィールドの名前は次のようになります。

`actualCompletionDate`

## 様々なレポート要素のテキストモード構文

テキストモードを使用してレポート要素を作成する場合の、以下に示す一連のレポート要素の構文の間には、次のような類似点があります。

* ビューやグループ化では、コードと構文の行は似ています。

  テキストモードでビューとグループを作成する際のコードのキーラインについては、次を参照してください。

   * [テキストモードを使用したビューの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [グループ化でのテキストモードの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* コードと構文の行は、フィルターとカスタムプロンプトで似ています。

  詳しくは、以下を参照してください。

   * [テキストモードを使用したフィルターの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [レポートにプロンプトを追加する](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### ビューおよびグループの構文

ビューやグループを作成する際のコードの行は似ています。

ビューおよびグループの作成について詳しくは、次の記事を参照してください。

* [Adobe Workfrontの概要を表示](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfrontでのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

ビューまたはグループ化のコードの最も重要な行は、ビューの列またはグループ内で参照されているオブジェクトを識別する行です。 このコード行は、 `valuefield` または `valueexpression` このフィールドがWorkfrontデータベースフィールドへの直接参照か、複数のフィールド間の計算かに基づきます。

次の表に、ビューまたはグループ化で最も一般的なコード行を示します。

| コードライン | 説明 |
|-----------------|------------------------------------------------------------------------------------------------------------------------------|
| `valuefield` | ビューの列またはグループで参照されるオブジェクトを識別します。 これは、参照されるオブジェクトへの直接参照です。 |
| `valueexpression` | ビューの列またはグループで参照されるオブジェクトを識別します。 これは、複数のフィールド間の計算です。 |
| `valueformat` | 値フィールドまたは値式行で指定された値をWorkfrontが返す形式を識別します。 |
| `width` | 列の幅をピクセル単位で指定します。 |
| `stretch` | ビューで不要な領域を占める列を示します。 |

>[!TIP]
>
>* 以下の例のコード行は表示とグループの間で似ていますが、グループ化のコード行はすべてグループ番号で始まることに注意してください。
>
>  プロジェクトリストまたはレポートでプロジェクト名でグループ化するには、第 1 層グループに対して次の行を使用します。
>
>  `group.0.valuefield=name`
>  
>* ビュー内の複数の列を同じ列で編集する場合（共有列の場合と同様）、各列のコードの各行は列番号で始まることに注意してください。
>
>  ビューの最初の列を識別するには、次の形式を使用します。
>
>  `column.0.valuefield=name`
>  
>  列の共有について詳しくは、 [表示：1 つの共有列の複数の列から情報を結合](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).
>

#### `Valuefield` ビューとグループの構文の概要

`Valuefield=` は、ビューとグループの中で、直接参照するオブジェクトを識別するコードの重要な行です。

フィールドを直接参照する構文は、グループ化とビューで同じです。

次のルールは、 `valuefield` 行：

* フィールドを直接参照するには、キャメルケースを使用します。

  **例：** タスクビューでタスクの実績完了日を参照するには、次の行を使用します。

  `valuefield=actualCompletionDate`

* キャメルケースとコロンを使用して、同じオブジェクトに対して互いに関連するフィールドを区切ります。

  **例：** タスク・ビューでプロジェクト計画完了日を参照するには、次の行を使用します。

  `valuefield=project:plannedCompletionDate`

  Workfrontデータベース内でオブジェクトが相互に参照している方法について詳しくは、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

* カスタムフィールドを参照する場合は、インターフェイスに表示されるとおりに、フィールドの名前を使用します。

  **例：** タスクビューで Additional Details というラベルの付いたプロジェクトカスタムフィールドを参照するには、次の行を使用します。

  `valuefield=project:Additional Details`

#### `Valueexpression` ビューとグループの構文の概要

次を `valuefield=` 次のコード行： `valueexpression=` 2 つ以上のフィールド間の計算を参照する場合に、テキストモードでビューとグループを作成するとき。

>[!TIP]
>
>レポートに表示できる計算フィールドを作成できますが、計算ビューとグループ化はより動的です。 計算済みのビューとグループは、レポートを実行したりリストを表示したりするたびに、新しい情報で更新されます。
>
>ビューでの計算列の作成について詳しくは、 [計算カスタムフィールドと計算列の比較](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

計算されたグループを作成する方法は、ビューで計算された列を作成する方法と似ています。

次のルールは、 `valueexpression` 行：

* フィールドを直接参照し、各フィールドを中括弧で囲むには、キャメルケースを使用します。

  **例：** タスク列に [ タスク名 ] フィールドを表示するには、次のコマンドを使用します。 `valueexpression`、次の行を使用します。

  `valueexpression={name}`


* キャメルケースとピリオドを使用して、関連するフィールドを区切ります。

  **例：** タスクレポートで、タスク名と連結されたプロジェクト名を表示するには、次の行を使用します。

   * ビューでは、次のようになります。

     `valueexpression=CONCAT({project}.{name},' - ',{name})`

   * グループ内：

     `group.0.valueexpression=CONCAT({project}.{name},' - ',{name})`

  Workfrontデータベース内でオブジェクトが相互に参照している方法について詳しくは、 [API エクスプローラ](../../../wf-api/general/api-explorer.md).

* カスタムフィールドを参照する場合は、次のルールを使用します。

   * フィールドの名前は、インターフェイスに表示されるとおりに使用します。
   * フィールドの名前の前に「DE:」を付けます。
   * フィールドを中括弧で囲みます。
   * オブジェクトに関連するフィールドはピリオドで区切ります。

  **例：** 値式行のタスクビューに [ 追加の詳細プロジェクトのカスタムフィールド ] を表示するには、次の行を使用します。

  `valueexpression={project}.{DE:Additional Details}`

* ワイルドカードを `valueexpression` しかし、 `valuefield` 行。

  ワイルドカードについて詳しくは、 [ワイルドカードフィルター変数の概要](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).


#### `Valueformat` ビューとグループの概要

ビューまたはグループ化で 2 番目に重要なコード行は、 `valueformat=` 行。 これにより、Workfrontは、 `valuefield` または `valueexpression` 行。 ただし、 `valueformat` 行の数を指定する場合、 `valueexpression`:

`valueformat=HTML`

追加の `valueformat` の値については、次の記事も参照してください。

* [テキストモードのレポートで日付を書式設定する](../../reports/text-mode/format-dates-in-text-mode-reports.md)
* [テキストモードのレポートで数値、通貨、割合の値を書式設定します](../../reports/text-mode/format-numbers-in-text-mode-reports.md)

#### `width` ビューの概要

`width=` は、各列の幅をピクセル単位で指定できるコード行です。 Workfrontでは各フィールドに推奨される幅が提供されますが、フィールドの種類や形式に応じて異なりますが、調整を行うこともできます。

追加の `usewidths=true` 列に指定された幅を適用するコード行。

**例：** 幅が 80 ピクセルの列を表示するには、次の行を使用します。

`width=80`

`usewidths=true`

#### `stretch` ビューの概要

The `stretch` は、ビューで不要な領域を占める列を識別するために使用されます。 一般的なユーザーのワークスペースのユーザーインターフェイスの幅は、約 850 ピクセルです。 つまり、4 列（それぞれ 150 ピクセル）のビューがあり、そのビューが 850 ピクセルのうち 600 ピクセルを占有している場合です。 UI には、ストレッチの割合が指定された列に追加される、250 個の追加のピクセルがあります。

追加のコード行を使用する場合、列の拡張は適用されます。 `usewidths=true` ビュー内の列の少なくとも 1 つに対して

**例：** 列がビュー内の空白スペースの 70%を使用できることを示すには、次の行を使用します。

`stretch=70`

`usewidths=true`

### フィルターとカスタムプロンプトの構文

フィルタを作成する構文は、カスタムプロンプトを作成する構文と似ています。

>[!TIP]
>
>カスタムプロンプトを作成するには、最初にプロンプトに含める文のフィルタを作成します。 フィルター内のすべてのコード行を「&amp;」で接続し、行間にスペースを入れず、カスタムプロンプトになります。

フィルタとカスタムプロンプトの作成については、次を参照してください。

* [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [レポートにプロンプトを追加する](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

テキストモードでのフィルターの作成について詳しくは、 [テキストモードを使用したフィルターの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

次の要素を使用して、テキストモードでフィルタとカスタムプロンプトを作成できます。

* filter ステートメントのオブジェクトを参照するコードの行。 フィルターオブジェクトにキャメルケースを使用します。
* フィルターオブジェクトと、フィルターオブジェクトの値の修飾子を参照するコードの行。 この行のフィルターオブジェクトにキャメルケースを使用します。

  >[!TIP]
  >
  >範囲を参照する場合は、2 つの修飾子行が必要です。

* 複数のフィルターステートメントを接続するステートメントコネクタ：

   * および

     これは、フィルターステートメント間のデフォルトのコネクタです。

   * または

     >[!TIP]
     >
     >Statement Connectors では大文字と小文字が区別され、常に大文字が使用されます。 「AND」はテキストモードで省略できます。

* ワイルドカードを使用してフィルターをより動的にし、現在の時刻やログインしているユーザーに合わせてカスタマイズできます。 ワイルドカードについて詳しくは、 [ワイルドカードフィルター変数の概要](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
