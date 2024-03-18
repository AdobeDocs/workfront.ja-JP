---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Lightroomモジュール
description: Adobe Lightroomモジュールでは、Adobe Lightroomアカウント内のイベントに基づいて、Adobe Workfront Fusion シナリオを開始できます。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: e99bd69c712a7685512eecc7fccc8211013a259d
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 23%

---

# [!DNL Adobe Lightroom] モジュール

<!--Add Connection info-->

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Adobe Lightroom] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについては、[モジュール： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)を参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
      <td>
        <p>[!UICONTROL Pro] 以降</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
      <td>
        <p>[!UICONTROL Plan]、[!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 前提条件

[!DNL Adobe Lightroom] コネクタを使用する前に、次の前提条件が満たされていることを確認する必要があります。

* アクティブな [!DNL Adobe Lightroom] アカウントが必要です。

## Adobe Lightroomへの接続の作成



## Adobe Lightroomモジュールとそのフィールド

[!DNL Adobe Lightroom] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Adobe Lightroom] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [その他](#other)
* [アセット](#assets)
* [アルバム](#albums)

### その他

* [ヘルスチェック](#health-check)
* [ユーザカタログメタデータの取得](#retrieve-user-catalog-metadata)

#### ヘルスチェック

このアクションモジュールは、Lightroomサーバーのバージョン ID を取得し、Lightroomサービスが現在実行中かどうかを確認します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credentials]</td>
      <td>
        <p>特定のサーバーが実行されていることを確認するために特定の資格情報を指定する場合は、「項目を追加」をクリックし、資格情報を入力します。</p><p>認証ヘッダーは自動的に追加されます。</p>
      </td>
    </tr>
  </tbody>
</table>

#### ユーザカタログメタデータの取得

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credentials]</td>
      <td>
        <p>特定の資格情報を指定して正しいユーザーアカウントにアクセスできるようにする場合は、「項目を追加」をクリックし、資格情報を入力します。</p><p>認証ヘッダーは自動的に追加されます。</p>
      </td>
    </tr>
  </tbody>
</table>

### アセット

* [アセットの元のファイルの作成](#create-an-asset-external-xmp-develop-setting-file)
* [アセットの作成](#create-an-asset)
* [アセットの外部XMP開発設定ファイルの作成](#create-an-asset-external-xmp-develop-setting-file)
* [元のファイルのレンディションを生成](#generate-renditions-for-an-original-file)
* [カタログアセットの取得](#get-a-catalog-asset)
* [最新のアセットの外部XMP開発設定の取得](#get-the-latest-asset-external-xmp-develop-setting-file)
* [最新のアセットレンディションを取得する](#get-the-latest-asset-rendition)
* [アセットの取得](#retrieve-assets)

#### アセットの元のファイルの作成

このアクションモジュールは、アセットの元のファイルを作成し、アップロードします。


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを含むカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>ファイルを作成してアップロードするアセットの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL コンテンツの長さ（バイト単位）]</td>
      <td>
        <p>コンテンツの長さをバイト単位で入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL バイト範囲 ]</td>
      <td>
        <p>RFC 2616 で定義されている最初と最後のバイトおよびエンティティの長さを含む、要求のバイト範囲を入力またはマップします。 1 回の呼び出しでアップロードするデータが大きすぎる場合にのみ含める必要があります。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content type]</td>
      <td>
        <p>新しいファイルのコンテンツタイプを選択します。</p>
      </td>
    </tr>
  </tbody>
</table>

#### アセットの作成

このアクションモジュールは、最初のメタデータと読み込み情報を持つ新しいアセットを作成します。


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを作成するカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>新しいアセットの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アセットタイプ ]</td>
      <td>
        <p>アセットを画像かビデオかを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 作成日時ユーザー ]</td>
      <td>
        <p>日付を形式で入力またはマッピング <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime ユーザーが更新されました ]</td>
      <td>
        <p>日付を形式で入力またはマッピング <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 取得日 ]</td>
      <td>
        <p>日付を形式で入力またはマッピング <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### アセットの外部XMP開発設定ファイルの作成

このアクションモジュールは、2 つのワークフローをサポートします。 1 つ目のワークフローは、アセットの外部XMP開発設定ファイルをアップロードすることです。 2 つ目のワークフローは、別のアセットの外部 xmp 開発設定ファイルからコピーして、外部XMP開発設定ファイルを作成することです。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL コンテンツの長さ（バイト単位）]</td>
      <td>
        <p>コンテンツの長さをバイト単位で入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 新規ファイルをアップロードまたはXMP/develop ファイルをコピー ]</td>
      <td>
        <p>新しいファイルをアップロードするか、既存のアセットからファイルをコピーするかを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを含むカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>アップロード先のアセットの ID を入力またはマッピングするか、ファイルをコピーします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XMP/develop ファイルへのリンク ]</td>
      <td>
        <p>アップロードまたはコピーするファイルへのリンクを入力またはマッピングします。</p><p>ファイルをコピーする場合は JSON ファイル、ファイルをアップロードする場合は XML ファイルを指定する必要があります。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 元のファイルのレンディションを生成

このアクションモジュールは、元のファイルのレンディションを非同期的に生成します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レンディションの種類（セミコロン区切り）]</td>
      <td>
        <p>作成するレンディションのレンディションタイプを入力します。 複数のタイプを入力する場合は、セミコロン (;) で区切ります。 <p>選択可能なタイプ：</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL コンテンツの長さ（バイト単位）]</td>
      <td>
        <p>コンテンツの長さをバイト単位で入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを含むカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>ファイルのレンディションを作成するアセットの ID を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### カタログアセットの取得

このアクションモジュールは、カタログ内の 1 つのアセットに関する情報を取得します。 カタログは、このモジュールで使用される接続で資格情報が表されるユーザーが所有する必要があります。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを含むカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>情報を取得するアセットの ID を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>


#### 最新のアセットの外部XMP開発設定ファイルを取得します

このアクションモジュールは、最新のアセット外部XMP設定ファイルを取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを含むカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>XMP開発設定ファイルに関連付けられているアセットの ID を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### 最新のアセットレンディションを取得する

このアクションモジュールは、指定されたタイプの最新のアセットレンディションを取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを含むカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>XMP開発設定ファイルに関連付けられているアセットの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レンディションタイプ ]</td>
      <td>
        <p>取得するレンディションのタイプを選択します。</p>
      </td>
    </tr>
  </tbody>
</table>

#### アセットの取得

このアクションモジュールは、このモジュールで使用される接続に資格情報が表示されるユーザーが所有するアセットを取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを含むカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 開始タイムスタンプ ]</td>
      <td>
        <p>タイムスタンプを入力またはマッピングします。 モジュールは、このタイムスタンプの後に更新されたレコードを返します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 以前に取り込んだアセットを返す ]</td>
      <td>
        <p>フォーマットを持つ日付を入力 <code>YYYY-MM-DDT00:00:00</code>. このモジュールは、この日付より前にキャプチャされた結果を返します。</p><p> このフィールドは、フィールドと共に使用できません <code>Return assets captured after</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 返されるアセットの最大数 ]</td>
      <td>
        <p>アセットの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。 この数は 100 以下にする必要があります。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SHA256 元のファイルのハッシュ値 ]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL スタック内のアセットを非表示にする？"]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アセットサブタイプ値 ]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset IDs]</td>
      <td>
        <p>最大 100 個のアセット ID をコンマで区切って入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 除外するアセットのタイプ ]</td>
      <td>
        <p>完全なアセットまたは不完全なアセットを除外する場合に選択します。 すべてのアセットを含める場合は、このフィールドを空白のままにします。</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL グループ値 ]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 名前の値 ]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL お気に入りのステータス ]</td>
      <td>
        <p></p>
      </td>
    </tr>
    </tr>
  </tbody>
</table>

### アルバム

* [アルバムへのアセットの追加](#add-assets-to-an-album)
* [アルバムの作成](#create-an-album)
* [アルバムの削除](#delete-an-album)
* [アルバムの取得](#get-an-album)
* [アルバムのアセットのリスト](#list-assets-of-an-album)
* [アルバムの取得](#retrieve-albums)
* [アルバムの更新](#update-album)

#### アルバムへのアセットの追加

このアクションモジュールは、指定したアルバムに 1 つ以上のアセットを追加します。 1 回の実行サイクルで最大 50 個のアセットを追加できます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アセットを追加するアルバムが含まれるカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アルバム ID]</td>
      <td>
        <p>アセットを追加するアルバムの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Assets]</td>
      <td>
        <p>アルバムに追加するアセットごとに、 <b>項目を追加</b> 次のフィールドを入力します。</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>アルバムに追加するアセットの ID を入力またはマッピングします</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL このアセットはアルバムの表紙ですか？]</td>
      <td>
        <p>このアセットをアルバムを表す画像として表示するかどうかを選択します。</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Order]</td>
      <td>
        <p></p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Metadata]</td>
      <td>
        <p>アセットに含めるメタデータを入力またはマッピングします。 最大長が 1 ～ 24 文字の 1 つのテキスト文字列を指定する必要があります。</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL リモート ID]</td>
      <td>
        <p>アセットの識別子を入力します。</p>
      </td>
    </tr>
  </tbody>
</table>

#### アルバムの作成

このアクションモジュールは、Lightroomで新しいアルバムを作成します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>アルバムを作成するカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アルバム ID]</td>
      <td>
        <p>新しいアルバムの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtype]</td>
      <td>
        <p>アルバムのサブタイプを選択します。</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL API キー ]</td>
      <td>
        <p>アルバムを作成するサービスの API キーを入力します。</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 作成日時ユーザー ]</td>
      <td>
        <p>日付を形式で入力またはマッピング <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime ユーザーが更新されました ]</td>
      <td>
        <p>日付を形式で入力またはマッピング <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アルバム名 ]</td>
      <td>
        <p>新しいアルバムの名前を入力またはマッピングします。</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL カバー ID]</td>
      <td>
        <p>このアルバムのカバーとして使用するアセットの ID を入力またはマッピングします。</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL リモート ID]</td>
      <td>
        <p>アセットの識別子を入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Created date]</td>
      <td>
        <p>日付を形式で入力またはマッピング <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL 更新日 ]</td>
      <td>
        <p>日付を形式で入力またはマッピング <code>YYYY-MM-DDT00:00:00-00:00Z</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アルバムは削除されますか？]</td>
      <td>
        <p>外部関連コンテンツが削除された場合は、このオプションを有効にします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 関連コンテンツを編集する場所の URL]</td>
      <td>
        <p>ユーザーがこのアルバムのコンテンツを編集できる URL がある場合は、ここに URL を入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 関連コンテンツを表示する場所の URL]</td>
      <td>
        <p>ユーザーがこのアルバムのコンテンツを表示できる URL がある場合は、ここに URL を入力します。</p>
      </td>
    </tr>
  </tbody>
</table>

#### アルバムの削除

このアクションモジュールはアルバムを削除します。

削除されたアルバムは、削除中のクライアントアプリと同じクライアントアプリで作成されている必要があります。また、サブタイプである必要があります `project` または `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>削除するアルバムを含むカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アルバム ID]</td>
      <td>
        <p>削除するアルバムの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 子アルバムを削除しますか？]</td>
      <td>
        <p>削除したアルバムの子アルバムを削除するかどうかを選択します。</p>
      </td>
    </tr>
  </tbody>
</table>

### アルバムの取得

このアクションモジュールは、指定されたアルバムを取得します

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>取得するアルバムが含まれるカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アルバム ID]</td>
      <td>
        <p>取得するアルバムの ID を入力またはマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### アルバムのアセットのリスト

このアクションモジュールは、指定したアルバム内のアセットのリストを取得します。



#### アルバムの取得

このアクションモジュールは、指定されたカタログ内のアルバムのリストを取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>取得するアルバムが含まれるカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Subtypes]</td>
      <td>
        <p>取得するアルバムの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 現在の結果の前に配置するアルバムの名前 ]</td>
      <td>
        <p>結果にページ番号を付ける場合は、前のページの最後のアルバムの名前を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 返されるアルバムの最大数 ]</td>
      <td>
        <p>アセットの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。 このフィールドのデフォルト値は 100 です。制限の境界にある複数のアルバムが同じである場合、このモジュールはこの制限を超えるアルバムを返す可能性があります <code>name_after</code> の値です。</p>
      </td>
    </tr>
  </tbody>
</table>

#### アルバムを更新

このアクションモジュールは、指定されたアルバムを更新します。

更新されたアルバムは、更新中のクライアントアプリと同じクライアントアプリで作成されている必要があり、サブタイプである必要があります `project` または `project_set`.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Lightroom] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >[!DNL Adobe Lightroom]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL カタログ ID]</td>
      <td>
        <p>更新するアルバムが含まれるカタログの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アルバム ID]</td>
      <td>
        <p>更新するアルバムの ID を入力またはマッピングします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">その他のフィールド</td>
      <td>
      <td>このモジュールの他のフィールドの説明については、 <a href="#create-an-album" class="MCXref xref" >アルバムの作成</a> 」を参照してください。</td>
      </td>
    </tr>
  </tbody>
</table>










