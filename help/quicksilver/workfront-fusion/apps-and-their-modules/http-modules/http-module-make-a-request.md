---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: http-modules
title: HTTP &gt;リクエストモジュールの作成
description: Adobe Workfront Fusion HTTP &gt;Make a request module は、HTTP リクエストを設定し、サーバーに送信できる汎用モジュールです。 受け取った HTTP 応答は、出力バンドルに含まれます。
author: Becky
feature: Workfront Fusion
exl-id: 7857c395-ce84-480e-8fa2-065035ac5b95
source-git-commit: 58db2129dd764d24b0a681735c2405be402d8b43
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# [!UICONTROL HTTP] >[!UICONTROL リクエストを実行] モジュール

>[!NOTE]
>
>Adobe Workfront Fusion には、 [!DNL Adobe Workfront Fusion] に加えてライセンス [!DNL Adobe Workfront] ライセンス。

この [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL リクエストモジュールの作成] は、HTTP リクエストを設定し、サーバーに送信できる汎用モジュールです。 受け取った HTTP 応答は、出力バンドルに含まれます。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [Adobe Workfront Fusion ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL リクエストを実行] モジュール構成

次を設定する場合、 [!UICONTROL HTTP] >[!UICONTROL リクエストを実行] モジュール [!DNL Adobe Workfront Fusion] 以下のフィールドが表示されます。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL すべての状態をエラーとして評価（2xx および 3xx を除く）] </td> 
   <td> <p>エラー処理を設定するには、このオプションを使用します。</p> <p>詳しくは、 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">でのエラー処理 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>API エンドポイント、Web サイトなど、リクエストの送信先 URL を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> 目的のクエリのキーと値のペアを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 本文の種類 ]</p> </td> 
   <td> <p>HTTP Body は、使用するヘッダーがある場合、そのヘッダーの直後に HTTP トランザクションメッセージで送信されるデータバイトです。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Raw body タイプは、開発者向けドキュメントで送信するデータが指定されていない場合でも、通常、ほとんどの HTTP body リクエストに適しています。</p> <p>データを解析する形式を「[!UICONTROL コンテンツタイプ ]」フィールドに指定します。</p> <p>選択したコンテンツタイプにもかかわらず、デベロッパードキュメントで規定または必要な任意の形式でデータが入力されます。</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>この本文タイプは、 <code>[!UICONTROL application/x-www-form-urlencoded]</code>.</p> <p>の場合 <code>application/x-www-form-urlencoded</code>を指定した場合、サーバーに送信される HTTP メッセージの本文は基本的に 1 つのクエリ文字列になります。 キーと値は、 <code>&amp;</code> そして <code>=</code> キーと値の間。 </p> <p>バイナリデータの場合は、 <code>[!UICONTROL multipart/form-data]</code> 代わりに、</p> 
      <div class="example" data-mc-autonum="<b>Example: </b>">
       <span class="autonumber"><span><b>例: </b></span></span> 
       <p>結果の HTTP リクエスト形式の例：</p> 
       <p><code>field1=value1&amp;field2=value2</code> </p> 
      </div> </li> 
     <li> <p><strong>[!UICONTROL Multipart/form-data]</strong> </p> <p>[!UICONTROL Multipart/form-data] は、ファイルとデータの送信に使用される HTTP マルチパートリクエストです。 通常、ファイルをサーバーにアップロードする際に使用されます。</p> <p>リクエストで送信するフィールドを追加します。 各フィールドには、キーと値のペアが含まれている必要があります。</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL テキスト ]</strong> </p> <p>リクエスト本文内で送信するキーと値を入力します。</p> </li> 
       <li> <p><strong>[!UICONTROL ファイル ]</strong> </p> <p>キーを入力し、リクエスト本文で送信するソースファイルを指定します。</p> <p>前のモジュールからアップロードするファイルをマッピングする ([!UICONTROL HTTP] &gt;[!UICONTROL ファイルを取得 ] または [!UICONTROL Google Drive] &gt;[!UICONTROL ファイルをダウンロード )) か、ファイル名とファイルデータを手動で入力します。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 応答を解析 ]</p> </td> 
   <td> <p>このオプションを有効にすると、応答を自動的に解析し、JSON および XML 応答を変換して、[!UICONTROL JSON] / [!UICONTROL JSON を解析 ] または [!UICONTROL XML] / [!UICONTROL XML] モジュールを使用する必要がなくなります。</p> <p>解析された JSON または XML コンテンツを使用する前に、モジュールを手動で 1 回実行して、モジュールが応答コンテンツを認識し、後続のモジュールにマッピングできるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ユーザー名 ]</p> </td> 
   <td> <p> 基本的な認証を使用してリクエストを送信する場合は、ユーザー名を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL パスワード ] </td> 
   <td> <p>基本的な認証を使用してリクエストを送信する場合は、パスワードを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タイムアウト ] </td> 
   <td> <p>リクエストのタイムアウトを秒単位で指定します (1 ～ 300)。 デフォルトは 40 秒です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 他の HTTP モジュールとの Cookie の共有 ]</td> 
   <td> <p> このオプションを有効にすると、シナリオ内のすべての HTTP モジュールとサーバーから Cookie を共有できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 自己署名証明書 ]</td> 
   <td> <p> 自己署名証明書を使用して TLS を使用する場合は、証明書をアップロードします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 未検証（自己署名）証明書を使用している接続を拒否します ] </td> 
   <td> <p>未検証の TLS 証明書を使用している接続を拒否する場合は、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL リダイレクトに従う ]</td> 
   <td> <p> このオプションを有効にすると、3xx 応答で URL リダイレクトに従います。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL すべてのリダイレクトに従う ] </td> 
   <td> <p>このオプションを有効にすると、すべての応答コードで URL リダイレクトに従います。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 配列と同じ複数のクエリ文字列キーのシリアル化を無効にする ]</p> </td> 
   <td> <p>デフォルトでは、 [!DNL Workfront Fusion] は、配列と同じ URL クエリー文字列パラメーターキーに対する複数の値を処理します。 例： <code>www.test.com?foo=bar&amp;foo=baz</code> が次に変換されます： <code>www.test.com?foo[0]=bar&amp;foo[1]=baz</code>. この機能を無効にするには、このオプションを有効にします。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 圧縮コンテンツをリクエスト ]</td> 
   <td> <p> Web サイトの圧縮バージョンを要求するには、このオプションを有効にします。</p> <p>を追加します。 <code>[!UICONTROL Accept-Encoding]</code> 圧縮コンテンツをリクエストするヘッダー。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 相互 TLS を使用 ]</td> 
   <td> <p>HTTP リクエストで相互 TLS を使用するには、このオプションを有効にします。</p> <p>相互 TLS について詳しくは、 <a href="../../../workfront-fusion/apps-and-their-modules/http-modules/use-mtls-in-http-modules.md" class="MCXref xref">の HTTP モジュールでの相互 TLS の使用 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** この例では、 [!UICONTROL POST] JSON ペイロードを使用したリクエスト：
>
>![](assets/make-a-request-example-350x522.png)

>[!NOTE]
>
>次の手順で [!UICONTROL JSON] が有効な場合は、次のような利用可能なオンラインサービスの 1 つを使用できます。 [https://jsonlint.com/](https://jsonlint.com/). また、 [!UICONTROL JSON] >[!UICONTROL JSON モジュールの作成] :JSON を動的に作成し、必要なエスケープをすべて処理します。
>
>JSON の要素と式および項目の直接の内での混合 [!UICONTROL コンテンツを要求] フィールドは、無効な JSON になる可能性があるので、お勧めしません。
