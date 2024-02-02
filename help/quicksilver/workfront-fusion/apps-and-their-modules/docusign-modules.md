---
title: DocuSign モジュール
description: ' [!DNL Adobe Workfront Fusion DocuSign] モジュールを使用すると、エンベロープのステータスを監視および取得したり、エンベロープを検索および取得したり、ドキュメントをダウンロードして送信し、 [!DNL DocuSign] アカウントにログインしたりできます。'
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: ht
source-wordcount: '1943'
ht-degree: 100%

---

# DocuSign モジュール

[!DNL Adobe Workfront Fusion] [!DNL DocuSign]モジュールを使用すると、エンベロープのステータスを監視および取得したり、エンベロープを検索および取得したり、ドキュメントをダウンロードして送信し、[!DNL DocuSign]アカウントにログインしたりできます。

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

[!DNL DocuSign] モジュールを使用するには、[!DNL DocuSign] アカウントが必要です。

## [!DNL Workfront Fusion] を [!DNL DocuSign] に接続 {#connect-docusign-to-workfront-fusion}

[!DNL DocuSign] モジュールへの接続を作成するには：

1. 最初の [!DNL DocuSign] モジュールの設定を開始するときは、「[!UICONTROL 接続]」ボックスの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 以下の情報を入力します。

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>新しい [!DNL DocuSign] 接続の名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Account type]</td> 
      <td>接続するアカウントが実稼動アカウントかデモアカウントかを選択します。</td> 
     </tr> 
    </tbody> 
   </table>

1. [ [!DNL Adobe Workfront Fusion]  への接続の作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md#connect)の手順に従って続けます。

## [!DNL DocuSign] モジュールとそのフィールド

[!DNL DocuSign] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL DocuSign] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) で 1 つのモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

#### [!UICONTROL エンベロープの監視]

このトリガーモジュールは、エンベロープが送信、配信、署名、完了または拒否されたときにシナリオを開始します。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL DocuSign] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオ作成の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">[!DNL Workfront Fusion]</a> にモジュールのアプリまたは web サービスを接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>監視するレコードを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event type]</td> 
   <td> <p> 監視するイベントのタイプを選択します。</p> 
    <ul> 
     <li>[!UICONTROL Document completed]</li> 
     <li>[!UICONTROL Document declined]</li> 
     <li>[!UICONTROL Document sent]</li> 
     <li>[!UICONTROL Document signed]</li> 
     <li>[!UICONTROL New document in Inbox]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Output fields]</p> </td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが操作するレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL ドキュメントのダウンロード]](#download-a-document)
* [[!UICONTROL エンベロープを読む]](#read-an-envelope)
* [[!UICONTROL エンベロープにファイルをアップロード]](#upload-a-file-to-an-envelope)
* [[!UICONTROL エンベロープの新規作成]](#create-a-new-envelope)
* [[!UICONTROL エンベロープへの受信者の追加]](#add-recipient-to-envelope)
* [[!UICONTROL カスタムフィールドの追加]](#add-custom-field)
* [[!UICONTROL カスタムフィールドの変更]](#modify-custom-field)
* [[!UICONTROL エンベロープを送信]](#send-envelope)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
   <td> <p>[!DNL DocuSign] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">[!DNL Workfront Fusion]</a>への [!DNL DocuSign] の接続を参照してください、</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Account]</td> 
   <td>[!DNL DocuSign] API アクセスに使用するアカウントを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>モジュールとやり取りする web サーバー上のアドレスを入力します。</p> <p>相対 URL を入力できます。つまり、<code>http://</code> などのプロトコルを最初に含める必要はありません。これは、web サーバー上でやり取りが発生していることを示しています。</p> <p>例： <code>[!DNL /api/conversations].create</code></p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a> での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。これにより、リクエストのコンテンツタイプが決まります。</p> <p>例：<code> {"Content-type":"application/json"}</code></p> <p>メモ：エラーが表示され、エラーの発生元を特定するのが困難な場合は、[!DNL Workfront] ドキュメントに基づいてヘッダーの変更を考慮してください。カスタム API 呼び出しで 422 HTTP リクエストエラーが返される場合は、"Content-Type":"text/plain"ヘッダーを使用してみてください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>1 回の実行サイクルで処理する結果の最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例**：エンベロープのリスト
>
>次の API 呼び出しは、[!DNL DocuSign] アカウントの指定された日付からのエンベロープを返します。
>
>**URL**：`/v2.1/accounts/{accountId}/envelopes/`
>
>**メソッド**：`GET`
>
>**クエリ文字列**：
>
>* **キー**：`from_date`
>
>* **値**：`YYYY-MM-DD`
>
>リクエストがアカウント内のエンベロープのステータス変更のチェックを開始する時期を指定します。
>
>![](assets/example-docusign-setup-350x770.png)
>
>結果は、モジュールの出力（バンドル／本文／エンベロープの下）にあります。
>
>この例では、6 個のエンベロープが返されました。
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL ドキュメントのダウンロード]

このアクションモジュールは、1 つのドキュメントをダウンロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL DocuSign] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事内の<a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">[!DNL DocuSign] を [!DNL Workfront Fusion]</a> へ接続を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>ダウンロードするドキュメントを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> ダウンロードするエンベロープの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Document ID]</p> </td> 
   <td> <p>ダウンロードするドキュメントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Certificate]</td> 
   <td>ダウンロードにエンベロープ署名証明書を含める場合は、<strong>[!UICONTROL Yes]</strong> を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Documents by User ID]</td> 
   <td>受信者がユーザー ID でドキュメントを取得できるようにする場合は、<strong>[!UICONTROL Yes]</strong> を選択します。例えば、ユーザーが異なる表示の 2 つの異なるルーティングオーダーに含まれている場合、このオプションを使用すると、両方のルーティングのすべてのドキュメントが戻されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encrypt]</td> 
   <td>[!DNL DocuSign] アカウントに設定されているすべての主要なマネージャーに対して応答で返される PDF バイトを暗号化する場合は、<strong>[!UICONTROL Yes]</strong> を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Language]</td> 
   <td>言語を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show Changes]</td> 
   <td><strong>[!UICONTROL Yes]</strong> に設定すると、返された PDF の変更されたフィールドは黄色でハイライト表示され、オプションの署名またはイニシャルは赤色で囲まれます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watermark]</td> 
   <td> <p><strong>[!UICONTROL No]</strong> を選択して、PDF ドキュメントから透かしを削除します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL エンベロープの読み取り]

このアクションモジュールは、エンベロープ ID を使用して、[!DNL DocuSign] にあるエンベロープに関する情報を読み取ります。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL DocuSign] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">[!DNL DocuSign] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>情報を読み取るドキュメントを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> 情報を読み取るドキュメントを含む ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールの出力に表示するプロパティを選択します。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL エンベロープへのファイルのアップロード]

このモジュールは、指定されたファイルを DocuSign の既存のエンベロープにアップロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL DocuSign] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">[!DNL DocuSign] を [!DNL Workfront Fusion]</a> へ接続を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>ファイルをアップロードするエンベロープを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> ファイルをアップロードするエンベロープの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータを入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新規エンベロープの作成]

このアクションモジュールは、テンプレートから新規エンベロープを作成します。新規エンベロープの ID と、新規エンベロープのステータスを返します。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td>

<td> <p>DocuSign アカウントを Workfront Fusion に接続する手順について詳しくは、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion でのシナリオの作成</a>の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Account] </td>
   <td> <p>ファイルをアップロードするエンベロープを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template]</td>
   <td> <p> 新規エンベロープを作成するテンプレートを選択します。テンプレートは、選択した [!UICONTROL Account] に基づいて使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL After creation]
   </td> 
   <td> <p>エンベロープをドラフトとして保存するか、署名用に送信するかを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Template recipients]</td>
    <td>このエンベロープの受信者を選択します。</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL エンベロープへの受信者の追加]

このアクションモジュールは、1 人以上の受信者を既存のエンベロープに追加します。エンベロープが既に送信されている場合は、受信者にメールが送信されます。このモジュールは、既に完了しているエンベロープに対しては無効です。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL Connection] </td>
   <td> <p>DocuSign アカウントを Workfront Fusion に接続する手順について詳しくは、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion でのシナリオの作成</a>の記事の<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは web サービスを Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL Account] </td>
   <td> <p>受信者を追加するエンベロープを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Envelope ID]</td>
    <td>受信者を追加するエンベロープの ID を選択またはマッピングします。</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL Recipient type]</td>
   <td> <p> エンベロープに追加する受信者のタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL Agent]</p> </li> 
     <li> <p>[!UICONTROL Carbon copy]</p> </li> 
     <li> <p>[!UICONTROL Certified delivery]</p> </li> 
     <li> <p>[!UICONTROL In-person signer]</p> </li> 
     <li> <p>[!UICONTROL Intermediary]</p> </li> 
     <li> <p>[!UICONTROL Signer]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Email]</td>
   <td> <p>エンベロープに追加する受信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Name]</td>
   <td>エンベロープに追加する受信者の名前を入力またはマッピングします。</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Routing order]</td>
   <td> <p>受信者のルーティング番号を入力またはマッピングします。ルーティング番号は、受信者がドキュメントを受け取り署名する順序を指定するものです。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Email body]</td>
   <td>受信者に送信するメールの本文（コンテンツ）を入力またはマッピングします。</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL Email subject]</td>
   <td>受信者に送信するメールの件名を入力またはマッピングします。</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL Private message]</td>
   <td> <li> <p>選択した受信者にのみ、一般メッセージと共にプライベートメッセージも表示されます。プライベートメッセージの長さは 1000 文字までです。</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Authentication]</td> 
   <td> <p>受信者の ID の確認に使用する認証メソッドを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL None]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Access code]</strong> </p> <p>アクセスコードを入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL Phone]</strong> </p> <p>電話番号の入力またはマッピング</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>電話番号の入力またはマッピング</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタムフィールドの追加]

このアクションモジュールは、カスタムフィールドをドキュメントに追加します

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL DocuSign] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">[!DNL DocuSign] を [!DNL Workfront Fusion]</a> へ接続を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>カスタムフィールドを追加するドキュメントを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> カスタムフィールドを追加するドキュメントが含まれるエンベロープの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field name]</td> 
   <td>追加する新しいフィールドの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Required]</td> 
   <td>追加したフィールドを必須フィールドにする場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show field]</td> 
   <td>フィールドを表示する場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>追加したフィールドの値（コンテンツ）を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタムフィールドの変更]

このアクションモジュールは、フィールド名を使用してカスタムフィールドを変更します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL DocuSign] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">[!DNL DocuSign] を [!DNL Workfront Fusion]</a> へ接続を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>カスタムフィールドを変更するドキュメントを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> カスタムフィールドを変更するドキュメントが含まれるエンベロープの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field ID]</td> 
   <td>変更するフィールドの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field name]</td> 
   <td>変更するフィールドの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Required]</td> 
   <td>変更したフィールドを必須フィールドにする場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show field]</td> 
   <td>フィールドを表示する場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Value]</td> 
   <td>変更したフィールドの値（コンテンツ）を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL エンベロープの送信]

このアクションモジュールは、受信者に下書きエンベロープを送信します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL DocuSign] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">[!DNL DocuSign] を [!DNL Workfront Fusion]</a> へ接続を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Account] </td> 
   <td> <p>受信者に送信する下書きエンベロープを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Envelope ID]</td> 
   <td> <p> 受信者に送信する下書きエンベロープの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
