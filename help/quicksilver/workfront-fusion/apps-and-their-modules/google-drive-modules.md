---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google Drive のモジュール
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '3012'
ht-degree: 95%

---

# [!DNL Google Drive] モジュール

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [Google ドライブ モジュール ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-drive-modules.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

[!DNL Adobe Workfront Fusion] [!DNL Google Drive] モジュールを使用すると、[!DNL Google Drive] 内のファイル、フォルダー、または共有ドライブを監視、検索、作成、更新、削除、管理できます。

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Google Drive] アカウントを複数のサードパーティのアプリケーションとサービスに接続できます。

シナリオの作成手順について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) のシナリオの作成を参照してください。

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
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] の [!DNL Adobe Workfront] プランがある場合、この記事に記載されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] の購入 [!DNL Adobe Workfront] 必要です。 [!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## Google Drive API に関する情報

Google ドライブコネクタは以下を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ベース URL</td> 
   <td> https://www.googleapis.com/drive/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API バージョン</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API タグ</td> 
   <td>v4.1.22</td> 
  </tr>
 </tbody> 
 </table>



## [!DNL Google Drive] を [!DNL Workfront Fusion] に接続

[!DNL @gmail.com] または [!DNL @googlemail.com] ユーザーの場合は、[!UICONTROL クライアント ID] と[!UICONTROL クライアントシークレット]を取得するために、[ [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) に OAuth クライアントを作成する必要があります。

OAuth クライアントを作成（および[!UICONTROL クライアント ID] と[!UICONTROL クライアントシークレット]を取得）する手順について詳しくは、[カスタム OAuth クライアントを使用した  [!DNL Adobe Workfront Fusion]  と  [!DNL Google Services]  の接続](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)を参照してください。

[!DNL Google Drive] アカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、[[!UICONTROL Adobe Workfront Fusion] への接続の作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)を参照してください。

## [!DNL Google Drive] モジュールとそのフィールド

[!DNL Google Drive] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Google Drive] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) におけるモジュール間の情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)



* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

* [[!UICONTROL フォルダー内のファイルを監視]](#watch-files-in-folder)
* [[!UICONTROL すべてのファイルを監視]](#watch-all-files)
* [[!UICONTROL 共有ファイルを監視]](#watch-shared-files)
* [[!UICONTROL コメントを監視]](#watch-comments)

#### [!UICONTROL フォルダー内のファイルを監視]

指定されたフォルダーにファイルが追加または変更されると、ファイルの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Select the folder to be watched]</td>
    <td >ファイルを監視したいドライブ上のフォルダーを選択します。</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL What files to watch]</td>
   <td> <p>監視するファイルの種類を選択します。</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convert [!DNL Google Documents] files to format]</td>
    <td>[!DNL Google Documents] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Spreadsheets] files to format]</td>
    <td>[!DNL Google Spreadsheets] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Slides] files to format]</td>
    <td>[!DNL Google Slides] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Drawings] files to format]</td>
    <td>[!DNL Google Drawings] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Watch]</td>
    <td>新規ファイルとすべての変更を監視するか、新規ファイルのみを監視するかを選択します。</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL Maximum number of downloaded files]</td>
    <td>1 回のサイクル中に [!DNL Workfront Fusion] がダウンロードする結果の最大数（シナリオ実行あたりの繰り返し数）を設定します。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL すべてのファイルの監視]

[!DNL Google Drive] 内のファイルが追加または変更されたときに、ファイルの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] への [!DNL Google Drive] の接続</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL What files to watch]</td> 
   <td> <p>監視するファイルの種類を選択します。</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convert [!DNL Google Documents] files to format]</td>
    <td>[!DNL Google Documents] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Spreadsheets] files to format]</td>
    <td>[!DNL Google Spreadsheets] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Slides] files to format]</td>
    <td>[!DNL Google Slides] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Drawings] files to format]</td>
    <td>[!DNL Google Drawings] の変換先のファイル形式を選択します。</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>新規ファイルとすべての変更を監視するか、新規ファイルのみを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of downloaded files]</td> 
   <td>1 回のサイクル中に [!DNL Workfront Fusion] がダウンロードする結果の最大数（シナリオ実行あたりの繰り返し回数）を設定します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 共有ファイルの監視]

新規ファイルが共有されたときや、既存の共有ファイルが更新されたときにトリガーされます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select the folder to be watched]</td> 
   <td>監視するファイルが含まれている共有フォルダーを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL What files to watch]</td> 
   <td> <p>監視するファイルの種類を選択します。</p> 
    <ul> 
     <li>[!UICONTROL All]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL Convert [!DNL Google Documents] files to format]</td>
    <td>[!DNL Google Documents] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Spreadsheets] files to format]</td>
    <td>[!DNL Google Spreadsheets] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Slides] files to format]</td>
    <td>[!DNL Google Slides] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Convert [!DNL Google Drawings] files to format]</td>
    <td>[!DNL Google Drawings] の変換先のファイル形式を選択します。</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>新規ファイルとすべての変更を監視するか、新規ファイルのみを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of downloaded files]</td> 
   <td>1 回のサイクル中で [!DNL Workfront Fusion] がダウンロードする結果の最大数（シナリオ実行あたりの繰り返し数）を設定します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントを監視]

選択したファイルにコメントが追加または変更されたときにトリガーされます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File]</td> 
   <td>コメントを監視するファイルを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td>すべての変更を監視するか、新しいコメントのみを監視するかを選択</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned comments]</td> 
   <td>1 回のサイクル中で [!DNL Workfront Fusion] が返すコメントの最大数（シナリオ実行ごとの繰り返し数）を設定します。</td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL ファイルをアップロード]](#upload-a-file)
* [[!UICONTROL ファイルを更新]](#update-a-file)
* [[!UICONTROL ファイルをコピー]](#copy-a-file)
* [[!UICONTROL ファイルを削除]](#delete-a-file)
* [[!UICONTROL ファイル／フォルダーをごみ箱に移動]](#move-a-filefolder-to-trash)
* [[!UICONTROL ファイルを取得]](#get-a-file)
* [[!UICONTROL ファイル／フォルダを検索]](#search-for-filesfolders)
* [[!UICONTROL フォルダーを作成]](#create-a-folder)
* [[!UICONTROL 共有リンクを取得]](#get-a-share-link)

#### [!UICONTROL ファイルをアップロード]

ファイルを [!DNL Google Drive] にアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Destination]</td> 
   <td> <p>ファイルのアップロード先を選択します。</p> 
    <ul> 
     <li>[!DNL My Drive]</li> 
     <li>[!DNL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target folder]</td> 
   <td>ファイルをアップロードするフォルダーを選択します。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td>以前のモジュールから渡されたファイルを使用するか、ファイルを手動でマッピングするかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td>ファイル名を選択します。このオプションは、「[!UICONTROL source file]」フィールドで「[!UICONTROL Map]」を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>アップロードするデータファイルを選択します。このオプションは、「[!UICONTROL source file]」フィールドで「[!UICONTROL Map]」を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>新規ファイルのタイトルを入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert a file]</td> 
   <td>このオプションを有効にすると、モジュールはファイルを対応する [!DNL Google] 形式に変換できます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルを更新]

ファイルのメタデータまたはコンテンツを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>ファイルのアップロード先を選択します。</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Move to a folder]</td> 
   <td>ファイルを別のフォルダーに移動する場合は、ファイルの移動先のフォルダーを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>更新するファイルの ID をマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Title]</td> 
   <td>更新されたファイルのタイトルを入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Change a file content]</td> 
   <td>ファイルのコンテンツを置き換えるかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td>以前のモジュールから渡されたファイルを使用するか、ファイルを手動でマッピングするかを選択します。このフィールドは、前のフィールドでファイルの内容を変更することを選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td>ファイル名を選択します。このオプションは、「[!UICONTROL source file]」フィールドで「[!UICONTROL Map]」を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data]</td> 
   <td>アップロードするデータファイルを選択します。このオプションは、「[!UICONTROL source file]」フィールドで「[!UICONTROL Map]」を選択した場合に使用できます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをコピー]

ファイルを新しい場所にコピーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>ファイルのアップロード先を選択します。</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Target folder]</td> 
   <td>コピーするファイルが存在するフォルダーを選択します</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>更新するファイルの ID をマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL The name of the copy]</td> 
   <td>新規ファイルのタイトルを入力します。元のファイル名を変更しない場合は、このフィールドを空白のままにしておきます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルを削除]

ファイルまたはフォルダを完全に削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>削除するファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル／フォルダーをごみ箱に移動]

ファイルまたはフォルダーをごみ箱に移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>ゴミ箱に移動するファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルを取得]

指定された ID を持つファイルを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Documents] files to format]</td> 
   <td>[!DNL Google Documents] の変換先のファイル形式を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Spreadsheets] files to format]</td> 
   <td>[!DNL Google Spreadsheets] の変換先のファイル形式を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Slides] files to format]</td> 
   <td>[!DNL Google Slides] の変換先のファイル形式を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Convert [!DNL Google Drawings] files to format]</td> 
   <td>[!DNL Google Drawings] の変換先のファイル形式を選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>取得するファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル／フォルダを検索]

検索条件に基づいてファイルまたはフォルダーを検索します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>検索先を選択します。</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL List a folder]</td> 
   <td>ファイルまたはフォルダーを検索するフォルダーに移動します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Retrieve]</td> 
   <td> <p> 検索対象を、ファイル、フォルダまたはその両方から選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Search]</p> </td> 
   <td> <p>実行する検索のタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Search within file/folder names]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>検索するファイル名の一部または完全なファイル名（拡張子を含む）を入力します。</p> </li> 
       <li> <p><strong>[!UICONTROL Search Options]</strong> </p> <p>完全に一致する用語を検索するか、検索語を含む名前を検索するかを選択します。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Fulltext]検索</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>[!DNL Google Drive] で検索する検索語を入力します。</p> </li> 
      </ul> </li> 
     <li> <p><strong>カスタム検索クエリを入力</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Query]</strong> </p> <p>カスタム検索クエリを入力します。詳しくは、この記事の[!UICONTROL Search for Files]の節を参照してください。</p> </li> 
       <li> <p><strong>上記で選択したフォルダをクエリに追加</strong> </p> <p>親コレクション内のフォルダーを検索します。これにより、上記で選択したフォルダー内にあるすべてのファイルとフォルダーが検索されます。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned results]</td> 
   <td>[!DNL Workfront Fusion] の 1 回の実行サイクルで返されるファイルまたはフォルダーの最大数を設定します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td>モジュールが結果を返さない場合にシナリオが停止しないようにするには、このオプションを有効にします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーを作成]

指定された場所にフォルダーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination]</td> 
   <td> <p>ファイルのアップロード先を選択します。</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared with Me]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New folder location]</td> 
   <td>新規フォルダーを作成する場所に移動します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL The name of the new folder]</td> 
   <td>作成するフォルダーの名前を入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Share folder]</td> 
   <td>[!UICONTROL Share]リンクを使用してこのフォルダーを他のユーザーと共有する場合は、このオプションを選択します。選択しない場合、共有リンクを使用できるのは所有者のみになります。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 共有リンクの取得]

Google Drive 内のファイルの共有リンクを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Google Drive] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">[!DNL Google Drive] を [!UICONTROL Workfront Fusion] に接続する</a> を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File ID]</td> 
   <td>取得する共有リンクの対象ファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

## トラブルシューティング

### ファイルをアップロードまたは更新できない

ファイルのアップロードまたは更新に失敗する状況はいくつかあります。

* アップロードされたファイルが大きすぎて、[!DNL Google Drive] プランで許可されている最大ファイルサイズ制限を超えているか、[!DNL Google Drive] のストレージ制限を超えています。ストレージプランをアップグレードするか、[!DNL Google Drive] サービスから既存のファイルを削除することができます。
* ファイルのアップロード先として選択したフォルダーが存在しません。シナリオが停止するので、ターゲットフォルダーを再度選択する必要があります。

## ファイルの検索

フォルダーの「ファイルのリスト」モジュールでは、次の要素で構成される独自のクエリを使用できます。

* **[!UICONTROL フィールド]** - 検索するファイルの属性（例：ファイルの `name` 属性）。

* **[!UICONTROL 演算子]** - 照合するためにデータに対して実行されるテスト（例：`contains`）。

* **[!UICONTROL 値]** - テストされる属性の内容（例：ファイル名 `My cool document`）

接続詞「`and`」または「`or`」で句を結合したり、「`not`」でクエリを否定したりできます。

* [フィールド](#fields)
* [値のタイプ](#value-types)
* [演算子](#operators)
* [例](#examples)

### フィールド

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>フィールド </th> 
   <th>値のタイプ </th> 
   <th>演算子</th> 
   <th> <p> 説明</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>[!UICONTROL title]</code></td> 
   <td>文字列</td> 
   <td><code>contains</code><sup>1</sup>、<code>=</code>、 <code>!=</code></td> 
   <td> <p> ファイルの名前</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>文字列 </td> 
   <td><code>contains</code><sup>2、3</sup> </td> 
   <td> <p> ファイルのテキスト全体（名前、説明、内容、インデックス付け可能なテキストなどを含む）。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> 文字列</td> 
   <td><code>contains</code>、<code>=</code>、 <code>!=</code></td> 
   <td> <p> ファイルの MIME タイプ</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> 日付<sup>4</sup></td> 
   <td><code> &lt;=</code>、<code>&lt;</code>、<code>=</code>、<code>!=</code>、<code>></code>、 <code>>=</code></td> 
   <td> <p> ファイルが最後に変更された日付。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> ユーザーが最後にファイルを表示した日付。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>ブール値 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> ファイルがごみ箱に入っているかどうか。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>ブール値 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>ファイルがスター付きかどうか。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>コレクション </td> 
   <td><code>in </code> </td> 
   <td> <p>[!UICONTROL parents]コレクションに指定した ID が含まれているかどうか。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL owners]</code></td> 
   <td>コレクション </td> 
   <td><code>in </code> </td> 
   <td> <p>ファイルを所有しているユーザー。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL writers]</code></td> 
   <td>コレクション </td> 
   <td><code>in </code> </td> 
   <td> <p>ファイルを変更する権限を持つユーザー。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL readers] </code> </td> 
   <td>コレクション </td> 
   <td><code>in </code> </td> 
   <td> <p>ファイルを読み取る権限を持つユーザー。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL sharedWithMe]</code> </td> 
   <td>ブール値 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> ユーザーの「自分と共有」コレクションにあるファイル。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL properties] </code> </td> 
   <td>コレクション</td> 
   <td><code>has </code> </td> 
   <td> <p> パブリックカスタムファイルプロパティ。</p> </td> 
  </tr> 
 </tbody> 
</table>

これらのフィールドの演算子について、次の点を考慮してください。

* `contains` 演算子は、`title` に対する接頭辞一致検索のみを実行します。

  例えば、「HelloWorld」というタイトルは、`title contains 'Hello'` に一致しますが、`title contains 'World'` には一致しません。

* `contains` 演算子は、`fullText` 文字列トークン全体に対してのみ一致検索を実行します。

  例えば、ドキュメントの全文に「HelloWorld」という文字列が含まれている場合、クエリ `fullText contains 'HelloWorld'` のみが結果を返します。このシナリオでは、クエリ `fullText contains 'Hello'` は結果を返しません。

* `contains` 演算子は、二重引用符で囲まれた英数字句と完全一致します。

  例えば、ドキュメントの `fullText` が「Hello there world」という文字列を含む場合、クエリ `fullText contains '"Hello there"'` は結果を返しますが、クエリは `fullText contains '"Hello world"'` は結果を返しません。

  さらに、検索は英数字なので、ドキュメントの `fullText` に「Hello_world」という文字列が含まれている場合、クエリ `fullText contains '"Hello world"'` は結果を返します。

* `type`が日付のフィールドは現在、互いに比較することはできず、定数の日付とのみ比較できます。

### 値のタイプ

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>値のタイプ</th> 
   <th> <p> メモ</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>文字列 </td> 
   <td> <p>一重引用符 ’ で囲みます。クエリ内の一重引用符は <code>\'</code> でエスケープします、例：<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>ブール値 </td> 
   <td> <p><code>true </code>または <code>false</code></p> </td> 
  </tr> 
  <tr> 
   <td>日付 </td> 
   <td> <p>RFC 3339 形式。デフォルトタイムゾーンは UTC です。例：<code>2012-06-04T12:00:00-08:00</code></p> </td> 
  </tr> 
 </tbody> 
</table>

### 演算子

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>演算子 </th> 
   <th> <p>メモ</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>一方の文字列の内容がもう一方の文字列に存在します。</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> 文字列またはブール値の内容が他の内容と同じです。</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> 文字列またはブール値の内容が他の内容と等しくありません。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> 日付が別の日付より前です。</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> 日付が別の日付より前か等しいです。</p> </td> 
  </tr> 
  <tr> 
   <td><code>></code> </td> 
   <td> <p> 日付が別の日付より後です。</p> </td> 
  </tr> 
  <tr> 
   <td><code>>=</code> </td> 
   <td> <p> 日付が他の日付より後か等しいです。</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>要素がコレクション内に含まれます。</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>両方の句に一致するファイルを返します。</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>どちらかの句に一致するファイルを返します。</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>検索句を否定します。</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>コレクションには、パラメーターに一致する要素が含まれます。</p> </td> 
  </tr> 
 </tbody> 
</table>

複合句の場合は、括弧を使用して句をグループ化できます。例：
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` この検索では、2012年6月4日（PT）以降に最終変更された画像またはビデオのうち、MIME タイプを持つすべてのファイルが返されます。`and` 演算子と `or` 演算子は括弧なしで左から右に評価されるため、上記の例では、画像に関しては、2012年6月4日（PT）以降に変更された画像のみが返されますが、ビデオに関しては、2012年6月4日（PT）より前のビデオも含めすべてのビデオが返されます。

### 例

このページのすべての例は、エンコードされていない `<q>q</q>` パラメーターを示しています。`title = 'hello'` は `title+%3d+%27hello%27` としてエンコードされています。クライアントライブラリは、このエンコーディングを自動的に処理します。

* 「hello」という名前のファイルを検索する
  <pre>title = 'hello'</pre>
* フォルダー固有の MIME タイプを使用したフォルダーを検索する
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* フォルダー以外のファイルを検索する
  <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* 「hello」と「goodbye」という単語を含む名前のファイルを検索する
  <pre>title contains 'hello' and [!UICONTROL name] contains 'goodbye'</pre>
* 「hello」という語を含まない名前のファイルを検索する
  <pre>not title contains 'hello'</pre>
* コンテンツ内に「hello」という単語を含むファイルを検索する
  <pre>fullText contains 'hello'</pre>
* コンテンツ内に「hello」という単語を含まないファイルを検索する
  <pre>not fullText contains 'hello'</pre>
* コンテンツ内に「hello world」という完全なフレーズを含むファイルを検索する
  <pre>fullText contains '"hello world"'fullText contains '"hello_world"'</pre>
* クエリに「\」文字を含むファイルを検索する（例：「\authors」）
  <pre>fullText contains '\\authors'</pre>
* ユーザー `test@example.org` によって書き込み可能なファイルを検索します。
  <pre>'test@example.org' in [!DNL writers]</pre>
* `parents` コレクションで ID `1234567` を検索する。これにより、ID が `1234567` のフォルダーの直下にあるすべてのファイルとフォルダーを検索されます。
  <pre>'1234567' in [!UICONTROL parents]</pre>
* `parents` コレクションでエイリアス ID `appDataFolder` を検索する。これにより、[Application Data フォルダー](https://developers.google.com/drive/api/v2/appdata)の直下にあるすべてのファイルとフォルダーが検索されます。
  <pre>'appDataFolder' in parents</pre>
* ユーザー `test@example.org` および `test2@example.org` によって書き込み可能なファイルを検索します。
  <pre>'test@example.org' in writers and 'test2@example.org' in writers</pre>
* ごみ箱に入っている、「important」というテキストを含むファイルを検索する
  <pre>fullText contains 'important' and trashed = true</pre>
* 2012年6月4日（PT）以降に変更されたファイルを検索する
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' //デフォルトタイムゾーンは UTC©</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* 名前に「hello」を含む、認証済みユーザーと共有されているファイルを検索する
  <pre>sharedWithMe and title contains 'hello'</pre>
* 値 `8e8aceg2af2ge72e78` を含む `additionalID` という名前の[カスタムファイルプロパティ](https://developers.google.com/drive/api/v2/properties)を持つファイルを検索する
  <pre>properties has { key='additionalID' and value='8e8aceg2af2ge72e78' and visibility='PRIVATE' }</pre>

このガイドの出典は、[[!DNL Google Drive]  ドキュメント](https://developers.google.com/drive/api/v2/search-shareddrives)です。
