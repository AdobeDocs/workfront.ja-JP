---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Marketoモジュール
description: 内、 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Marketo]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2068'
ht-degree: 0%

---

# [!DNL Marketo] モジュール

内、 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Marketo]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

Marketoコネクタの紹介ビデオについては、次を参照してください。

* [Marketo](https://video.tv.adobe.com/v/3427026/){target=_blank}

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
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
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件： [!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織は購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

次を使用するには： [!DNL Marketo] モジュールの場合は、 [!DNL Marketo] アカウント。

## 接続 [!DNL Marketo] Workfront Fusion {#connect-marketo-to-workfront-fusion}

次に対する接続を作成できます： [!DNL Marketo] 内部から直接口座を開く [!DNL Marketo] モジュール。

1. 任意の [!DNL Marketo] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. を入力します。 [!DNL Marketo] アカウントまたは [!DNL Marketo] [!UICONTROL Munchkin] ID。 これは、アカウントに割り当てられたベース URL またはエンドポイントの一意の部分で、アクセスに使用するものです [!DNL Marketo] を介して [!UICONTROL REST] API. これを見つける手順については、 [ベース URL](https://developers.marketo.com/rest-api/base-url/) （内） [!DNL Marketo] ドキュメント。
1. を入力します。 [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵]. これらの場所の特定方法については、 [認証](https://developers.marketo.com/rest-api/authentication/) （内） [!DNL Marketo] ドキュメント。
1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Marketo] モジュールとそのフィールド

設定時に [!DNL Marketo] モジュール、 [!DNL Workfront Fusion] に、以下のフィールドを示します。 これらと共に、 [!DNL Marketo] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [であるモジュールから別のモジュールに情報をマッピングします。 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

* [[!UICONTROL レコードを監視]](#watch-records)
* [[!UICONTROL イベントを視聴する（即時）]](#watch-events-instant)

#### [!UICONTROL レコードを監視]

このトリガーモジュールは、レコードが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL アクティビティ ]</strong> </p> <p>監視するアクティビティのタイプを選択します。 </p> <p>モジュールは、新しいアクティビティを監視するだけです。<br></p> </li> 
     <li> <p><strong>[!UICONTROL リード ]</strong> </p> <p>新しいレコード、更新されたレコード、新しいレコードと更新されたレコードの両方、または特定のフィールドの更新を監視するかどうかを選択します。 特定のフィールドの更新を監視する場合は、モジュールで監視するフィールドを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL プログラム ]</strong> </p> <p>新しいレコード、更新されたレコード、または新しいレコードと更新されたレコードの両方を監視するかどうかを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL イベントを視聴する（即時）]

このトリガーモジュールは、レコードが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>モジュールで使用する Webhook を入力します。</p> <p>Web フックの詳細については、 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">のインスタントトリガー（Web フック） [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL レコードの作成]](#create-a-record)
* [[!UICONTROL レコードの更新]](#update-a-record)
* [[!UICONTROL ファイルのダウンロード]](#download-a-file)
* [[!UICONTROL ファイルのアップロード]](#upload-a-file)
* [[!UICONTROL レコードを読み取る]](#read-a-record)
* [[!UICONTROL リードをリストに追加]](#add-leads-to-a-list)
* [[!UICONTROL リストからリードを削除]](#remove-leads-from-a-list)
* [[!UICONTROL キャンペーンのスケジュール設定]](#schedule-a-campaign)
* [[!UICONTROL プログラムのコピー]](#copy-a-program)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Marketo] API. これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Marketo] モジュール。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力 <code>https://{your-base-url}.mktorest.com/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">での HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>注意：  <p>条件ステートメント ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが操作するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの作成]

このアクションモジュールは、に新しいレコードを作成します。 [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL 会社 ]</p> </li> 
     <li> <p>[!UICONTROL フォルダー ]</p> </li> 
     <li> <p>[!UICONTROL リード ]</p> </li> 
     <li> <p>[!UICONTROL プログラム ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL マッピングするフィールドを選択 ]</td> 
   <td>会社またはリードを作成する場合は、新しいレコードの作成時に値を設定するフィールドを選択し、これらのフィールドに値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プログラムタイプ ]</td> 
   <td>プログラムを作成する場合は、作成するプログラムのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プログラムチャネル ] </td> 
   <td>プログラムを作成する場合は、プログラムを作成するプログラムチャネルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ] / [!UICONTROL プログラム名 ]</td> 
   <td>フォルダまたはプログラムを作成する場合は、新しいレコードの名前を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 説明 ]</td> 
   <td> <p>フォルダまたはプログラムを作成する場合は、新しいレコードの説明を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 親フォルダー ID]</td> 
   <td>フォルダまたはプログラムを作成する場合は、新しいレコードを作成する親フォルダの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コスト ]</td> 
   <td>プログラムを作成する場合は、コストを追加します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タグ ]</td> 
   <td>プログラムを作成する場合は、タグを追加します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの更新]

このアクションモジュールは、ID を使用して既存のレコードを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL 会社 ]</p> </li> 
     <li> <p>[!UICONTROL リード ]</p> </li> 
     <li> <p>[!UICONTROL プログラム ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 会社 ] / [!UICONTROL リード ] / [!UICONTROL プログラム ID]</td> 
   <td>更新するレコードの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL マッピングするフィールドを選択 ]</td> 
   <td>会社またはリードを更新する場合は、値を更新するフィールドを選択し、これらのフィールドに値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プログラム名 ]</td> 
   <td>プログラムを更新する場合は、プログラムの新しい名前を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 説明 ]</td> 
   <td> <p>プログラムを更新する場合は、プログラムの新しい説明を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 開始日 ]</td> 
   <td>プログラムを更新する場合は、プログラムの新しい開始日を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 終了日 ]</td> 
   <td>プログラムを更新する場合は、プログラムの新しい終了日を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コスト ]</td> 
   <td>プログラムを更新する場合は、コストを追加します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タグ ]</td> 
   <td>プログラムを更新する場合は、タグを追加します</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのダウンロード]

このアクションモジュールは、ファイル ID を使用してファイルをダウンロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ID]</td> 
   <td>ダウンロードするファイルの ID をマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのアップロード]

このアクションモジュールは、新しいファイルをアップロードします。 [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID]</td> 
   <td>新しいファイルを配置するフォルダの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 説明 ]</td> 
   <td>アップロードするファイルの説明を入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、ID を使用してレコードに関する情報を読み取ります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>作成するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL 会社 ]</p> </li> 
     <li> <p>[!UICONTROL リード ]</p> </li> 
     <li> <p>[!UICONTROL リスト ]</p> </li> 
     <li> <p>[!UICONTROL プログラム ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。 フィールドは、選択した [!UICONTROL レコードタイプ ] に基づいて使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;object&gt; ID]</td> 
   <td>情報を取得するオブジェクトの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リードをリストに追加]

このアクションモジュールは、リード ID を使用して 1 つ以上のリードをリストに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リスト ID]</td> 
   <td>リードを追加するリストの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リード ID]</td> 
   <td> <p>リストに追加するリードごとに、 <b>[!UICONTROL 追加 ]</b>次に、追加するリードの ID を入力またはマッピングします。 モジュールがリストに追加するリードは 300 件まで追加できます。</p> <p>マップの切り替えをクリックして、リストに追加する既存のリードのコレクションをマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL リストからリードを削除]

このアクションモジュールは、リード ID を使用して、1 つ以上のリードをリストから削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リスト ID]</td> 
   <td>リードを削除するリストの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リード ID]</td> 
   <td> <p>リストから削除するリードごとに、 <b>[!UICONTROL 追加 ]</b>次に、削除するリードの ID を入力またはマッピングします。 モジュールがリストから削除するリードは最大 300 名まで追加できます。 </p> <p>マップの切り替えをクリックして、リストから削除する既存のリードのコレクションをマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL キャンペーンのスケジュール設定]

このアクションモジュールは、特定の日付の既存のキャンペーンをスケジュールします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL キャンペーン ID]</td> 
   <td>スケジュールを設定するキャンペーンの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 日付のスケジュール ]</p> </td> 
   <td>キャンペーンを実行する日付を選択します。 このフィールドを空白にした場合、キャンペーンはシナリオが開始されてから 5 分後に実行されます。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL プログラムのコピー]

このアクションモジュールは、既存のプログラムの ID を使用してプログラムのコピーを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 既存のプログラム ID]</td> 
   <td>コピーするプログラムの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 新規プログラム名 ]</p> </td> 
   <td> <p>新しいプログラムの名前を入力またはマッピングします</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID]</td> 
   <td>新しいプログラムを配置するフォルダの ID を入力またはマップします。</td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL レコードのリスト]](#list-records)
* [[!UICONTROL レコードを検索]](#update-a-record)

#### [!UICONTROL レコードのリスト]

このアクションモジュールは、特定のタイプのすべてのレコードを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>リストに表示するレコードの種類を選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL すべてのキャンペーンを読み取る ]</p> </li> 
     <li> <p>[!UICONTROL すべてのプログラムを読み取る ]</p> </li> 
     <li> <p>[!UICONTROL すべてのリードを読み取り ] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド ]</td> 
   <td>リードの取得を選択した場合は、リストからリードを取得するか、プログラムからリードを取得するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>このモジュールの出力バンドルに含める情報を選択します。 フィールドは、選択した [!UICONTROL レコードタイプ ] に基づいて使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
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
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法については、 [!DNL Marketo] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">接続 [!DNL Marketo] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>検索するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL キャンペーン ]</p> </li> 
     <li> <p>[!UICONTROL リード ]</p> </li> 
     <li> <p>[!UICONTROL プログラム ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL フィールド ]</p> </td> 
   <td> <p>名前、プログラム名、またはワークスペース名で検索するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 値 ]</td> 
   <td>検索する値ごとに、 <b>[!UICONTROL 項目を追加 ]</b> 値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
