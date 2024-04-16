---
title: ' [!DNL Adobe Workfront Fusion] HTTP／OAuth 2.0 リクエストを実行モジュールを使用して、MS Graph REST API を呼び出します。'
description: ' [!DNL Adobe Workfront Fusion] HTTP／OAuth 2.0 リクエストを実行モジュールを使用して、MS Graph REST API を呼び出します。'
author: Becky
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 80%

---

# [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 リクエストを実行]モジュールを使用して、[!UICONTROL MS Graph REST API] を呼び出します。

<!-- Audited: 3/2024-->

多くの [!DNL Microsoft] web サービスは、[!DNL Microsoft Graph API] を通じてアクセスされます。への接続を作成できます [!DNL Microsoft Graph API]を使用する [!DNL Workfront Fusion] [!DNL HTTP] > [!UICONTROL OAuth 2.0 リクエストの作成] モジュール。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p><p>または</p><p>現在：[!UICONTROL 作業 ] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在：いいえ [!DNL Workfront Fusion] ライセンス要件</p>
   <p>または</p>
   <p>レガシー：任意 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>新規：</p> <ul><li>[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Workfront] プラン：組織による購入が必要です [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] プラン： [!DNL Workfront Fusion] が含まれます。</li></ul>
   <p>または</p>
   <p>現在：組織による購入が必要です。 [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL Microsoft Application Registration Portal] での [!DNL Workfront Fusion] の登録

[!DNL Microsoft Graph REST API] への接続を作成するには、まず [!DNL Adobe Workfront Fusion] を登録する必要があります。

1. [!DNL Microsoft] ドキュメントの[アプリを登録する](https://docs.microsoft.com/en-us/graph/auth-register-app-v2)の説明に従って、新しいアプリケーションの登録を開始します。

   登録の一環として、[!DNL Microsoft] は次の情報を必要とします。

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Application name]</td>
        <td>「マイ [!DNL Workfront Fusion] アプリケーション」などのアプリケーション名を入力します。</td>
      </tr>
      <tr>
        <td>[!UICONTROL Redirect URL]</td>
        <td><code>https://app.workfrontfusion.com/oauth/cb/oauth2</code></td>
      </tr>
    </table>

1. アプリの登録が完了したら、[!UICONTROL アプリケーション ID] をメモします。

   >[!IMPORTANT]
   >
   >[!DNL Workfront Fusion] で接続を設定するには、アプリケーション ID が必要になります。

1. [!UICONTROL アプリケーションシークレット]を生成します。このシークレットをメモしておいてください。

   手順については、[!DNL Microsoft] ドキュメントの[アプリを登録する](https://docs.microsoft.com/en-us/graph/auth-register-app-v2)を参照してください。

   >[!IMPORTANT]
   >
   >[!DNL Workfront Fusion] で接続を設定するには、[!UICONTROL アプリケーションシークレット]が必要になります。

1. アプリケーションの権限を設定します。

   これらのフィールドの検索と構成について詳しくは、[!UICONTROL Microsoft] ドキュメントの[ユーザーなしでアクセスを取得](https://docs.microsoft.com/en-us/graph/auth-v2-service)の「Microsoft Graph のアクセス許可を構成する」節を参照してください。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL What type of permissions does your application require?]</td> 
      <td><code>[!UICONTROL Delegated permissions]</code>を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Select permissions]</td> 
      <td> <p>次の権限を選択します。</p> 
       <ul> 
        <li> <p><code>offline_access</code> </p> </li> 
        <li> <p><code>openid</code> </p> </li> 
        <li> <p>統合に必要なその他の権限（例：<code>User.Read</code>）</p> </li> 
       </ul> <p><b>重要</b>：で接続を設定するには、選択した権限が必要です [!DNL Workfront Fusion].</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. [ [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion) での [!DNL MS Graph API] 接続の設定に進みます。

## [!DNL Workfront Fusion] での [!DNL MS Graph API] 接続の設定

登録後 [!DNL Workfront Fusion] ～で議論されているように [登録 [!DNL Workfront Fusion] が含まれる [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal)：接続の設定は [!UICONTROL HTTP] > [!UICONTROL Oauth 2.0 の作成] リクエストモジュール。

1. を追加 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 呼び出しを行う] モジュールをシナリオに追加します。
1. 「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 接続フィールドを次のように設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Connection name]</td> 
      <td>接続に名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Flow type]</p> </td> 
      <td><code>[!UICONTROL Authorization Code]</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/authorize</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token URI]</td> 
      <td><code>https://login.microsoftonline.com/common/oauth2/v2.0/token</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p><a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">[!DNL Workfront Fusion] を [!DNL Microsoft Application Registration Portal]</a> に登録する手順 4 で選択した権限を入力します。</p> <p>範囲ごとに、<b>[!UICONTROL Add]</b> をクリックし、権限を入力します。</p> <p>例：<code>offline_access</code>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope separator]</td> 
      <td><code>SPACE</code> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td><a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">[!DNL Microsoft Application Registration Portal]</a>に[!DNL Workfront Fusion]を登録する手順 2 の [!UICONTROL Application ID] を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client Secret]</td> 
      <td>の手順 3 で生成した [!UICONTROL アプリケーション秘密鍵 ] を入力します <a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">登録 [!DNL Workfront Fusion] が含まれる [!DNL Microsoft Application Registration Portal]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Authorize parameters]</td> 
      <td> <p>次の承認パラメーターを追加します。</p> 
       <ul> 
        <li> <p>[!UICONTROL Key]：<code> response_mode</code> [!UICONTROL Value]： <code>query</code></p> </li> 
        <li> <p>[!UICONTROL Key]：<code>prompt </code>[!UICONTROL Value]： <code>consent</code></p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Access token parameters]</td> 
      <td>このフィールドには何も入力する必要はありません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Refresh token parameters]</td> 
      <td> 
       <ol> 
        <li value="1"> <p>「<b>[!UICONTROL Add]</b>」をクリックします。</p> </li> 
        <li value="2"> <p>「<b>[!UICONTROL Key]</b>」フィールドに、<code>scope</code> を入力します。</p> </li> 
        <li value="3"> <p>「<b>[!UICONTROL Value]</b>」フィールドに、スコープフィールドに入力したすべての [!UICONTROL scope] を、スペースで区切って入力します。</p> <p>例： <code>offline_access openid User.Read</code></p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Headers]</td> 
      <td>このフィールドには何も入力する必要はありません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Placement]</td> 
      <td><code>[!UICONTROL In the header]</code> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 続行]**」をクリックします。
1. 表示されるウィンドウで、「**[!UICONTROL 確定]**」をクリックして接続を完了し、モジュールに戻ります。
