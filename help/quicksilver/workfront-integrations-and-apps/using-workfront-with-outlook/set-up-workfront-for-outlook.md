---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: ' [!DNL Adobe Workfront]  for  [!DNL Outlook] の設定'
description: ' [!DNL Adobe Workfront] [!DNL Outlook] アドインを使用すると、主要なタスク [!DNL Workfront] を Outlook から直接実行できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 86%

---

# [!DNL Adobe Workfront for Outlook] の設定 

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] [!DNL Outlook] アドインを使用すると、次の主要な [!DNL Workfront] タスクを Outlook から直接実行できます。

* メールからの情報を使用して、既存のプロジェクト、タスクまたはイシューを更新します。詳しくは、[ [!DNL Outlook] メールからの既存のオブジェクトの更新](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md)を参照してください。
* [!DNL Outlook] 内で、メールに基づく [!DNL Workfront] リクエストを作成します。詳しくは、[ [!DNL Outlook]  からの Adobe Workfront リクエストの作成](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md)を参照してください。
* [!UICONTROL 担当作業]領域にメールをタスクとして追加します。詳しくは、[作業リストに  [!DNL Outlook]  メールをタスクとして追加する](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md)を参照してください。
* [!DNL Outlook] 用の [!DNL Workfront] アドインを使用してコメントに返信します。Workfront for [!DNL Outlook] からのコメントへの返信については、[ [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md) からコメントに返信するを参照してください。
* タスクやイシューを最初から作成するか、（ドラッグ&amp;ドロップ機能を使用して）既存のメールから作成します。詳しくは、[プロジェクトに [!DNL Outlook] メールをタスクとして追加する](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md)を参照してください。

[!DNL Workfront for Outlook] を使用する前に、[!DNL Workfront] アドインを [!DNL Outlook] アカウントに追加する必要があります。

[!DNL Outlook] アカウントで [!DNL Workfront] アドインをインストールできない場合は、[!DNL Workfront] 管理者に問い合わせて、[!DNL Outlook] アドインが組織で有効になっていることを確認してください。

組織で [!DNL Outlook] 統合を有効にする方法については、[有効化 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> 
   <p>新規プラン：[!UICONTROL Standard]</p> 
   <p>現在のプラン：[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

担当の [!DNL Workfront] 管理者はこの統合を使用する前に [!DNL Workfront] で [!DNL Outlook for Office] を有効にする必要があります。

## 必要システム構成

次のアプリケーションを使用できます。

* **[!DNL Outlook]Web 上：**[!DNL Workfront] アドインは、デスクトップまたはモバイルデバイスの web ブラウザーから [!DNL Outlook] を使用しているときに利用できます。この機能は [!DNL Outlook] web アプリの使用時にも利用できます。
* **[!DNL Outlook]デスクトップアプリケーション：**[!DNL Workfront] アドインは、[!DNL Office] パッケージに含まれる [!DNL Outlook] のデスクトップバージョン [!DNL Windows] および [!DNL Mac] を使用する場合に使用できます。

[!DNL Outlook] 用の [!DNL Workfront] アドインは、次の要件を満たす環境でサポートされます。

* [クライアント要件](#client-requirements-client-requirements)
* [メールサーバー要件](#mail-server-requirements-mail-server-requirements)

### クライアント要件 {#client-requirements}

Workfront は、[!DNL Outlook] の次のバージョンをサポートしています。

* [!DNL Windows] で [!DNL Outlook 2013] 以降
* [!DNL Windows] で [!DNL Outlook 2016] 以降
* [!DNL Mac] 版 [!DNL Outlook]（[!DNL Microsoft 365]）
* [!DNL Windows] 版 [!DNL Outlook]（[!DNL Microsoft 365]）
* Web 版 [!DNL Outlook]

直接接続を使用して [!DNL Exchange Server] または [!DNL Office 365] に接続する必要があります。

クライアントを設定する際、ユーザーは次のアカウントタイプのいずれかを選択する必要があります。

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] クライアントが POP3 または IMAP で接続するように設定されている場合、[!DNL Workfront] アドインは読み込まれません。

### メールサーバー要件 {#mail-server-requirements}

[!DNL Office 365] または [!DNL Outlook.com] に接続する場合に、メールサーバーの要件は、デフォルトで満たされます。ただし、[!DNL Exchange Server] のオンプレミスインストールに接続される場合、次の要件が適用されます。

* Workfront は、すべての [!DNL Exchange On-Premise] サーバーをサポートします。
* [!DNL Exchange Web Services] （EWS）を有効にし、インターネットに公開する必要があります。
* サーバーが有効な ID トークンを発行するには、サーバーに有効な認証証明書が必要です。[!DNL Exchange Server] の新規インストールでは、デフォルトの認証証明書が含まれます。

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* [[!DNL Office]  ストア](https://store.office.com/)から [!DNL Workfront] アドインにアクセスするために、クライアントアクセスサーバーは[https://store.office.com](https://store.office.com/)と通信できる必要があります。

サポートされる環境について詳しくは、[[!DNL Microsoft Office 365]  ホームページ](https://products.office.com/en-us/office-365-home)を参照してください。

## アドインのインストール

Outlook 用 Workfront アドインは、[Microsoft ストア](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)から入手できます。

### [!DNL Outlook 365] 向け [!DNL Workfront] {#workfront-for-outlook-365}

1. [!DNL Outlook 365] で、Office 365 インターフェイスの上部にある **[!UICONTROL アドインを参照]** アイコン ![ アドインを参照 ](assets/outlook-add-in-26x26.png) アイコンをクリックし、**[!UICONTROL アドインの管理]** をクリックします。

1. **[!UICONTROL アドインを検索]**&#x200B;ボックスで、**[!DNL Workfront]** を検索し、[!UICONTROL Enter キー]を押します。

1. 「**[!UICONTROL 追加]**」をクリックします。

### Web 版 [!DNL Workfront] for [!DNL Outlook] {#workfront-for-outlook-on-the-web}

1. Web ブラウザーで [!DNL Microsoft Outlook] を開きます。
1. **[!UICONTROL アドインを参照 ] アイコン** アドインを参照 ![ をクリック ](assets/outlook-add-in-web-version-20x20.png) ます。

   アイコンを見つけるには、[Web 版 ](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) でのアドインの使用 [!DNL Outlook] を参照してください。

1. 「**[!UICONTROL アドインを検索]**」フィールドで **[!DNL Workfront]** を検索して、**[!UICONTROL Enter]** を押します。

1. リストに表示されたら、「**追加**」をクリックします。

### [!UICONTROL Windows]または [!DNL Mac] 版 [!DNL Workfront for Outlook] {#workfront-for-outlook-on-windows-or-mac}

1. リボン上の&#x200B;**[!UICONTROL ホーム]**／**[!UICONTROL ストア]**&#x200B;をクリックします。

1. 「**[!UICONTROL 検索]**」フィールド内の **[!DNL Workfront]** を検索して、**[!UICONTROL Enter]** キーを押します。

1. 切替スイッチをクリックして **[!UICONTROL [!DNL Workfront]アドイン]**&#x200B;を有効にします。

## [!DNL Outlook] から [!DNL Workfront] へのログイン

1. [!DNL Outlook] では、メールメッセージを選択し、メールヘッダー内の **[!DNL Workfront]** アイコンをクリックします。
1. ログインページで、「**Workfrontにログイン**」をクリックします。
1. 画面の指示に従い、OAuth 2.0 を使用して [!DNL Workfront] にログインします。<!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* [!DNL Workfront] アカウントのドメインを入力するプロンプトが表示されたら、次の形式で入力します：*yourCompany&#39;sDomain.my.workfront.com*。 会社のドメインは通常、会社の名前です。

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
