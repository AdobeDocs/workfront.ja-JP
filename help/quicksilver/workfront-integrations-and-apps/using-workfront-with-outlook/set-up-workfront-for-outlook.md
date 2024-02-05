---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: ' [!DNL Adobe Workfront]  for  [!DNL Outlook] の設定'
description: The [!DNL Adobe Workfront] [!DNL Outlook] アドインでは、キーを実行できます。 [!DNL Workfront] タスクを Outlook から直接実行します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 90%

---

# [!DNL Adobe Workfront for Outlook] の設定 

<!-- Audited: 12/2023 -->

The [!DNL Adobe Workfront] [!DNL Outlook] アドインでは、次のキーを実行できます。 [!DNL Workfront] Outlook から直接のタスク：

* メールからの情報を使用して、既存のプロジェクト、タスクまたはイシューを更新します。詳しくは、[ [!DNL Outlook] メールからの既存のオブジェクトの更新](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md)を参照してください。
* [!DNL Outlook] 内で、メールに基づく [!DNL Workfront] リクエストを作成します。詳しくは、[ [!DNL Outlook]  からの Adobe Workfront リクエストの作成](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md)を参照してください。
* [!UICONTROL 担当作業]領域にメールをタスクとして追加します。詳しくは、[作業リストに  [!DNL Outlook]  メールをタスクとして追加する](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md)を参照してください。
* [!DNL Outlook] 用の [!DNL Workfront] アドインを使用してコメントに返信します。Workfront for [!DNL Outlook] からのコメントへの返信については、[ [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md) からコメントに返信するを参照してください。
* タスクやイシューを最初から作成するか、（ドラッグ&amp;ドロップ機能を使用して）既存のメールから作成します。詳しくは、[プロジェクトに [!DNL Outlook] メールをタスクとして追加する](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md)を参照してください。

[!DNL Workfront for Outlook] を使用する前に、[!DNL Workfront] アドインを [!DNL Outlook] アカウントに追加する必要があります。

[!DNL Outlook] アカウントで [!DNL Workfront] アドインをインストールできない場合は、[!DNL Workfront] 管理者に問い合わせて、[!DNL Outlook] アドインが組織で有効になっていることを確認してください。

組織で [!DNL Outlook] 統合を有効にする方法については、[有効化 [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> 
   <p>新しいプラン： [!UICONTROL Standard]</p> 
   <p>現在のプラン：[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Workfrontは、次のバージョンの [!DNL Outlook]:

* [!DNL Outlook 2013] 以降（[!DNL Windows]）
*[!DNL  Outlook 2016] 以降（[!DNL Windows]）
* [!DNL Mac] 版 [!DNL Outlook]（[!DNL Microsoft 365]）
* [!DNL Windows] 版 [!DNL Outlook]（[!DNL Microsoft 365]）
* Web 版 [!DNL Outlook]

直接接続を使用して [!DNL Exchange Server] または [!DNL Office 365] に接続する必要があります。

クライアントを設定する際、ユーザーは次のアカウントタイプのいずれかを選択する必要があります。

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]****&#x200B;クライアントが POP3 または IMAP に接続するように設定されている場合、[!DNL Workfront] アドインが読み込まれません。

### メールサーバー要件 {#mail-server-requirements}

[!DNL Office 365] または [!DNL Outlook.com] に接続する場合に、メールサーバーの要件は、デフォルトで満たされます。ただし、[!DNL Exchange Server] のオンプレミスインストールに接続される場合、次の要件が適用されます。

* Workfrontはすべてをサポート [!DNL Exchange On-Premise] サーバー
* [!DNL Exchange Web Services] （EWS）を有効にし、インターネットに公開する必要があります。
* サーバーが有効な ID トークンを発行するには、サーバーに有効な認証証明書が必要です。[!DNL Exchange Server] の新規インストールでは、デフォルトの認証証明書が含まれます。

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* [[!DNL Office]  ストア](https://store.office.com/)から [!DNL Workfront] アドインにアクセスするために、クライアントアクセスサーバーは[https://store.office.com](https://store.office.com/)と通信できる必要があります。

サポートされる環境について詳しくは、[[!DNL Microsoft Office 365]  ホームページ](https://products.office.com/en-us/office-365-home)を参照してください。

## アドインのインストール

Outlook 用Workfrontアドインは、 [Microsoftストア](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] for [!DNL Outlook 365] {#workfront-for-outlook-365}

1. [!DNL Outlook 365] で、Office 365 インターフェイスの上部から「**[!UICONTROL アドインの参照]**」アイコン ![](assets/outlook-add-in-26x26.png)、「**[!UICONTROL アドインの管理]**」の順にクリックします。

1. **[!UICONTROL アドインを検索]**&#x200B;ボックスで、**[!DNL Workfront]** を検索し、[!UICONTROL Enter キー]を押します。

1. 「**[!UICONTROL 追加]**」をクリックします。

### Web 版 [!DNL Workfront] for [!DNL Outlook] {#workfront-for-outlook-on-the-web}

1. Web ブラウザーで [!DNL Microsoft Outlook] を開きます。
1. **アドインの参照**&#x200B;アイコン ![](assets/outlook-add-in-web-version-20x20.png) をクリックします。

   アイコンを見つけるには、[Web 版 ](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) でのアドインの使用 [!DNL Outlook] を参照してください。

1. 「**[!UICONTROL アドインを検索]**」フィールドで **[!DNL Workfront]** を検索して、**[!UICONTROL Enter]** を押します。

1. リストに表示されたら、「**追加**」をクリックします。

### [!UICONTROL Windows]または [!DNL Mac] 版 [!DNL Workfront for Outlook] {#workfront-for-outlook-on-windows-or-mac}

1. リボン上の&#x200B;**[!UICONTROL ホーム]**／**[!UICONTROL ストア]**&#x200B;をクリックします。

1. 「**[!UICONTROL 検索]**」フィールド内の **[!DNL Workfront]** を検索して、**[!UICONTROL Enter]** キーを押します。

1. 切替スイッチをクリックして **[!UICONTROL [!DNL Workfront]アドイン]**&#x200B;を有効にします。

## [!DNL Outlook] から [!DNL Workfront] へのログイン

1. [!DNL Outlook] では、メールメッセージを選択し、メールヘッダー内の **[!DNL Workfront]** アイコンをクリックします。
1. 画面の指示に従って、拡張認証、OAuth 2.0、または Security Assertion Markup Language（SAML）URL を使用し、[!DNL Workfront] にログインします。

   ユーザーが SAML を使用した [!DNL Workfront] アドインにログインする前に、[!DNL Workfront] 管理者は SAML 2.0 ソリューションを使用して認証するための [!DNL Office 365] アドインを最初に有効にする必要があります。詳しくは、[SAML 2.0 による  [!DNL Adobe Workfront]  の設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)記事で [SAML 2.0 による  [!DNL Adobe Workfront]  の設定](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365)の節を参照してください。

   >[!NOTE]
   >
   >* [!DNL Workfront] アカウントのドメインの入力を求められたら、「*yourCompany&#39;sDomain.my.workfront.com*」の形式で入力します。会社のドメインは通常、会社の名前です。
   >* [!DNL Workfront] 管理者がこの統合に対して有効にするまで、拡張認証は利用できません。

