---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: ' [!DNL Adobe Workfront Fusion] で、あるモジュールから別のモジュールに情報をマッピングします。'
description: マッピングとは、項目に構造化されたモジュールの出力を、別のモジュールの入力フィールドに割り当てるプロセスです。
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 3772223938008e3a54ce0a48aaae1f3edb5bf252
workflow-type: ht
source-wordcount: '1567'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] で、あるモジュールから別のモジュールに情報をマッピングします。

マッピングとは、項目に構造化されたモジュールの出力を、別のモジュールの入力フィールドに割り当てるプロセスです。

マッピングパネルは、シナリオで前のモジュールから出力された値を挿入するフィールドをクリックすると表示されます。モジュール内では、マッピングに使用できる任意のフィールドで、入力した静的テキストを含むマッピングパネルから、任意の関数とマッピングされた項目の組み合わせを使用して数式を作成できます。これらの要素は、互いに内部にネストできます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## バンドルと項目

モジュールの操作により、その出力として 0 個、1 個または複数のバンドルが生成されます。バンドルは、1 つ以上の項目で構成されます。

モジュールの出力を調べるには、次の操作を実行します。

1. 「**[!UICONTROL 1 回実行]**」をクリックして、モジュールを実行します。
1. モジュールの上のバブルをクリックします。

   モジュールのすべてのフェーズを含むログが表示されます。モジュールの操作フェーズで出力されるバンドルまたは複数のバンドルは、**[!UICONTROL 出力]**&#x200B;の見出しの下にあります。各バンドルには、項目と各項目の値が含まれます。

>[!INFO]
>
>**例：**&#x200B;この例では、モジュール[!UICONTROL メール]／[!UICONTROL メールを監視]を示します。1 回の操作を実行し、`Date`、`Email ID (UID)`、`size` などの様々な項目を含む単一のバンドルを生成したことがわかります。
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>[!UICONTROL イテレータ]および[!UICONTROL アグリゲータ]間でラップされたモジュールの出力は、[!UICONTROL アグリゲータ]モジュールから先にはアクセスできません。

## 項目のマッピング

2 つ以上のモジュールをリンクして一連のモジュールを作成した後、各モジュールは、それより前のモジュールが出力する項目の値を処理できます。

モジュールの入力フィールドに項目を割り当てるには、次の操作を実行します。

1. 前のモジュールまたはモジュールの出力を処理するモジュールをクリックします。
1. 表示されるモジュール設定パネルで、前のモジュールから出力された項目の値を使用するフィールドをクリックします。

   マッピングパネルが開きます。

1. マッピングパネルから項目をクリックして、フィールドに挿入します。
1. （オプション）マッピングパネルで特定のフィールドを検索するには、マッピングパネルの検索バーをクリックし、検索する語句を入力します。リストに表示されるフィールドをクリックします。

   検索結果には検索語が含まれ、大文字と小文字は区別されません。

詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md) でのモジュールの設定を参照してください。

## 数式

複数の項目を 1 つのフィールドにマッピングし、リテラル（固定値）と組み合わせ、演算子と関数を使用して複雑な数式を作成できます。

![](assets/operators-and-functions.png)

関数と演算子は、そのタブの 1 つの下のマッピングパネルにあります。

![](assets/functions-toolbar-350x189.png)

（パネルを開く際に表示される）最初のタブ ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) は、他のモジュールからマッピングできる項目を表示します。

その他のタブには、次のような関数が含まれます。

* **一般的な関数** ![](assets/toolbar-icon-general-function.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) の一般的な機能を参照してください。

* **数式** ![](assets/toolbar-icon-math-functions.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) の数式を参照してください。

* **テキスト関数とバイナリ関数** ![](assets/toolbar-icon-text&binary-functions.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) の文字列関数を参照してください。

* **日付と時間** ![](assets/toolbar-icon-date&time-functions.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) の日付と時間の関数および次の記事を参照してください。

   * [ [!DNL Adobe Workfront Fusion] の日付と時刻の書式設定のトークン](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Adobe Workfront Fusion の日付と時間の解析用トークン](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **配列操作の関数** ![](assets/toolbar-icon-functions-for-arrays.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) の配列関数を参照してください。

>[!TIP]
>
>別のフィールドで再利用する複雑な数式を作成する場合は、その組み合わせを含むフィールドをクリックし、Command + A キーまたは Ctrl + A キーで選択し、コピーして他のフィールドに貼り付けます。

関数を使った項目のマッピングについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) で関数を使用して項目をマッピングするを参照してください。

## コレクション

一部の項目には、様々なタイプの複数の値を含めることができます。コレクションタイプの項目です。

[!UICONTROL コレクション]タイプの項目は、項目のラベルと自動的に展開されるサブ項目のリストの右側に表示される小さな黒い長方形で識別できます。

![](assets/collection.png)

>[!NOTE]
>
>ほとんどの場合、コレクション全体を表す項目ではなく、コレクションのサブ項目をマッピングします。

コレクションについて詳しくは、[[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md) の項目データタイプを参照してください。

## 配列

一部の項目には、同じタイプの複数の要素を含めることができます。これらは配列タイプの項目です。

配列タイプの項目は、項目のラベルの最後にある角括弧で識別できます。項目のラベルの右にある小さな黒い長方形をクリックすると、その要素の項目が表示されます。

![](assets/array.png)

配列について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md) の項目データタイプを参照してください。

### 配列の最初の要素をマッピングする

配列の `Recipient name` の項目を選択すると、次のようにフィールドに表示されます。

![](assets/map-array-1st-element.png)

角括弧内の数値は、配列のどの要素を使用するかを決定するインデックスです。デフォルトでは 1 に設定されています。

### 配列の n 番目の要素をマッピングする

別の要素にアクセスする場合は、角括弧をクリックし、インデックス値を編集します。

![](assets/access-another-element.png)

### 指定されたキーで配列の要素をマッピングする

一部の配列には、キーと値の項目を持つ複数のコレクションが含まれています。これらは通常、様々なメタデータや属性などです。

次の例は、[!DNL Jira] アプリの出力を示しています。

![](assets/output-of-jira-app-350x100.png)

この例では、ID が 10108 の特定の添付ファイルについて、添付ファイルの配列からファイル名を取得しています。

[!DNL Jira] の出力は、次のようになります。

![](assets/output-from-jira-350x261.png)

一般的な要件は、指定されたキー値で要素を検索し、値項目から対応する値を取得することです。これは、`map()` および `get()` の関数の組み合わせにより、達成できます。

次に、数式について詳細な分類を示します。

1. `map()` の最初のパラメーター関数は配列の項目全体です。
1. 2 つ目のパラメーターは、値の項目の未加工の名前です。未加工の名前を取得するには、[!UICONTROL マッピング]パネルの項目にポインタを合わせます。

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >すべてのパラメーターでは大文字と小文字が区別されます。この特定の例では、項目のラベルと未加工の名前は大文字と小文字しか違いがありませんが、ラベルの値とは異なり、すべて小文字の値である未加工の名前を使う必要があります。

1. 3 番目のパラメーターは、キー項目の未加工の名前です。

   ![](assets/3rd-parameter-350x166.png)

1. 4 番目のパラメーターは、指定されたキー値です。

`map()` 関数は配列を返すので（指定されたキー値を持つ他の要素が存在する可能性があるため）、その最初の要素を取得するために `get()` 関数を適用する必要があります。

* `get()` 関数の最初のパラメーターは `map()` 関数の結果です。

* 2 番目のパラメーターは、要素のインデックスで、1 です。

`map()` 関数について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) の配列関数を参照してください。

`get()` 関数について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) の一般的な関数を参照してください。

## 要素を一連のバンドルに変換する

配列は[!UICONTROL イテレータ]モジュールを使用して、一連のバンドルに変換することができます。詳しくは、[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) の[[!UICONTROL イテレータ]モジュールを参照してください。

![](assets/series-of-bundles-350x169.png)

## トラブルシューティング

### マッピングパネルに項目がありません

マッピングパネルには、モジュールごとに、モジュールの作成者が一覧表示するすべての出力項目が表示されます。場合によっては、このリストが様々な理由で未完了になったり、一部の項目が欠落していることがあります。[!DNL Workfront Fusion] では、シナリオエディターでモジュールを実行する際に、不足している出力項目を自動検出できます。正確な手順は、モジュールのタイプによって少し異なります。

#### インスタントトリガー

1. モジュールを右クリックし、表示されるメニューで「**[!UICONTROL このモジュールのみを実行]**」をクリックします。

   キュー内の web フックがない場合、モジュールは新しい web フックが処理されるまで待機します。

1. Web フックを生成します。

   例えば、web フックモジュール **[!DNL Slack]／[!UICONTROL 新しいイベントをリッスンする]**（チャネル内の新しいチャネルメッセージを監視します）は、チャネルにメッセージを送信します。

1. モジュールの実行が終了したら、モジュールの上のバブルをクリックして、その出力全体を確認します。

   マッピングパネルには、モジュールの出力で検出されたすべての項目が含まれます。

#### ポーリングトリガー

1. モジュールを右クリックし、表示されるメニューで「**[!UICONTROL このモジュールのみを実行]**」をクリックします。
1. 出力がない場合は、「**[!UICONTROL 開始場所を選択]**」をクリックして設定を調整します。
1. 処理するイベントがない場合は、イベントを作成し、手順 2 に戻ります。

   例えば、web フックモジュール **[!UICONTROL Gmail]／[!UICONTROL メールを監視]**&#x200B;は、モジュールが監視しているフォルダーにメールを送信します。

1. モジュールの実行が終了したら、モジュールの上のバブルをクリックして、その出力全体を確認します。

   マッピングパネルには、モジュールの出力で検出されたすべての項目が含まれるようになりました。

#### その他のモジュール

以下を実行することもできます。

* シナリオ全体（またはモジュールを含む部分のみ）

  シナリオがトリガーで始まる場合は、上記の「[インスタントトリガー](#instant-trigger)」または「[ポーリングトリガー](#polling-trigger)」の節を参照してください。

* 単一のモジュールのみ

単一のモジュールのみを実行する場合：

1. モジュールを右クリックし、表示されるメニューで「**[!UICONTROL このモジュールのみを実行]**」をクリックします。
1. 入力項目のサンプル値を指定し、「**[!UICONTROL OK]**」をクリックします。
1. モジュールの実行が終了したら、モジュールの上のバブルをクリックして、その出力全体を確認します。

   マッピングパネルには、モジュールの出力で検出されたすべての項目が含まれるようになりました。
