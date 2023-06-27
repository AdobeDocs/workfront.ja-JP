---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: AWS S3 モジュール
description: この [!DNL Adobe Workfront Fusion AWS] S3 モジュールを使用すると、S3 バケットに対して操作を実行できます。
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 1%

---

# AWS S3 モジュール

この [!DNL Adobe Workfront Fusion AWS] S3 モジュールを使用すると、S3 バケットに対して操作を実行できます。

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

使用する [!UICONTROL AWS S3] モジュールの場合、 [!DNL Amazon Web Service] アカウント

## 接続 [!DNL AWS] から [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

接続するには [!DNL AWS S3] から [!DNL Workfront Fusion] 接続する必要があります [!DNL AWS] アカウント [!DNL Workfront Fusion]. これをおこなうには、まず [!DNL AWS] [!UICONTROL IAM].

1. ログイン先 [!DNL AWS] [!UICONTROL IAM] アカウント
1. に移動します。 **[!UICONTROL ID とアクセスの管理]** > **[!UICONTROL アクセス管理]** > **[!UICONTROL ユーザー]**.

1. クリック **[!UICONTROL ユーザーを追加]**.
1. 新しいユーザーの名前を入力し、 **[!UICONTROL プログラムアクセス]** オプション [!UICONTROL アクセスタイプ] 」セクションに入力します。
1. クリック **[!UICONTROL 既存のポリシーを直接添付]**&#x200B;を検索し、 **[!UICONTROL AmazonS3FullAccess]** をクリックします。 表示されたらクリックし、 **[!UICONTROL 次へ]**.

1. 他のダイアログ画面を進み、「 **[!UICONTROL ユーザーを作成]**.
1. 提供されたをコピーします。 **[!UICONTROL アクセスキー ID]** および **[!UICONTROL 秘密アクセスキー]**.

1. に移動します。 [!DNL Workfront Fusion] をクリックし、 [!DNL AWS S3] モジュール **[!UICONTROL 接続の作成]** ダイアログ。
1. 次を入力します。 [!UICONTROL アクセスキー ID] および [!UICONTROL 秘密アクセスキー] 手順 7 から各フィールドに移動し、 **[!UICONTROL 続行]** 接続を確立するために。

接続が確立されました。 モジュールの設定に進むことができます。

## [!DNL AWS S3] モジュールとそのフィールド

設定時に [!DNL AWS S3] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL AWS S3] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)

### アクション

* [[!UICONTROL バケットを作成]](#create-bucket)
* [[!UICONTROL ダウンロード]](#get-file)
* [[!UICONTROL ファイルをアップロード]](#upload-file)
* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)

#### [!UICONTROL バケットを作成]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL AWS] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">接続 [!DNL AWS] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>新しいバケットの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 地域 ] </td> 
   <td> <p>地域のエンドポイントを選択します。 詳しくは、 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a> (AWSドキュメント ) を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ダウンロード]

バケットからファイルをダウンロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL AWS] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">接続 [!DNL AWS] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 地域 ] </td> 
   <td> <p>地域のエンドポイントを選択します。 詳しくは、 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a> 内 [!DNL AWS] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL バケット ] </td> 
   <td> <p>ファイルのダウンロード元のバケットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL パス ]</p> </td> 
   <td> <p>ファイルのパスを入力します。 例: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをアップロード]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL AWS] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">接続 [!DNL AWS] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 地域 ] </td> 
   <td> <p>地域のエンドポイントを選択します。 詳しくは、 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a> 内 [!DNL AWS] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL フォルダー ] （オプション） </p> </td> 
   <td> <p>ファイルのアップロード先のフォルダーを指定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers] （オプション）</p> </td> 
   <td> <p> リクエストヘッダーを挿入します。 使用可能なヘッダーは、 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] ドキュメント — [!UICONTROLPUT] オブジェクト</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 呼び出しを実行する]

詳しくは、 [!DNL Amazon S3] API（を参照） [[!DNL Amazon S3] [!UICONTROL REST] API の概要](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL AWS] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">接続 [!DNL AWS] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 地域 ] </td> 
   <td> <p>地域のエンドポイントを選択します。 詳しくは、 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a> 内 [!DNL AWS] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL ホスト URL を入力します。 パスは次を基準として指定する必要があります：<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある [!UICONTROL HTTP] リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP] リクエストメソッド ( [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>リクエストヘッダーを追加します。 次の共通のリクエストヘッダーを使用できます。 リクエストヘッダーの詳細については、 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API ドキュメント</a>.</p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>ヘッダー名</th> 
       <th> <p> 説明</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>RFC 2616 に従ったメッセージの長さ（ヘッダーなし）。 このヘッダーは、[!UICONTROLPUT] や、XML を読み込む操作（ログや ACL など）に必要です。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>リソースのコンテンツタイプ（リクエストコンテンツが本文にある場合）。 例: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>RFC 1864 に従って、base64 エンコードされた 128 ビットの MD5 ダイジェスト（ヘッダーなし）。 このヘッダーは、メッセージの整合性チェックとして使用し、データが最初に送信されたのと同じデータであることを検証できます。 これはオプションですが、[!UICONTROL Content-MD5] メカニズムをエンドツーエンドの整合性チェックとして使用することをお勧めします。 [!UICONTROL REST] リクエスト認証について詳しくは、 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST] 認証</a> 内 <i>[!DNL Amazon] シンプルストレージサービス開発者ガイド</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL 日付 ]</p> </td> 
       <td> <p>要求者に応じた現在の日時。 例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 次の場合、 <code>Authorization </code>ヘッダーの場合は、 <code>x-amz-date</code> または <code>Date </code>ヘッダー。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>アプリケーションで [!UICONTROL 100-continue] を使用する場合、確認を受け取るまでリクエスト本文は送信されません。 ヘッダーに基づいてメッセージを拒否した場合、メッセージの本文は送信されません。 このヘッダーは、本文を送信する場合にのみ使用できます。</p> <p>有効な値：[!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL ホスト ]</p> </td> 
       <td> <p>パススタイルのリクエストの場合、値は <code>s3.amazonaws.com</code>. 仮想スタイルのリクエストの場合、値は <code>BucketName.s3.amazonaws.com</code>. 詳しくは、 <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">仮想ホスティング</a> 内 <i>[!DNL Amazon] シンプルストレージサービス開発者ガイド</i>.</p> <p>このヘッダーは HTTP 1.1 で必要です（ほとんどのツールキットはこのヘッダーを自動的に追加します）。HTTP/1.0 要求の場合はオプションです。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>署名バージョン 4 を使用して要求を認証する場合、このヘッダーは要求ペイロードのハッシュを提供します。 オブジェクトをチャンク単位でアップロードする場合は、値をに設定します。 <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> 署名がヘッダーのみを対象とし、ペイロードがないことを示す場合。 詳しくは、 <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">認証ヘッダーの署名の計算：複数のチャンクでのペイロードの転送（チャンクアップロード） ([!DNL AWS] 署名のバージョン 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>要求者に応じた現在の日時。 例: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. 次の場合、 <code>Authorization </code>ヘッダーの場合は、 <code>x-amz-date</code> または <code>Date </code>ヘッダー。 両方を指定した場合、 <code>x-amz-date</code> ヘッダーが優先されます。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>このヘッダーは、次のシナリオで使用できます。</p> 
        <ul> 
         <li>のセキュリティトークンを提供 [!DNL Amazon DevPay] 操作。 を使用する各リクエスト [!DNL Amazon DevPay] 2 つ必要 <code>x-amz-security-token</code> headers:1 つは製品トークン用、もう 1 つはユーザートークン用です。 条件 [!DNL Amazon S3] は認証済み要求を受け取り、計算済みの署名と指定された署名を比較します。 形式が適切でない複数値ヘッダーが署名の計算に使用されている場合、認証に問題が発生する可能性があります。</li> 
         <li>一時的なセキュリティ資格情報を使用する場合は、セキュリティトークンを指定します。 IAM から取得した一時的なセキュリティ認証情報を使用して要求を行う場合は、このヘッダーを使用してセキュリティトークンを提供する必要があります。 一時的なセキュリティ認証情報の詳細については、 Making Requests を参照してください。</li> 
        </ul> <p>このヘッダーは、 [!DNL Amazon DevPay] とは、一時的なセキュリティ資格情報を使用して署名された要求を指します。</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>パラメーターやフォームフィールドなど、必要なクエリ文字列を追加します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:   <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL リストファイル]](#list-files)
* [[!UICONTROL フォルダのリスト]](#list-folders)

#### [!UICONTROL リストファイル]

指定された場所からファイルのリストを返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL AWS] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">接続 [!DNL AWS] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 地域 ] </td> 
   <td> <p>地域のエンドポイントを選択します。 詳しくは、 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a> 内 [!DNL AWS] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL バケット ] </td> 
   <td> <p>を選択します。 [!DNL Amazon S3] バケットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL プレフィックス ] （オプション）</p> </td> 
   <td> <p> ファイルを検索するフォルダーのパス（例： ） <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダのリスト]

指定された場所からフォルダの一覧を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL AWS] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">接続 [!DNL AWS] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 地域 ] </td> 
   <td> <p>地域のエンドポイントを選択します。 詳しくは、 <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a> (AWSドキュメント ) を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL バケット ] </td> 
   <td> <p>を選択します。 [!DNL Amazon S3] バケットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL プレフィックス ] （オプション）</p> </td> 
   <td> <p> フォルダーを検索するフォルダーのパス（例： ） <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
