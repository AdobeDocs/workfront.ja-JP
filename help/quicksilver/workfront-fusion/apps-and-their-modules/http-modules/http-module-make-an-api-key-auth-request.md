---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: http-modules
title: HTTP &gt;API キー認証リクエストの作成
description: この [!DNL Adobe Workfront Fusion] アクションモジュールは、API キー認証認証を必要とする指定された URL に HTTPS リクエストを送信し、応答を処理します。
author: Becky
feature: Workfront Fusion
exl-id: 70bf87c7-6d51-4ef4-9dce-80ad004e613f
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 0%

---

# HTTP >[!UICONTROL API キー認証リクエストの作成]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] にはが必要です [!DNL Adobe Workfront Fusion] ライセンスを追加してください。Adobe Workfrontライセンス。

この [!DNL Adobe Workfront Fusion] アクションモジュールは、API キー認証認証を必要とする指定された URL に HTTPS リクエストを送信し、応答を処理します。

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

詳しくは、 [!UICONTROL Adobe Workfront Fusion] ライセンス， 「 [Adobe Workfront Fusion ライセンス](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!UICONTROL HTTP] >[!UICONTROL API キー認証リクエストの作成] モジュール構成

次を設定する場合、 [!UICONTROL HTTP] >[!UICONTROL API キー認証リクエストの作成] モジュール [!DNL Adobe Workfront Fusion] 以下のフィールドが表示されます。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/mapping/map-information-between-modules.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 資格情報 ]</td> 
   <td> <p>API キー認証資格情報を含むキーを選択します。 新しいキーを追加するには、 <strong>[!UICONTROL 追加 ]</strong> 次の情報を設定します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL キー名 ]</strong></p> <p>この API 資格情報セットの名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL キー ]</strong> </p> <p>API キーを入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL API キーの配置 ]</strong> </p> <p>API キーをヘッダーに配置するか、API 呼び出しのクエリに配置するかを選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL API キーパラメーター名 ]</strong> </p> <p>API 呼び出しで API キーを識別する名前（「apiKey」や「X-API-Key」など）を入力します。 この情報は、モジュールが接続する Web サービスのドキュメントに記載されています。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL すべての状態をエラーとして評価（2xx および 3xx を除く）] </td> 
   <td> <p>エラー処理を設定するには、このオプションを使用します。</p> <p>詳しくは、 <a href="../../../workfront-fusion/errors/error-handling.md" class="MCXref xref">Adobe Workfront Fusion でのエラー処理</a>.</p> </td> 
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
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。 以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> 目的のクエリのキーと値のペアを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 本文の種類 ]</p> </td> 
   <td> <p>HTTP Body は、使用するヘッダーがある場合、そのヘッダーの直後に HTTP トランザクションメッセージで送信されるデータバイトです。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Raw]</strong> </p> <p>Raw body タイプは、開発者向けドキュメントで送信するデータが指定されていない場合でも、通常、ほとんどの HTTP body リクエストに適しています。</p> <p>データを解析する形式を「[!UICONTROL コンテンツタイプ ]」フィールドに指定します。</p> <p>選択したコンテンツタイプにもかかわらず、モジュールは開発者ドキュメントで規定または必要な任意の形式でデータを入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Application/x-www-form-urlencoded]</strong> </p> <p>この本文タイプは、 <code>application/x-www-form-urlencoded</code>.</p> <p>の場合 <code>[!UICONTROL application/x-www-form-urlencoded]</code>を指定した場合、サーバーに送信される HTTP メッセージの本文は基本的に 1 つのクエリ文字列になります。 キーと値は、 <code>&amp;</code> そして <code>=</code> キーと値の間。 </p> <p>バイナリデータの場合は、 <code>[!UICONTROL multipart/form-data]</code> 代わりに、</p> 
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
