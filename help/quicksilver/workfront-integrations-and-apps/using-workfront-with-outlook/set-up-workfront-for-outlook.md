---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: 設定 [!DNL Adobe Workfront] 対象： [!DNL Outlook]
description: The [!DNL Adobe Workfront] [!DNL Outlook] アドインでは、キーを実行できます。 [!DNL Workfront] タスクを Outlook から直接実行します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 設定 [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

The [!DNL Adobe Workfront] [!DNL Outlook] アドインでは、次のキーを実行できます。 [!DNL Workfront] Outlook から直接のタスク：

* 電子メールからの情報を使用して、既存のプロジェクト、タスクまたはイシューを更新します。 詳しくは、 [からの既存のオブジェクトの更新 [!DNL Outlook] 電子メール](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* の作成 [!DNL Workfront] 内の E メールに基づくリクエスト [!DNL Outlook]. 詳しくは、 [からのAdobe Workfrontリクエストの作成 [!DNL Outlook] 電子メール](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* E メールをタスクとして [!UICONTROL 自分の仕事] 領域。 詳しくは、 [を追加します。 [!DNL Outlook] タスクとしてのメールを作業リストに送信する](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* 次を使用してコメントに返信 [!DNL Workfront] アドイン [!DNL Outlook]. Workfrontからのコメントへの返信に関する情報 [!DNL Outlook]を参照してください。 [コメントに返信 [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* タスクやイシューを最初から作成するか、（ドラッグ&amp;ドロップ機能を使用して）既存の E メールから作成します。 詳しくは、 [を追加します。 [!DNL Outlook] タスクまたはイシューとしてプロジェクトに電子メールを送信する](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

次を追加する必要があります： [!DNL Workfront] アドインを [!DNL Outlook] アカウントを使用する前に [!DNL Workfront for Outlook].

をインストールできない場合は、 [!DNL Workfront] アドイン [!DNL Outlook] アカウント、 [!DNL Workfront] 管理者が以下を確認する必要があります。 [!DNL Outlook] 組織でアドインが有効になっている。

を有効にする方法について詳しくは、 [!DNL Outlook] 組織の統合については、 [有効にする [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
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

お使いの [!DNL Workfront] 管理者は有効にする必要があります [!DNL Outlook for Office] 次を使用 [!DNL Workfront] この統合を使用する前に。

## 必要システム構成

次のアプリケーションを使用できます。

* **[!DNL Outlook]Web 上：** The [!DNL Workfront] アドインは、 [!DNL Outlook] デスクトップまたはモバイルデバイス上の web ブラウザーから。 この機能は、 [!DNL Outlook] Web アプリ。
* **[!DNL Outlook]デスクトップアプリケーション：** The [!DNL Workfront] アドインは、 [!DNL Windows] および [!DNL Mac] のデスクトップバージョン [!DNL Outlook] 次に含まれる [!DNL Office] パッケージ。

The [!DNL Workfront] アドイン [!DNL Outlook] は、次の要件を満たす環境でサポートされます。

* [クライアント要件](#client-requirements-client-requirements)
* [メールサーバーの要件](#mail-server-requirements-mail-server-requirements)

### クライアント要件 {#client-requirements}

Workfrontは、次のバージョンの [!DNL Outlook]:

* [!DNL Outlook 2013] 以降 [!DNL Windows]
*[!DNL  Outlook 2016] 以降 [!DNL Windows]
* [!DNL Outlook] オン [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] オン [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] ウェブ上で

次に接続する必要があります： [!DNL Exchange Server] または [!DNL Office 365] 直接接続を使用する。

クライアントを設定する際、ユーザーは次のアカウントタイプのいずれかを選択する必要があります。

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B;ク&#x200B;ライアントが POP3 または IMAP に接続するように設定されている場合、 [!DNL Workfront] アドインが読み込まれません。

### メールサーバーの要件 {#mail-server-requirements}

メールサーバーの要件は、 [!DNL Office 365] または [!DNL Outlook.com]. ただし、オンプレミスインストールの [!DNL Exchange Server]の場合、次の要件が適用されます。

* Workfrontはすべてをサポート [!DNL Exchange On-Premise] サーバー
* [!DNL Exchange Web Services] (EWS) を有効にし、インターネットに公開する必要があります。
* サーバーが有効な ID トークンを発行するには、サーバーに有効な認証証明書が必要です。 の新規インストール [!DNL Exchange Server] デフォルトの認証証明書を含めます。

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* 次にアクセスするために： [!DNL Workfront] からのアドイン [[!DNL Office] ストア](https://store.office.com/)を使用する場合、クライアントアクセスサーバーはと通信できる必要があります  [https://store.office.com](https://store.office.com/).

サポートされる環境について詳しくは、 [[!DNL Microsoft Office 365] ホームページ](https://products.office.com/en-us/office-365-home).

## アドインのインストール

Outlook 用Workfrontアドインは、 [Microsoftストア](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] 対象： [!DNL Outlook 365] {#workfront-for-outlook-365}

1. In [!DNL Outlook 365]をクリックし、 **[!UICONTROL アドインの参照]** アイコン ![](assets/outlook-add-in-26x26.png)Office 365 インターフェイスの上部で、 **[!UICONTROL アドインの管理]**.

1. Adobe Analytics の **[!UICONTROL アドインを検索]** ボックス、検索 **[!DNL Workfront]** を押します。 [!UICONTROL 入力].

1. クリック **[!UICONTROL 追加]**.

### [!DNL Workfront] 対象： [!DNL Outlook] Web 上 {#workfront-for-outlook-on-the-web}

1. 開く [!DNL Microsoft Outlook] （Web ブラウザー）を使用して、
1. 次をクリック： **[!UICONTROL 参照] アドイン** アイコン ![](assets/outlook-add-in-web-version-20x20.png).

   アイコンを見つけるには、 [でのアドインの使用 [!DNL Outlook] ウェブ上で](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) (Microsoftドキュメント ) を参照してください。

1. を検索 **[!DNL Workfront]** （内） **[!UICONTROL アドインを検索]** 「 」フィールドで「 」をクリックし、 **[!UICONTROL 入力]**.

1. リストに表示されたら、 **追加**.

### [!DNL Workfront for Outlook] オン [!UICONTROL Windows] または [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. クリック **[!UICONTROL ホーム]** > **[!UICONTROL ストア]** をリボンに貼り付けます。

1. を検索 **[!DNL Workfront]** （内） **[!UICONTROL 検索]** 「 」フィールドで「 」をクリックし、 **[!UICONTROL 入力]**.

1. 切り替えボタンをクリックして、 **[!UICONTROL [!DNL Workfront]アドイン]**.

## にログインします。 [!DNL Workfront] から [!DNL Outlook]

1. In [!DNL Outlook]、電子メールメッセージを選択し、 **[!DNL Workfront]** アイコンをクリックします。
1. 画面の指示に従ってにログインします。 [!DNL Workfront] 拡張認証、OAuth 2.0、または Security Assertion Markup Language(SAML)URL を使用する。

   ユーザーが [!DNL Workfront] SAML を使用したアドイン、 [!DNL Workfront] 管理者は最初に有効にする必要があります [!DNL Office 365] SAML 2.0 ソリューションを使用して認証するためのアドイン。 詳しくは、 [設定 [!DNL Adobe Workfront] SAML 2.0 を使用](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) 記事内 [設定 [!DNL Adobe Workfront] SAML 2.0 を使用](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* のドメインの入力を求められたら、 [!DNL Workfront] アカウントに次の形式で入力します。 *yourCompany&#39;sDomain.my.workfront.com*. 会社のドメインは通常、会社の名前です。
   >* 拡張認証は、 [!DNL Workfront] 管理者がこの統合に対して有効にします。

