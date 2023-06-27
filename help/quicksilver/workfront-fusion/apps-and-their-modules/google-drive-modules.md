---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google Drive モジュール
description: この [!DNL Adobe Workfront Fusion Google Drive] モジュールを使用すると、内のファイル、フォルダ、または共有ドライブを監視、検索、作成、更新、削除、管理できます [!DNL Google Drive].
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 7d620c93-d1bf-4451-9f76-1d6fd850cec9
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2956'
ht-degree: 0%

---

# [!DNL Google Drive] モジュール

この [!DNL Adobe Workfront Fusion] [!DNL Google Drive] モジュールを使用すると、内のファイル、フォルダ、または共有ドライブを監視、検索、作成、更新、削除、管理できます [!DNL Google Drive].

内 [!DNL Adobe Workfront Fusion] シナリオに従って、 [!DNL Google Drive] を複数のサードパーティのアプリケーションおよびサービスにアカウントする。

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## 接続中 [!DNL Google Drive] から [!DNL Workfront Fusion]

次の場合、 [!DNL @gmail.com] または [!DNL @googlemail.com] OAuth クライアントを [の [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 得るために [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵].

OAuth クライアントの作成 ( および [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵]) を参照してください。 [接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントの使用](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

接続方法 [!DNL Google Drive] アカウント [!UICONTROL Workfront Fusion]を参照してください。 [への接続の作成 [!UICONTROL Adobe Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Google Drive] モジュールとそのフィールド

設定時に [!DNL Google Drive] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Google Drive] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

* [[!UICONTROL フォルダ内のファイルを監視する]](#watch-files-in-folder)
* [[!UICONTROL すべてのファイルを監視]](#watch-all-files)
* [[!UICONTROL 共有ファイルを監視する]](#watch-shared-files)
* [[!UICONTROL コメントを見る]](#watch-comments)

#### [!UICONTROL フォルダ内のファイルを監視する]

指定されたフォルダー内でファイルが追加または変更された場合に、ファイルの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL 接続 ] </td>
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL 監視するフォルダーを選択 ]</td>
    <td >ファイルを監視するドライブ上のフォルダを選択します。</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL 監視するファイル</td>
   <td> <p>監視するファイルの種類を選択します。</p> 
    <ul> 
     <li>[!UICONTROL すべて ]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL 変換 [!DNL Google Documents] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Documents] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Spreadsheets] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Spreadsheets] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Slides] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Slides] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Drawings] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Drawings] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ウォッチ ]</td>
    <td>新しいファイルとすべての変更を監視するか、新しいファイルのみを監視するかを選択します。</td>
  </tr> 
  <tr> 
    <td>[!UICONTROL ダウンロードされたファイルの最大数 ]</td>
    <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクル（シナリオ実行あたりの繰り返し数）中にダウンロードされます。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL すべてのファイルを監視]

ファイルが [!DNL Google Drive] が追加または変更された。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 監視するファイル</td> 
   <td> <p>監視するファイルの種類を選択します。</p> 
    <ul> 
     <li>[!UICONTROL すべて ]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL 変換 [!DNL Google Documents] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Documents] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Spreadsheets] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Spreadsheets] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Slides] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Slides] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Drawings] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Drawings] からへ</td>
  </tr>  
  <tr> 
   <td>[!UICONTROL ウォッチ ]</td> 
   <td>新しいファイルとすべての変更を監視するか、新しいファイルのみを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ダウンロードされたファイルの最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクル（シナリオ実行あたりの繰り返し数）中にダウンロードされます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 共有ファイルを監視する]

トリガー：新しいファイルが自分に共有されたとき、または既存の共有ファイルが更新されたとき。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 監視するフォルダーを選択 ]</td> 
   <td>ファイルを監視する共有フォルダを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 監視するファイル</td> 
   <td> <p>監視するファイルの種類を選択します。</p> 
    <ul> 
     <li>[!UICONTROL すべて ]</li> 
     <li>[!DNL Google Documents]</li> 
     <li>[!DNL Google Spreadsheets]</li> 
     <li>[!DNL Google Slides]</li> 
     <li>[!DNL Google Drawings]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >[!UICONTROL 変換 [!DNL Google Documents] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Documents] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Spreadsheets] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Spreadsheets] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Slides] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Slides] からへ</td>
  </tr> 
  <tr>
    <td>[!UICONTROL 変換 [!DNL Google Drawings] 形式設定するファイル</td>
    <td>変換するファイル形式を選択します [!DNL Google Drawings] からへ</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL ウォッチ ]</td> 
   <td>新しいファイルとすべての変更を監視するか、新しいファイルのみを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ダウンロードされたファイルの最大数 ]</td> 
   <td>結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクル（シナリオ実行あたりの繰り返し数）中にダウンロードされます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントを見る]

トリガー（選択したファイルにコメントが追加または変更された場合）

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ]</td> 
   <td>コメントを監視するファイルを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ウォッチ ]</td> 
   <td>すべての変更を監視するか、新しいコメントのみを監視するかを選択します</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返されたコメントの最大数 ]</td> 
   <td>コメントの最大数を設定 [!DNL Workfront Fusion] は、1 サイクル（シナリオ実行あたりの繰り返し数）中に返されます。</td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL ファイルのアップロード]](#upload-a-file)
* [[!UICONTROL ファイルの更新]](#update-a-file)
* [[!UICONTROL ファイルのコピー]](#copy-a-file)
* [[!UICONTROL ファイルの削除]](#delete-a-file)
* [[!UICONTROL ファイル/フォルダーをごみ箱に移動]](#move-a-filefolder-to-trash)
* [[!UICONTROL ファイルの取得]](#get-a-file)
* [[!UICONTROL ファイル/フォルダを検索]](#search-for-filesfolders)
* [[!UICONTROL フォルダーの作成]](#create-a-folder)
* [[!UICONTROL 共有リンクを取得]](#get-a-share-link)

#### [!UICONTROL ファイルのアップロード]

ファイルを [!DNL Google Drive].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
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
   <td>[!UICONTROL ターゲットフォルダー ]</td> 
   <td>ファイルのアップロード先のフォルダーを選択します。 </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソースファイル ]</td> 
   <td>以前のモジュールから渡されたファイルを使用するか、手動でファイルをマッピングするかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル名 ]</td> 
   <td>ファイル名を選択します。 このオプションは、[!UICONTROL ソースファイル ] フィールドで「[!UICONTROL Map]」を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL データ ]</td> 
   <td>アップロードするデータファイルを選択します。 このオプションは、[!UICONTROL ソースファイル ] フィールドで「[!UICONTROL Map]」を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイトル ]</td> 
   <td>新しいファイルのタイトルを入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルの変換 ]</td> 
   <td>このオプションを有効にすると、モジュールは、 [!DNL Google] 形式</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの更新]

ファイルのメタデータまたはコンテンツを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 宛先 ]</td> 
   <td> <p>ファイルのアップロード先を選択します。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダーに移動 ]</td> 
   <td>ファイルを別のフォルダーに移動する場合は、ファイルの移動先のフォルダーを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td>更新するファイルの ID をマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイトル ]</td> 
   <td>更新したファイルのタイトルを入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルコンテンツの変更 ]</td> 
   <td>ファイルのコンテンツを置き換えるかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソースファイル ]</td> 
   <td>以前のモジュールから渡されたファイルを使用するか、手動でファイルをマッピングするかを選択します。 このフィールドは、前のフィールドでファイルの内容を変更することを選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル名 ]</td> 
   <td>ファイル名を選択します。 このオプションは、[!UICONTROL ソースファイル ] フィールドで「[!UICONTROL Map]」を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL データ ]</td> 
   <td>アップロードするデータファイルを選択します。 このオプションは、[!UICONTROL ソースファイル ] フィールドで「[!UICONTROL Map]」を選択した場合に使用できます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのコピー]

ファイルを新しい場所にコピーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 宛先 ]</td> 
   <td> <p>ファイルのアップロード先を選択します。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ターゲットフォルダー ]</td> 
   <td>コピーするファイルが存在するフォルダを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td>更新するファイルの ID をマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コピーの名前 ]</td> 
   <td>新しいファイルのタイトルを入力します。 元のファイル名を変更しない場合は、このフィールドを空白のままにします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの削除]

ファイルまたはフォルダを完全に削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td>削除するファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル/フォルダーをごみ箱に移動]

ファイルまたはフォルダをごみ箱に移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td>ごみ箱に移動するファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの取得]

指定された ID を持つファイルを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Documents] 形式設定するファイル</td> 
   <td>変換するファイル形式を選択します [!DNL Google Documents] からへ</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Spreadsheets] 形式設定するファイル</td> 
   <td>変換するファイル形式を選択します [!DNL Google Spreadsheets] からへ</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Slides] 形式設定するファイル</td> 
   <td>変換するファイル形式を選択します [!DNL Google Slides] からへ</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Drawings] 形式設定するファイル</td> 
   <td>変換するファイル形式を選択します [!DNL Google Drawings] からへ</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td>取得するファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル/フォルダを検索]

検索条件に基づいてファイルまたはフォルダを検索します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 宛先 ]</td> 
   <td> <p>検索する宛先を選択します。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダーのリストを表示 ]</td> 
   <td>ファイルまたはフォルダーを検索するフォルダーに移動します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 取得 ]</td> 
   <td> <p> ファイル、フォルダ、またはその両方を検索するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 検索 ]</p> </td> 
   <td> <p>実行する検索のタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイル名/フォルダー名内を検索 ]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL クエリ ]</strong> </p> <p>検索するファイル名の一部または完全なファイル名（サフィックスを含む）を入力します。</p> </li> 
       <li> <p><strong>[!UICONTROL 検索オプション ]</strong> </p> <p>正確な語句を検索するか、検索語句を含む名前を検索するかを選択します。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL フルテキスト ] 検索</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL クエリ ]</strong> </p> <p>検索したい検索語句を [!DNL Google Drive].</p> </li> 
      </ul> </li> 
     <li> <p><strong>カスタム検索クエリを入力</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL クエリ ]</strong> </p> <p>カスタム検索クエリを入力します。 詳しくは、この記事の [!UICONTROL ファイルの検索 ] の節を参照してください。</p> </li> 
       <li> <p><strong>上で選択したフォルダーをクエリに追加します。</strong> </p> <p>親コレクション内のフォルダーを検索します。 これにより、上で選択したフォルダー内にあるすべてのファイルとフォルダーが検索されます。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返される結果の最大数 ]</td> 
   <td>ファイルまたはフォルダーの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL モジュールが結果を返さない場合でも、ルートの実行を続行します ]</td> 
   <td>モジュールが結果を返さない場合にシナリオが停止しないようにするには、このオプションを有効にします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーの作成]

指定された場所にフォルダを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 宛先 ]</td> 
   <td> <p>ファイルのアップロード先を選択します。</p> 
    <ul> 
     <li>[!UICONTROL マイドライブ ]</li> 
     <li>[!UICONTROL 自分と共有 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 新しいフォルダーの場所 ]</td> 
   <td>新しいフォルダーを作成する場所に移動します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 新しいフォルダーの名前 ]</td> 
   <td>作成するフォルダの名前を入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダーを共有 ]</td> 
   <td>[!UICONTROL 共有 ] リンクを使用しているすべてのユーザーとフォルダーを共有する場合は、このオプションを選択します。 そうしないと、共有リンクは所有者専用になります。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 共有リンクを取得]

Google Drive 内のファイルの共有リンクを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">接続中 [!DNL Google Drive] から [!UICONTROL Workfront Fusion]</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td>共有リンクを取得するファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

## トラブルシューティング

### ファイルをアップロードまたは更新できません

ファイルのアップロードまたは更新に失敗する状況はいくつかあります。

* アップロードされたファイルが大きすぎて、ファイルサイズの上限を超えています [!DNL Google Drive] プランを作成するか、 [!DNL Google Drive] ストレージの制限。 ストレージプランをアップグレードするか、 [!DNL Google Drive] サービス。
* ファイルのアップロード先として選択したフォルダは存在しません。 シナリオが停止し、ターゲットフォルダーを再度選択する必要があります。

## ファイルを検索

フォルダー内のモジュールリストファイルでは、次の部分で構成される独自のクエリを使用できます。

* **[!UICONTROL フィールド]**  — 検索するファイルの属性（例：属性） `name` ファイルの。

* **[!UICONTROL 演算子]**  — 一致を提供するためにデータに対して実行されるテスト（例： ） `contains`.

* **[!UICONTROL 値]**  — テストする属性の内容（ファイル名など） `My cool document`.

句と接続詞の結合 `and` または `or`をクリックし、 `not`.

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
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> ファイルの名前。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL fullText]</code> </td> 
   <td>文字列 </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> 名前、説明、コンテンツ、インデックス付け可能なテキストを含む、ファイルの全文。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL mimeType]</code> </td> 
   <td> 文字列</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> ファイルの MIME タイプ。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL modifiedDate]</code> </td> 
   <td> 日付<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> ファイルが最後に変更された日付。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL lastViewedByMeDate]</code> </td> 
   <td> 日付<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>></code>, <code>>=</code></td> 
   <td> <p> ユーザーが最後にファイルを表示した日付。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL trashed]</code></td> 
   <td>ブール型 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> ファイルがごみ箱に入っているかどうか。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL starred]</code></td> 
   <td>ブール型 </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>ファイルがスターリングされているかどうか。</p> </td> 
  </tr> 
  <tr> 
   <td><code>[!UICONTROL parents]</code></td> 
   <td>コレクション </td> 
   <td><code>in </code> </td> 
   <td> <p>[!UICONTROL parents] コレクションに指定した ID が含まれているかどうかを示します。</p> </td> 
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
   <td>ブール型 </td> 
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

* この `contains` 演算子は、 `title`.

  例えば、「HelloWorld」というタイトルは、 `title contains 'Hello'` しかし、 `title contains 'World'`.

* この `contains` 演算子は、次の文字列トークン全体に対してのみ一致を実行します： `fullText`.

  例えば、ドキュメントの全文に「HelloWorld」という文字列が含まれている場合、クエリは `fullText contains 'HelloWorld'` 結果を返します。 クエリ： `fullText contains 'Hello'` このシナリオでは、の結果は返されません。

* この `contains` 演算子が二重引用符で囲まれている場合、英数字と完全に一致するフレーズが見つかります。

  例えば、 `fullText` ドキュメントの「Hello there world」という文字列を含む場合、 `fullText contains '"Hello there"'` は結果を返しますが、クエリは `fullText contains '"Hello world"'` は実行しません。

  さらに、検索が英数字なので、 `fullText` ドキュメントに「Hello_world」という文字列が含まれている場合、 `fullText contains '"Hello world"'` 結果を返します。

* のフィールド `type` 現在、日付は一定の日付にのみ相当し、互いに比較することはできません。

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
   <td>String </td> 
   <td> <p>一重引用符で囲みます。 次を使用したクエリで一重引用符をエスケープ <code>\'</code>例：<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>ブール値 </td> 
   <td> <p><code>true </code>または <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>日付 </td> 
   <td> <p>RFC 3339 形式。デフォルトタイムゾーンは UTC です ( 例： <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
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
   <td> <p> 文字列またはブール値の内容が他の内容と等しい。</p> </td> 
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
   <td> <p> 日付が別の日付以降です。</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>要素は、コレクション内に含まれます。</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>両方の句に一致するファイルを返します。</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>どちらの句にも一致するファイルを返します。</p> </td> 
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

複合句の場合は、括弧を使用して句をグループ化できます。 例：
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` この検索では、2012 年 6 月 4 日以降に最終変更された画像またはビデオの MIME タイプを持つすべてのファイルが返されます。 理由： `and` および `or` 演算子は、括弧なしで左から右に評価されます。上記の例では、2012 年 6 月 4 日より後に変更された画像のみが返されますが、2012 年 6 月 4 日より前の画像も含め、すべてのビデオが返されます。

### 例

このページのすべての例では、エンコードされていない `<q>q</q>` パラメータ `title = 'hello'` は次のようにエンコードされます： `title+%3d+%27hello%27`. クライアントライブラリは、このエンコーディングを自動的に処理します。

* 「hello」という名前のファイルを検索します。
  <pre>title = 'hello'</pre>
* フォルダー固有の MIME タイプを使用したフォルダーの検索
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* フォルダー以外のファイルを検索
  <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* 「hello」と「goodbye」という単語を含む名前のファイルを検索します。
  <pre>タイトルに「hello」が含まれ、[!UICONTROL name] に「goodbye」が含まれています</pre>
* 「hello」という語を含まない名前のファイルを検索します。
  <pre>タイトルに「hello」が含まれていません</pre>
* コンテンツ内に「hello」という単語を含むファイルを検索します
  <pre>fullText に「hello」が含まれています</pre>
* コンテンツ内に「hello」という語を含まないファイルを検索します。
  <pre>fullText に「hello」が含まれていません</pre>
* コンテンツ内に「hello world」という完全なフレーズを含むファイルを検索します。
  <pre>fullText には「"hello world"」が含まれます。「fullText には「"hello_world"」が含まれます</pre>
* クエリに「\」文字を含むファイルを検索します（例：「\authors」）。
  <pre>fullText には「\\authors」が含まれます</pre>
* ユーザー「test@example.org」が書き込み可能なファイルを検索します
  <pre>test@example.org [!DNL writers]</pre>
* ID を検索します。 `1234567` 内 `parents` コレクション。 これにより、ID がのフォルダー内に直接存在するすべてのファイルとフォルダーを検索します `1234567`.
  <pre>[!UICONTROL 親 ] の「1234567」</pre>
* エイリアス ID を検索します。 `appDataFolder` 内 `parents` コレクション。 これにより、 [アプリケーションデータフォルダー](https://developers.google.com/drive/api/v2/appdata).
  <pre>親の「appDataFolder」</pre>
* ユーザー「test@example.org」と「test2@example.org」が書き込み可能なファイルを検索
  <pre>ライターでは「test@example.org」、ライターでは「test2@example.org」</pre>
* ごみ箱に入っている「重要」というテキストを含むファイルを検索します
  <pre>fullText は、「important」を含み、trashed = true を含みます</pre>
* 2012 年 6 月 4 日以降に変更されたファイルを検索
  <pre>modifiedDate &gt; '2012-06-04T12:00:00' //デフォルトタイムゾーンは UTC です</pre><pre>modifiedDate &gt; '2012-06-04T12:00:00-08:00'</pre>
* 名前に「hello」を含む、認証済みユーザーと共有されているファイルを検索します
  <pre>sharedWithMe とタイトルに「hello」が含まれている</pre>
* を含むファイルの検索 [カスタムファイルプロパティ](https://developers.google.com/drive/api/v2/properties) 名前付き `additionalID` 値 `8e8aceg2af2ge72e78`.
  <pre>プロパティには、{ key='additionalID'および value='8e8aceg2af2ge72e78'および visibility='PRIVATE' } が含まれます</pre>

このガイドのソースは、 [[!DNL Google Drive] ドキュメント](https://developers.google.com/drive/api/v2/search-shareddrives).
