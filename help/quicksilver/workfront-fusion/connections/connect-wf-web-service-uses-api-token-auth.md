---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: API トークン認証を使用する Web サービスに  [!DNL Adobe Workfront Fusion]  を接続
description: 一部のサービスでは、シナリオで簡単に使用できるアプリを  [!DNL Adobe Workfront Fusion]  のような統合ソリューションで作成することは許可されません。
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: e61dc6646e221cffb30aad055663dcf8fd3299e2
workflow-type: ht
source-wordcount: '946'
ht-degree: 100%

---

# API トークン認証を使用する Web サービスに [!DNL Adobe Workfront Fusion] を接続

一部のサービスでは、シナリオで簡単に使用できるアプリを [!DNL Adobe Workfront Fusion] のような統合ソリューションで作成することは許可されません。

この状況に対する回避策があります。[!DNL Workfront Fusion] の [!UICONTROL HTTP] モジュールを使用して、目的のサービス（アプリ）を [!DNL Workfront Fusion] に接続できます。

この記事では、API キーまたは API トークンを使用して、ほとんどすべての web サービスを [!DNL Workfront Fusion] に接続する方法を説明します。

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

## API トークンを使用する web サービスへの接続

API トークンを介してサービスに接続する手順は、ほとんどの web サービスで同様です。

1. Web サービスの web サイト上にアプリケーションを作成します。詳しくは、この記事の[新しいアプリケーションを作成して API トークンを取得](#create-a-new-application-and-obtain-the-api-token)を参照してください。
1. API キーまたは API トークンを取得します。
1. [!DNL Workfront Fusion] の [!UICONTROL HTTP] > [!UICONTROL リクエストの作成]モジュールをシナリオに追加します。
1. Web サービスの API ドキュメントに従ってモジュールを設定し、シナリオを実行します。詳しくは、この記事の [[!UICONTROL HTTP] モジュールの設定](#set-up-the-http-module)の節を参照してください。

>[!NOTE]
>
>この記事では、全体を通して [!DNL Pushover] 通知サービスを例として使用します。

## 新しいアプリケーションを作成して API トークンを取得

>[!NOTE]
>
>Web サービスで API キーまたは API トークンを作成および配布するには、多くの異なる方法があります。目的の web サービスの API キーとトークンの取得手順については、サービスの web サイトにアクセスし、「API キー」または「API トークン」を検索してください。
>
>Pushover API キーを取得する手順は、検索対象の例として記載しているだけです。

1. [!DNL Pushover] アカウントにログインします。
1. ページの下部にある「**[!UICONTROL Create an Application/API Token]**」をクリックします。
1. アプリケーション情報を入力し、「**[!UICONTROL Create an Application]**」をクリックします。
1. 提供された API トークンを安全な場所に保存します。これは、[!DNL Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL リクエストの作成]モジュールで目的の Web サービス（この場合は [!DNL Pushover]）に接続するために必要となります。

## [!UICONTROL HTTP] モジュールを設定

Web サービスを [!DNL Workfront Fusion] シナリオに接続するには、シナリオで [!UICONTROL HTTP] > [!UICONTROL リクエストの作成]モジュールを使用して、web サービスの API ドキュメントに従ってモジュールを設定する必要があります。

1. [!UICONTROL HTTP] > [!UICONTROL リクエストの作成]モジュールをシナリオに追加します。
1. [!DNL Workfront Fusion] を使用してメッセージをプッシュするには、HTTP モジュールを次のように設定します。

   >[!NOTE]
   >
   >これらのモジュール設定は、[!DNL Pushover] web サービスの API ドキュメントに対応します。他の web サービスでは設定が異なる場合があります。例えば、API トークンを[!UICONTROL 本文]フィールドではなく[!UICONTROL ヘッダー]に挿入するなどです。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>URL フィールドには、web サービスの API ドキュメントで確認できるエンドポイントが含まれます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>使用されるメソッドは、対応するエンドポイントによって異なります。メッセージをプッシュするための Pushover エンドポイントでは、POST メソッドを使用します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>一部の web サービスでは、ヘッダーを使用して API トークン認証や他のパラメーターを指定します。メッセージをプッシュする際、Pushover エンドポイントはすべてのリクエストタイプで本文を使用するので、この例ではそうではありません（以下を参照）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Query String]</p> </td> 
      <td> <p>一部の web サービスでは、クエリ文字列を使用して他のパラメーターを指定します。この件は、[!DNL Pushover] web サービスは、すべてのリクエストタイプで [!UICONTROL Body]（以下を参照）を使用するという例とは異なります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>この設定を使用すると、以下の [!UICONTROL Content Type] フィールドで JSON コンテンツタイプを選択できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON は、[!UICONTROL Pushover] アプリで必要なコンテンツタイプです。これは、他の web サービスとは異なる場合があります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Request Content]</p> </td> 
      <td> <p>[!UICONTROL Body] リクエストコンテンツを JSON 形式で入力します。[!UICONTROL JSON]／[!UICONTROL Create JSON] モジュールを使用できます。詳しくは、この記事の<a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">[!UICONTROL JSON]／[!UICONTROL Create JSON] モジュールを使用してマッピングされた JSON 本文</a>を参照してください。または、JSON コンテンツを手動で入力することもできます。詳しくは、この記事の<a href="#json-body-entered-manually" class="MCXref xref">手動で入力した JSON 本文</a>を参照してください。</p> <p>その web サービスに必要なパラメーターについて詳しくは、web サービスの API ドキュメントを参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 手動で入力した JSON 本文

パラメーターと値を JSON 形式で指定します。

>[!INFO]
>
>**例：**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>"token":"123459evz8aepwtxydndydgyumbfx",
>"message":"Hello World!",
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>USER_KEY。これは、[!DNL Pushover] ダッシュボードに表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>生成した API トークン／API キーの [!DNL Pushover] アプリを作成します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>デバイスに送信されるプッシュ通知のテキストコンテンツ。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>（オプション）メッセージのタイトル。値を入力しない場合は、アプリの名前が使用されます。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL JSON]／[!UICONTROL JSON を作成]モジュールを使用してマッピングされた JSON 本文

[!UICONTROL JSON を作成]モジュールを使用すると、JSON の指定が容易になります。また、値を動的に定義することもできます。

JSON モジュールについて詳しくは、[JSON モジュール](../../workfront-fusion/apps-and-their-modules/json-modules.md)を参照してください。

1. JSON を作成する元となる値を入力またはマッピングします。

   ![](assets/json-values-350x288.png)

1. [!UICONTROL JSON]／[!UICONTROL JSON を作成]モジュールを HTTP／リクエストを実行モジュールに接続します。
1. [!UICONTROL HTTP]／[!UICONTROL リクエストを実行]モジュール内で、[!UICONTROL JSON を作成]モジュールから「[!UICONTROL コンテンツを要求]」フィールドまで JSON 文字列をマッピングします。

   これで、シナリオを実行すると、プッシュ通知が、[!DNL Pushover] アカウントで登録されたデバイスに送信されます。
