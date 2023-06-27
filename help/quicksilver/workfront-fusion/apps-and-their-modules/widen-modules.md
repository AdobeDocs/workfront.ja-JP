---
title: モジュールを広げる
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!UICONTROL 幅を広げる]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1586'
ht-degree: 1%

---

# [!DNL Widen] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!UICONTROL 幅を広げる]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!UICONTROL 幅を広げる] モジュールの場合、 [!UICONTROL 幅を広げる] アカウント

## 接続 [!DNL Widen] から [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

次に、 [!DNL Widen] 内部から直接アカウントを取得する [!DNL Widen] モジュール。

1. 任意の [!DNL Widen] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. を選択します。 [!DNL Widen] 接続先のドメイン。
1. のトークンを入力 [!DNL Widen] アカウント このトークンの場所については、 [[!DNL Widen] API に関する FAQ](https://community.widen.com/collective/s/article/API-FAQs).
1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Widen] モジュールとそのフィールド

設定時に [!DNL Widen] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Widen] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガーモジュール](#trigger-modules)
* [アクションモジュール](#action-modules)
* [モジュールを検索](#search-modules)

### トリガーモジュール

#### [!UICONTROL アセットを見る]

このトリガーモジュールは、アセットが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベントタイプ ]</td> 
   <td> <p>新しいアセットと更新されたアセットのどちらを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 展開 ]</td> 
   <td> <p>アセットフィールドに加えて、モジュール出力に含めるプロパティを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュール出力に含めるフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールで使用するアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクションモジュール

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL アセット情報の読み取り]](#read-asset-info)
* [[!UICONTROL コレクションへのアセットの追加]](#add-assets-to-collections)
* [[!UICONTROL コレクションからアセットを削除]](#remove-assets-from-collection)
* [[!UICONTROL アセットメタデータの更新]](#update-asset-metadata)
* [[!UICONTROL ファイルをダウンロード]](#download-file)
* [[!UICONTROL アップロード] ファイル](#upload-a-file)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Widen] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Widen] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API バージョン ]</td> 
   <td>最新バージョンのを使用するかどうかを選択します [!DNL Widen] API、またはバージョン 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>API 呼び出しの URL を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] によって認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
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
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>情報を読み取るアセットの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 展開 ]</td> 
   <td> <p>アセットフィールドに加えて、モジュール出力に含めるプロパティを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュール出力に含めるフィールドを選択します。</td> 
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
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コレクション ID]</td> 
   <td> <p>アセットの追加先の各コレクションについて、次の操作をおこないます。</p> 
    <ol> 
     <li value="1"> <p> クリック <strong>[!UICONTROL 追加 ]</strong>.</p> </li> 
     <li value="2"> <p>[!UICONTROL コレクション ID] を入力またはマッピングします。</p> </li> 
     <li value="3"> <p>クリック <strong>[!UICONTROL 項目を追加 ]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>コレクションに追加する各アセットに対して、次の操作をおこないます。</p> 
    <ol> 
     <li value="1"> <p> クリック <strong>[!UICONTROL 追加 ]</strong>.</p> </li> 
     <li value="2"> <p>アセット ID を入力またはマッピングします。</p> </li> 
     <li value="3"> <p>クリック <strong>[!UICONTROL 項目を追加 ]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールで使用するアセットの最大数を入力またはマッピングします。</p> </td> 
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
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コレクション ID]</td> 
   <td> <p>アセットを削除する各コレクションの場合：</p> 
    <ol> 
     <li value="1"> <p> クリック <strong>[!UICONTROL 追加 ]</strong>.</p> </li> 
     <li value="2"> <p>コレクション ID を入力またはマッピングします。</p> </li> 
     <li value="3"> <p>クリック <strong>[!UICONTROL 項目を追加 ]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アセット ID</td> 
   <td> <p>コレクションから削除する各アセットに対して、次の操作を実行します。</p> 
    <ol> 
     <li value="1"> <p> クリック <strong>[!UICONTROL 追加 ]</strong>.</p> </li> 
     <li value="2"> <p>アセット ID を入力またはマッピングします。</p> </li> 
     <li value="3"> <p>クリック <strong>[!UICONTROL 項目を追加 ]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールで使用するアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットメタデータの更新]

このアクションモジュールは、アセットのメタデータフィールドを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>メタデータを更新するアセットの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メタデータタイプ ]</td> 
   <td> <p>更新するメタデータのメタデータタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メタデータ ]</td> 
   <td>更新するメタデータフィールドを選択します。 各フィールドに、フィールドの新しい値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールで使用するアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをダウンロード]

このアクションモジュールは、 [!DNL Widen] アカウント

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>ダウンロードするアセットの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのアップロード]

このアクションモジュールは、 [!DNL Widen] アカウント

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロファイルをアップロード ]</td> 
   <td> <p>モジュールで使用するアップロードプロファイルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アップロードメソッド ]</td> 
   <td> <p>ファイルのアップロード方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイルから ]</strong> </p> <p>前のモジュールからソースファイルを選択またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL URL 別 ]</strong> </p> <p>アップロードするファイルの URL を入力またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td>アップロードしたファイルの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メタデータタイプ ]</td> 
   <td>アップロードするファイルのメタデータタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メタデータ ]</td> 
   <td>ファイルのアップロードに含めるメタデータフィールドを選択します。 各フィールドに、フィールドに [!UICONTROL 値 ] を入力します。</td> 
  </tr> 
 </tbody> 
</table>

### モジュールを検索

* [[!UICONTROL コレクションアセットの読み取り]](#read-collection-assets)
* [[!UICONTROL アセットの検索]](#search-assets)

#### [!UICONTROL コレクションアセットの読み取り]

このアクションモジュールは、コレクション内のアセットのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コレクション ID]</td> 
   <td> <p>読み取るアセットを含むコレクションの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 開始 ]</td> 
   <td>リストする最初の項目の番号を入力またはマップします。 これは、レコードをページ番号付けする方法です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 最大 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え基準 ]</td> 
   <td> <p>アセットの並べ替えに使用するプロパティを選択します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 順序 ]</td> 
   <td>アセットを昇順または降順に並べ替えるかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュール出力に含めるフィールドを選択します。</td> 
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
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
  <td> <p>接続方法 [!DNL Widen] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">接続 [!DNL Widen] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 検索クエリ ]</td> 
   <td> <p>アセットを検索する条件を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え基準 ]</td> 
   <td> <p>アセットの並べ替え方法を選択します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 順序 ]</td> 
   <td>アセットを昇順または降順に並べ替えるかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 削除済みを含める ]</td> 
   <td>削除されたアセットを検索に含めるには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL アーカイブ済みを含める ]</p> </td> 
   <td> <p>アーカイブしたアセットを検索に含めるには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドキュメントテキストを検索 ]</td> 
   <td>検索にドキュメントテキストを含める場合はこのオプションを有効にし、検索条件に一致するタイトルを持つアセットのみを含める場合は false にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL オフセット ]</td> 
   <td>詳細を取得する最初の項目の番号を入力またはマップします。 これは、レコードをページ番号付けする方法です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スクロール ]</td> 
   <td>スクロールを許可するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 展開 ]</td> 
   <td> <p>アセットフィールドに加えて、モジュール出力に含めるプロパティを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュール出力に含めるフィールドを選択します。</td> 
  </tr> 
 </tbody> 
</table>
