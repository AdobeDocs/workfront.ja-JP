---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Google Team Drive モジュール
description: この [!DNL Adobe Workfront Fusion Google Team Drive] モジュールを使用すると、ファイルを監視、アップロード、更新、コピー、削除または取得したり、 [!DNL Google Shared] ドライブ。
author: Becky
feature: Workfront Fusion
exl-id: 8b4c057f-bb98-44d1-9b71-cbeaa402a1c3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# [!DNL Google Team Drive] モジュール

この [!DNL Adobe Workfront Fusion] [!DNL Google Team Drive] モジュールを使用すると、ファイルを監視、アップロード、更新、コピー、削除または取得したり、 [!DNL Google Shared Drive].

を使用するには [!DNL Google Team Drive] と [!DNL Adobe Workfront Fusion]の場合、 [!DNL G Suite] アカウント これがない場合は、 [!DNL G Suite] 次の場所のアカウント [[!DNL G Suite] サインアップサイト](https://gsuite.google.com/signup/businessstarter/welcome).

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Google Team Drive]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

## 前提条件

使用する [!DNL Google Team Drive] モジュールの場合、 [!DNL Google Team Drive].

## [!DNL Google Team Drive] モジュールとそのフィールド

設定時に [!DNL Google Team Drive] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Google Team Drive] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

モジュールダイアログのフィールドが **太字** ( [!DNL Workfront Fusion] シナリオ、 **not** このドキュメントの記事では ) は必須です。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### トリガー

#### [!UICONTROL 監視ファイル]

指定されたフォルダ内で新しいファイルが追加または変更された場合に、ファイルの詳細を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL チームドライブ ]</td> 
   <td> <p> 監視する共有ドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>共有ドライブ内のフォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 監視するファイル</td> 
   <td> <p> 監視するファイルの種類を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Documents] 形式設定するファイル </td> 
   <td> <p>監視する形式を選択 [!DNL Google Documents] に変換されたファイル。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Sheets] 形式設定するファイル </td> 
   <td> <p>監視する形式を選択 [!DNL Google Sheets] に変換されたファイル。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Slides] 形式設定するファイル </td> 
   <td> <p>監視する形式を選択 [!DNL Google Slides] に変換されたファイル。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Drawings] 形式設定するファイル </td> 
   <td> <p>監視する形式を選択 [!DNL Google Drawings] に変換されたファイル。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ウォッチ ]</td> 
   <td> <p> 新しいファイルと変更されたファイルのフォルダを監視するか、新しいファイルのみを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ダウンロードされたファイルの最大数 ]</td> 
   <td> <p> ファイルの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL ファイルのアップロード]](#upload-a-file)
* [[!UICONTROL ファイルの更新]](#update-a-file)
* [[!UICONTROL ファイルのコピー]](#copy-a-file)
* [[!UICONTROL ファイルの削除]](#delete-a-file)
* [[!UICONTROL ファイルをごみ箱に移動]](#move-a-file-to-trash)
* [[!UICONTROL ファイルの取得]](#get-a-file)
* [[!UICONTROL ファイルリストを取得]](#get-a-file-list)
* [[!UICONTROL フォルダーの作成]](#create-a-folder)

#### [!UICONTROL ファイルのアップロード]

指定した共有ドライブにファイルをアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL チームドライブ ] </td> 
   <td> <p>ファイルのアップロード先の共有ドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>共有ドライブ内のフォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL ソースファイル ]</p> </td> 
   <td> <p>共有ドライブにアップロードするファイルを指定します。</p> <p>前のモジュールからアップロードするファイルをマッピングします ( 例：[!UICONTROL HTTP] &gt;[!UICONTROL ファイルを取得 ] または [!UICONTROLDropbox] &gt;[!UICONTROL ファイルを取得 )]、またはファイル名とファイルデータを手動で入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイトル ]</td> 
   <td> <p> 共有フォルダに表示するファイルのタイトルを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルの変換 ]</td> 
   <td> <p> このオプションを有効にすると、共有フォルダーの対応するGoogle形式にファイルが変換されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの更新]

ファイル名やファイルの内容を変更できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL チームドライブ ]</td> 
   <td> <p> 更新するファイルが含まれている共有ドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>共有ドライブ内のフォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td> <p> 更新するファイルの ID を入力（マップ）します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL ソースファイル ]</p> </td> 
   <td>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL タイトル ] </td> 
   <td> <p>更新したファイルの新しいタイトルを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルの変換 ]</td> 
   <td> <p> このオプションを有効にすると、対応する [!DNL Google] の形式を共有フォルダーに保存します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのコピー]

指定したファイルを選択したフォルダにコピーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL チームドライブ ]</td> 
   <td> <p> コピーするファイルを含む共有ドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>ファイルのコピー先となるターゲットフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td> <p> コピーするファイルの ID を入力（マップ）します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL コピーファイルの名前 ]</p> </td> 
   <td> <p>ターゲットの場所で変更する場合は、新しいファイル名を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの削除]

指定したファイルを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td> <p> 削除するファイルの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをごみ箱に移動]

指定したファイルをごみ箱に移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td> <p> ごみ箱に移動するファイルの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの取得]

指定されたファイルに関する詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Documents] 形式設定するファイル </td> 
   <td> <p>使用する形式を選択します。 [!DNL Google Documents] に変換されたファイル。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Sheets] 形式設定するファイル </td> 
   <td> <p>使用する形式を選択します。 [!DNL Google Sheets] に変換されたファイル。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Slides] 形式設定するファイル </td> 
   <td> <p>使用する形式を選択します。 [!DNL Google Slides] に変換されたファイル。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 変換 [!DNL Google Drawings] 形式設定するファイル </td> 
   <td> <p>使用する形式を選択します。 [!DNL Google Drawings] に変換されたファイル。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td> <p> 取得するファイルの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルリストを取得]

検索語句に基づいてファイルやフォルダーの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL チームドライブ ]</td> 
   <td> <p> ファイルの一覧を表示する共有ドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>ファイルの一覧表示元のフォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 検索 ] </td> 
   <td> <p>実行する検索のタイプを選択します（以下を参照）。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL クエリ ]</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>[!UICONTROL ファイル名内を検索 ]</p> <p style="font-weight: normal;">[!UICONTROL 検索で完全な検索語を検索 ] オプションが選択されている場合はファイル名（ファイル拡張子を含む）を入力するか、[!UICONTROL 検索で検索語を含む名前を検索 ] オプションが選択されている場合は名前の一部を入力します。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL フルテキスト検索 ]</p> <p>検索語句を入力して、ファイル名、説明、内容を検索します。</p> </li> 
     <li> <p style="font-weight: bold;">[!UICONTROL カスタム検索クエリ ]</p> <p>次を入力します。 [!DNL Google] 検索クエリの語句。 詳しくは、 [!DNL Google]'s <a href="https://developers.google.com/drive/api/v2/ref-search-terms">検索クエリドキュメント</a>. 例: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 取得 ]</td> 
   <td>ファイル、フォルダ、またはその両方を取得するかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 返される結果の最大数 ]</td> 
   <td> <p> ファイルまたはフォルダーの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーの作成]

新しいフォルダーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Google Team Drive] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL チームドライブ ]</td> 
   <td> <p> フォルダを作成する共有ドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>フォルダーを作成するフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 新しいフォルダーの名前 ]</td> 
   <td> <p> 新しいフォルダの名前を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>
