---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Bynder モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL Bynder] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1664'
ht-degree: 100%

---

# [!DNL Bynder] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Bynder] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

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
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Bynder] モジュールを使用するには、[!DNL Bynder] アカウントが必要です。

## [!DNL Bynder] を Workfront Fusion に接続  {#connect-bynder-to-workfront-fusion}

* [ [!DNL Workfront Fusion] から  [!DNL Bynder]  への接続の作成](#create-a-connection-to-bynder-from-workfront-fusion)
* [ [!DNL Bynder]  での[!UICONTROL クライアント ID] と [!UICONTROL クライアントシークレット]の生成（オプション）](#generate-a-client-id-and-client-secret-in-bynder-optional)

### [!DNL Workfront Fusion] から [!DNL Bynder] への接続の作成

[!DNL Workfront Fusion] から [!DNL Bynder] アカウントへの接続を、[!DNL Bynder] モジュール内から直接作成できます。

1. 任意の [!DNL Bynder] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 接続する [!DNL Bynder] ドメインを選択します。
1. （オプション）「**[!UICONTROL 詳細設定]**」を選択し、「[!UICONTROL クライアント ID]」および「[!UICONTROL クライアントシークレット]」を入力します。

   クライアント ID とクライアントシークレットの生成手順については、[ [!DNL Bynder]  でのクライアント ID とクライアントシークレットの生成（オプション）](#generate-a-client-id-and-client-secret-in-bynder-optional) を参照してください。

1. [!UICONTROL ログイン]ウィンドウで、ユーザー名（メールアドレス）とパスワードを入力します。
1. 「**[!UICONTROL 続行]**」をクリックし、接続を作成して、モジュールに戻ります。

### [!DNL Bynder] での[!UICONTROL クライアント ID] と[!UICONTROL クライアントシークレット]の生成（オプション）

クライアント ID とクライアントシークレットを使用して接続を作成する場合は、[!DNL Bynder] アカウントから生成できます。クライアント ID とクライアントシークレットは、[!DNL Bynder] でアプリを作成するときに生成されます。

[!DNL Bynder] でアプリを作成する手順については、[!DNL Bynder] ドキュメントの [Oauth 2.0 アプリ](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) を参照してください。

>[!NOTE]
>
>[!DNL Bynder] でアプリを作成する場合、`redirect uri` として次を入力します。
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] モジュールとそのフィールド

[!DNL Bynder] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Bynder] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[モジュール間での情報のマッピング： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)を参照してください。

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)
* [トリガー](#triggers)

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL アセットメタデータの読み取り]](#read-asset-metadata)
* [[!UICONTROL アセットメタデータの更新]](#update-asset-metadata)
* [[!UICONTROL コレクションへのアセットの追加]](#add-assets-to-a-collection)
* [[!UICONTROL コレクションからアセットを削除]](#remove-assets-from-collection)
* [[!UICONTROL アセットへのタグの追加]](#add-a-tag-to-assets)
* [アセットからの[!UICONTROL タグの削除] ](#remove-a-tag-from-assets)
* [[!UICONTROL アセットのダウンロード]](#download-asset)
* [[!UICONTROL アセットのアップロード]](#upload-asset)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールでは、[!DNL Bynder] API への認証済みのカスタム呼び出しを実行できます。これにより、他の [!DNL Bynder] モジュールでは不可能なデータフロー自動処理を実現できます。

このモジュールを設定する際には、次のフィールドが表示されます。

このモジュールは、ステータスコードと共に、API 呼び出しのヘッダーと本文を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td><code>https://{your-bynder-domain}/api/{api-version}/</code> への相対パスを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は認証ヘッダーを追加します。</p> </td> 
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

#### [!UICONTROL アセットメタデータの読み取り]

このアクションモジュールは、アセットのメタデータを読み取ります。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>メタデータを取得するアセットの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットメタデータを更新]

このアクションモジュールは、既存のアセットのメタデータを更新します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>メタデータを更新するアセットの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields]</td> 
   <td> <p>情報を入力するフィールドを選択し、メタデータを更新する情報をこれらのフィールドに入力またはマッピングします。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metaproperties]</p> </td> 
   <td>更新するオプションを選択し、情報を入力するか、これらのプロパティにマッピングします。メタプロパティは、アセット内の特定のフィールドを表さないアセットに関する情報です。</td> 
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
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion] への [!DNL Bynder] の接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>アセットを追加するコレクションの ID を入力またはマッピングします。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>コレクションに追加するアセットごとに、「<strong>[!UICONTROL Add item]</strong>」をクリックし、アセット ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コレクションからアセットを削除]

このアクションモジュールは、1 つ以上のアセットをコレクションから削除します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>アセットを削除するコレクションの ID を入力またはマッピングします。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>コレクションから削除するアセットごとに、<strong>[!UICONTROL Add item]</strong> をクリックし、アセット ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットへのタグの追加]

1 つ以上のアセットへのタグの追加

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag ID]</td> 
   <td> <p>アセットに追加するタグの ID を入力またはマッピングします。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>タグを付けるアセットごとに、<strong>[!UICONTROL Add item]</strong> をクリックし、アセット ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットからのタグの削除]

1 つ以上のアセットからのタグの削除

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag ID]</td> 
   <td> <p>アセットから削除するタグの ID を入力またはマッピングします。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset IDs]</td> 
   <td> <p>タグを削除するアセットごとに、<strong>[!UICONTROL Add item]</strong> をクリックし、アセット ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットのダウンロード]

このアクションモジュールは、1 つのアセットをダウンロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>ダウンロードするアセットの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset version]</td> 
   <td> <p>ダウンロードするアセットのバージョンを入力またはマッピングします。アセットの最新バージョンをダウンロードするには、フィールドを空のままにします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットのアップロード]

このアクションモジュールは、1 つのアセットをアップロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save as]</td> 
   <td> <p>アップロードするファイルの保存方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL New asset]</strong> </p> <p>情報を入力するフィールドおよびメタプロパティを選択し、それらのフィールドに情報を入力します。</p> <p>アップロードしたアセットに使用するブランドの ID を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL New asset version]</strong> </p> <p>新しいバージョンをアップロードするアセットの ID を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL レコードをリスト]](#list-record)
* [[!UICONTROL アセットを検索]](#search-for-assets)

#### [!UICONTROL レコードをリスト]

この検索モジュールは、特定のタイプのすべての項目を取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>リストするレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Read all collections]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Read information about all tags]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Read all assets of a collection]</strong> </p> <p>アセットのリストを表示するコレクションの ID を入力またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットを検索]

この検索モジュールは、指定した条件に基づいてアセットを検索します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Bynder] を [!DNL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Criteria]</td> 
   <td> <p>検索条件を入力します。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>検索で使用するフィールドを選択します</p> </li> 
     <li> <p><strong>[!UICONTROL Logical Operator]</strong> </p> <p>検索に使用する演算子を選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>選択したフィールドに、検索する値を入力またはマッピングします。値のタイプは、選択したフィールドのデータタイプと同じである必要があります。 </p> <p>データタイプについて詳しくは、<a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> の項目データタイプを参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>最初に一致したアセットを返すか、一致したすべてのアセットを返すかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort by]</td> 
   <td> <p>並べ替えの基準となるフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort Direction]</td> 
   <td> <p>昇順と降順のどちらで並べ替えるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### トリガー

#### [!UICONTROL アセットの監視]

このトリガーモジュールは、アセットが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Bynder] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion] への [!DNL Bynder] の接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Collections]</td>
   <td> <p>新しいアセットを監視するコレクションを選択します。すべてのコレクションを監視するには、このフィールドを空のままにします。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limit]</td>

<td> <p>シナリオの実行サイクルごとにモジュールが返すレコードの最大数を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>
