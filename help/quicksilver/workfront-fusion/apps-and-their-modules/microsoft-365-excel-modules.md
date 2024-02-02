---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel モジュール
description: ' [!DNL Adobe Workfront Fusion]  シナリオの場合、Microsoft 365 Excel を使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションおよびサービスに接続することができます。'
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '2625'
ht-degree: 100%

---

# [!DNL Microsoft Office 365 Excel] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Microsoft 365 Excel] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Microsoft office 365 Excel] を使用するには、Microsoft アカウントが必要です。

## [!DNL Microsoft Office 365 Excel] モジュールとそのフィールド

[!DNL Microsoft 365 Excel] モジュールを設定する際に、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらとともに、アプリやサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Microsoft 365 Excel] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [ワークブック](#workbook)
* [ワークシート](#worksheet)
* [テーブル](#table)
* [その他](#other)

### ワークブック

* [ワークブックを監視](#watch-workbooks)
* [ワークブックを検索](#search-workbooks)
* [ワークブックをダウンロード](#download-a-workbook)

#### [!UICONTROL ワークブックを監視]

このトリガーモジュールは、ワークブックの作成時にシナリオを開始します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>新規ワークブックを監視するフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>選択した条件を満たすワークブックのみを監視するフィルターを設定できます。</p> <p>各フィルターに対して、フィルターを評価するフィールド、演算子、およびフィルターに許可する値を入力します。AND または OR ルールを追加すると、複数のフィルターを使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すワークブックの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークブックを検索]

このアクションモジュールは、[!DNL Excel] ワークブックを検索します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>ワークブックを監視するフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>選択した条件を満たすワークブックのみを検索するフィルターを設定できます。</p> <p>各フィルターに対して、フィルターを評価するフィールド、演算子、およびフィルターに許可する値を入力します。AND または OR ルールを追加すると、複数のフィルターを使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが返すワークシートの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークブックをダウンロード]

このアクションモジュールは、指定した Excel ブックの内容をダウンロードします。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Download a workbook]</td> 
   <td> <p>モジュールでダウンロードするワークブックを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By entering an ID manually]</strong> </p> <p>「[!UICONTROL Workbook ID]」フィールドに、モジュールでダウンロードする特定のワークブックの ID を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL By selecting from the path]</strong> </p> <p>「[!UICONTROL Workbook]」フィールドで、モジュールでダウンロードするワークブックを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ワークシート

* [[!UICONTROL ワークシート行を監視]](#watch-worksheet-rows)
* [[!UICONTROL ワークシートをリスト]](#list-worksheets)
* [[!UICONTROL リストワークシート行をリスト]](#list-worksheet-rows)
* [[!UICONTROL ワークシートを追加]](#add-a-worksheet)
* [[!UICONTROL ワークシート行を追加]](#add-a-worksheet-row)
* [[!UICONTROL ワークシート行を更新]](#update-a-worksheet-row)
* [[!UICONTROL ワークシート行の削除]](#delete-a-worksheet-row)

#### [!UICONTROL ワークシート行を監視]

このトリガーモジュールは、新しい行がシートに追加されると、シナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>新しい行を見るワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>新しい行を見る Excel シートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すワークシート行の最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシートをリスト]

このアクションモジュールは、指定されたワークブック内のワークシートのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>モジュールのリストを表示するワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すワークシートの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシート行をリスト]

このアクションモジュールは、指定されたワークシートの行のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>リストに表示する行が含まれているワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>リストする行を含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すワークシート行の最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシートを追加]

このアクションモジュールは、選択したワークブック内に新しいワークシートを作成します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>ワークシートを追加するワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>新しいワークシートの名前を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシート行を追加]

このアクションモジュールは、選択したワークシートに新しい行を追加します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>行を追加するワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>行を追加するワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type of values being entered]</p> </td> 
   <td> <p>ワークシートに入力する値のタイプを選択します。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel は、指定された式の評価を試みます。数式内の関数名は英語です。例： <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel は、指定された式の評価を試みます。関数名は、Excel アプリケーションの言語で表示されます。例：<code>=SUM(A1, 1.5)</code> と <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel では値は評価されません。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>各列に、新しい行で列に表示する値を入力します。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシート行の更新]

このアクションモジュールは、既存のワークシートの行を更新します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>更新する行が含まれているワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>更新する行を含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type of values being entered]</p> </td> 
   <td> <p>ワークシートに入力する値のタイプを選択します。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel は、指定された式の評価を試みます。数式内の関数名は英語です。例： <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel は、指定された式の評価を試みます。関数名は、Excel アプリケーションの言語で表示されます。例：<code>=SUM(A1, 1.5)</code> と <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel では値は評価されません。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row ID]</td> 
   <td>更新する行数を選択します。</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>各列に、新しい行で列に表示する値を入力します。</td>
   --&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシート行を削除]

このアクションモジュールは、ワークシートから行を削除します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>削除する行が含まれているワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet]</td>
   <td> <p> 削除する行を含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row ID]</td>
   <td>削除する行の ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### テーブル

* [[!UICONTROL テーブル行を監視]](#watch-table-rows)
* [[!UICONTROL テーブルをリスト]](#list-tables)
* [[!UICONTROL テーブル行をリスト]](#list-table-rows)
* [[!UICONTROL テーブルを取得]](#get-a-table)
* [[!UICONTROL テーブルを追加]](#add-a-table)
* [[!UICONTROL テーブル行を追加]](#add-a-table-row)
* [[!UICONTROL テーブルを更新]](#update-a-table)
* [[!UICONTROL テーブルを削除]](#delete-a-table)

#### [!UICONTROL テーブル行を監視]

これは、テーブルに新しい行が追加されるとシナリオを開始するトリガーです。

>[!NOTE]
>
>このテーブルは、ワークブックに埋め込まれたテーブル要素を参照します。テーブル全体（ワークブックやシート）ではありません。

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Workbook]</p> </td> 
   <td> <p>監視するテーブルを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p> 監視するテーブルを含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Table]</p> </td> 
   <td> <p>監視するテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返す最大行数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルをリスト]

この検索モジュールは、すべてのテーブルオブジェクトのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365]アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>リストアップするテーブルを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>リストアップするテーブルを含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すテーブルの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブル行をリスト]

この検索モジュールは、ワークブック内のすべてのテーブル行のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>リストする行が含まれているテーブルを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>リストする行が含まれているテーブルを含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table] </td>
   <td> <p>リストする行を含むテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すテーブル行の最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルを取得]

このアクションモジュールは、指定されたテーブルのメタデータを取得します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>Office 365 アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a table]</td> 
   <td> <p>取得するテーブルを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>[!UICONTROL Workbook ID] フィールドに、取得するテーブルを含むワークブックの ID を入力またはマッピングします。</p> <p>[!UICONTROL Table Name] フィールドに、取得するテーブルの名前を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>取得するテーブルを含むワークブックとワークシートを選択し、テーブルを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルを追加]

このアクションモジュールは、Excel ワークシート内にテーブル要素を作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>テーブルを追加するワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>テーブルを追加するワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Has headers]</td> 
   <td> <p>最初の行をテーブルヘッダーとして定義するには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Address]</p> </td> 
   <td> <p>左上と右下のセルを指定して、テーブルのサイズを設定します。例：<code>A1:C10</code> は、3 列 10 行のテーブルを作成します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブル行を追加]

このアクションモジュールは、既存のテーブルを変更します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>行を追加するテーブルを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>行を追加するテーブルを含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table]</td>
   <td>行を追加するテーブルを選択します。</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>各列に、新しい行で列に表示する値を入力します。</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Row ID]</p> </td> 
   <td> <p>テーブル上の特定の場所に行を追加するには、行番号を入力またはマッピングします。その行の後に新しい行が挿入されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルを更新]

このアクションモジュールは、既存のテーブルを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update a table]</td> 
   <td> <p>更新するテーブルを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>手動で入力</strong> </p> <p>[!UICONTROL Workbook ID] フィールドに、更新するテーブルを含むワークブックの ID を入力またはマッピングします。</p> <p>[!UICONTROL Table Name] フィールドに、更新するテーブルの名前を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>更新するテーブルを含むワークブックおよびワークシートを選択し、テーブルを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table] </td> 
   <td> <p>更新するテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>テーブルの名前を変更する場合は、テーブルの新しい名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show Headers]</td> 
   <td> <p>更新されたテーブルのヘッダーを表示するには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show totals]</td> 
   <td>テーブルの合計値を表示するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Style]</td> 
   <td>新しいテーブルのスタイルを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルを削除]

このアクションモジュールは、指定されたテーブルを [!DNL Excel] ワークシートから削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a table]</td> 
   <td> <p>削除するテーブルを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>[!UICONTROL Workbook ID] フィールドに、削除するテーブルを含むワークブックの ID を入力またはマッピングします。</p> <p>[!UICONTROL Table Name] フィールドに、削除するテーブルの名前を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>削除するテーブルを含むワークブックおよびワークシートを選択し、テーブルを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### その他

* [[!UICONTROL データを取得]](#retrieve-data)
* [[!UICONTROL API 呼び出しを実行]](#make-an-api-call)

#### [!UICONTROL データを取得]

このアクションは、定義されたワークシート範囲からデータを取得し、各行のバンドルを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>取得するデータを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>取得するデータを含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Range] </td> 
   <td> <p>左上と右下のセルを指定して、データを取得するシートのエリアを指定します。例： <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 呼び出しを実行]

このアクションモジュールを使用すると、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの作成の記事で、<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td><code>https://graph.microsoft.com</code> への相対パスを入力します。例：<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：   <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
