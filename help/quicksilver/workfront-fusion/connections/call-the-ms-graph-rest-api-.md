---
title: を介して MS Graph REST API を呼び出します。 [!DNL Adobe Workfront Fusion] HTTP &gt;OAuth 2.0 リクエストモジュールを作成する
description: を介して MS Graph REST API を呼び出します。 [!DNL Adobe Workfront Fusion] HTTP &gt;OAuth 2.0 リクエストモジュールを作成する
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# を[!UICONTROL  MS Graph REST API] 経由 [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール

多数 [!DNL Microsoft] web サービスには、 [!DNL Microsoft Graph API]. この記事では、 [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール。

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

## 登録 [!DNL Workfront Fusion] 内 [!DNL Microsoft Application Registration Portal]

への接続を作成するには、以下を実行します。 [!DNL Microsoft Graph REST API]、最初にを登録する必要があります [!DNL Adobe Workfront Fusion].

1. 新しいアプリケーションの登録を開始します ( [アプリを登録](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 内 [!DNL Microsoft] ドキュメント。

   登録の一環として [!DNL Microsoft] には、次の情報が必要です。

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL アプリケーション名 ]</td>
        <td>アプリケーションの名前を入力します（例： 「My」）。 [!DNL Workfront Fusion] 申請」</td>
      </tr>
      <tr>
        <td>[!UICONTROL リダイレクト URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. アプリの登録が完了したら、 [!UICONTROL アプリケーション ID].

   >[!IMPORTANT]
   >
   >接続を設定するには、アプリケーション ID が必要です。 [!DNL Workfront Fusion].

1. を生成 [!UICONTROL アプリケーション秘密鍵]. この秘密を書き留めておけ。

   手順については、 [アプリを登録](https://docs.microsoft.com/en-us/graph/auth-register-app-v2) 内 [!DNL Microsoft] ドキュメント。

   >[!IMPORTANT]
   >
   >次が必要です： [!UICONTROL アプリケーション秘密鍵] 接続を設定するには、以下を使用します。 [!DNL Workfront Fusion].

1. アプリケーションの権限を設定します。

   これらのフィールドの配置と設定について詳しくは、 Microsoft Graph の権限の設定の節 ( [ユーザーを使用しないでアクセスを取得する](https://docs.microsoft.com/en-us/graph/auth-v2-service) 内 [!UICONTROL Microsoft] ドキュメント。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL アプリケーションにはどのような種類の権限が必要ですか？]</td> 
      <td>選択 <code>[!UICONTROL Delegated permissions]</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 権限を選択 ]</td> 
      <td> <p>次の権限を選択します。</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>統合に必要なその他の権限 ( 例： <code>User.Read</code>)</p> </li> 
       </ul> <p>重要：接続を設定するには、選択した権限が必要です。 [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 次に進む [の設定 [!DNL MS Graph API] 接続 [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion).

## の設定 [!DNL MS Graph API] 接続 [!DNL Workfront Fusion]

登録後 [!DNL Workfront Fusion] で説明されているように [登録 [!DNL Workfront Fusion] 内 [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)を設定すると、 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 を作成する] リクエストモジュール。

1. を追加します。 [!UICONTROL HTTP] >[!UICONTROL OAuth 2.0 呼び出しの実行] モジュールをシナリオに追加します。
1. クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 接続フィールドを次のように設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 接続名 ]</td> 
      <td>接続の名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL フロータイプ ]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URI を許可 ]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL トークン URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL スコープ ]</td> 
      <td> <p>の手順 4 で選択した権限を入力します <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">登録 [!DNL Workfront Fusion] 内 [!DNL Microsoft Application Registration Portal]</a>.</p> <p>範囲ごとに、 <b>[!UICONTROL 追加 ]</b> 権限を入力します。</p> <p>例: <code>offline_access</code>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL スコープ区切り文字 ]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント ID]</td> 
      <td>手順 2 の [!UICONTROL アプリケーション ID] ( <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">登録 [!DNL Workfront Fusion] 内 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td> 
      <td>手順 2 で生成した [!UICONTROL Application Secret] ( <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">登録 [!DNL Workfront Fusion] 内 [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL パラメーターを許可 ]</td> 
      <td> <p>以下の Authorize パラメーターを追加します。</p> 
       <ul> 
        <li> <p>[!UICONTROL キー ]:<code> response_mode</code> [!UICONTROL 値 ]: <code>query</code></p> </li> 
        <li> <p>[!UICONTROL キー ]: <code>prompt </code>[!UICONTROL 値 ]: <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL アクセストークンパラメーター ]</td> 
      <td>このフィールドには何も入力する必要はありません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL トークンパラメーターを更新 ]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>クリック <b>[!UICONTROL 追加 ]</b>.</p> </li> 
        <li value="2"> <p>内 <b>[!UICONTROL キー ]</b> フィールドに入力 <code>scope</code>.</p> </li> 
        <li value="3"> <p>内 <b>[!UICONTROL 値 ]</b> 「 」フィールドに、スコープフィールドに入力したすべての [!UICONTROL スコープ ] をスペースで区切って入力します。</p> <p>例: <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL カスタムヘッダー ]</td> 
      <td>このフィールドには何も入力する必要はありません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL トークンの配置 ]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]**.
1. 表示されるウィンドウで、 **[!UICONTROL 確定]** 接続を完了し、モジュールに戻ります。
