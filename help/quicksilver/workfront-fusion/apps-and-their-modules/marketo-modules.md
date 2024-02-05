---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Marketo モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL Marketo] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2068'
ht-degree: 99%

---

# [!DNL Marketo] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Marketo] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

Marketoコネクタの紹介ビデオについては、次を参照してください。

* [Marketo](https://video.tv.adobe.com/v/3427026/){target=_blank}

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
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

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Marketo] モジュールを使用するには、[!DNL Marketo] アカウントが必要です。

## [!DNL Marketo] を Workfront Fusion に接続 {#connect-marketo-to-workfront-fusion}

[!DNL Marketo] アカウントへの接続を、[!DNL Marketo] モジュール内から直接作成できます。

1. 任意の [!DNL Marketo] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. [!DNL Marketo] アカウントまたは [!DNL Marketo] [!UICONTROL Munchkin] ID を入力します。これは、アカウントに割り当てられたベース URL またはエンドポイントの一意の部分で、[!UICONTROL REST] API 経由で [!DNL Marketo] にアクセスするために使用します。これを検索する手順については、[!DNL Marketo] ドキュメントの[ベース URL](https://developers.marketo.com/rest-api/base-url/) を参照してください。
1. [!UICONTROL クライアント ID] および[!UICONTROL クライアントシークレット]を入力します。これらを検索する手順については、[!DNL Marketo] ドキュメントの[認証](https://developers.marketo.com/rest-api/authentication/)を参照してください。
1. 「**[!UICONTROL 続行]**」をクリックして接続を作成し、モジュールに戻ります。

## [!DNL Marketo] モジュールとそのフィールド

[!DNL Marketo] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Marketo] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) におけるモジュール間の情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

* [[!UICONTROL レコードを監視]](#watch-records)
* [[!UICONTROL イベントを監視（即時）]](#watch-events-instant)

#### [!UICONTROL レコードを監視]

このトリガーモジュールは、レコードが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Activity]</strong> </p> <p>監視するアクティビティのタイプを選択します。 </p> <p>モジュールは、新しいアクティビティのみを監視します。<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>新しいレコード、更新されたレコード、新しいレコードと更新されたレコードの両方、または特定のフィールドの更新を監視するかどうかを選択します。特定のフィールドの更新を監視する場合は、モジュールで監視するフィールドを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL Program]</strong> </p> <p>新しいレコード、更新されたレコード、または新しいレコードと更新されたレコードの両方を監視するかどうかを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントを監視（即時）]

このトリガーモジュールは、レコードが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>モジュールで使用する web フックを入力します。</p> <p>Web フックについて詳しくは、<a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> のインスタントトリガー（web フック）を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL レコードを作成]](#create-a-record)
* [[!UICONTROL レコードを更新]](#update-a-record)
* [[!UICONTROL ファイルをダウンロード]](#download-a-file)
* [[!UICONTROL ファイルをアップロード]](#upload-a-file)
* [[!UICONTROL レコードの読み取り]](#read-a-record)
* [[!UICONTROL リードをリストに追加]](#add-leads-to-a-list)
* [[!UICONTROL リストからリードを削除]](#remove-leads-from-a-list)
* [[!UICONTROL キャンペーンをスケジュール]](#schedule-a-campaign)
* [[!UICONTROL プログラムをコピー]](#copy-a-program)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールでは、[!DNL Marketo] API への認証済みのカスタム呼び出しを実行できます。これにより、他の [!DNL Marketo] モジュールでは不可能なデータフロー自動処理を実現できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事内の <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo]を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td><code>https://{your-base-url}.mktorest.com/</code> への相対パスを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] によって認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが操作するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを作成]

このアクションモジュールは、[!DNL Marketo] に新しいレコードを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Folder]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select fields to map]</td> 
   <td>会社またはリードを作成する場合は、新しいレコードの作成時に値を設定するフィールドを選択し、これらのフィールドに値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Type]</td> 
   <td>プログラムを作成する場合は、作成するプログラムのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Channel] </td> 
   <td>プログラムを作成する場合は、プログラムを作成するプログラムチャネルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]／[!UICONTROL Program Name]</td> 
   <td>フォルダーまたはプログラムを作成する場合は、新しいレコードの名前を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>フォルダーまたはプログラムを作成する場合は、新しいレコードの説明を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID]</td> 
   <td>フォルダーまたはプログラムを作成する場合は、新しいレコードを作成する親フォルダの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td>プログラムを作成する場合は、コストを追加します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>プログラムを作成する場合は、タグを追加します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを更新]

このアクションモジュールは、ID を使用して既存のレコードを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Company]／[!UICONTROL Lead]／[!UICONTROL Program ID]</td> 
   <td>更新するレコードの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select fields to map]</td> 
   <td>会社またはリードを更新する場合は、値を更新するフィールドを選択し、これらのフィールドに値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Name]</td> 
   <td>プログラムを更新する場合は、プログラムの新しい名前を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>プログラムを更新する場合は、プログラムの新しい説明を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start Date]</td> 
   <td>プログラムを更新する場合は、プログラムの新しい開始日を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL End Date]</td> 
   <td>プログラムを更新する場合は、プログラムの新しい終了日を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td>プログラムを更新する場合は、コストを追加します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>プログラムを更新する場合は、タグを追加します</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをダウンロード]

このアクションモジュールは、ファイル ID を使用してファイルをダウンロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する手順について詳しくは、この記事の <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td>ダウンロードするファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをアップロード]

このアクションモジュールは、新しいファイルを [!UICONTROL Marketo] にアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-marketo-to-workfront-fusion" class="MCXref xref"> [!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>新しいファイルを配置するフォルダーの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>アップロードするファイルの説明を入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、ID を使用してレコードに関する情報を読み取ります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL List]</p> </li> 
     <li> <p>[!UICONTROL Program]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。フィールドは、選択した [!UICONTROL Record Type] に基づいて使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;Object&gt; ID]</td> 
   <td>情報を取得するオブジェクトの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リードをリストに追加]

このアクションモジュールは、リード ID を使用して 1 つまたは複数のリードをリストに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウント [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-marketo-to-workfront-fusion" class="MCXref xref"> [!DNL Marketo] を [!DNL Workfront Fusion]</a> へ接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>リードを追加するリストの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead IDs]</td> 
   <td> <p>リストに追加するリードごとに、<b>[!UICONTROL Add]</b> をクリックし、追加するリードの ID を入力またはマッピングします。モジュールがリストに追加できるリードは 300 件までです。</p> <p>マップの切り替えをクリックして、リストに追加する既存のリードのコレクションをマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストからリードを削除]

このアクションモジュールは、リード ID を使用して、1 つまたは複数のリードをリストから削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウント [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-marketo-to-workfront-fusion" class="MCXref xref"> [!DNL Marketo] を [!DNL Workfront Fusion]</a> へ接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td>リードを削除するリストの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead IDs]</td> 
   <td> <p>リストから削除するリードごとに、<b>[!UICONTROL Add]</b> をクリックし、削除するリードの ID を入力するかマッピングします。モジュールがリストから削除するリードは最大 300 人まで追加できます。 </p> <p>マップの切り替えをクリックして、リストから削除する既存のリードのコレクションをマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL キャンペーンをスケジュール]

このアクションモジュールは、特定の日付の既存のキャンペーンをスケジュールします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>スケジュールを設定するキャンペーンの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Schedule for Date]</p> </td> 
   <td>キャンペーンを実行する日付を選択します。このフィールドを空白にした場合、キャンペーンはシナリオが開始されてから 5 分後に実行されます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL プログラムをコピー]

このアクションモジュールは、既存のプログラムの ID を使用してプログラムのコピーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Existing Program ID]</td> 
   <td>コピーするプログラムの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL New Program Name]</p> </td> 
   <td> <p>新しいプログラムの名前を入力またはマッピング</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td>新しいプログラムを配置するフォルダーの ID を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL レコードをリスト]](#list-records)
* [[!UICONTROL レコードを検索]](#update-a-record)

#### [!UICONTROL レコードをリスト]

このアクションモジュールは、特定のタイプのすべてのレコードを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>リストに表示するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Read all campaigns]</p> </li> 
     <li> <p>[!UICONTROL Read all programs]</p> </li> 
     <li> <p>[!UICONTROL Read all leads] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field]</td> 
   <td>リードの取得を選択した場合は、リストからリードを取得するか、プログラムからリードを取得するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。フィールドは、選択した [!UICONTROL Record Type] に基づいて使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを検索]

この検索モジュールは、特定の検索条件に一致するレコードのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Marketo] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事で<a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion]</a> への [!DNL Marketo] の接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>検索するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaigns]</p> </li> 
     <li> <p>[!UICONTROL Leads]</p> </li> 
     <li> <p>[!UICONTROL Programs]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Field]</p> </td> 
   <td> <p>名前、プログラム名またはワークスペース名で検索するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Values]</td> 
   <td>検索する値ごとに、<b>[!UICONTROL Add item]</b> をクリックして、値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
