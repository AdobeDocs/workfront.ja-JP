---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: connections-annd-webhooks
title: ' [!DNL Adobe Workfront Fusion]で接続を作成'
description: 接続は、接続先のアプリまたは web サービスの API で設定された要件に従う必要があります。このため、接続を設定する手順は、アプリや web サービスによって異なります。この記事は、 [!DNL Adobe Workfront Fusion] を選択したアプリや web サービスに接続するための手順を確認するのに役立ちます。
author: Becky
feature: Workfront Fusion
exl-id: fb1a2af4-da58-48ba-85b5-1903d6a3ceda
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: ht
source-wordcount: '567'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion]での接続を作成

接続は、接続先のアプリまたは web サービスの API で設定された要件に従う必要があります。このため、接続を設定する手順は、アプリや web サービスによって異なります。この記事は、[!DNL Adobe Workfront Fusion]を選択したアプリや web サービスに接続するための手順を確認するのに役立ちます。

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
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront]プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td>

</tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL Adobe Workfront] を [!DNL Workfront Fusion] に接続

Workfront と [!DNL Workfront Fusion] は、連携するように設計されています。作成した接続によって、[!DNL Workfront Fusion] が Workfront でアクションを実行するために使用するアカウントが決定されます。

手順については、[ [!DNL Workfront]  を  [!DNL Workfront Fusion]](../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect) in [[!DNL Adobe Workfront]  モジュール に接続](../../workfront-fusion/apps-and-their-modules/workfront-modules.md)を参照してください。

## 設定が不要なアプリまたは web サービスに接続

ほとんどの場合、このモジュールを使用して、追加の情報をほとんど含まない接続を作成することができます。[!DNL Workfront Fusion] は認証を自動的に処理します。

特別な考慮事項のない接続を作成する手順について詳しくは、[ [!DNL Adobe Workfront Fusion]  への接続の作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)を参照してください。

## [!DNL Microsoft] アプリまたは web サービスに接続

[!DNL Workfront Fusion] のほとんどの [!DNL Microsoft] アプリでは、追加情報なしで接続を作成することができます。

以下の状況では、接続を作成する際に追加の手順が必要になります。

* [!DNL Microsoft Dynamics 365] モジュールの使用。

  手順については、[[!DNL Microsoft Dynamics 365]  モジュール](../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md)を参照してください。

* [!UICONTROL HTTP] モジュールを使用して[!DNL Microsoft Graph API] に接続

  手順については、[ [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] 経由で [!DNL MS Graph REST API] を呼び出す／[!UICONTROL OAuth 2.0 リクエスト]モジュール](../../workfront-fusion/connections/call-the-ms-graph-rest-api-.md)を作成を参照してください。

## [!DNL Google] アプリまたは web サービスに接続

[!DNL Google] アプリに接続するプロセスは、使用している [!DNL Google] アカウントの種類によって異なる場合があります。さらに、[!DNL Workfront Fusion] に接続する場合、[!DNL Google] のセキュリティ対策により追加の設定が必要になる場合があります。

詳しくは、以下を参照してください。

* [カスタム OAuth クライアントを使用して  [!DNL Adobe Workfront Fusion]  を  [!DNL Google Services]  に接続](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)
* [最新のセキュリティ対策を使用して  [!DNL Adobe Workfront Fusion]  を  [!DNL Google Services]  に接続](../../workfront-fusion/connections/connect-to-google-with-new-security-measures.md)

## 追加の設定が必要なその他のアプリ

以下のアプリは、[!DNL Workfront Fusion] 接続の基本設定に従っていません。これらのアプリに接続する手順は、当該のアプリの記事で確認できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>アプリ/ web サービス</th> 
   <th>接続に関する追加情報</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/workfront-modules.md" class="MCXref xref">[!DNL Adobe Workfront] モジュールで [!DNL Adobe Workfront] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Allocadia]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/allocadia-modules.md" class="MCXref xref">[!DNL Allocadia] モジュールで [!DNL Allocadia] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Anaplan]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/anaplan-modules.md" class="MCXref xref">[!DNL Anaplan] モジュールで [!DNL Anaplan] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL AWS S3]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md#connecti" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/aws-s3-modules.md" class="MCXref xref">[!DNL AWS S3] モジュールで [!DNL AWS] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Azure DevOps]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md" class="MCXref xref">[!DNL Azure DevOps] モジュールで [!DNL Azure DevOps] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Bynder]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/bynder-modules.md" class="MCXref xref">[!DNL Bynder] モジュールで [!DNL Bynder] を [!DNL Workfront Fusion]</a> に接続</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL CloudConvert]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/cloud-convert-modules.md" class="MCXref xref">[!DNL CloudConvert] モジュールで [!DNL CloudConvert] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr>   <tr> 
   <td role="rowheader"> <p>[!DNL Cvent]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/cvent-modules.md" class="MCXref xref">[!DNL Cvent] モジュールで [!DNL Cvent] を </a> に接続[!DNL Adobe Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Datadog]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/datadog-modules.md" class="MCXref xref">[!DNL Datadog] モジュールで [!DNL Datadog] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL DocuSign]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/docusign-modules.md" class="MCXref xref">[!DNL DocuSign] モジュールで [!DNL DocuSign] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>メール</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md#connecti" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/email-modules.md" class="MCXref xref">[!UICONTROL Email] モジュールで、メールを </a> に接続[!DNL Workfront Fusion]</a></td>

<tr> 
   <td role="rowheader"> <p>[!DNL Gmail]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md#connect3" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/gmail-modules.md" class="MCXref xref">[!DNL Gmail] モジュールで [!DNL Gmail] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Cloud]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] モジュールで [!DNL Jira Cloud] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira Server]</td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md#connect2" class="MCXref xref"><a href="../../workfront-fusion/apps-and-their-modules/jira-software-modules.md" class="MCXref xref">[!DNL Jira Software] モジュールで [!DNL Jira Server] を </a> に接続[!DNL Workfront Fusion]</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MariaDB]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md" class="MCXref xref">[!DNL MariaDB] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/mariadb-modules.md#connect" class="MCXref xref">[!DNL MariaDB] を [!DNL Workfront Fusion]</a> に接続</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Marketo]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md" class="MCXref xref">[!DNL Marketo] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/marketo-modules.md#connect" class="MCXref xref">[!DNL Marketo] を [!DNL Workfront Fusion]</a> に接続</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL MS Dynamics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md" class="MCXref xref">[!DNL Microsoft Dynamics 365] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md#connect" class="MCXref xref">[!DNL Microsoft Dynamics 365] を [!DNL Workfront Fusion]</a> に接続</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Qualtrics]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md" class="MCXref xref">[!DNL Qualtrics] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/qualtrics-modules.md#connecti" class="MCXref xref">[!DNL Qualtrics] を [!DNL Workfront Fusion]</a> に接続</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL ServiceNow]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md" class="MCXref xref">[!DNL ServiceNow] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/servicenow-modules.md#connect" class="MCXref xref">[!DNL ServiceNow] を [!DNL Workfront Fusion]</a> に接続</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>SFTP</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sftp.md" class="MCXref xref">[!UICONTROL SFTP] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/sftp.md#connect" class="MCXref xref">SFTP を [!DNL Workfront Fusion]</a> に接続</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL SharePoint]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md" class="MCXref xref">[!DNL SharePoint] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/sharepoint-modules.md#connect" class="MCXref xref">[!DNL SharePoint] を [!DNL Workfront Fusion]</a> に接続</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Split.io]</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md" class="MCXref xref">[!DNL Split.io] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/split-io-modules.md#connect" class="MCXref xref">[!DNL Split.io] を [!DNL Workfront Fusion] に接続</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Widen</p> </td> 
   <td><a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md" class="MCXref xref">[!DNL Widen] モジュール</a>で <a href="../../workfront-fusion/apps-and-their-modules/widen-modules.md#connect" class="MCXref xref">[!DNL Widen] を [!DNL Workfront Fusion] に接続</a></td> 
  </tr> 
 </tbody> 
</table>
