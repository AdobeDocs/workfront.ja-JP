---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google Sheets モジュール
description: を使用するには [!DNL Google Sheets] と [!DNL Adobe Workfront Fusion],you need the [!UICONTROL Workfront Fusion Google Sheets] 拡張機能 ( オプション。ただし、インスタントトリガーに必要 )。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 11d62222-df34-472d-93d7-f0d53eb95c9b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '3894'
ht-degree: 0%

---

# [!DNL Google Sheets] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Google Sheets]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 [への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

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

使用する [!UICONTROL Google Sheets] モジュールの場合、 [!UICONTROL Google] アカウント

## トリガー

### [!UICONTROL 監視行]

スプレッドシートに新しく追加されたすべての行から値を取得します。

このモジュールは、以前に入力されたことのない新しい行のみを取得します。 このトリガーは、上書きされた行を処理しません。

>[!IMPORTANT]
>
>ワークシートに空白の行が含まれている場合、空白の行の後の行は処理されません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スプレッドシート ] </td> 
   <td> <p>監視するシートが含まれているスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シート ] </td> 
   <td> <p>新しい行を監視するシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL テーブルにヘッダーが含まれています ]</td> 
   <td> <p> スプレッドシートにヘッダー行を含めるかどうかを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL はい ]</strong> </p> <p>モジュールは、出力データとしてヘッダー行を取得しません。 </p> <p>出力内の変数名は、ヘッダーによって呼び出されます。</p> </li> 
     <li> <p><strong>[!UICONTROL いいえ ]</strong> </p> <p>また、このモジュールは、最初のテーブル行を取得します</p> <p>出力内の変数名は、A、B、C、D などと呼ばれます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ヘッダー付き行 ] </td> 
   <td> <p>ヘッダー行の範囲を入力します。 例： <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 最初のテーブル行 ]</td> 
   <td> <p>テーブルの最初の行の範囲を入力します。 例： <code>A1:F1</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 値レンダリングオプション ]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL 形式の値 ]</p> <p>値は、セルの書式設定に従って計算され、返信の形式設定されます。 書式設定は、要求元のユーザーのロケールではなく、スプレッドシートのロケールに基づいておこなわれます。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻る <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL 形式設定されていない値 ]</p> <p>値は計算されますが、返信の形式は設定されません。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> は数値を返します <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL 数式 ]</p> <p>値は計算されません。 返信には数式が含まれます。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻る <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 日時レンダリングオプション ]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL シリアル番号 ]</p> <p>日付、時刻、日時、期間の各フィールドを、Lotus 1-2-3によって一般化された「シリアル番号」形式で倍精度に出力するように指示します。 値の整数部分（小数の左側）は、1899 年 12 月 30 日からの日数を数えます。 小数部分（小数の右側）は、時間を日の端数としてカウントします。 例えば、1900 年 1 月 1 日の正午は、1899 年 12 月 30 日の 2 日後なので 2.5、1999 年 12 月 30 日の半日後なので 0.5 となります。 1900 年 2 月 1 日の午後 3 時には 33.625 となります。これにより、1900 年を閏年ではないとして正しく処理します。</p> <p style="font-weight: bold;">[!UICONTROL 形式の文字列 ]</p> <p>日付、時間、日時、期間の各フィールドを指定された数値形式（スプレッドシートのロケールに依存）で文字列として出力するように指示します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>結果の最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルでと連携します。</p> </td> 
  </tr> 
 </tbody> 
</table>

## アクション

* [[!UICONTROL 行を追加]](#add-a-row)
* [[!UICONTROL 行の更新]](#update-a-row)
* [[!UICONTROL 行をクリア]](#clear-a-row)
* [[!UICONTROL 行の削除]](#delete-a-row)
* [[!UICONTROL セルの取得]](#get-a-cell)
* [[!UICONTROL セルの更新]](#update-a-cell)
* [[!UICONTROL セルをクリア]](#clear-a-cell)
* [[!UICONTROL シートを追加]](#add-a-sheet)
* [[!UICONTROL スプレッドシートの作成]](#create-a-spreadsheet)
* [[!UICONTROL シートを削除する]](#delete-a-sheet)
* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)

### [!UICONTROL 行を追加]

このモジュールは、シートに行を追加します。

設定時に [!DNL Google Sheets] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Google Sheets] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL モード ]</td> 
   <td> <p>スプレッドシートとシートを手動で選択するか、マッピングを行うかを選択します。</p> <p>注意：手動マッピングは、例えば、 [!DNL Workfront Fusion] シナリオに追加し、新しく作成したスプレッドシートにデータを直接追加する場合は、このシナリオを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] スプレッドシート。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>行を追加するシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 列の範囲 ]</td> 
   <td>使用する列の範囲を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL テーブルにヘッダーが含まれています ]</td> 
   <td> <p> スプレッドシートにヘッダー行を含めるかどうかを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL はい ]</strong> </p> <p>モジュールは、出力データとしてヘッダー行を取得しません。 </p> <p>出力内の変数名は、ヘッダーによって呼び出されます。</p> </li> 
     <li> <p><strong>[!UICONTROL いいえ ]</strong> </p> <p>また、このモジュールは、最初のテーブル行を取得します</p> <p>出力内の変数名は、A、B、C、D などと呼ばれます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値 ] </td> 
   <td> <p>追加する行の目的のセルを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値入力オプション ]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL ユーザーが入力 ]</strong></p> <p>値は、ユーザーが UI に入力したかのように解析されます。 数値は保持されますが、文字列は、 [!DNL Google Sheets] UI</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> ユーザーが入力した値は解析されず、そのまま保存されます。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL データ挿入オプション ]</td> 
   <td> <p>新しいデータが入力されたときの既存のデータの変更方法を指定します。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 行の挿入 ]</strong></p> <p>行が新しいデータ用に挿入されます。</p> </li> 
     <li> <p><strong>[!UICONTROL 上書き ]</strong> </p> <p>新しいデータは、書き込まれた領域の既存のデータを上書きします。 シートの末尾にデータを追加すると、新しい行または列が挿入され、データを書き込むことができます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 行の更新]

このモジュールでは、選択した行のセルの内容を変更できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL モード ]</td> 
   <td> <p>スプレッドシートとシートを手動で選択するか、マッピングを行うかを選択します。</p> <p>注意：手動マッピングは、[!UICONTROL Workfront Fusion] シナリオで新しいスプレッドシートが作成され、新しく作成されたスプレッドシートにデータをシナリオで直接追加する場合などに便利です。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] スプレッドシート。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>行を更新するシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 行番号 ]</td> 
   <td> <p> 更新する行の数を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL テーブルにヘッダーが含まれています ]</td> 
   <td> <p> スプレッドシートにヘッダー行を含めるかどうかを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL はい ]</strong> </p> <p>モジュールは、出力データとしてヘッダー行を取得しません。 </p> <p>出力内の変数名は、ヘッダーによって呼び出されます。</p> </li> 
     <li> <p><strong>[!UICONTROL いいえ ]</strong> </p> <p>また、このモジュールは、最初のテーブル行を取得します</p> <p>出力内の変数名は、A、B、C、D などと呼ばれます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値 ] </td> 
   <td> <p>変更（更新）する行の目的のセルに値を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値入力オプション ]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL ユーザーが入力 ]</strong></p> <p>値は、ユーザーが UI に入力したかのように解析されます。 数値は保持されますが、文字列は、 [!DNL Google Sheets] UI</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> ユーザーが入力した値は解析されず、そのまま保存されます。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 行をクリア]

指定した行から値を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] 行を消去するシートを含むスプレッドシート。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p> データを消去するシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 行番号 ]</td> 
   <td> <p>データを消去する行の数を入力します。 例： <code> 23</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 行の削除]

指定した行を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>行を削除するシートが含まれているGoogleスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>スプレッドシート </td> 
   <td> <p>行を削除するシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>行番号</td> 
   <td> <p>削除する行の数を入力します。 例: <code>23</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL セルの取得]

選択したセルから値を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] スプレッドシート。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>データを取得するセルを含むシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL セル ] </td> 
   <td> <p>データの取得元のセルの ID を入力します。 例: <code>A6</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値レンダリングオプション ]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL 形式の値 ]</p> <p>値は、セルの書式設定に従って計算され、返信の形式設定されます。 書式設定は、要求元のユーザーのロケールではなく、スプレッドシートのロケールに基づいておこなわれます。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻る <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Unformatted value]</p> <p>値は計算されますが、返信の形式は設定されません。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> は数値を返します <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!DNL Formula]</p> <p>値は計算されません。 返信には数式が含まれます。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻る <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Date and time render option]</td> 
   <td> <p style="font-weight: bold;">[!DNL Serial number]</p> <p>日付、時刻、日時、期間の各フィールドを、Lotus 1-2-3によって一般化された「シリアル番号」形式で倍精度に出力するように指示します。 値の整数部分（小数の左側）は、1899 年 12 月 30 日からの日数を数えます。 小数部分（小数の右側）は、時間を日の端数としてカウントします。 例えば、1900 年 1 月 1 日の正午は、1899 年 12 月 30 日の 2 日後なので 2.5、1999 年 12 月 30 日の半日後なので 0.5 となります。 1900 年 2 月 1 日の午後 3 時には 33.625 となります。これにより、1900 年を閏年ではないとして正しく処理します。</p> <p style="font-weight: bold;">[!DNL Formatted string]</p> <p>日付、時間、日時、期間の各フィールドを指定された数値形式（スプレッドシートのロケールに依存）で文字列として出力するように指示します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL セルの更新]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] スプレッドシート。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL セル ] </td> 
   <td> <p>更新するセルの ID を入力します。 例: <code>A5</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値 ]</td> 
   <td> <p>セルの新しい値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値入力オプション ]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL ユーザーが入力 ]</strong></p> <p>値は、ユーザーが UI に入力したかのように解析されます。 数値は保持されますが、文字列は、 [!DNL Google Sheets] UI</p> </li> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p> ユーザーが入力した値は解析されず、そのまま保存されます。 </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL セルをクリア]

指定したセルから値を削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>セルを消去するシートが含まれているGoogleスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>セルを消去するシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL セル ] </td> 
   <td> <p>消去するセルの ID を入力します。 例: <code>A5</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL シートを追加]

選択したスプレッドシートに新しいシートを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>シートを追加するGoogleスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL プロパティ ]</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">[!UICONTROL タイトル ]</p> <p>新しいシートの名前を入力します。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL インデックス ]</p> <p>シートの位置を入力します。 既定値は 0 （シートを最初の場所に配置）です</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL スプレッドシートの作成]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイトル ] </td> 
   <td> <p>新しいスプレッドシートの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ロケール ]</td> 
   <td> <p>スプレッドシートのロケールを次のいずれかの形式で入力します。</p> 
    <ul> 
     <li>ISO 639-1 言語コード ( 例： <code>en</code></li> 
     <li>ISO 639-2 言語コード ( 例： <code>haw</code>（639-1 コードが存在しない場合）</li> 
     <li>ISO 言語コードと国コードの組み合わせ（例： ） <code>en_US</code></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 再計算間隔 ]</td> 
   <td> <p>揮発性関数が再計算されるまでの待機時間：</p> <p style="font-weight: bold;">[!UICONTROL 変更時 ]</p> <p>揮発性関数は、変更のたびに更新されます。</p> <p style="font-weight: bold;">[!UICONTROL 変更時刻と変更時刻（毎分）]</p> <p>揮発性関数は、変化のたびに毎分更新されます。</p> <p style="font-weight: bold;">[!UICONTROL 変更時間と時間単位 ]</p> <p>揮発性関数は、変更のたびに 1 時間ごとに更新されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイムゾーン ]</td> 
   <td> <p> スプレッドシートのタイムゾーンを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 数値の形式 ]</td> 
   <td> <p>スプレッドシート内のすべてのセルのデフォルトの形式を選択します。</p> <p><strong>[!UICONTROL テキスト ]</strong>:テキストの書式設定。 例: <code>1000. 12</code></p> <p><strong>[!UICONTROL 数値 ]</strong>:数値の書式設定。 例: <code>1,000.12</code></p> <p><strong>[!UICONTROL Percent]</strong>:割合の書式設定。 例: <code>10. 12%</code></p> <p><strong>[!UICONTROL 通貨 ]</strong>:通貨の書式設定。 例: <code>$1,000.12</code></p> <p><strong>[!UICONTROL 日付 ]</strong>:日付の書式設定。 例: <code>9/26/2008</code></p> <p><strong>[!UICONTROL 時間 ]</strong>:時間の形式設定。 例: <code>3:59:00 PM</code></p> <p><strong>[!UICONTROL 日時 ]</strong>:日付と時刻の形式。 例: <code>9/26/08 15:59:00</code> </p> <p><strong>[!UICONTROL 科学的方法 ]</strong>指数の書式。 例: <code>1. 01E+03</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>クリック <strong>[!UICONTROL 追加 ]</strong> をクリックして、シートをスプレッドシートに追加します。 各シートに、シートとシートのインデックスのタイトルを入力またはマップします。 インデックス 0 は最初のシートを表します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL シートを削除する]

特定のシートを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] スプレッドシート。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>削除するシートを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL API 呼び出しを実行する]

このアクションモジュールを使用すると、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>[Fusion App] アカウントをに接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>相対パスを入力 <code>https://sheets.googleapis.com/v4/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> 標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:   <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 検索

* [[!UICONTROL 行を検索]](#search-rows)
* [[!UICONTROL 検索行（詳細）]](#search-rows-advanced)
* [[!UICONTROL 範囲の値を取得]](#get-range-values)
* [[!UICONTROL リストシート]](#list-sheets)

### [!UICONTROL 行を検索]

フィルターオプションを使用して行を検索します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>[Fusion App] アカウントをに接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] スプレッドシート。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>行を検索するシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL テーブルにヘッダーが含まれています ]</td> 
   <td> <p> スプレッドシートにヘッダー行を含めるかどうかを選択します。 [!UICONTROL はい ] オプションが選択されている場合、出力データと出力内の変数名がヘッダーによって呼び出されるので、モジュールはヘッダー行を取得しません。 [!UICONTROL いいえ ] オプションが選択されている場合、モジュールはまた、出力内の最初のテーブル行と変数名を取得し、その後 A、B、C、D などのみと呼び出します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 列の範囲 ]</td> 
   <td>操作する列の範囲を選択します。 例: <code>A-F</code></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フィルター ]</td> 
   <td> <p>検索する行のフィルターを設定します。</p> <p>フィルターについて詳しくは、 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] のシナリオへのフィルターの追加</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 並べ替え順 ]</td> 
   <td>昇順と降順のどちらで並べ替えるかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Order by]</td> 
   <td>並べ替える列を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値レンダリングオプション ]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL 形式の値 ]</p> <p>値は、セルの書式設定に従って計算され、返信の形式設定されます。 書式設定は、要求元のユーザーのロケールではなく、スプレッドシートのロケールに基づいておこなわれます。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻る <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL 形式設定されていない値 ]</p> <p>値は計算されますが、返信の形式は設定されません。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> は数値を返します <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL 数式 ]</p> <p>値は計算されません。 返信には数式が含まれます。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻る <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 日時レンダリングオプション ]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL シリアル番号 ]</p> <p>日付、時刻、日時、期間の各フィールドを、Lotus 1-2-3によって一般化された「シリアル番号」形式で倍精度に出力するように指示します。 値の整数部分（小数の左側）は、1899 年 12 月 30 日からの日数を数えます。 小数部分（小数の右側）は、時間を日の端数としてカウントします。 例えば、1900 年 1 月 1 日の正午は、1899 年 12 月 30 日の 2 日後なので 2.5、1999 年 12 月 30 日の半日後なので 0.5 となります。 1900 年 2 月 1 日の午後 3 時には 33.625 となります。これにより、1900 年を閏年ではないとして正しく処理します。</p> <p style="font-weight: bold;">[!UICONTROL 形式の文字列 ]</p> <p>日付、時間、日時、期間の各フィールドを指定された数値形式（スプレッドシートのロケールに依存）で文字列として出力するように指示します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返される行の最大数 ]</td> 
   <td>最大行数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 検索行（詳細）]

指定された条件に一致する結果を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>検索するシートが含まれているGoogleスプレッドシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>検索する行を含むシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL クエリ ]</td> 
   <td> <p>以下を使用： [!DNL Google Charts Query Language]. 例: <code>select * where B = "John"</code></p> <p>詳しくは、 [!DNL Google Charts Query Language]を参照してください。 <a href="https://developers.google.com/chart/interactive/docs/querylanguage">クエリ言語リファレンス</a> 内 [!DNL Google] ドキュメント。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 範囲の値を取得]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] スプレッドシート。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL シート ] </td> 
   <td> <p>範囲の内容を取得するシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 範囲 ] </td> 
   <td> <p>取得する範囲を入力します。 例: <code>A1:D25</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL テーブルにヘッダーが含まれています ]</td> 
   <td> <p>シートにヘッダー行がある場合は、このチェックボックスをオンにします</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ヘッダー付き行 ]</td> 
   <td>テーブルヘッダーの範囲を入力します。 例 <code>A1:F1</code>. このフィールドを空のままにした場合、 [!DNL Workfront Fusion] 指定した範囲の最初の行にヘッダーがあるとします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 値レンダリングオプション ]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL 形式の値 ]</p> <p>値は、セルの書式設定に従って計算され、返信の形式設定されます。 書式設定は、要求元のユーザーのロケールではなく、スプレッドシートのロケールに基づいておこなわれます。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻る <code>"$1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL 形式設定されていない値 ]</p> <p>値は計算されますが、返信の形式は設定されません。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> は数値を返します <code>"1.23"</code>.</p> <p style="font-weight: bold;">[!UICONTROL 数式 ]</p> <p>値は計算されません。 返信には数式が含まれます。 例えば、 <code>A1</code> が <code>1.23</code> および <code>A2</code> が <code>=A1</code> 通貨形式で書式設定されます。 <code>A2</code> 戻る <code>"=A1"</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 日時レンダリングオプション ]</td> 
   <td> <p style="font-weight: bold;">[!UICONTROL シリアル番号 ]</p> <p>日付、時刻、日時、期間の各フィールドを、Lotus 1-2-3によって一般化された「シリアル番号」形式で倍精度に出力するように指示します。 値の整数部分（小数の左側）は、1899 年 12 月 30 日からの日数を数えます。 小数部分（小数の右側）は、時間を日の端数としてカウントします。 例えば、1900 年 1 月 1 日の正午は、1899 年 12 月 30 日の 2 日後なので 2.5、1999 年 12 月 30 日の半日後なので 0.5 となります。 1900 年 2 月 1 日の午後 3 時には 33.625 となります。これにより、1900 年を閏年ではないとして正しく処理します。</p> <p style="font-weight: bold;">[!UICONTROL 形式の文字列 ]</p> <p>日付、時間、日時、期間の各フィールドを指定された数値形式（スプレッドシートのロケールに依存）で文字列として出力するように指示します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL リストシート]

このモジュールは、スプレッドシート内のすべてのシートのリストを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Sheets] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スプレッドシート ] </td> 
   <td> <p>を選択します。 [!DNL Google] リストに表示するシートを含むスプレッドシート。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用の制限

エラーが `429: RESOURCE_EXHAUSTED` が発生した場合に、API のレート制限を超えています。

この [!DNL Google Sheets] API には、1 プロジェクトあたり 100 秒あたり 500 個のリクエストと、1 ユーザーあたり 100 秒あたり 100 個のリクエストという制限があります。 読み取りと書き込みの制限は、別々に追跡されます。 1 日の使用制限はありません。

詳しくは、 [developers.google.com/sheets/api/limits](https://developers.google.com/sheets/api/limits).

## ヒントとテクニック

* [から空のセルを取得する方法 [!DNL Google] シート](#how-to-get-empty-cells-from-a-google-sheet)
* [シナリオを実行するためのボタンをシートに追加する](#add-a-button-in-a-sheet-to-run-a-scenario)

### から空のセルを取得する方法 [!DNL Google Sheet]

以下を使用： [!UICONTROL 検索行（詳細）] この式を使用して、空の列を取得します。
<pre>「* [!UICONTROL E が null の場合は​]」を選択します。</pre>ここでは、「E」が列で、「is null」が条件です。 [Google Query Lang] を使用して、より高度なクエリを作成できます。](https://developers.google.com/chart/interactive/docs/querylanguage)

### シナリオを実行するためのボタンをシートに追加する

1. In [!DNL Workfront Fusion]、 **[!UICONTROL ウェブフック]** > **[!UICONTROL カスタムウェブフック]** モジュール/トリガーを設定します ( [ウェブフック](../../workfront-fusion/apps-and-their-modules/webhooks-updated.md)) をクリックします。

1. Webhook の URL をコピーします。
1. シナリオを実行します。
1. Google Sheet で、「 **[!UICONTROL 挿入]** > **[!UICONTROL 図面]**&#x200B;メインメニューバーから

1. 内 [!UICONTROL 図面] ウィンドウで、 **[!UICONTROL テキストボックス]** アイコン ![](assets/text-box.png) 窓の上の方に
1. ボタンをデザインし、 **[!UICONTROL 保存して閉じる]** ボタンを使用して、次の操作を実行できます。
1. 「 」ボタンがワークシートに配置されます。 ボタンの右上隅にある 3 つの縦のドットをクリックします。
1. 選択 **[!UICONTROL スクリプトを割り当て…].** を選択します。
1. スクリプトの名前（関数）を入力します。例： `runScenario` をクリックし、 **[!UICONTROL OK]**:
1. 選択 **[!UICONTROL ツール]** > **[!UICONTROL スクリプトエディター]** をメインメニューバーから選択します。

1. 次のコードを挿入します。

   * 関数の名前は、手順 9 で指定した名前に対応している必要があります。
   * URL を手順 2 でコピーした Webhook の URL に置き換えます。

      <pre>function runScenario() {</pre><pre>UrlFetchApp.fetch("<webhook you copied>");</pre><pre>}</pre>

1. 押す **[!UICONTROL Ctrl + S]** スクリプトファイルを保存するには、プロジェクト名を入力し、 **[!UICONTROL OK]**.

1. 戻る [!DNL Google Sheets] をクリックし、新しいボタンをクリックします。
1. スクリプトに必要な認証を付与します。
1. In [!DNL Workfront Fusion]」で、シナリオが正常に実行されたことを確認します。

## スプレッドシートに日付を保存する

日付の値を書式設定なしでスプレッドシートに格納した場合、ISO 8601 形式のテキストとしてスプレッドシートに表示されます。 しかし、 [!DNL Google Sheets] このテキストを理解しない日付に対して機能する数式または関数 ( 例：式 `=A1+10`) を呼び出すと、次のエラーが表示されます。

![](assets/mceclip6-350x87.png)

許可に役立つように [!DNL Google Sheets] 日付を理解するには、 [[!UICONTROL formatDate] （日付）形式；[timezone])](../../workfront-fusion/functions/date-and-time-functions.md#formatda) 関数に置き換えます。 2 番目の引数として関数に渡される正しい形式は、スプレッドシートのロケール設定によって異なります。

正しい形式を判断するには、次の手順を実行します。

1. 選択 **[!UICONTROL ファイル]** > **[!UICONTROL スプレッドシート]** の設定を使用して、ロケールを確認または設定します。

1. 適切なロケールを検証/設定したら、 **[!UICONTROL 形式]** > **[!UICONTROL 数値]** を選択します。 形式は、「日付と時刻」メニュー項目の横に表示されます。

1. に渡す正しい形式を作成するには [!UICONTROL formatDate()] 関数の場合は、 [の日付と時刻の書式設定のトークン [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md).

**例：** の使用 `MM/DD/YYYY HH:mm:ss` 米国ロケールの形式：

![](assets/locale-time-350x83.png)

## 活用 [!DNL Google Sheets] 関数

組み込みの関数が見つからなかった場合、その関数は [!DNL Google Sheets]を使用する場合は、利用できます。 詳しくは、 [用途 [!DNL Google Sheets] 関数](../../workfront-fusion/functions/map-using-functions.md#exploiti) in [で関数を使用して項目をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md) .

## 保持 [!DNL Google Sheets] 数を日付に変えること

数値の文字列が [!DNL Google] ワークシート。 例えば、テキストとして使用する場合は「1-2019」と入力しますが、Googleはこれを日付として解釈します。 これを防ぐために、数値をプレーンテキストとして書式設定できます。

1. In [!DNL Google Sheets]、数値を含む列またはセルをハイライト表示します。
1. クリック **[!UICONTROL 形式]** > **[!UICONTROL 数値]** > **[!UICONTROL プレーンテキスト]**.

の別の回避策 [!DNL Workfront Fusion] が数値の前にアポストロフィ (&#39;) を入力する場合は、「1-2019」や「1/47」などです。 データの送信元のセルにアポストロフィが表示されない [!DNL Workfront Fusion].
