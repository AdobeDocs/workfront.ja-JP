---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Dropboxモジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオでは、Dropboxを使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続できます。これにより、Dropbox内のファイルやフォルダの監視、検索、取得、一覧表示、作成、編集などのアクティビティを自動化できます。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3061'
ht-degree: 0%

---

# [!DNL Dropbox] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!UICONTROL Dropbox]複数のサードパーティのアプリケーションおよびサービスに接続できます。これにより、内のファイルおよびフォルダーの監視、検索、取得、リスト、作成、編集などのアクティビティを自動化できます [!UICONTROL Dropbox].

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

使用する [!DNL Dropbox] モジュールの場合、 [!DNL Dropbox] アカウント

## [!DNL Dropbox] モジュールとそのフィールド

設定時に [!DNL Dropbox] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Dropbox] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガーモジュール](#trigger-modules)
* [を取得するためのモジュール [!DNL Dropbox] ファイルとフォルダ](#modules-for-getting-dropbox-files-and-folders)
* [作成および編集用のモジュール [!DNL Dropbox] ファイルとフォルダ](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [その他のモジュール](#other-modules)

### トリガーモジュール

#### [!UICONTROL 監視ファイル]

このトリガータイプモジュールは、指定されたフォルダ内のファイルが変更された場合、ファイルの詳細を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>変更を監視するフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch もサブフォルダーを監視 ]</td> 
   <td> <p> このオプションを有効にすると、選択したフォルダのサブフォルダに変更されたファイルがないかも監視されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ] </td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### を取得するためのモジュール [!DNL Dropbox] ファイルとフォルダ

* [[!UICONTROL ファイル/フォルダを検索]](#search-filesfolders)
* [[!UICONTROL ファイルのダウンロード]](#download-a-file)
* [[!UICONTROL フォルダーメタデータの取得]](#get-a-folder-metadata)
* [[!UICONTROL フォルダ内のすべてのファイル/サブフォルダのリスト]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL ファイルリビジョンのリスト]](#list-file-revisions)

#### [!UICONTROL ファイル/フォルダを検索]

この検索モジュールは、 [!DNL Dropbox] 指定した検索クエリに一致する

この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 検索 ] </td> 
   <td> <p>検索語句を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>検索するフォルダを選択します。 このモジュールは、 [!DNL Dropbox] （フォルダーを選択しない場合）。</p> </td> 
  </tr> 
  <tr> 
   <td>ファイルステータス</td> 
   <td> <p> ファイルのステータスを選択し、検索を選択したファイルのステータスに制限します。</p> </td> 
  </tr> 
  <tr> 
   <td>ファイルカテゴリ</td> 
   <td> <p> ファイルカテゴリを選択して、選択したカテゴリに検索を制限します。</p> </td> 
  </tr> 
  <tr> 
   <td>ファイル拡張子</td> 
   <td> <p> 検索するファイル拡張子を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>制限 </td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのダウンロード]

このアクションモジュールは、フォルダーからファイルをダウンロードします。

ファイルとその場所を指定します。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

>[!NOTE]
>
>このモジュールは、後続のモジュールにファイルを提供する場合に役立ちます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>ファイルの選択方法</td> 
   <td> <p> ファイルパスをマップするか、手動でファイルを選択するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>ファイルパス/ファイル</p> </td> 
   <td> <p style="font-weight: bold;">ファイルパス</p> <p>ターゲットパスを入力またはファイルにマッピングします。</p> <p style="font-weight: bold;">ファイル</p> <p>メニューからファイルを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーメタデータの取得]

このアクションモジュールは、共有フォルダーの詳細を取得します。

フォルダーの ID を指定します。

このモジュールは、フォルダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>共有フォルダー ID</td> 
   <td> <p> 詳細を取得するフォルダーの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダ内のすべてのファイル/サブフォルダのリスト]

このアクションモジュールは、特定のフォルダー内のファイルまたはフォルダーを一覧表示します。

フォルダーの ID を指定します。

このモジュールは、ファイルまたはフォルダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>リスト </td> 
   <td> <p>ファイルを取得するか、フォルダを取得するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>ダウンロード可能なファイルのみを表示</td> 
   <td> <p> ダウンロード可能なファイルのみを返すには、このオプションを有効にします。 Google Docs など、一部のタイプのファイルはダウンロードできません。</p> </td> 
  </tr> 
  <tr> 
   <td>フォルダー </td> 
   <td> <p>ファイルまたはフォルダを取得するフォルダを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>制限 </td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールでリストするレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルリビジョンのリスト]

このアクションモジュールは、特定のファイルのすべてのファイルリビジョン（バージョン履歴）を取得します。\
ファイルの ID を指定します。

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>ファイルの選択方法</td> 
   <td> <p> ファイルパスをマップするか、手動でファイルを選択するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>ファイルパス/ファイル</p> </td> 
   <td> <p style="font-weight: bold;">ファイルパス</p> <p>ターゲットパスを入力またはファイルにマッピングします。</p> <p style="font-weight: bold;">ファイル</p> <p>メニューからファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>制限</p> </td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールでリストするレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 作成および編集用のモジュール [!DNL Dropbox] ファイルとフォルダ

* [[!UICONTROL アップロード] ファイル](#upload-a-file)
* [[!UICONTROL フォルダーの作成]](#create-a-folder)
* [[!UICONTROL テキストファイルの作成/上書き]](#createoverwrite-a-text-file)
* [[!UICONTROL 共有リンクの作成/更新]](#createupdate-a-share-link)
* [[!UICONTROL ファイルの復元]](#restore-a-file)
* [[!UICONTROL ファイル/フォルダの移動]](#move-a-filefolder)
* [[!UICONTROL ファイル/フォルダ名を変更する]](#rename-a-filefolder)
* [[!UICONTROL ファイル/フォルダの削除]](#delete-a-filefolder)

#### [!UICONTROL ファイルのアップロード]

このアクションモジュールは、ファイルをフォルダーにアップロードします。

ファイルの場所、アップロードするファイル、ファイルの新しい名前（オプション）などの情報を指定します。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ]</td> 
   <td> <p> 次のフォルダーを選択： [!DNL Dropbox] ファイルのアップロード先です。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL ソースファイル ]</p> </td> 
   <td> <p>に追加するファイルを入力またはマッピングします [!DNL Dropbox] 上で選択したフォルダー。</p> <p style="font-weight: bold;">[!UICONTROL ファイル名 ]</p> <p>ファイル拡張子を含むファイル名を入力またはマッピングします。</p> <p style="font-weight: bold;">[!UICONTROL ファイルデータ ]</p> <p>([!UICONTROL Google Drive] &gt;[!UICONTROL ファイルの取得 ] など、以前のモジュールから ) ファイルデータを入力またはマッピングします。</p> <p>注意：アップロードされるファイルの最大サイズは 150 MB です。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 既存のファイルを上書き ]</td> 
   <td> <p> 既存のファイルを新しいファイルで置き換えるには、このオプションを有効にします。 このオプションを無効にしたままにすると、アップロードされたファイルの名前が変更されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーの作成]

このアクションモジュールは、新しいフォルダーを作成します。

フォルダーのパスと名前を指定します。

このモジュールは、フォルダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー名 ] </td> 
   <td> <p>新しいフォルダの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL フォルダー ]</p> </td> 
   <td> <p>新しいフォルダーを作成する場所のパスを入力またはマッピングします。</p> <p>メモ:   <p>を使用している場合、 [!DNL Dropbox Business] アカウント（チームスペースを含む）、スラッシュを削除する必要があります <code>/</code>をクリックしない <strong>[!UICONTROL フォルダーを選択するには、ここをクリック ] してください</strong> をクリックして、ルートにチームフォルダを作成します。</p> <p>スラッシュが削除されない場合は、エラー <code>[409] path/malformed_path/..</code> が返されます。</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 自動名変更 ]</td> 
   <td> <p> 同じ名前のフォルダが既にターゲットの場所に存在する場合、このオプションを有効にして、新しいフォルダの名前を変更します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL テキストファイルの作成/上書き]

このアクションモジュールは、DOC ファイルを作成するか、既存のファイルの内容を上書きします。

ソースファイルとフォルダーを指定します。

このモジュールは、フォルダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 選択して ]</td> 
   <td> <p> DOC ファイルを作成するか上書きするかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>ファイルを作成するターゲットの場所を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL ソースファイル ]</p> </td> 
   <td> <p>に追加するファイルを入力またはマッピングします [!DNL Dropbox] フォルダー。</p> <p style="font-weight: bold;">ファイル名</p> <p>新しい DOC ファイルのファイル名（拡張子なし）を入力します。</p> <p style="font-weight: bold;">ファイルコンテンツ</p> <p>DOC ファイルのテキストコンテンツを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 共有リンクの作成/更新]

このアクションモジュールは、ファイルへのパブリックリンクを作成します。

ファイルおよびリンクに関する情報を指定します。

モジュールは、リンクの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルの選択方法 ]</td> 
   <td> <p> マップするかファイルパスを入力するかを選択するか、手動でファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path / File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL ファイルパス ]</p> <p>ターゲットパスを入力またはファイルにマッピングします。</p> <p style="font-weight: bold;">[!UICONTROL ファイル ]</p> <p>メニューからファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL リクエストされた表示 ]</p> </td> 
   <td> <p>リンクをパブリックにするか、チームにするか、パスワードを制限するかを選択します。</p> <p>注意：[!UICONTROL チームのみ ] および [!UICONTROL パスワードを使用したアクセス ] オプションは、 [!DNL Dropbox Pro] またはそれ以降のバージョン。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL リンクの有効期限 ]</td> 
   <td> <p> リンクの有効期限が切れ、アクセスできなくなる日時を入力します。 このフィールドを空のままにした場合、リンクの有効期限は切れません。 サポートされる日付と時刻の形式の一覧については、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">強制入力 [!DNL Adobe Workfront Fusion]</a>.</p> <p>注意：[!UICONTROLDropboxのみ ] および [!UICONTROL パスワードを使用したアクセス ] オプションは、[!UICONTROL チームプロ ] 以降のバージョンを持つユーザーのみが使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL リンクのアクセスレベル ]</p> </td> 
   <td> <p>リンクの受信者の権限を設定します。</p> <p><strong>[!UICONTROL ビューア ]</strong> リンクを使用するユーザーは、コンテンツの表示とコメントを行うことができます。</p> <p><strong>[!UICONTROL エディター ]</strong> リンクを使用するユーザーは、コンテンツの編集、表示、コメントを行うことができます。</p> <p><strong>[!UICONTROL 最大 ]</strong> リンクを使用するユーザーは、リンク先として設定できる最大アクセスレベルを受け取ります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの復元]

このアクションモジュールは、ファイルの以前のバージョンを復元します。

必要なリビジョンのファイルと番号を指定します。

このモジュールは、バージョンと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルの選択方法 ]</td> 
   <td> <p> マップするかファイルパスを入力するかを選択するか、手動でファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p><strong>[!UICONTROL ファイルパス ]</strong> </p> <p>ターゲットパスを入力またはファイルにマッピングします。</p> <p><strong>[!UICONTROL ファイル ]</strong> </p> <p>メニューからファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL リビジョン ]</p> </td> 
   <td> <p>復元するリビジョンのリビジョン番号を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル/フォルダの移動]

このアクションモジュールは、ファイルまたはフォルダを別の場所に移動します。

ファイルまたはフォルダー、および移動する方法と場所を指定します。

このモジュールは、ファイルまたはフォルダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルの選択方法 ] </td> 
   <td> <p>マップするかファイルパスを入力するかを選択するか、手動でファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL ファイル/フォルダーパス ] / [!UICONTROL ファイル/フォルダー ]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL ファイル/フォルダーパス ]</p> <p>ターゲットパスを入力またはファイルまたはフォルダーにマッピングします。</p> <p style="font-weight: bold;">[!UICONTROL ファイル/フォルダー ]</p> <p>メニューからファイルまたはフォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL フォルダへ ]</p> </td> 
   <td> <p>ファイルまたはフォルダのターゲットの場所を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 新しい名前 ]</p> </td> 
   <td> <p>新しい場所にファイルまたはフォルダの新しい名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 自動名前変更 ]</p> </td> 
   <td> <p>このオプションを有効にすると、同じ名前のファイルまたはフォルダーが存在する場合、モジュールはファイルまたはフォルダー名の後に ([!UICONTROL NUMBER]) を追加して、新しいファイルまたはフォルダーの名前を変更します。 それ以外の場合は、ターゲットの場所にあるファイルまたはフォルダが上書きされます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 所有権の転送を許可 ]</p> </td> 
   <td> <p>コンテンツが移動される結果となる場合でも、所有者による移動を許可するには、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル/フォルダ名を変更する]

このアクションモジュールは、ファイルまたはフォルダーの名前を変更します。

ファイルまたはフォルダー、および新しい名前を指定します。

このモジュールは、ファイルまたはフォルダーの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>ファイルの選択方法</td> 
   <td> <p> マップするかファイルパスを入力するかを選択するか、手動でファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>ファイル/フォルダーのパス/ファイル/フォルダー</p> </td> 
   <td> <p style="font-weight: bold;">ファイル/フォルダーのパス</p> <p>ターゲットパスを入力またはファイルまたはフォルダーにマッピングします。</p> <p style="font-weight: bold;">ファイル/フォルダー</p> <p>メニューからファイルまたはフォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>名前を変更 </td> 
   <td> <p>ファイルのターゲット名を、ファイル拡張子を含めて入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイル/フォルダの削除]

このアクションモジュールは、ファイルまたはフォルダを削除します。

ファイルまたはフォルダを指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイルの選択方法 ]</td> 
   <td> <p> マップするかファイルパスを入力するかを選択するか、手動でファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL ファイルパス ]</p> <p>ターゲットパスを入力またはファイルにマッピングします。</p> <p style="font-weight: bold;">[!UICONTROL ファイル ]</p> <p>メニューからファイルを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他のモジュール

#### [!UICONTROL API 呼び出しを実行する]

このアクションモジュールを使用すると、 [!DNL Dropbox] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Dropbox] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Dropbox] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>相対パスを入力してください相対パスを入力してください <code>https://api.dropboxapi.com</code>. 以下に例を挙げます。 <code>/2/files/list_folder</code></p> <p>注意：使用可能なエンドポイントの一覧については、 <a href="https://www.dropbox.com/developers/documentation/http/documentation">DropboxAPI v2 ドキュメント</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL メソッド ]</p> </td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers] </td> 
   <td> <p>目的のリクエストヘッダーを入力します。 [!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> リクエストクエリ文字列を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 本文 ] </td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:   <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** 次の API 呼び出しは、 [!DNL /Text files] の [!DNL Dropbox] アカウント：
>
>URL: `/2/files/list_folder`
>
>本文:
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>検索結果は、モジュールの「出力」の「 [!UICONTROL バンドル] > [!UICONTROL 本文] > エントリ。
>
>この例では、10 枚のチケットが返送されています。

## 一般的な問題

* [ファイルをアップロードまたは更新できません](#unable-to-upload-or-update-a-file)
* [共有リンクで参照された画像はレンダリングされません](#image-referenced-via-a-shared-link-does-not-render)

### ファイルをアップロードまたは更新できません

ファイルのアップロードまたは更新に失敗する状況はいくつかあります。

* アップロードされたファイルが大きすぎて、が許可されている最大ファイルサイズを超えています [!DNL Dropbox] プランを作成するか、すべての [!DNL Dropbox] アカウントのストレージクォータ。 既存のファイルを [!DNL Dropbox] アカウントを作成するか、プランをアップグレードします。
* ファイルのアップロード先となる、以前に選択したフォルダーは存在しなくなりました。 シナリオが停止し、ターゲットフォルダーを再度選択する必要があります。

### 共有リンクで参照された画像はレンダリングされません

が返す URL [!UICONTROL Dropbox] >[!UICONTROL 共有リンクを作成] は画像に直接リンクするのではなく、 [!DNL Dropbox] ページ。 画像を強制的にダウンロードするには、末尾の `?dl=0` と `?dl=1`. (Web ブラウザーやFacebook Messenger などで ) 画像を強制的にレンダリングするには、次のコマンドを追加します。 `&raw=1` を URL に追加します。

Web サイトまたはその他のユーザーに対して、画像の直接リンクまたは生のリンクを取得する必要がある場合 [!DNL Workfront Fusion] モジュールの場合は、次の方法で最初の共有 URL を変更する必要があります。

オリジナル URL :

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. 置換 `www` と `dl`.
1. 削除 `?dl=0`.

最終 URL:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

URL を自動的に変更するには、 `replace()` 関数を 2 回実行します。

* www を dl に置き換えます。

  ![](assets/www-to-dl-350x32.png)

* また、?dl=0 を削除するには

  ![](assets/remove-dl0-350x33.png)

これを 1 つの手順でおこなうには、次の関数を組み合わせます。

![](assets/replace-both-350x47.png)

コピーして、「 」フィールドに貼り付けることもできます。 置換 `1.url` を URL に置き換えます。

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
