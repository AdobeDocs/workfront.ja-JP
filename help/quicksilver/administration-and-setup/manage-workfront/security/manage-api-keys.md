---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: API キーの管理
description: API セキュリティ脆弱性を最小限に抑えるために、Adobe Workfront 管理者は、アプリケーションがユーザーに代わって Workfront へのアクセスに使用される API キーを管理できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 93%

---

# API キーの管理

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->



>[!IMPORTANT]
>
>Workfront では、`/login` エンドポイントまたは API キーの使用を推奨していません。代わりに、次のいずれかの認証方法を使用してください。
>
>* JWT を使用したサーバー認証
>* OAuth2 を使用したユーザー認証
>
>これらの認証方法の設定手順については、[Workfront 統合用の OAuth2 アプリケーションの作成](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください
>
>Workfront でのサーバー認証の使用手順については、[JWT フローを使用した組織のカスタム OAuth 2 アプリケーションの設定および使用](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)を参照してください
>
>Workfront でのユーザー認証を使用する手順については、[認証コードフローを使用した組織のカスタム OAuth 2 アプリケーションの設定および使用](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)を参照してください

API セキュリティ脆弱性を最小限に抑えるために、Adobe Workfront 管理者は、アプリケーションがユーザーに代わって Workfront へのアクセスに使用される API キーを管理できます。

現在の管理者 API キーのリセットまたは削除、API キーを期限切れに設定、すべてのユーザーの API キーの削除を行うことができます。

Workfront API を活用するアプリケーションの例を次に示します。

* Dropbox、Google Drive、Workfront DAM などのドキュメントの統合
* Workfront モバイルアプリケーション

>[!IMPORTANT]
>
>API キーをリセットまたは削除する場合、Workfront API を利用し、この API キーを介して Workfront に対して認証するアプリケーションは、Workfront へのアクセス権を取り戻すために再設定する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p><p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront API キー

Workfront のそれぞれのユーザーが、一意の API キーを持っています。このキーは、ユーザーが Workfront API（Workfront モバイルアプリやドキュメント統合など）を活用する統合にアクセスする際に、ユーザーごとに生成されます。

>[!NOTE]
>
> 本番環境で生成した API キーは、毎週の更新中にプレビュー環境にコピーされます。プレビュー環境で生成した API キーは、毎週の更新中に実稼動用 API キーで上書きされます。

Workfront 管理者には一意の API キーが割り当てられています。アプリケーションが管理者 API キーを使用して Workfront にアクセスすると、アプリケーションは Workfront への管理アクセス権を持つことになります。

## 管理者 API キーの管理

管理者ユーザーアカウントの API キーを生成、リセットまたは削除することができます。

{{step-1-to-setup}}

1. **システム**／**顧客情報**&#x200B;をクリックします。
1. （条件付き）次のアクションのいずれかを実行します。

   API キーを生成するには、「**API キーを設定**」セクションで、「**API キーを生成**」をクリックします。

   または\
   API キーをリセットするには：「**API キー設定**」セクションで、**リセット**、**リセット**」の順にクリックします。

   または

   API キーを削除するには、「**API キーの設定**」セクションで、「**削除**&#x200B;をクリックし、「**削除**」をクリックします。

<!--

   Remove me October 2026

## Generate an API Key for Non-Admin Users

You can generate and manage API Keys for users in roles other than Workfront administrator.

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

1. (Conditional) If your organization uses Single Sign-On (SSO) access management, temporarily disable the option requiring SSO authentication.

   {{step-1-to-setup}} 
   
   1. Expand **System**, then click **Single Sign-on (SSO)**. 
   1. In the **Type** field, select the type of SSO your organization uses.
   1. With the type selected, scroll down and clear the **Enable** checkbox. 
      ![Enable SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)  
   1. Click **Save**.


1. In the address bar of a browser, enter the following API call:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&username=**username**&password=**password**&method=PUT

   Replace `<domain>` with your Workfront domain name, and username and password with the user's Workfront credentials.

1. (Conditional) Enable the option requiring SSO authentication if you disabled it in Step 1.

   {{step-1-to-setup}}
   
   1. Expand **System**, then click **Single Sign-on (SSO)**.
   
   1. Select your SSO method in the **Type** drop down menu.
   1. Check the checkbox requiring SSO authentication.

   -->

## API キーの有効期限を設定

API キーは、システム内のすべてのユーザーの有効期限が切れるように設定できます。ユーザーの API キーの有効期限が切れると、ユーザーは Workfront API を使用して Workfront にアクセスするアプリケーションに対して再認証する必要があります。API キーの有効期限が切れる頻度を変更できます。ユーザーのパスワードの有効期限が切れた場合に、API キーを期限切れにするかどうかを設定することもできます。

{{step-1-to-setup}}

1. **システム**／**顧客情報**&#x200B;をクリックします。
1. **API キー設定**&#x200B;エリア内の、**作成後**&#x200B;の&#x200B;**API キーの有効期限：**&#x200B;ドロップダウンリストから、API キーを期限切れにする時間枠を選択します。

   このオプションを変更すると、変更を加えた時点から新しい期間が開始されます。例えば、このオプションを *1 か月*&#x200B;から *6 か月*&#x200B;に変更すると、API キーの有効期限は変更を行ってから 6 か月になります。

   デフォルトでは、API キーは毎月期限が切れます。

1. ユーザーのパスワードの有効期限が切れるときにAPI キーを期限切れにするように設定するには、**ユーザーのパスワードの有効期限が切れたときにAPI キーを削除**&#x200B;を有効にします。

   デフォルトでは、このオプションは有効になっていません。

   ユーザーパスワードが失効するように設定する方法については、[システムセキュリティの環境設定の指定](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。

1. 「**保存**」をクリックします。

## すべてのユーザーの API キーを削除

Workfront システムに関する特定のセキュリティ違反を懸念する場合は、すべてのユーザーの API キーを同時に削除できます。

>[!IMPORTANT]
>
>すべてのユーザーの API キーを削除すると、システム内のすべてのユーザーの API キーがすべて無効になります。このアクションにより、Workfront で新しい API キーを生成して統合をすべてアップデートするまで、Workfront でのすべての統合が失敗します。

{{step-1-to-setup}}

1. **システム**&#x200B;を展開して、「**顧客情報**」をクリックします。

1. **API キー設定**&#x200B;領域で、**すべての API キーを削除**、**削除**／**すべて**&#x200B;の順にクリックします。

<!--

Remove me October 2026

## Restricting API logins with an X.509 certificate

>[!IMPORTANT]
>
>The procedure described in this section applies only to organizations that have not yet been onboarded to the Adobe Business Platform. Logging in to Workfront through the Workfront API is not available if your organization has been onboarded to the Adobe Business Platform.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>This is not available if your organization's Workfront instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

Third-party applications can communicate with Workfront through the API. To increase the security of your Workfront site, you can configure Workfront to restrict API login requests by uploading an X.509 certificate to Workfront. Once enabled, all login requests through the API must include a client certificate in addition to username and password.

* [Obtain the X.509 certificate](#obtain-the-x-509-certificate) 
* [Upload the certificate to Workfront](#upload-the-certificate-to-workfront) 
* [Verify API login calls are restricted](#verify-api-login-calls-are-restricted)

### Obtain the X.509 certificate {#obtain-the-x-509-certificate}

Obtain a valid X.509 certificate from a trusted Certificate Authority (such as Verisign), and save it to a temporary location on your workstation. 

### Upload the certificate to Workfront {#upload-the-certificate-to-workfront}

After you have obtained the X.509 certificate from your Certificate Authority, you need to upload it to Workfront.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).  

1. Expand **System**, then click **Customer Info**.

1. In the **API Key Settings** area, select **Require X.509 Certificate for API logins**.
1. Click **Change Certificate**.
1. On your workstation, browse to and select the X.509 certificate that you previously downloaded.
1. (Optional) Click **View Details** next to the certificate name to view the following details about the certificate:

   * Subject Common Name
   * Subject Organization
   * Subject Organization Unit
   * Issuer Common Name
   * Issuer Organization
   * Issuer Organization Unit
   * Serial Number
   * Issue Date
   * Expiration Date

1. Click **Save**. 

### Verify API login calls are restricted {#verify-api-login-calls-are-restricted}

Prior to configuring your instance of Workfront to require an X.509 certificate, perform an API request to the `/login` endpoint using valid username and password parameters. You will receive a 200 response that contains a sessionID.

After making the X.509 certificate a requirement via the customer info page in your instance of Workfront, make another login attempt. This time you will receive a 500 error response with the following message: "Untrusted request. Please contact your system administrator and attach certificate."

After confirming that the X.509 certificate is required, perform the same login request with an additional parameter for apiCertificate set to the value of your certificate. If this operation was performed correctly you will receive a 200 response that contains a valid sessionID.

-->
