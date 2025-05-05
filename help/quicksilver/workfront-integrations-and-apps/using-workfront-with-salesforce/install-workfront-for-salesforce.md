---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: ' [!DNL Adobe Workfront] for [!DNL Salesforce] のインストール'
description: ' [!DNL Salesforce]  AppExchange で利用可能になる前にアプリをインストールするには、AppExchange Marketplace で利用可能になる前に  [!DNL Workfront]  for Salesforce をインストールを参照してください。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: b088c305cbd16aea1b6b79a9f3a9c5ac326cd0b8
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 91%

---

# [!DNL Adobe Workfront for Salesforce] のインストール

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>[!DNL Salesforce AppExchange] で利用可能になる前にアプリをインストールするには、[ [!DNL AppExchange]  Marketplace で利用可能になる前に  [!DNL Workfront for Salesforce]  をインストール](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)を参照してください。

[!DNL Salesforce] および [!DNL Adobe Workfront] 管理者は、[!DNL Workfront for Salesforce] をインストールすると、[!DNL Salesforce] ユーザーが Salesforce を離れることなく、[!DNL Workfront] リクエストを送信し、プロジェクトを自動的に作成できます。

[!DNL Workfront for Salesforce] のインストールによって期待される内容に関する一般的な理解については、[[!DNL Adobe Workfront for Salesforce] 概要](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md)を参照してください。

* [ [!DNL Workfront for Salesforce] のインストールおよび使用の前提条件](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [ [!DNL Workfront for Salesforce] のインストール](#installing-workfrontfor-salesforce)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事で説明されている機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p><p>または</p><p>現在：[!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront for Salesforce] のインストールおよび使用の前提条件 {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* アプリをインストールするには、システム管理者アカウントにアクセスできる [!DNL Salesforce] インスタンスが必要です。
* 統合を設定するには、システム管理者アカウントにアクセスできる [!DNL Workfront] インスタンスが必要です。
* [!UICONTROL Salesforce] ユーザーが次のことを行うには、[!DNL Workfront] アカウントが必要です。

   * [!DNL Salesforce] から [!DNL Workfront] リクエストを作成する
   * Salesforce で [!DNL Workfront] リクエストまたはプロジェクトを表示する

## [!DNL Workfront for Salesforce] のインストール {#installing-workfront-for-salesforce}

[!DNL Workfront for Salesforce] をインストールして設定するには、[!DNL Salesforce] および [!DNL Workfront] のシステム管理者である必要があります。

次のサブセクションでは、[!DNL Salesforce] 実稼動環境に [!DNL Workfront] をインストールする方法について説明します。同じ手順に従って、[!DNL Salesforce] サンドボックス環境に [!DNL Workfront] をインストールできます。

* [ [!DNL AppExchange]  Marketplace で利用可能になる前に  [!DNL Workfront for Salesforce]  をインストール](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [ [!DNL Salesforce Classic]  フレームワークに  [!DNL Workfront for Salesforce]  をインストール](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [ [!DNL Salesforce Lightning Experience] フレームワークに  [!DNL Workfront for Salesforce]  をインストール](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### [!DNL AppExchange] Marketplace で利用可能になる前に [!DNL Workfront for Salesforce] をインストール {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] はまもなく [!DNL Salesforce AppExchange] で利用可能になります。

利用可能になる前にアプリをインストールするには、以下を行います。

1. 実稼働環境で、次の場所に移動します。

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   サンドボックス環境で、次の場所に移動します。

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >これらのページにアクセスするには、Salesforce にログインする必要があります。

1. 「**[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]**」ボックスをオンにします。

   読み込み画面が表示されます。インストールには時間がかかる場合があります。

1. インストールの完了後に、「**[!UICONTROL 完了]**」をクリックします。

1. **[!UICONTROL 設定]**／**[!UICONTROL セキュリティ]コントロール**／**[!UICONTROL リモートサイト設定]**&#x200B;に移動します。
1. （条件付き）リストから「Workfront」を選択します。

   または

   [!DNL Workfront] URL が&#x200B;**[!UICONTROL すべてのリモートサイト]**&#x200B;リストに表示されない場合は、**[!UICONTROL 新しいリモートサイト]**&#x200B;をクリックします。

1. （条件付き）サイトを追加する場合は、**[!UICONTROL リモートサイト名]**&#x200B;を指定します。

   例えば、*[!DNL Workfront]*。

1. （条件付き）サイトを追加する場合は、**[!UICONTROL リモートサイトの URL]** を指定します。

   例えば、*yourDomain.my.workfront.com*。

1. 「**[!UICONTROL 保存]**」をクリックします。

   [!DNL Workfront] アプリが [!DNL Salesforce]インスタンスにインストールされ、**[!UICONTROL WorkfrontOpportunities]** および **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] ページがお使いの環境に作成されました。

   [!DNL Salesforce] ユーザーは、[!UICONTROL 商談]または[!UICONTROL アカウント]のページレイアウトに「[!DNL Workfront]」セクションを追加すると、アプリを使用できるようになります。\
   ユーザー向けの Workfront セクションの設定について詳しくは、[Salesforce ユーザー向けの Adobe Workfront セクションの設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)を参照してください。

### [!DNL Salesforce Classic] フレームワークでの [!DNL Salesforce] に関する [!DNL Workfront] のインストール

1. システム管理者として [!DNL Salesforce] にログインします。
1. **設定**&#x200B;に移動します。
1. 「**ビルド**」セクションで、「**AppExchangeMarketplace**」をクリックします。

1. 「**AppExchange アプリを検索**」ボックスに「**Workfront**」と入力します。

1. Workfront アプリが見つかったら選択し、「**今すぐ入手**」をクリックします。
1. お使いの [!DNL Salesforce] 実稼動環境の [!DNL Workfront] アプリをインストールするには「**[!UICONTROL 実稼動にインストール]**」をクリックします。（推奨）
1. 利用条件を読んで同意したら、「**[!UICONTROL 利用条件を読み、同意しました]**」フィールドを選択します。
1. 「**[!UICONTROL 確認してインストール]**」をクリックします。
1. 「**[!UICONTROL すべてのユーザーにインストール]**」を選択し（推奨）、「**[!UICONTROL インストール]**」をクリックします。

1. （条件付き）サードパーティへのアクセスを承認するかどうかを尋ねられた場合、「**[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]**」を選択し、「**[!UICONTROL 続行]**」をクリックします。

1. インストールの完了後に、「**[!UICONTROL 完了]**」をクリックします。

   [!DNL Workfront] アプリは、**[!UICONTROL インストール済みパッケージ]**&#x200B;に表示されます。


1. **[!UICONTROL 設定／セキュリティコントロール／リモートサイトの設定]**&#x200B;に移動します。
1. （条件付き）**[!UICONTROL すべてのリモートサイト]**&#x200B;リストに [!DNL Workfront] URL が表示されない場合は、「**[!UICONTROL 新しいリモートサイト]**」をクリックします。

1. （条件付き）サイトを追加する場合は、**[!UICONTROL リモートサイト名]**&#x200B;を指定します。
例えば、*[!DNL Workfront]*。

1. （条件付き）サイトを追加する場合は、**[!UICONTROL リモートサイトの URL]** を指定します。
例えば、*yourDomain.my.workfront.com*。

1. 「**[!UICONTROL 保存]**」をクリックします。\
   [!DNL Workfront] アプリが [!DNL Salesforce] インスタンスにインストールされました。**[!UICONTROL WorkfrontOpportunities]** と **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] ページが環境に作成されました。\
   [!DNL Salesforce] ユーザーは、[!UICONTROL 商談]または[!UICONTROL アカウント]ページレイアウトに「[!DNL Workfront]」セクションが追加されるまで、アプリを使用できません。\
   ユーザーの [!DNL Workfront] セクションの設定について詳しくは、[ [!DNL Salesforce]  ユーザー向け  [!DNL Adobe Workfront]  セクションの設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)を参照してください。

### [!DNL Salesforce Lightning Experience] フレームワークでの [!DNL Workfront for Salesforce] のインストール

1. システム管理者として [!DNL Salesforce] にログインします。
1. **[!UICONTROL 設定]アイコン** をクリックし、「**[!UICONTROL 設定]**」をクリックします。

1. 「**[!UICONTROL プラットフォームツール]**」セクションで、**[!UICONTROL アプリ]**&#x200B;を展開します。

1. **[!DNL AppExchange Marketplace]** をクリックします。
1. 「**[!UICONTROL [!DNL AppExchange] アプリを検索]**」ボックスに、「**[!DNL Workfront]**」と入力します。

1. Workfront アプリを見つけたらクリックし、「**今すぐ入手**」をクリックします。
1. 「**[!UICONTROL ログイン画面を開く]**」をクリックします。\
   お使いの [!DNL Workfront] 管理者アカウントを使って [!DNL Salesforce] にログインする必要があります。

1. 「**[!UICONTROL 許可]**」をクリックします。
1. 「**[!UICONTROL この組織にインストール]**」ボックスで、「**[!UICONTROL ここにインストール]**」をクリックし、お使いの [!DNL Salesforce] 実稼動に [!DNL Workfront] をインストールしてください。（推奨）

1. 利用条件を読んで同意したら、「**[!UICONTROL 利用条件を読み、同意しました]**」フィールドを選択します。
1. 「**[!UICONTROL 確認してインストール]**」をクリックします。
1. 「**[!UICONTROL すべてのユーザーにインストール]**」を選択し（推奨）、「**[!UICONTROL インストール]**」をクリックします。

1. （条件付き）サードパーティへのアクセスを承認するかどうかを尋ねられた場合、「**[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]**」を選択し、「**[!UICONTROL 続行]**」をクリックします。

1. インストールの完了後に、「**[!UICONTROL 完了]**」をクリックします。

   [!DNL Workfront] アプリは、**[!UICONTROL インストール済みパッケージ]**&#x200B;に表示されます。

1. **[!UICONTROL 設定]**&#x200B;に移動します。
1. 「**[!UICONTROL 設定]**」セクションで、「**[!UICONTROL セキュリティ]」を展開します。**

1. 「**[!UICONTROL リモートサイトの設定]**」をクリックします。
1. （条件付き）**[!UICONTROL すべてのリモートサイト]**&#x200B;リストに表示されたお使いの [!DNL Workfront] URL が見つからない場合は、「**[!UICONTROL 新しいリモートサイト]**」をクリックします。

1. （条件付き）サイトを追加する場合は、**[!UICONTROL リモートサイト名]**&#x200B;を指定します。
例えば、*[!DNL Workfront]*。

1. （条件付き）サイトを追加する場合は、**[!UICONTROL リモートサイトの URL]** を指定します。
例えば、*yourDomain.my.workfront.com*。

1. 「**[!UICONTROL 保存]**」をクリックします。

   [!DNL Workfront] アプリが [!DNL Salesforce] インスタンスにインストールされ、**[!DNL Workfront]** コンポーネントが環境に追加されました。

   [!UICONTROL Salesforce] ユーザーは、「[!DNL Workfront]」セクションを[!UICONTROL 商談]ページレイアウトまたは [!UICONTROL アカウント]ページレイアウトに追加すると [!DNL Workfront] アプリを使用できます。\
   ユーザーに対する「[!DNL Workfront]」セクションの設定について詳しくは、[ [!DNL Salesforce]  ユーザーに対する  [!DNL Adobe Workfront]  セクションの設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)を参照してください。

## Workfront for Salesforce 統合の権限の設定

### `workfront_business` の権限

1. **設定**/**セキュリティ**/**信頼できる URL** に移動します。
1. リストから「`workfront_business`」を選択します。
1. 「**編集**」をクリックします。
1. 「CSP 指令」で、次のオプションを確認します。

   * connect-src （スクリプト）
   * font-src （fonts）
   * frame-src （iframe コンテンツ）
   * img-src （images）
   * media-src （オーディオおよびビデオ）
   * style-src （スタイルシート）

1. **保存**&#x200B;をクリックします。


### Workfront_session の権限

1. **設定**/**セキュリティ**/**信頼できる URL** に移動します。
1. リストから「`workfront_session`」を選択します。
1. 「**編集**」をクリックします。
1. 「CSP 指令」で、次のオプションを確認します。

   * connect-src （スクリプト）
   * font-src （fonts）
   * frame-src （iframe コンテンツ）
   * img-src （images）
   * media-src （オーディオおよびビデオ）
   * style-src （スタイルシート）

1. **保存**&#x200B;をクリックします。

