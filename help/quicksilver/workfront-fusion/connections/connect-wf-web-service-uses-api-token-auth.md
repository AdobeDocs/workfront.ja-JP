---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: 接続 [!DNL Adobe Workfront Fusion] API トークン認証を使用する Web サービスに追加する
description: 一部のサービスでは、次のような統合ソリューションが許可されません。 [!DNL Adobe Workfront Fusion] ：シナリオで簡単に使用できるアプリを作成します。
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# 接続 [!DNL Adobe Workfront Fusion] API トークン認証を使用する Web サービスに追加する

一部のサービスでは、次のような統合ソリューションが許可されません。 [!DNL Adobe Workfront Fusion] ：シナリオで簡単に使用できるアプリを作成します。

この状況に対する回避策があります。 目的のサービス（アプリ）を [!DNL Workfront Fusion] using [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] モジュール。

この記事では、ほとんどの Web サービスをに接続する方法を説明します。 [!DNL Workfront Fusion] API キー/ API トークンを使用して、

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## API トークンを使用する Web サービスへの接続

API トークンを介してサービスに接続する手順は、ほとんどの Web サービスで同様です。

1. Web サービスの Web サイト上にアプリケーションを作成します。詳しくは、 [新しいアプリケーションを作成し、API トークンを取得します](#create-a-new-application-and-obtain-the-api-token) 」を参照してください。
1. API キーまたは API トークンを取得します。
1. 追加 [!DNL Workfront Fusion]&#39;s [!UICONTROL HTTP] > [!UICONTROL リクエストの作成] モジュールをシナリオに追加します。
1. Web サービスの API ドキュメントに従ってモジュールを設定し、シナリオを実行します（の節を参照）。 [設定 [!UICONTROL HTTP] モジュール](#set-up-the-http-module) 」を参照してください。

>[!NOTE]
>
>以下を使用します。 [!DNL Pushover] この記事全体で例として使用される通知サービス。

## 新しいアプリケーションを作成し、API トークンを取得します

>[!NOTE]
>
>Web サービスで API キーまたは API トークンを作成および配布する方法は様々です。 目的の Web サービスの API キーとトークンの取得手順については、サービスの Web サイトにアクセスし、「API キー」または「API トークン」を検索してください。
>
>Pushover API キーを取得する手順は、見つけるものの例としてのみ記載されています。

1. にログインします。 [!DNL Pushover] アカウント
1. クリック **[!UICONTROL アプリケーション/API トークンの作成]** をクリックします。
1. 「申込情報」に入力し、 **[!UICONTROL アプリケーションの作成]**.
1. 提供された API トークンを安全な場所に保存します。 次のために必要になります。 [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL リクエストの作成] 目的の Web サービスに接続するモジュール ([!DNL Pushover]（この場合は）。

## 設定 [!UICONTROL HTTP] モジュール

Web サービスを [!DNL Workfront Fusion] シナリオの場合、 [!UICONTROL HTTP] >[!UICONTROL リクエストを実行] モジュールを設定し、Web サービスの API ドキュメントに従ってモジュールを設定します。

1. を [!UICONTROL HTTP] >[!UICONTROL リクエストの作成] モジュールをシナリオに追加します。
1. 次を使用してメッセージをプッシュするには [!DNL Workfront Fusion]で、次のように HTTP モジュールを設定します。

   >[!NOTE]
   >
   >これらのモジュール設定は、 [!DNL Pushover] web サービス API ドキュメント。 設定は、他の Web サービスで異なる場合があります。 例えば、API トークンを [!UICONTROL ヘッダー] ではなく [!UICONTROL 本文] フィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>「 URL 」フィールドには、Web サービスの API ドキュメントで確認できるエンドポイントが含まれています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL メソッド ]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>使用されるメソッドは、対応するエンドポイントによって異なります。 メッセージをプッシュするための Pushover エンドポイントでは、POSTメソッドを使用します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>一部の Web サービスでは、Headers を使用して API トークン認証や他のパラメーターを指定できます。 メッセージをプッシュする際、Pushover のエンドポイントはすべてのリクエストタイプで本文を使用するので、この例ではそうではありません（以下を参照）。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL クエリ文字列 ]</p> </td> 
      <td> <p>一部の Web サービスでは、クエリ文字列を使用して他のパラメーターを指定できます。 この例では、とは異なります。 [!DNL Pushover] Web サービスは、すべてのリクエストタイプで [!UICONTROL Body] （以下を参照）を使用します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 本文の種類 ]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>この設定を使用すると、以下の「[!UICONTROL コンテンツタイプ ]」フィールドで JSON コンテンツタイプを選択できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL コンテンツタイプ ]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON は、[!UICONTROL Pushover] アプリで必要なコンテンツタイプです。 これは、他の Web サービスとは異なる場合があります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL コンテンツをリクエスト ]</p> </td> 
      <td> <p>[!UICONTROL Body] リクエストコンテンツを JSON 形式で入力します。 [!UICONTROL JSON] / [!UICONTROL JSON を作成 ] モジュールを使用できます ( <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">[!UICONTROL JSON] / [!UICONTROL JSON を作成 ] モジュールを使用してマッピングされた JSON 本文</a> 」を参照してください。 または、JSON コンテンツを手動で入力することもできます。詳しくは、 <a href="#json-body-entered-manually" class="MCXref xref">手動で入力した JSON 本文</a> 」を参照してください。</p> <p>その Web サービスに必要なパラメーターについては、 Web サービスの API ドキュメントを参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## 手動で入力した JSON 本文

パラメーターと値を JSON 形式で指定します。

>[!INFO]
>
>**例:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>
>"token":"123459evz8aepwtxydndydgyumbfx",
>
>"message":"Hello World!",
>
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ユーザー ]</p> </td> 
   <td> <p>USER_KEY。 これは、 [!DNL Pushover] ダッシュボード。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL トークン ] </td> 
   <td> <p>作成した API トークン/API キー [!DNL Pushover] アプリを使用します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>デバイスに送信されるプッシュ通知のテキストコンテンツ。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>（オプション）メッセージのタイトル。 値を入力しない場合は、アプリの名前が使用されます。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## を使用してマッピングされた JSON 本文 [!UICONTROL JSON] >[!UICONTROL JSON を作成] モジュール

この [!UICONTROL JSON を作成] モジュールを使用すると、JSON の指定が容易になります。 また、値を動的に定義することもできます。

JSON モジュールの詳細については、 [JSON モジュール](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. JSON を作成する値を入力またはマッピングします。

   ![](assets/json-values-350x288.png)

1. 接続 [!UICONTROL JSON] > [!UICONTROL JSON を作成] モジュールを HTTP / Make a Request モジュールに追加します。
1. JSON 文字列を [!UICONTROL JSON を作成] モジュールを [!UICONTROL コンテンツを要求] フィールド [!UICONTROL HTTP] >[!UICONTROL リクエストの作成] モジュール。

   これで、シナリオを実行すると、プッシュ通知が、 [!DNL Pushover] アカウント
