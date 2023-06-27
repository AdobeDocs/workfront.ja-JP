---
title: DocuSign モジュール
description: この [!DNL Adobe Workfront Fusion DocuSign] モジュールを使用すると、封筒のステータスを監視および取得したり、封筒を検索および取得したり、文書をダウンロードして送信し、サインインできます [!DNL DocuSign] アカウント
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: a6ebfe6f-dc3f-41f7-8129-bbc5775cff33
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1943'
ht-degree: 0%

---

# DocuSign モジュール

この [!DNL Adobe Workfront Fusion] [!DNL DocuSign] モジュールを使用すると、封筒のステータスを監視および取得したり、封筒を検索および取得したり、文書をダウンロードして送信し、サインインできます [!DNL DocuSign] アカウント

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

使用する [!DNL DocuSign] モジュールの場合、 [!DNL DocuSign] アカウント

## 接続 [!DNL DocuSign] から [!DNL Workfront Fusion] {#connect-docusign-to-workfront-fusion}

の接続を作成するには、以下を実行します。 [!DNL DocuSign] モジュール：

1. クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] 最初の [!DNL DocuSign] モジュール。
1. 以下を入力します。

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 接続名 ]</p> </td> 
      <td>新しい [!DNL DocuSign] 接続</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL アカウントタイプ ]</td> 
      <td>接続するアカウントが実稼動アカウントかデモアカウントかを選択します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 引き続き、 [への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md#connect).

## [!DNL DocuSign] モジュールとそのフィールド

設定時に [!DNL DocuSign] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL DocuSign] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)

### トリガー

#### [!UICONTROL 封筒を監視]

このトリガーモジュールは、エンベロープが送信、配信、署名、完了または拒否されたときにシナリオを開始します。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL DocuSign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">でのシナリオの作成 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アカウント ] </td> 
   <td> <p>監視するレコードを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベントタイプ ]</td> 
   <td> <p> 監視するイベントのタイプを選択します。</p> 
    <ul> 
     <li>[!UICONTROL ドキュメントが完了しました ]</li> 
     <li>[!UICONTROL ドキュメントが却下されました ]</li> 
     <li>[!UICONTROL ドキュメント送信済み ]</li> 
     <li>[!UICONTROL 署名済みドキュメント ]</li> 
     <li>[!UICONTROL インボックスに新しいドキュメントを追加 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 出力フィールド ]</p> </td> 
   <td> <p>モジュール出力に含めるフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが操作するレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL ドキュメントのダウンロード]](#download-a-document)
* [[!UICONTROL 封筒を読む]](#read-an-envelope)
* [[!UICONTROL エンベロープにファイルをアップロード]](#upload-a-file-to-an-envelope)
* [[!UICONTROL 新しいエンベロープを作成]](#create-a-new-envelope)
* [[!UICONTROL 受信者をエンベロープに追加]](#add-recipient-to-envelope)
* [[!UICONTROL カスタムフィールドを追加]](#add-custom-field)
* [[!UICONTROL カスタムフィールドを変更]](#modify-custom-field)
* [[!UICONTROL 封筒を送信]](#send-envelope)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL DocuSign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">接続 [!DNL DocuSign] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アカウント ]</td> 
   <td>アクセスに使用するアカウントを入力またはマッピングします [!DNL DocuSign] API</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>モジュールとやり取りする Web サーバーのアドレスを入力します。</p> <p>相対 URL を入力できます。つまり、プロトコルを含める必要はありません ( 例えば、 <code>http://</code>) を最初にクリックします。 これは、Web サーバー上でインタラクションが発生していることを示しています。</p> <p>例： <code>[!DNL /api/conversations].create</code></p>  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。 これにより、リクエストのコンテンツタイプが決まります。</p> <p>以下に例を挙げます。<code> {"Content-type":"application/json"}</code></p> <p>注意：エラーが発生し、エラーの発生元を特定するのが困難な場合は、 [!DNL Workfront] ドキュメント。 カスタム API 呼び出しで 422 HTTP リクエストエラーが返される場合は、「Content-Type」:「text/plain」ヘッダーを使用してみてください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ]</td> 
   <td>1 回の実行サイクルで処理する結果の最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** 封筒のリスト
>
>次の API 呼び出しは、 [!DNL DocuSign] アカウント：
>
>**URL**: `/v2.1/accounts/{accountId}/envelopes/`
>
>**メソッド**: `GET`
>
>**クエリ文字列**:
>
>* **キー**: `from_date`
>
>* **値**: `YYYY-MM-DD`
>
>要求がアカウント内の封筒のステータス変更の確認を開始する時期を指定します。
>
>![](assets/example-docusign-setup-350x770.png)
>
>結果は、モジュールの出力（Bundle > Body > envelopes の下）にあります。
>
>この例では、6 個の封筒が返されました。
>
>![](assets/docusign-example-output-350x677.png)

#### [!UICONTROL ドキュメントのダウンロード]

このアクションモジュールは、1 つのドキュメントをダウンロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL DocuSign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">接続 [!DNL DocuSign] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アカウント ] </td> 
   <td> <p>ダウンロードするドキュメントを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンベロープ ID]</td> 
   <td> <p> ダウンロードするエンベロープの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ドキュメント ID]</p> </td> 
   <td> <p>ダウンロードするドキュメントの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 証明書 ]</td> 
   <td>選択 <strong>[!UICONTROL はい ]</strong> ダウンロードに封筒署名証明書を含める場合。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ユーザー ID 別ドキュメント ]</td> 
   <td>選択 <strong>[!UICONTROL はい ]</strong> 受信者がユーザー ID でドキュメントを取得することを許可する場合。 たとえば、ユーザーが異なる表示の 2 つの異なる工順オーダーに含まれている場合、このオプションを使用すると、両方の工順のすべてのドキュメントが戻されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 暗号化 ]</td> 
   <td>選択 <strong>[!UICONTROL はい ]</strong> 応答で返されるPDFのバイト数を暗号化する場合は、 [!DNL DocuSign] アカウント</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 言語 ]</td> 
   <td>言語を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 変更を表示 ]</td> 
   <td>に設定する場合 <strong>[!UICONTROL はい ]</strong>を指定した場合、返されたPDFの変更されたフィールドは黄色でハイライト表示され、オプションの署名またはイニシャルは赤でアウトライン表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 透かし ]</td> 
   <td> <p>選択 <strong>[!UICONTROL いいえ ]</strong> 透かしドキュメントから透かしをPDFします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 封筒を読む]

このアクションモジュールは、 [!DNL DocuSign] エンベロープ ID を使用する。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL DocuSign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">接続 [!DNL DocuSign] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アカウント ] </td> 
   <td> <p>情報を読み取るドキュメントを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンベロープ ID]</td> 
   <td> <p> 情報を読み取るドキュメントを含む ID を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュールの出力に表示するプロパティを選択します。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL エンベロープにファイルをアップロード]

このモジュールは、指定されたファイルを DocuSign の既存のエンベロープにアップロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL DocuSign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">接続 [!DNL DocuSign] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アカウント ] </td> 
   <td> <p>ファイルをアップロードするエンベロープを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンベロープ ID]</td> 
   <td> <p> ファイルをアップロードするエンベロープの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータを入力します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新しいエンベロープを作成]

このアクションモジュールは、テンプレートから新しいエンベロープを作成します。 新しい封筒の ID と、新しい封筒のステータスを返します。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td>

<td> <p>DocuSign アカウントをWorkfront Fusion に接続する手順については、 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスをWorkfront Fusion に接続する</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion でシナリオを作成する</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL アカウント ] </td>
   <td> <p>ファイルをアップロードするエンベロープを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL テンプレート ]</td>
   <td> <p> 新しいエンベロープを作成するテンプレートを選択します。 テンプレートは、選択した [!UICONTROL アカウント ] に基づいて使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">
     [!UICONTROL 作成後 ]
   </td> 
   <td> <p>封筒を下書きとして保存するか、署名用に送信するかを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL テンプレート受信者 ]</td>
    <td>この封筒の受信者を選択</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 受信者をエンベロープに追加]

このアクションモジュールは、1 人以上の受信者を既存のエンベロープに追加します。 封筒が既に送信されている場合は、受信者に E メールが送信されます。 このモジュールは、既に完了している封筒に対しては無効です。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
    <td>[!UICONTROL 接続 ] </td>
   <td> <p>DocuSign アカウントをWorkfront Fusion に接続する手順については、 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">モジュールのアプリまたは Web サービスをWorkfront Fusion に接続する</a> 記事内 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion でシナリオを作成する</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="">
    <td>[!UICONTROL アカウント ] </td>
   <td> <p>受信者を追加するエンベロープを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL エンベロープ ID]</td>
    <td>を選択するか、受信者を追加するエンベロープの ID をマッピングします。</td>
  </tr> 
  <tr data-mc-conditions="">
    <td role="rowheader">[!UICONTROL 受信者のタイプ ]</td>
   <td> <p> 封筒に追加する受信者のタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL エージェント ]</p> </li> 
     <li> <p>[!UICONTROL Carbon Copy]</p> </li> 
     <li> <p>[!UICONTROL 認定配信 ]</p> </li> 
     <li> <p>[!UICONTROL 担当者署名者 ]</p> </li> 
     <li> <p>[!UICONTROL 中間者 ]</p> </li> 
     <li> <p>[!UICONTROL 署名者 ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL 電子メール ]</td>
   <td> <p>封筒に追加する受信者の電子メールアドレスを入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL 名前 ]</td>
   <td>封筒に追加する受信者の名前を入力またはマップします。</td> 
  </tr> 
  <tr>
    <td>[!UICONTROL ルーティング順序 ]</td>
   <td> <p>受信者のルーティング番号を入力またはマッピングします。 ルーティング番号は、受信者がドキュメントを受け取り、署名する順序を決定します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL 電子メール本文 ]</td>
   <td>受信者に送信する E メールの本文（コンテンツ）を入力またはマッピングします。</td> 
  </tr> 
  <tr>
    <td role="rowheader">[!UICONTROL 電子メールの件名 ]</td>
   <td>受信者に送信する E メールの件名を入力またはマッピングします。</td> 
  </tr> 
    <td role="rowheader">[!UICONTROL プライベートメッセージ ]</td>
   <td> <li> <p>選択した受信者にのみ、プライベートメッセージと一般メッセージが表示されます。 プライベートメッセージの長さは 1000 文字までです。</p> </li> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 認証 ]</td> 
   <td> <p>受信者の ID の確認に使用する認証方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL なし ]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL アクセスコード ]</strong> </p> <p>アクセスコードを入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL Phone]</strong> </p> <p>電話番号を入力またはマッピング</p> </li> 
     <li> <p><strong>[!UICONTROL SMS]</strong> </p> <p>電話番号を入力またはマッピング</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタムフィールドを追加]

このアクションモジュールは、カスタムフィールドをドキュメントに追加します

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL DocuSign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">接続 [!DNL DocuSign] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アカウント ] </td> 
   <td> <p>カスタムフィールドを追加するドキュメントを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンベロープ ID]</td> 
   <td> <p> カスタムフィールドを追加する文書が含まれる封筒の ID を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド名 ]</td> 
   <td>追加する新しいフィールドの名前を入力またはマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 必須 ]</td> 
   <td>追加したフィールドを必須フィールドにする場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールドを表示 ]</td> 
   <td>フィールドを表示する場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 値 ]</td> 
   <td>追加したフィールドの値（コンテンツ）を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタムフィールドを変更]

このアクションモジュールは、フィールド名を使用してカスタムフィールドを変更します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL DocuSign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">接続 [!DNL DocuSign] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アカウント ] </td> 
   <td> <p>カスタムフィールドを変更するドキュメントを含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンベロープ ID]</td> 
   <td> <p> カスタムフィールドを変更する文書が含まれる封筒の ID を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド ID]</td> 
   <td>変更するフィールドの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド名 ]</td> 
   <td>変更するフィールドの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 必須 ]</td> 
   <td>変更したフィールドを必須フィールドにする場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールドを表示 ]</td> 
   <td>フィールドを表示する場合は、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 値 ]</td> 
   <td>変更したフィールドの値（コンテンツ）を入力またはマッピングします。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 封筒を送信]

このアクションモジュールは、受信者に下書きエンベロープを送信します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL DocuSign] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-docusign-to-workfront-fusion" class="MCXref xref">接続 [!DNL DocuSign] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アカウント ] </td> 
   <td> <p>受信者に送信する下書き封筒を含むアカウントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンベロープ ID]</td> 
   <td> <p> 受信者に送信する下書き封筒の ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
