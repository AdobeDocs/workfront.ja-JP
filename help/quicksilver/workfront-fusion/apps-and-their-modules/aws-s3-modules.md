---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: AWS S3 モジュール
description: ' [!DNL Adobe Workfront Fusion AWS]  S3 モジュールを使用すると、S3 バケットに対して操作を実行できます。'
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1429'
ht-degree: 100%

---

# AWS S3 モジュール

[!DNL Adobe Workfront Fusion AWS] S3 モジュールを使用すると、S3 バケットに対して操作を実行できます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件はありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!UICONTROL AWS S3] モジュールを使用するには [!DNL Amazon Web Service] アカウントが必要です。

## [!DNL AWS] を [!DNL Workfront Fusion] に接続 {#connect-aws-to-workfront-fusion}

[!DNL AWS S3] を [!DNL Workfront Fusion] に接続するには、[!DNL AWS] アカウントを [!DNL Workfront Fusion] に接続する必要があります。これを行うには、まず [!DNL AWS] [!UICONTROL IAM] で API ユーザーを作成します。

1. [!DNL AWS] [!UICONTROL IAM] アカウントにログインします。
1. **[!UICONTROL ID とアクセスの管理]**／**[!UICONTROL アクセス管理]**／**[!UICONTROL ユーザー]**&#x200B;に移動します。

1. 「**[!UICONTROL ユーザーを追加]**」をクリックします。
1. 新しいユーザーの名前を入力し、「[!UICONTROL アクセスタイプ]」セクションで「**[!UICONTROL プログラムアクセス]**」オプションを選択します。
1. 「**[!UICONTROL 既存のポリシーを直接添付]**」をクリックして、検索バーで **[!UICONTROL AmazonS3FullAccess]** を検索します。それが表示されたら選択して「**[!UICONTROL 次へ]**」をクリックします。

1. 他のダイアログ画面を進み、「**[!UICONTROL ユーザーを作成]**」をクリックします。
1. 提供された&#x200B;**[!UICONTROL アクセスキー ID]** および&#x200B;**[!UICONTROL 秘密アクセスキー]**&#x200B;をコピーします。

1. [!DNL Workfront Fusion] に移動して、[!DNL AWS S3] モジュールの&#x200B;**[!UICONTROL 接続を作成]**&#x200B;ダイアログを開きます。
1. 手順7の「[!UICONTROL アクセスキー ID]」および「[!UICONTROL 秘密アクセスキー]」をそれぞれのフィールドに入力し、「**[!UICONTROL 続行]**」をクリックして接続を確立します。

接続が確立されました。モジュールの設定に進むことができます。

## [!DNL AWS S3] モジュールとそのフィールド

[!DNL AWS S3]モジュールを設定すると、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL AWS S3] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)

### アクション

* [[!UICONTROL バケットを作成]](#create-bucket)
* [[!UICONTROL ファイルを取得]](#get-file)
* [[!UICONTROL ファイルをアップロード]](#upload-file)
* [[!UICONTROL API 呼び出しを実行]](#make-an-api-call)

#### [!UICONTROL バケットを作成]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事内の<a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>新しいバケットの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>地域のエンドポイントを選択します。詳しくは、AWS ドキュメント内の<a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a>の説明を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルを取得]

バケットからファイルをダウンロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事内の<a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>地域のエンドポイントを選択します。詳しくは、[!DNL AWS] ドキュメント内の<a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a>の説明を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>ファイルのダウンロード元のバケットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>ファイルにパスを入力します。例：<code>/photos/2019/February/image023.jpg</code>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルをアップロード]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事内の<a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>地域のエンドポイントを選択します。詳しくは、[!DNL AWS] ドキュメント内<a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a>の説明を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Folder]（オプション） </p> </td> 
   <td> <p>ファイルのアップロード先であるターゲットフォルダーを指定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers]（オプション）</p> </td> 
   <td> <p> リクエストヘッダーを挿入します。使用可能なヘッダーについては、<a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] ドキュメントの [!UICONTROL PUT] オブジェクト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 呼び出しを実行]

[!DNL Amazon S3] API の詳細な説明については、[[!DNL Amazon S3] [!UICONTROL REST]  API の概要](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html)を参照してください。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事内の<a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>地域のエンドポイントを選択します。詳しくは、[!DNL AWS] ドキュメント内の<a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a>の説明を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL でホスト URL を入力します。パスは <code> https://s3.&lt;selected-region>.amazonaws.com/</code> を基準として指定する必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しを設定する必要がある [!UICONTROL HTTP] リクエストメソッドを選択します。詳細情報は、[!DNL Adobe Workfront Fusion]</a> の <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP] リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers]</td> 
   <td> <p>リクエストヘッダーを追加します。次の共通のリクエストヘッダーを使用できます。リクエストヘッダーについて詳細は、<a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3]API ドキュメント</a>を参照してください。</p> <p>[!DNL Workfront Fusion] 認証ヘッダーを自動的に追加します。</p> 
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
       <td> <p>RFC 2616 に従ったメッセージの長さ（ヘッダーなし）。このヘッダーは、[!UICONTROL PUT] や、XML を読み込む操作（ログや ACL など）に必要です。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>リソースのコンテンツタイプ（リクエストコンテンツが本文にある場合）。例：<code>text/plain</code>。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>RFC 1864 に従って、base64 エンコードされた 128 ビットの MD5 ダイジェスト（ヘッダーなし）。このヘッダーをメッセージの整合性チェックとして使用し、データが最初に送信されたのと同じデータであることを検証できます。これはオプションですが、[!UICONTROL Content-MD5] メカニズムをエンドツーエンドの整合性チェックとして使用することをお勧めします。[!UICONTROL REST] リクエスト認証について詳しくは、<i>[!DNL Amazon]シンプルストレージサービス開発者ガイド</i>の <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST] 認証</a>を参照してください。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Date]</p> </td> 
       <td> <p>リクエスターに応じた現在の日時。例：<code>Wed, 01 Mar 2006 12:00:00 GMT</code>。<code>Authorization </code> ヘッダーを指定する場合は、<code>x-amz-date</code> ヘッダーまたは <code>Date </code> ヘッダーを指定する必要があります。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>アプリケーションで [!UICONTROL 100-continue] を使用する場合、確認を受け取るまでリクエスト本文は送信されません。ヘッダーに基づいてメッセージを拒否した場合、メッセージの本文は送信されません。このヘッダーは、本文を送信する場合にのみ使用できます。</p> <p>有効な値：[!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>パススタイルのリクエストの場合、値は <code>s3.amazonaws.com</code> です。仮想スタイルのリクエストの場合、値は <code>BucketName.s3.amazonaws.com</code> です。詳細情報については、<i>[!DNL Amazon]シンプルストレージサービス開発者ガイド</i>の<a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">仮想ホスティング</a>を参照してください。</p> <p>このヘッダーは HTTP 1.1 に必要であり、ほとんどのツールキットで自動的に追加されます。HTTP/1.0 リクエストの場合はオプションです。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>署名バージョン 4 を使用してリクエストを認証する場合は、このヘッダーによってリクエストペイロードのハッシュが提供されます。オブジェクトをチャンク単位でアップロードする場合は、値を <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> に設定して、署名がヘッダーのみを対象とし、ペイロードがないことを示します。詳細情報については、<a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">認証ヘッダーの署名の計算：複数チャンクでのペイロードの転送（チャンクアップロード）（[!DNL AWS]署名バージョン 4）</a>を参照してください。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>リクエスターに応じた現在の日時。例：<code>Wed, 01 Mar 2006 12:00:00 GMT</code>。<code>Authorization </code> ヘッダーを指定する場合は、<code>x-amz-date</code> ヘッダーまたは <code>Date </code> ヘッダーを指定する必要があります。両方を指定した場合は、<code>x-amz-date</code> ヘッダーの値が優先されます。</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>このヘッダーは、次のシナリオで使用できます。</p> 
        <ul> 
         <li>[!DNL Amazon DevPay]操作のためにセキュリティトークンを提供します。[!DNL Amazon DevPay]を使用する各リクエストには、製品トークン用とユーザートークン用の 2 つの<code>x-amz-security-token</code>ヘッダーが必要です。[!DNL Amazon S3] が認証済みリクエストを受け取ると、計算済みの署名と提供された署名を比較します。署名の計算に使用されている複数値ヘッダーの形式が適切でない場合、認証の問題が発生する可能性があります。</li> 
         <li>一時的なセキュリティ資格情報を使用する場合は、セキュリティトークンを提供します。IAM から取得した一時的なセキュリティ認証情報を使用してリクエストを行う際には、このヘッダーを使用してセキュリティトークンを提供する必要があります。一時的なセキュリティ認証情報の詳細については、「リクエストの実行」を参照してください。</li> 
        </ul> <p>このヘッダーは、[!DNL Amazon DevPay] を使用するリクエストおよび一時的なセキュリティ認証情報を使用して署名されたリクエストに必要です。</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p>パラメーターやフォームフィールドなど、必要なクエリ文字列を追加します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：   <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL ファイルをリストする]](#list-files)
* [[!UICONTROL フォルダーをリストする]](#list-folders)

#### [!UICONTROL ファイルをリストする]

指定された場所からファイルのリストを返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>地域のエンドポイントを選択します。詳しくは、[!DNL AWS] ドキュメントで<a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a>についての説明を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>ファイルを検索する [!DNL Amazon S3] バケットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix]（オプション）</p> </td> 
   <td> <p> ファイルを検索するフォルダーのパス（例： <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL フォルダーをリストする]

指定された場所からフォルダーのリストを返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL AWS] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-aws-to-workfront-fusion" class="MCXref xref">[!DNL AWS] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>地域のエンドポイントを選択します。詳しくは、AWS ドキュメントで<a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">地域エンドポイント</a>についての説明を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>フォルダーを検索する [!DNL Amazon S3] バケットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Prefix]（オプション）</p> </td> 
   <td> <p> フォルダーを検索するフォルダーのパス（例： <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
