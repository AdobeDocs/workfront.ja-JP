---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: テキストパーサー
description: テキストパーサーツールを使用すると、他の [!DNL Adobe Workfront Fusion] シナリオモジュールで使用できるようにテキストを解析できます。テキストパーサーには接続は必要ありません。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: ht
source-wordcount: '1044'
ht-degree: 100%

---

# [!UICONTROL テキストパーサー]

[!UICONTROL テキストパーサーツール]を使用すると、他の [!DNL Adobe Workfront Fusion] シナリオモジュールで使用できるようにテキストを解析できます。[!UICONTROL テキストパーサー]には接続は必要ありません。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion]ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL テキストパーサー]モジュールとそのフィールド

[!UICONTROL テキストパーサー]モジュールを設定すると、[!DNL Adobe Workfront Fusion] には、以下のフィールドが表示されます。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でのモジュール間の情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

### 変換サービス

* [[!UICONTROL HTML から要素を取得]](#get-elements-from-html)
* [[!UICONTROL テキストから要素を取得]](#get-elements-from-text)
* [[!UICONTROL HTML をテキストに変換]](#html-to-text)
* [[!UICONTROL パターンを照合]](#match-pattern)
* [[!UICONTROL 置き換え]](#replace)

#### [!UICONTROL HTML から要素を取得]

必要な要素を HTML コードから取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module finds no matches]</td> 
   <td> <p>結果が返されない場合にモジュールがシナリオを停止しないようにするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Element type]</td> 
   <td> <p> HTML コードから取得する要素のタイプを選択します。 </p> 
    <ul> 
     <li>[!UICONTROL Image]</li> 
     <li>[!UICONTROL Link]</li> 
     <li>[!UICONTROL iFrame element(s)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>指定した要素タイプを取得する HTML コードを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テキストから要素を取得]

指定されたパターンに基づいてテキストから要素を解析します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Input text]</td> 
   <td> <p>解析するテキストを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Pattern]</td> 
   <td> <p>テキストから解析する要素を反映するパターンを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ignore Duplicate Occurrences]</td> 
   <td> <p>テキスト要素の重複発生を無視する場合は、このチェックボックスをオンにします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTML からテキスト]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL HTML] </td> 
   <td> <p>プレーンテキストに変換する HTML コードを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Line break] </td> 
   <td> <p>新規行（改行）のタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Uppercase headings]</p> </td> 
   <td> <p>見出しタグ（&lt;h2&gt; &lt;/h2&gt; など）で囲まれたテキストを大文字テキストに変換する場合は、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 一致パターン]

[!UICONTROL 一致パターン]モジュールを使用すると、指定したテキストから検索パターンに一致する文字列要素を検索して抽出できます。このモジュールは正規表現（regex または regexp と表記される場合もあります）を使用します。

正規表現とは、各文字が特別な意味を持つメタ文字、またはリテラルの意味を持つ正規文字のいずれかである文字のシーケンスです。これらの文字とメタ文字は、テキストの検索に使用できるパターンを識別します。例えば、名前を検索する場合、大文字で始まる 2 つの連続した単語で構成されるパターンを検索する正規表現を設定できます。正規表現は、テキストを検索および操作するための強力なツールです。

正規表現についての詳しい説明は、この記事の範囲外です。次のリソースをお勧めします。

* メタ文字の完全なリストについては、MDN web ドキュメントの[正規表現](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions)を参照してください。
* 正規表現の作成方法を説明するチュートリアルについては、[RegexOne](https://regexone.com/) をお勧めします。
* 正規表現を試したい方には、[正規表現 101](https://regex101.com/) web サイトをお勧めします。左パネルで ECMAScript（JavaScript）FLAVOR を選択します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>正規表現のパターンを入力します。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例：</b></span></span><code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> で指定されたテキスト内のすべての数字を抽出します。</p> <p>メモ：  <p>パターンでは、少なくとも 1 つのキャプチャグループが括弧内に含まれている必要があります<code>()</code>。パターンにキャプチャグループが含まれていない場合、出力バンドルは空になります。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>テキスト内のすべての一致を取得するには、このオプションを有効にします。一致はそれぞれ、個別のバンドルに出力されます。このオプションが無効になっている場合、モジュールは最初のエントリのみを取得します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> このモジュールでテキストの大文字と小文字を区別して扱うには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>このオプションを有効にすると、開始メタ文字と終了メタ文字（<code>^</code> および <code>$</code>）が、入力文字列全体の先頭または末尾だけでなく、各行の先頭または末尾と一致するようになります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>ピリオド（.）が改行文字（<code>\n</code>）と一致するようにするには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p>結果が返されない場合にモジュールがシナリオを停止しないようにするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>パターンと一致させるテキストを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 置き換え]

指定した値または正規表現について入力したテキストを検索し、結果を新しい値に置き換えます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Pattern] </td> 
   <td> <p>検索語句を入力します。また、正規表現を使用することもできます。正規表現について詳しくは、<a href="#match-pattern" class="MCXref xref">[!UICONTROL Match Pattern]</a> モジュールを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New value]</td> 
   <td> <p> 検索語句を置き換える値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Global match]</td> 
   <td> <p>テキスト内のすべての一致を取得するには、このオプションを有効にします。一致はそれぞれ、個別のバンドルに出力されます。このオプションが無効になっている場合、モジュールは最初のエントリのみを取得します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Case sensitive]</td> 
   <td> <p> このモジュールでテキストの大文字と小文字を区別して扱うには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Multiline] </td> 
   <td> <p>このオプションを有効にすると、開始メタ文字と終了メタ文字（<code>^</code> および <code>$</code>）が、入力文字列全体の先頭または末尾だけでなく、各行の先頭または末尾と一致するようになります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Singleline]</td> 
   <td>ピリオド（.）が改行文字（<code>\n</code>）に一致します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text] </td> 
   <td> <p>検索するテキストを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### データスクレーピング

データスクレーピング（web スクレーピング、データ抽出、web 収集とも呼ばれます）とは、web サイトからデータを収集し、ローカルのデータベースまたはスプレッドシートに保存するプロセスです。Web サイトからデータを削除する場合で、かつ正規表現に慣れていない場合は、データスクレーピングツールを使用できます。

データスクレーピングツールが REST API を提供している場合は、ユニバーサル [[!UICONTROL HTTP] モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md)および [Web フック](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)モジュールを通じて接続できます。
