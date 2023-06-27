---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive for Business モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Microsoft OneDrive for Business]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: b7175cb9-aade-49b7-a28b-25fc9805a078
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# [!DNL Microsoft OneDrive for Business] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Microsoft OneDrive for Business]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL Microsoft OneDrive for Business] と [!DNL Adobe Workfront Fusion]、 [!DNL Microsoft] アカウント

接続方法 [!DNL OneDrive for Business] アカウント [!DNL Workfront Fusion]を参照してください。 [Adobeへの接続を作成 [!DNL Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!DNL Microsoft OneDrive for Business] モジュールとそのフィールド

設定時に [!DNL Microsoft OneDrive for Business] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Microsoft OneDrive for Business] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

* [[!UICONTROL 監視ファイル]](#watch-files)
* [[!UICONTROL 監視フォルダー]](#watch-folders)

#### [!UICONTROL 監視ファイル]

このトリガーモジュールは、監視対象のフォルダーに新しいファイルが追加または更新されるとアクティブになります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ドライブ ID]</p> </td> 
   <td> <p>監視するドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td> <p> 監視するフォルダーを選択します。 1 つのシナリオでは、監視できるフォルダーは 1 つだけです。</p> <p>ヒント：複数のフォルダーを追跡するには、それぞれに個別のシナリオを作成します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 視聴する</p> </td> 
   <td> <p>新しいファイルとすべての変更を監視するか、新しいファイルのみを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返される行の最大数 ]</td> 
   <td> <p> 結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 監視フォルダー]

このトリガーモジュールは、監視対象のフォルダーに新しいフォルダーが追加されるとアクティブになります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ドライブ ID]</p> </td> 
   <td> <p>監視するドライブを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td> <p> 監視するフォルダーを選択します。 1 つのシナリオでは、監視できるフォルダーは 1 つだけです。</p> <p>ヒント：複数のフォルダーを追跡するには、それぞれに個別のシナリオを作成します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 視聴する</p> </td> 
   <td> <p>新しいフォルダとすべての変更を監視するか、新しいフォルダのみを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返される行の最大数 ]</td> 
   <td> <p> 結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL ファイルのアップロード]](#upload-a-file)
* [[!UICONTROL ファイルの削除]](#delete-a-file)
* [[!UICONTROL ファイルの取得]](#get-a-file)
* [[!UICONTROL フォルダーの作成]](#create-a-folder)
* [[!UICONTROL フォルダーの削除]](#delete-a-folder)
* [[!UICONTROL 共有リンクの取得]](#get-a-sharing-link)

#### [!UICONTROL ファイルのアップロード]

このアクションモジュールは、指定されたフォルダーにバイナリまたはテキストファイルをアップロードします

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ドライブ ID]</td> 
   <td> <p>ファイルのアップロード先のドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>ドライブ内のフォルダを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL ソースファイル ]</p> </td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 同じ名前のファイルが存在する場合 ]</td> 
   <td> <p> アップロードしようとしているファイルと同じ名前のファイルが既に存在する場合に実行する操作を選択します。</p> 
    <ul> 
     <li>[!UICONTROL 既存のファイルを置き換える ]</li> 
     <li>[!UICONTROL 新しいファイル名を変更 ]</li> 
     <li>[!UICONTROL エラーで終了 ]</li> 
    </ul> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの削除]

このアクションモジュールは、指定されたファイルをごみ箱に移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ドライブ ID]</td> 
   <td> <p>ファイルを削除するドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td> <p>削除するファイルの ID を入力します。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの取得]

このアクションモジュールは、指定された ID を持つファイルを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ドライブ ID]</td> 
   <td> <p>ファイルを取得するドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ファイル ID]</td> 
   <td> <p>取得するファイルの ID を入力します。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーの作成]

指定された親フォルダー内にフォルダーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL 接続 ]</strong> </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL ドライブ ID]</strong> </td> 
   <td> <p>新しいフォルダを作成するドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL フォルダー ]</strong> </td> 
   <td> <p>新しいフォルダーを作成するフォルダーを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL フォルダー名 ]</strong> </td> 
   <td>新しいフォルダの名前を入力またはマップします。</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーの削除]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ドライブ ID]</td> 
   <td> <p>ファイルを削除するドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ID]</td> 
   <td> <p>削除するフォルダーの ID を入力またはマッピングします。 </p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 共有リンクの取得]

このモジュールは、指定されたファイルにアクセスするために共有できるリンクを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ドライブ ID]</td> 
   <td> <p>ファイルのアップロード先のドライブを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enter]</td> 
   <td> <p>ファイル ID を使用してファイルを選択するか、ファイルパスを使用してファイルを選択するかを選択します。 表示されるフィールドに、ファイル ID またはパスを入力します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 権限のタイプ ]</p> </td> 
   <td> <p>リンクを受け取った人に読み取り/書き込み権限を付与するか、読み取り専用にするかを選択します。</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL スコープ ]</td> 
   <td> <p> リンクを持つユーザーのみがファイルにアクセスできるようにするか、組織のメンバーのみがファイルにアクセスできるようにするかを選択します。</p> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
