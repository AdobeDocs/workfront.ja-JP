---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Microsoft 365 Excel を使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションおよびサービスに接続することができます。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2577'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Microsoft 365 Excel]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td>  
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

使用する [!DNL Microsoft office 365 Excel]を使用するには、Microsoftアカウントが必要です。

## [!DNL Microsoft Office 365 Excel] モジュールとそのフィールド

設定時に [!DNL Microsoft 365 Excel] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Microsoft 365 Excel] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [ワークブック](#workbook)
* [ワークシート](#worksheet)
* [テーブル](#table)
* [その他](#other)

### ワークブック

* [ワークブックを見る](#watch-workbooks)
* [ワークブックの検索](#search-workbooks)
* [ワークブックのダウンロード](#download-a-workbook)

#### [!UICONTROL ワークブックを見る]

このトリガーモジュールは、ワークブックの作成時にシナリオを開始します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td> <p>新しいワークブックを監視するフォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL フィルター ]</p> </td> 
   <td> <p>選択した条件を満たすワークブックのみを監視するフィルターを設定できます。</p> <p>各フィルターに対して、フィルターを評価するフィールド、演算子およびフィルターに許可する値を入力します。 AND または OR ルールを追加すると、複数のフィルターを使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すワークブックの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークブックの検索]

このアクションモジュールは、 [!DNL Excel] ワークブック。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td> <p>ワークブックを検索するフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL フィルター ]</p> </td> 
   <td> <p>選択した条件を満たすワークブックのみを検索するフィルタを設定できます。</p> <p>各フィルターに対して、フィルターを評価するフィールド、演算子およびフィルターに許可する値を入力します。 AND または OR ルールを追加すると、複数のフィルターを使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが返すワークシートの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークブックのダウンロード]

このアクションモジュールは、指定した Excel ブックの内容をダウンロードします。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ワークブックのダウンロード ]</td> 
   <td> <p>モジュールをダウンロードするワークブックを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ID を手動で入力する ]</strong> </p> <p>「[!UICONTROL ワークブック ID]」フィールドに、モジュールでダウンロードする特定のワークブックの ID を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL パスから選択 ]</strong> </p> <p>「[!UICONTROL ワークブック ]」フィールドで、モジュールをダウンロードするワークブックを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ワークシート

* [[!UICONTROL ワークシート行を監視]](#watch-worksheet-rows)
* [[!UICONTROL ワークシートの一覧]](#list-worksheets)
* [[!UICONTROL リストワークシートの行]](#list-worksheet-rows)
* [[!UICONTROL ワークシートを追加]](#add-a-worksheet)
* [[!UICONTROL ワークシート行を追加]](#add-a-worksheet-row)
* [[!UICONTROL ワークシート行の更新]](#update-a-worksheet-row)
* [[!UICONTROL ワークシート行の削除]](#delete-a-worksheet-row)

#### [!UICONTROL ワークシート行を監視]

このトリガーモジュールは、新しい行がシートに追加されると、シナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>新しい行を監視するワークシートが含まれているブックを選択します。</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>新しい行を監視する Excel シートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 制限 ]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すワークシート行の最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシートの一覧]

このアクションモジュールは、指定されたワークブック内のワークシートのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>モジュールの一覧を表示するワークシートが含まれているワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 制限 ]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すワークシートの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストワークシートの行]

このアクションモジュールは、指定されたワークシートの行のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>リストに表示する行が含まれているワークシートを含むブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>リストする行を含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 制限 ]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すワークシート行の最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシートを追加]

このアクションモジュールは、選択したブック内に新しいワークシートを作成します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>ワークシートを追加するワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 名前 ] </td>
   <td> <p>新しいワークシートの名前を入力またはマップします。</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>行を追加するワークシートを含むブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>行を追加するワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 入力する値のタイプ ]</p> </td> 
   <td> <p>ワークシートに入力する値のタイプを選択します。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 数式 ]</strong> </p> <p> Excel は、指定された式を評価しようとします。 数式の関数名は英語です。 例: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL 式（ローカル）]</strong> </p> <p>Excel は、指定された式を評価しようとします。 関数名は、Excel アプリケーションの言語で指定します。 例： <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL 値 ]</strong> </p> <p>Excel では値は評価されません。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 行 ]</td>
    <td>各列に、新しい行に列に表示する値を入力します。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシート行の更新]

このアクションモジュールは、既存のワークシート行を更新します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>更新する行が含まれているワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>更新する行が含まれているワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 入力する値のタイプ ]</p> </td> 
   <td> <p>ワークシートに入力する値のタイプを選択します。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 数式 ]</strong> </p> <p> Excel は、指定された式を評価しようとします。 数式の関数名は英語です。 例: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL 式（ローカル）]</strong> </p> <p>Excel は、指定された式を評価しようとします。 関数名は、Excel アプリケーションの言語で指定します。 例： <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL 値 ]</strong> </p> <p>Excel では値は評価されません。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 行 ID]</td> 
   <td>更新する行の数を選択します。</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 行 ]</td>
    <td>各列に、新しい行に列に表示する値を入力します。</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ワークシート行の削除]

このアクションモジュールは、ワークシートから行を削除します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>削除する行を含むワークシートを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet]</td>
   <td> <p> 削除する行が含まれているワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 行 ID]</td>
   <td>削除する行の ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### テーブル

* [[!UICONTROL テーブル行を監視]](#watch-table-rows)
* [[!UICONTROL リストテーブル]](#list-tables)
* [[!UICONTROL テーブル行のリスト]](#list-table-rows)
* [[!UICONTROL テーブルの取得]](#get-a-table)
* [[!UICONTROL テーブルを追加]](#add-a-table)
* [[!UICONTROL テーブル行を追加]](#add-a-table-row)
* [[!UICONTROL テーブルの更新]](#update-a-table)
* [[!UICONTROL テーブルの削除]](#delete-a-table)

#### [!UICONTROL テーブル行を監視]

このトリガーは、新しい行がテーブルに追加されると、シナリオを開始します。

>[!NOTE]
>
>この表は、ワークブックに埋め込まれた表要素を示しています。 テーブル全体（ワークブック/シート）ではありません。

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ワークブック ]</p> </td> 
   <td> <p>監視するテーブルを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p> 監視するテーブルが含まれているワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 表 ]</p> </td> 
   <td> <p>監視するテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 制限 ]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返す最大行数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストテーブル]

この検索モジュールは、すべてのテーブルオブジェクトのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>リストするテーブルを含むワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>リストするテーブルを含むワークシートを選択します</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 制限 ]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すテーブルの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブル行のリスト]

この検索モジュールは、ワークブック内のすべてのテーブル行のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>一覧表示する行を含むテーブルを含むブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>リストする行を含むテーブルを含むワークシートを選択します</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 表 ] </td>
   <td> <p>リストする行を含むテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 制限 ]</td>
   <td> <p>各シナリオの実行サイクル中にモジュールが返すテーブル行の最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルの取得]

このアクションモジュールは、指定されたテーブルのメタデータを取得します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL 接続 ]</p>
   </td> 
   <td> 
     <p>Office 365 アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p>
    --&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL テーブルの取得 ]</td> 
   <td> <p>取得するテーブルを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>「[!UICONTROL ワークブック ID]」フィールドに、取得するテーブルが含まれるワークブックの ID を入力またはマッピングします。</p> <p>「[!UICONTROL テーブル名 ]」フィールドに、取得するテーブルの名前を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>取得するテーブルが含まれるワークブックおよびワークシートを選択し、テーブルを選択します。</p> </li> 
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
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ワークブック ] </td> 
   <td> <p>テーブルを追加するワークシートを含むブックを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>テーブルを追加するワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL にヘッダーがある ]</td> 
   <td> <p>最初の行をテーブルヘッダーとして定義するには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL アドレス ]</p> </td> 
   <td> <p>左上と右下のセルを指定して、テーブルのサイズを設定します。 例： <code>A1:C10</code> 3 列 10 行のテーブルを作成します。</p> </td> 
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
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL ワークブック ] </td>
   <td> <p>行を追加するテーブルを含むブックを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>行を追加するテーブルを含むワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL 表 ]</td>
   <td>行を追加するテーブルを選択します。</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL 行 ]</td>
    <td>各列に、新しい行に列に表示する値を入力します。</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 行 ID]</p> </td> 
   <td> <p>テーブル上の特定の場所に行を追加するには、行番号を入力またはマッピングします。 モジュールは、この行の後に新しい行を挿入します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルの更新]

このアクションモジュールは、既存のテーブルを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL テーブルの更新 ]</td> 
   <td> <p>更新するテーブルを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>手動で入力</strong> </p> <p>「[!UICONTROL ワークブック ID]」フィールドに、更新するテーブルが含まれるワークブックの ID を入力またはマッピングします。</p> <p>「[!UICONTROL テーブル名 ]」フィールドに、更新するテーブルの名前を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>更新するテーブルが含まれるワークブックおよびワークシートを選択し、テーブルを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表 ] </td> 
   <td> <p>更新するテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ]</td> 
   <td> <p>テーブルの名前を変更する場合は、テーブルの新しい名前を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ヘッダーを表示 ]</td> 
   <td> <p>更新されたテーブルのヘッダーを表示するには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 合計を表示 ]</td> 
   <td>テーブルの合計値を表示するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スタイル ]</td> 
   <td>新しい表のスタイルを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テーブルの削除]

このアクションモジュールは、指定されたテーブルを [!DNL Excel] ワークシート。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL テーブルの取得 ]</td> 
   <td> <p>削除するテーブルを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>「[!UICONTROL ワークブック ID]」フィールドに、削除するテーブルが含まれるワークブックの ID を入力またはマッピングします。</p> <p>「[!UICONTROL テーブル名 ]」フィールドに、削除するテーブルの名前を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>削除するテーブルを含むワークブックおよびワークシートを選択し、テーブルを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### その他

* [[!UICONTROL データを取得]](#retrieve-data)
* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)

#### [!UICONTROL データを取得]

このアクションは、定義されたワークシート範囲からデータを取得し、各行のバンドルを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ワークブック ] </td> 
   <td> <p>取得するデータが含まれているワークブックを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>取得するデータが含まれているワークシートを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 範囲 ] </td> 
   <td> <p>左上と右下のセルを指定して、データを取得するシートの領域を指定します。 例: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 呼び出しを実行する]

このアクションモジュールを使用すると、カスタム API 呼び出しをおこなうことができます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力 <code>https://graph.microsoft.com</code>. 例:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は、認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
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
