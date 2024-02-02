---
title: Widen モジュール
description: ' [!DNL Adobe Workfront Fusion]  シナリオでは、[!UICONTROL Widen] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。'
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1586'
ht-degree: 100%

---

# [!DNL Widen] モジュール

[!DNL Adobe Workfront Fusion] シナリオでは、[!UICONTROL Widen] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[モジュール： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)を参照してください。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件がありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織が [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織が [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!UICONTROL Widen] モジュールを使用するには、[!UICONTROL Widen] アカウントが必要です。

## [!DNL Widen] を [!DNL Workfront Fusion] に接続 {#connect-widen-to-workfront-fusion}

[!DNL Widen] アカウントへの接続を、[!DNL Widen] モジュール内から直接作成できます。

1. 任意の [!DNL Widen] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 接続する [!DNL Widen] ドメインを選択します。
1. [!DNL Widen] アカウントのトークンを入力します。このトークンの場所について詳しくは、[[!DNL Widen] API に関する FAQ](https://community.widen.com/collective/s/article/API-FAQs)を参照してください。
1. 「**[!UICONTROL 続行]**」をクリックして接続を作成し、モジュールに戻ります。

## [!DNL Widen] モジュールとそのフィールド

[!DNL Widen] モジュールを設定すると、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Widen] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガーモジュール](#trigger-modules)
* [アクションモジュール](#action-modules)
* [モジュールの検索](#search-modules)

### トリガーモジュール

#### [!UICONTROL アセットを監視]

このトリガーモジュールは、アセットが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] へ接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event type]</td> 
   <td> <p>新しいアセットまたは更新されたアセットのどちらを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>アセットフィールドに加えて、モジュールの出力に含めるプロパティを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが操作するアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクションモジュール

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL アセット情報の読み取り]](#read-asset-info)
* [[!UICONTROL コレクションへのアセットの追加]](#add-assets-to-collections)
* [[!UICONTROL コレクションからアセットを削除]](#remove-assets-from-collection)
* [[!UICONTROL アセットのメタデータの更新]](#update-asset-metadata)
* [[!UICONTROL ファイルをダウンロード]](#download-file)
* [ファイルを[!UICONTROL アップロード]](#upload-a-file)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールでは、[!DNL Widen] API への認証済みのカスタム呼び出しを実行できます。これにより、他の [!DNL Widen] モジュールでは不可能なデータフロー自動処理を実現できます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>最新バージョンの [!DNL Widen] API とバージョン 1.0 のどちらを使用するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>API 呼び出しの URL を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での HTTP リクエスト方法を参照してください。</p> </td> 
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
 </tbody> 
</table>

#### [!UICONTROL アセット情報の読み取り]

このアクションモジュールは、個々のアセットを一意の ID で取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>情報を読み取るアセットの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>アセットフィールドに加えて、モジュールの出力に含めるプロパティを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コレクションへのアセットの追加]

このアクションモジュールは、1 つ以上のアセットをコレクションに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事内の <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>アセットの追加先の各コレクションについて、次の操作を行います。</p> 
    <ol> 
     <li value="1"> <p> 「<strong>[!UICONTROL Add]</strong>」をクリックします。</p> </li> 
     <li value="2"> <p>[!UICONTROL Collection ID] を入力またはマッピングします。</p> </li> 
     <li value="3"> <p>「<strong>[!UICONTROL Add item]</strong>」をクリックします。</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>コレクションに追加する各アセットに対して、次の操作を行います。</p> 
    <ol> 
     <li value="1"> <p> 「<strong>[!UICONTROL Add]</strong>」をクリックします。</p> </li> 
     <li value="2"> <p>アセット ID を入力またはマッピングします。</p> </li> 
     <li value="3"> <p>「<strong>[!UICONTROL Add item]</strong>」をクリックします。</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが操作するアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コレクションからアセットを削除]

このアクションモジュールは、コレクションから 1 つ以上のアセットを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] へ接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>アセットを削除する各コレクションに対して、次の操作を実行します。</p> 
    <ol> 
     <li value="1"> <p> 「<strong>[!UICONTROL Add]</strong>」をクリックします。</p> </li> 
     <li value="2"> <p>コレクション ID を入力またはマッピングします。</p> </li> 
     <li value="3"> <p>「<strong>[!UICONTROL Add item]</strong>」をクリックします。</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アセット ID</td> 
   <td> <p>コレクションから削除する各アセットに対して、次の操作を実行します。</p> 
    <ol> 
     <li value="1"> <p> 「<strong>[!UICONTROL Add]</strong>」をクリックします。</p> </li> 
     <li value="2"> <p>アセット ID を入力またはマッピングします。</p> </li> 
     <li value="3"> <p>「<strong>[!UICONTROL Add item]</strong>」をクリックします。</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが操作するアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットメタデータを更新]

このアクションモジュールは、アセットのメタデータフィールドを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>メタデータを更新するアセットの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata type]</td> 
   <td> <p>更新するメタデータのメタデータタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>更新するメタデータフィールドを選択します。各フィールドに、フィールドの新しい値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが操作するアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをダウンロード]

このアクションモジュールは、[!DNL Widen] アカウントからアセットをダウンロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>ダウンロードするアセットの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをアップロード]

このアクションモジュールは、ファイルを [!DNL Widen] アカウントにアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Profile]</td> 
   <td> <p>モジュールで使用するアップロードプロファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Method]</td> 
   <td> <p>ファイルのアップロード方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL From File]</strong> </p> <p>前のモジュールからソースファイルを選択またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL By URL]</strong> </p> <p>アップロードするファイルの URL を入力またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>アップロードしたファイルの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata Type]</td> 
   <td>アップロードするファイルのメタデータタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>ファイルのアップロードに含めるメタデータフィールドを選択します。各フィールドに、そのフィールド用の [!UICONTROL value] を入力します。</td> 
  </tr> 
 </tbody> 
</table>

### モジュールの検索

* [[!UICONTROL コレクションアセットの読み取り]](#read-collection-assets)
* [[!UICONTROL アセットの検索]](#search-assets)

#### [!UICONTROL コレクションアセットの読み取り]

このアクションモジュールは、コレクション内のアセットのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>読み取るアセットを含むコレクションの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>リストする最初の項目の番号を入力またはマッピングします。これは、レコードをページ分割する方法です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort By]</td> 
   <td> <p>アセットの並べ替えに使用するプロパティを選択します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>アセットを昇順に並び替えるか、降順に並び替えるかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットの検索]

この検索モジュールは、特定の検索条件に一致するアセットのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>[!DNL Widen] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search query]</td> 
   <td> <p>アセットを検索する条件を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort By]</td> 
   <td> <p>アセットを並べ替える方法を選択します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>アセットを昇順に並び替えるか、降順に並び替えるかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include deleted]</td> 
   <td>削除されたアセットを検索に含めるには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Include archived]</p> </td> 
   <td> <p>アーカイブしたアセットを検索に含めるには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search document text]</td> 
   <td>検索にドキュメントテキストを含める場合はこのオプションを有効にし、検索条件に一致するタイトルを持つアセットのみを含める場合は false にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>詳細を取得する最初の項目の番号を入力またはマッピングします。これは、レコードをページ分割する方法です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>スクロールを許可するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>アセットフィールドに加えて、モジュールの出力に含めるプロパティを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールの出力に含めるフィールドを選択します。</td> 
  </tr> 
 </tbody> 
</table>
