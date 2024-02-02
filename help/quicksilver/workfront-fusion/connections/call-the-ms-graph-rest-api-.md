---
title: ' [!DNL Adobe Workfront Fusion] HTTP／OAuth 2.0 リクエストを実行モジュールを使用して、MS Graph REST API を呼び出します。'
description: ' [!DNL Adobe Workfront Fusion] HTTP／OAuth 2.0 リクエストを実行モジュールを使用して、MS Graph REST API を呼び出します。'
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: adae390d-8b9e-4dab-8551-605e50af5a1e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '616'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 リクエストを実行]モジュールを使用して、[!UICONTROL MS Graph REST API] を呼び出します。

多くの [!DNL Microsoft] web サービスは、[!DNL Microsoft Graph API] を通じてアクセスされます。この記事では、[!DNL Workfront Fusion] [!DNL HTTP]／[!UICONTROL OAuth 2.0 リクエストを実行]モジュールを使用して、その API への接続を作成する方法について説明します。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!DNL Adobe Workfront] の [!UICONTROL Select] または [!UICONTROL Prime] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] の [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

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
       </ul> <p>重要：[!DNL Workfront Fusion] で接続を設定するには、選択した権限が必要になります。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. [ [!DNL Workfront Fusion]](#configure-your-ms-graph-api-connection-in-workfront-fusion) での [!DNL MS Graph API] 接続の設定に進みます。

## [!DNL Workfront Fusion] での [!DNL MS Graph API] 接続の設定

[ [!DNL Microsoft Application Registration Portal]](#register-workfront-fusion-in-the-microsoft-application-registration-portal) での [!DNL Workfront Fusion] の登録での説明に従って [!DNL Workfront Fusion] を登録したら、[!UICONTROL HTTP]／[!UICONTROL Oauth 2.0 リクエストを実行]モジュールで接続を設定できます。

1. [!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 呼び出しを実行]モジュールをシナリオに追加します。
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
      <td><a href="#register-workfront-fusion-in-the-microsoft-application-registration-portal" class="MCXref xref">[!DNL Microsoft Application Registration Portal]</a> に [!DNL Workfront Fusion] を登録する手順 2 で生成した [!UICONTROL Application Secret] を入力します。</td> 
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
