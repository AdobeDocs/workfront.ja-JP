---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: テキストパーサー
description: テキストパーサーツールを使用して、他のユーザーで使用するテキストを解析できます [!DNL Adobe Workfront Fusion] シナリオモジュール。 テキストパーサーに接続は必要ありません。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d71cf64-4f86-42c5-81e7-8fc15333cbd7
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# [!UICONTROL テキストパーサー]

以下を使用して、 [!UICONTROL テキストパーサーツール] テキストを他で使用するために解析する [!DNL Adobe Workfront Fusion] シナリオモジュール。 この [!UICONTROL テキストパーサー] は接続を必要としません。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> <p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL テキストパーサー] モジュールとそのフィールド

設定時に [!UICONTROL テキストパーサー] モジュール [!DNL Adobe Workfront Fusion] 以下のフィールドが表示されます。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 変換サービス

* [[!UICONTROL 「Get Elements from」HTML]](#get-elements-from-html)
* [[!UICONTROL テキストから要素を取得]](#get-elements-from-text)
* [[!UICONTROL HTMLからテキスト]](#html-to-text)
* [[!UICONTROL 一致パターン]](#match-pattern)
* [[!UICONTROL 置き換え]](#replace)

#### [!UICONTROL 「Get Elements from」HTML]

必要な要素をHTMLコードから取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL モジュールで一致が見つからない場合でも、ルートの実行を続行します ]</td> 
   <td> <p>結果が返されない場合にモジュールがシナリオを停止しないようにするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 要素タイプ ]</td> 
   <td> <p> 要素コードから取得する要素のタイプをHTMLします。 </p> 
    <ul> 
     <li>[!UICONTROL 画像 ]</li> 
     <li>[!UICONTROL リンク ]</li> 
     <li>[!UICONTROL iFrame 要素 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROLHTML] </td> 
   <td> <p>指定したHTMLタイプを取得する要素コードを入力またはマッピングします。</p> </td> 
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
   <td>[!UICONTROL テキストを入力 ]</td> 
   <td> <p>解析するテキストを入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL パターン ]</td> 
   <td> <p>テキストから解析する要素を反映するパターンを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 重複する発生件数を無視 ]</td> 
   <td> <p>テキスト要素の重複部分を無視する場合は、このチェックボックスをオンにします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL HTMLからテキスト]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROLHTML] </td> 
   <td> <p>プレーンHTMLに変換するテキストコードを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 改行 ] </td> 
   <td> <p>改行のタイプ（改行）を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 大文字の見出し ]</p> </td> 
   <td> <p>見出しタグで囲まれたテキストを変換する場合は、このオプションを有効にします ( 例： &lt;h2&gt; &lt;/h2&gt;) を大文字に変換します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 一致パターン]

この [!UICONTROL 一致パターン] モジュールを使用すると、指定したテキストから検索パターンに一致する文字列要素を検索および抽出できます。 このモジュールは、正規表現（正規表現または正規表現とも呼ばれます）を使用します。

正規表現とは、各文字がメタ文字で、特殊な意味を持つ文字、またはリテラル意味を持つ正規文字のシーケンスです。 これらの文字とメタ文字は、テキストの検索に使用できるパターンを識別します。 例えば、名前を検索する場合、大文字で始まる 2 つの連続する単語で構成されるパターンを検索する正規表現を設定できます。 正規表現は、テキストを検索および操作するための強力なツールです。

正規表現の議論は、この記事の範囲外です。 次のリソースをお勧めします。

* メタ文字の完全なリストについては、 [正規表現](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions) MDN web ドキュメントの。
* 正規表現の作成方法に関するチュートリアルについては、 [RegexOne](https://regexone.com/).
* 正規表現を試す場合は、 [正規表現 101](https://regex101.com/) web サイト。 左側のパネルで ECMAScript (JavaScript) FLAVOR を選択します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL パターン ] </td> 
   <td> <p>正規表現のパターンを入力します。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span> <code>[+-]?(\d+(\.\d+)?|\.\d+)([eE][+-]?\d+)?</code> 指定されたテキスト内のすべての数字を抽出します。</p> <p>メモ:  <p>パターンには、少なくとも 1 つのキャプチャグループが括弧で囲まれている必要があります <code>()</code>. パターンにキャプチャグループが含まれていない場合、出力バンドルは空になります。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL グローバル一致 ]</td> 
   <td> <p>テキスト内のすべての一致を取得するには、このオプションを有効にします。 それぞれの一致は、別々のバンドルに出力されます。 このオプションが無効な場合、モジュールは最初のエントリのみを取得します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 大文字と小文字を区別 ]</td> 
   <td> <p> このモジュールで、テキストの大文字と小文字が区別されるようにこのオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 複数行 </td> 
   <td> <p>このオプションを有効にして、開始および終了のメタ文字 (<code>^</code> および <code>$</code>) は、入力文字列全体の先頭または末尾だけでなく、各行の先頭または末尾に一致します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シングルライン ]</td> 
   <td>このオプションを有効にして、必ずピリオド (.) 改行文字 (<code>\n</code>) をクリックします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL モジュールが結果を返さない場合でも、ルートの実行を続行します ]</td> 
   <td> <p>結果が返されない場合にモジュールがシナリオを停止しないようにするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL テキスト ] </td> 
   <td> <p>パターンに合わせるテキストを入力またはマッピングします。</p> </td> 
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
   <td>[!UICONTROL パターン ] </td> 
   <td> <p>検索語句を入力します。 また、正規表現を使用することもできます。 正規表現について詳しくは、 <a href="#match-pattern" class="MCXref xref">[!UICONTROL 一致パターン ]</a> モジュール。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 新しい値 ]</td> 
   <td> <p> 検索語句を置き換える値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL グローバル一致 ]</td> 
   <td> <p>テキスト内のすべての一致を取得するには、このオプションを有効にします。 それぞれの一致は、別々のバンドルに出力されます。 このオプションが無効な場合、モジュールは最初のエントリのみを取得します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 大文字と小文字を区別 ]</td> 
   <td> <p> このモジュールで、テキストの大文字と小文字が区別されるようにこのオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 複数行 </td> 
   <td> <p>このオプションを有効にして、開始および終了のメタ文字 (<code>^</code> および <code>$</code>) は、入力文字列全体の先頭または末尾だけでなく、各行の先頭または末尾に一致します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シングルライン ]</td> 
   <td>このオプションを有効にして、必ずピリオド (.) 改行文字 (<code>\n</code>) をクリックします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL テキスト ] </td> 
   <td> <p>検索するテキストを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### データスクレーピング

データスクレーピング（Web スクレーピング、データ抽出、Web 収集とも呼ばれます）とは、Web サイトからデータを収集し、ローカルのデータベースまたはスプレッドシートに保存するプロセスです。 Web サイトからデータを削除し、正規表現に慣れていない場合は、次のようなデータ削除ツールを使用できます。

* [指定](https://apify.com/)
* [2019 年の Best Data Scraping Tools](https://www.octoparse.com/blog/best-data-scraping-tools-for-2019-top-10-reviews)

データスクレーピングツールが REST API を提供している場合は、ユニバーサルアドビのユニバーサルアプリケーションを通じて接続できます [[!UICONTROL HTTP] モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md) および [ウェブフック](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md) モジュール。
