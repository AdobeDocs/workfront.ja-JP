---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google Formsモジュール
description: この [!DNL Adobe Workfront Fusion Google Forms] モジュールを使用すると、Google Formsで応答を監視、選択、追加、更新または削除できます。
author: Becky
feature: Workfront Fusion
exl-id: 45c86879-bc4e-4134-b63c-02410b9de43b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 0%

---

# [!DNL Google Forms] モジュール

この [!DNL Adobe Workfront Fusion] [!DNL Google Forms] モジュールを使用すると、 [!DNL Google Forms].

を使用するには [!DNL Google Docs] と [!DNL Adobe Workfront Fusion]の場合、 [!DNL Google] アカウント 次の条件を満たさない場合、 [!DNL Google] アカウントはまだ、 [!DNL Google] アカウントヘルプページ。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL Google Forms] モジュールの場合、 [!DNL Google] アカウント

## フォームからスプレッドシートを作成する

フォームの回答を処理するには、回答のスプレッドシートを作成する必要があります。

1. フォームを開きます。
1. 次に移動： **[!UICONTROL 応答]** タブをクリックします。
1. 次をクリック： **[!UICONTROL スプレッドシートを作成]** アイコン ![](assets/spreadsheet-icon.png).

1. 新しいスプレッドシートを作成するか、既存のスプレッドシートを作成するかを選択します
1. 「**[!UICONTROL 作成]**」をクリックします。

## [!DNL Google Forms] モジュールとそのフィールド

設定時に [!DNL Google Forms] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Google Forms] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL 応答を見る]

新しい回答のフォームを視聴します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スプレッドシート ]</td> 
   <td> <p>新しい回答を確認するフォームの回答を含むスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シート ]</td> 
   <td> <p> 回答フォームを含むシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ヘッダー付き行 ]</td> 
   <td>テーブルのヘッダー行を指定します。 デフォルトの行は <code>A1:Z1</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 値レンダリングオプション ]</td> 
   <td> <p>出力で値をレンダリングする方法を指定します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 形式の値 ]</strong> </p> <p>値は、セルの書式設定に従って計算され、返信の形式設定が行われます。 書式設定は、要求元のユーザーのロケールではなく、スプレッドシートのロケールに基づいておこなわれます。 例えば、 <code>A1</code> が <code>1. 23</code> および <code>A2 </code>が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻り値 <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL 形式設定されていない値 ]</strong> </p> <p>値は計算されますが、返信の形式は設定されません。 例えば、 <code>A1</code> が <code>1. 23</code> および <code>A2 </code>が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 数値を返します <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL 数式 ]</strong> </p> <p>値は計算されません。 返信には数式が含まれます。 例えば、 <code>A1</code> が <code>1. 23</code> および <code>A2 </code>が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻り値 <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 日時レンダリングオプション ]</td> 
   <td>日付、時間および期間を出力に表示する方法を選択します。 [!UICONTROL Value Render Option] が [!UICONTROL Formatted Value] に設定されている場合、このフィールドは無視されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p> 応答の最大数を設定 [!DNL Workfront Fusion] は、1 回のサイクルでと連携します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL 応答を追加]](#add-a-response)
* [[!UICONTROL 応答の更新]](#update-a-response)
* [[!UICONTROL 応答の削除]](#delete-a-response)

#### [!UICONTROL 応答を追加]

このモジュールは、フォームのスプレッドシートの下部に新しい応答を追加します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スプレッドシート ]</td> 
   <td> <p>応答を追加するシートが含まれているスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シート ]</td> 
   <td> <p> 回答フォームを含むシートを選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL 値 ]</p> </td> 
   <td> <p>シート列に必要な値を入力します。</p> <p>正しい形式の [!UICONTROL Timestamp] 列には、次の値を使用してください。</p><pre>formatDate(now;DD/MM/YYYY HH:mm;UTC)</pre> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 値入力オプション ]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> ユーザーが入力した値は解析されず、そのまま保存されます。 </p> </li> 
     <li> <p><strong>[!UICONTROL ユーザーが入力 ]</strong></p> <p>値は、ユーザーが UI に入力したかのように解析されます。 数値は保持されますが、文字列は、 [!DNL Google Sheets] UI</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL データ挿入オプション ]</td> 
   <td> <p>新しいデータが入力されたときの既存のデータの変更方法を指定します。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 上書き ]</strong> </p> <p>新しいデータは、書き込まれた領域の既存のデータを上書きします。 シートの末尾にデータを追加すると、新しい行または列が挿入され、データを書き込むことができます。</p> </li> 
     <li> <p><strong>[!UICONTROL 行の挿入 ]</strong></p> <p>行が新しいデータ用に挿入されます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 応答の更新]

このモジュールは、選択された応答を更新します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スプレッドシート ]</td> 
   <td> <p>応答を更新するシートが含まれているスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シート ]</td> 
   <td> <p> 回答フォームを含むシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 行番号 ]</p> </td> 
   <td> <p>更新する行の番号を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 値 ]</p> </td> 
   <td> <p>目的の列に新しい値を入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 値入力オプション ]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> ユーザーが入力した値は解析されず、そのまま保存されます。 </p> </li> 
     <li> <p><strong>[!UICONTROL ユーザーが入力 ]</strong></p> <p>値は、ユーザーが UI に入力したかのように解析されます。 数値は保持されますが、文字列は、 [!DNL Google Sheets] UI</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 応答の削除]

このモジュールは、選択した応答を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スプレッドシート ]</td> 
   <td> <p>応答を削除するシートを含むスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シート ]</td> 
   <td> <p> 回答フォームを含むシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 行番号 ]</p> </td> 
   <td> <p>削除する行の番号を入力またはマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL 応答を検索]](#search-responses)
* [[!UICONTROL 検索応答（詳細）])](#search-responses-advanced)

#### [!UICONTROL 応答を検索]

このモジュールは、指定された条件に一致する応答を返します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
    <td>接続</td>
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL スプレッドシート ]</td>
   <td> <p>検索するフォームを選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL シート ] </td>
   <td> <p>回答フォームを含むシートを選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL 列の範囲 ]</td>
   <td> <p> 検索する列の範囲を選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td> <p>回答の検索に使用するフィルターを定義します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL 並べ替え順 ] </td>
   <td> <p>返された応答を昇順または降順で並べ替えるかどうかを選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Order By]</td>
   <td> <p> 返信応答を並べ替える列を選択します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 値レンダリングオプション ]</td> 
   <td> <p>出力で値をレンダリングする方法を指定します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 形式の値 ]</strong></p> <p>値は、セルの書式設定に従って計算され、返信の形式設定が行われます。 書式設定は、要求元のユーザーのロケールではなく、スプレッドシートのロケールに基づいておこなわれます。 例えば、 <code>A1</code> が <code>1. 23</code> および <code>A2 </code>が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻り値 <code>$1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL 形式設定されていない値 ]</strong> </p> <p>値は計算されますが、返信の形式は設定されません。 例えば、 <code>A1</code> が <code>1. 23</code> および <code>A2 </code>が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 数値を返します <code>1. 23</code> .</p> </li> 
     <li> <p><strong>[!UICONTROL 数式 ]</strong> </p> <p>値は計算されません。 返信には数式が含まれます。 例えば、 <code>A1</code> が <code>1. 23</code> および <code>A2 </code>が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻り値 <code>=A1</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL 日時レンダリングオプション ]</td>
    <td>日付、時間および期間を出力に表示する方法を選択します。 [!UICONTROL Value Render] オプションが「Formatted Value」に設定されている場合、このフィールドは無視されます。 </td>
  </tr> 
  <tr>
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL 返された応答の最大数 ]</td>
   <td> <p> 応答の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にを返します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 検索応答（詳細）]

このモジュールは、 [[!DNL Google Charts Query Language]](https://developers.google.com/chart/interactive/docs/querylanguage). このモジュールは行番号を返しません。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL 接続 ]</td>
   <td> <p>接続方法 [!DNL Google] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL スプレッドシート ]</td>
   <td> <p>検索するシートが含まれているスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL シート ]</td>
   <td> <p> 回答フォームを含むシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td> <p>を使用して検索クエリを定義 <a href="https://developers.google.com/chart/interactive/docs/querylanguage">[!DNL Google Charts Query Language]</a>.</p> <p>例： <code>select * where C = "John"</code> は、C 列が「John」である行のすべての値を取得します。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL 返される行の最大数 ]</td>
   <td> <p> 応答の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にを返します。</p> </td> 
  </tr> 
 </tbody> 
</table>
