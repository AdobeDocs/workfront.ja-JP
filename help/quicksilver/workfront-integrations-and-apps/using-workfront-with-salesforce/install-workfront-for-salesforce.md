---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: インストール [!DNL Adobe Workfront] 対象： [!DNL Salesforce]
description: アプリがで使用可能になる前にインストールするには [!DNL Salesforce] AppExchange（「インストール」を参照） [!DNL Workfront] Salesforce の製品を Sales Marketplace で利用できるようにする前にAppExchange。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: e823589247a2231e038142ae8d19f366769060e2
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 0%

---

# インストール [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>アプリがで使用可能になる前にインストールするには [!DNL Salesforce AppExchange]を参照してください。 [インストール中 [!DNL Workfront for Salesforce] 次で使用可能になる前に： [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

As a [!DNL Salesforce] および [!DNL Adobe Workfront] 管理者、インストール可能 [!DNL Workfront for Salesforce] を許可する [!DNL Salesforce] 送信するユーザー [!DNL Workfront] 要求を行い、Salesforce から離れることなく、プロジェクトを自動的に作成します。

インストールによって何が期待されるかに関する一般的な理解 [!DNL Workfront for Salesforce]を参照してください。 [[!DNL Adobe Workfront for Salesforce] 概要](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [インストールおよび使用の前提条件 [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [インストール中 [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## アクセス要件

この記事で説明する機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td> <p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規： [!UICONTROL Standard]</p><p>または</p><p>現在： [!UICONTROL プラン ]</p> </td> 
  </tr>  </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## インストールおよび使用の前提条件 [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 次をお持ちの場合は、 [!DNL Salesforce] インスタンスをインストールして、システム管理者アカウントにアクセスできるようにします。
* 次をお持ちの場合は、 [!DNL Workfront] 統合を設定するために、システム管理者アカウントにアクセスできるインスタンス。
* [!UICONTROL Salesforce] ユーザーが [!DNL Workfront] アカウントで次のことが可能になります。

   * 作成 [!DNL Workfront] からのリクエスト [!DNL Salesforce]
   * 表示 [!DNL Workfront] Salesforce のリクエストまたはプロジェクト

## インストール中 [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

次の条件を満たす必要があります。 [!DNL Salesforce] および [!DNL Workfront] インストールと設定を行うシステム管理者 [!DNL Workfront for Salesforce].

次のサブセクションでは、をインストールする方法について説明します。 [!DNL Workfront] の [!DNL Salesforce] 実稼動環境。 同じ手順に従って、 [!DNL Workfront] の [!DNL Salesforce] サンドボックス環境。

* [インストール中 [!DNL Workfront for Salesforce] 次で使用可能になる前に： [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [インストール中 [!DNL Workfront for Salesforce] （内） [!DNL Salesforce Classic] フレームワーク](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [インストール中 [!DNL Workfront for Salesforce] （内） [!DNL Salesforce Lightning Experience] フレームワーク](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### インストール中 [!DNL Workfront for Salesforce] 次で使用可能になる前に： [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] が [!DNL Salesforce AppExchange] すぐに。

使用可能になる前にアプリをインストールするには：

1. 実稼動環境で、に移動します。

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   サンドボックス環境で、に移動します。

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   >[!NOTE]
   >
   >これらのページにアクセスするには、Salesforce にログインする必要があります。

1. 次を確認します。 **[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]** ボックス。

   読み込み画面が表示されます。 インストールには時間がかかる場合があります。

1. クリック **[!UICONTROL 完了]** インストールが完了したら、

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL セキュリティ] コントロール** > **[!UICONTROL リモートサイトの設定]**.
1. （条件付き）リストから「 Workfront 」を選択します。

   または

   表示されない場合は、 [!DNL Workfront] URL が **[!UICONTROL すべてのリモートサイト]** リスト、クリック **[!UICONTROL 新しいリモートサイト]**.

1. （条件付き）サイトを追加する場合は、 **[!UICONTROL リモートサイト名]**.

   例： *[!DNL Workfront]*.

1. （条件付き）サイトを追加する場合は、 **[!UICONTROL リモートサイトの URL]**.

   例： *yourDomain.my.workfront.com*.

1. 「**[!UICONTROL 保存]**」をクリックします。

   The [!DNL Workfront] アプリが [!DNL Salesforce] インスタンスと **[!UICONTROL WorkfrontOpportunity]** および **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] ページがお使いの環境で作成されました。

   [!DNL Salesforce] ユーザーは、 [!DNL Workfront] セクションに [!UICONTROL 商談] または [!UICONTROL アカウント] ページレイアウト。\
   ユーザー向けのWorkfrontの設定について詳しくは、 [Salesforce ユーザー用のAdobe Workfrontセクションの設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### インストール中 [!DNL Workfront] 対象： [!DNL Salesforce] （内） [!DNL Salesforce Classic] フレームワーク

1. にログインします。 [!DNL Salesforce] をシステム管理者として設定します。
1. に移動します。 **設定。**
1. Adobe Analytics の **ビルド** セクションで、 **AppExchangeMarketplace**.

1. Adobe Analytics の **検索AppExchangeアプリ** ボックス、タイプ **Workfront**.

1. 見つかったらWorkfrontアプリをクリックし、 **今すぐ入手**.
1. クリック **[!UICONTROL 実稼動環境にインストール]** をインストールするには、 [!DNL Workfront] アプリの [!DNL Salesforce] 実稼動環境。 （推奨）
1. 利用条件を読んで同意したら、 **[!UICONTROL 利用条件を読み、同意しました]** フィールドに入力します。
1. クリック **[!UICONTROL 確認してインストール]**.
1. 選択 **[!UICONTROL すべてのユーザーにインストール]** （推奨）」をクリックし、次に「 **[!UICONTROL インストール]**.

1. （条件付き）サードパーティへのアクセスを承認するかどうかを尋ねられた場合、 **[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]**&#x200B;を選択し、次に **[!UICONTROL 続行]**.

1. クリック **[!UICONTROL 完了]** インストールが完了したら、

   The [!DNL Workfront] アプリは、以下のリストに表示されます。 **[!UICONTROL インストール済みパッケージ]**.


1. に移動します。 **[!UICONTROL [ 設定 ]>[ セキュリティコントロール ]>[ リモートサイトの設定 ]]**.
1. （条件付き） [!DNL Workfront] URL が **[!UICONTROL すべてのリモートサイト]** リスト、クリック **[!UICONTROL 新しいリモートサイト]**.

1. （条件付き）サイトを追加する場合は、 **[!UICONTROL リモートサイト名]**.
例： *[!DNL Workfront]*.

1. （条件付き）サイトを追加する場合は、 **[!UICONTROL リモートサイトの URL]**.
例： *yourDomain.my.workfront.com*.

1. 「**[!UICONTROL 保存]**」をクリックします。\
   The [!DNL Workfront] アプリが [!DNL Salesforce] インスタンス。 The **[!UICONTROL WorkfrontOpportunity]** および **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] ページがお使いの環境で作成されました。\
   [!DNL Salesforce] ユーザーは、 [!DNL Workfront] セクションに [!UICONTROL 商談] または [!UICONTROL アカウント] ページレイアウト。\
   の設定に関する情報 [!DNL Workfront] のセクションを参照してください。 [を設定します。 [!DNL Adobe Workfront] のセクション [!DNL Salesforce] ユーザー](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### インストール中 [!DNL Workfront for Salesforce] （内） [!DNL Salesforce Lightning Experience] フレームワーク

1. にログインします。 [!DNL Salesforce] をシステム管理者として設定します。
1. 次をクリック： **[!UICONTROL 設定] アイコン**&#x200B;を選択し、次に **[!UICONTROL 設定]**.

1. Adobe Analytics の **[!UICONTROL PLATFORM ツール]** セクション、展開 **[!UICONTROL アプリ].**

1. クリック **[!DNL AppExchange Marketplace]**.
1. Adobe Analytics の **[!UICONTROL 検索 [!DNL AppExchange] アプリ]** ボックス、タイプ **[!DNL Workfront]**.

1. 見つかったらWorkfrontアプリをクリックし、 **今すぐ入手**.
1. クリック **[!UICONTROL ログイン画面を開く]**.\
   ログインする必要があるのは [!DNL Workfront] の管理者アカウント [!DNL Salesforce].

1. クリック **[!UICONTROL 許可]**.
1. Adobe Analytics の **[!UICONTROL この組織にインストール]** ボックス、 **[!UICONTROL ここにインストール]** インストールする [!DNL Workfront] の [!DNL Salesforce] 実稼動環境。 （推奨）

1. 利用条件を読んで同意したら、 **[!UICONTROL 利用条件を読み、同意しました]** フィールドに入力します。
1. クリック **[!UICONTROL 確認してインストール]**.
1. 選択 **[!UICONTROL すべてのユーザーにインストール]** （推奨）」をクリックし、次に「 **[!UICONTROL インストール]**.

1. （条件付き）サードパーティへのアクセスを承認するかどうかを尋ねられた場合、 **[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]**&#x200B;を選択し、次に **[!UICONTROL 続行]**.

1. クリック **[!UICONTROL 完了]** インストールが完了したら、

   The [!DNL Workfront] アプリは、以下のリストに表示されます。 **[!UICONTROL インストール済みパッケージ]**.

1. に移動します。 **[!UICONTROL 設定].**
1. Adobe Analytics の **[!UICONTROL 設定]** セクション、展開 **[!UICONTROL セキュリティ].**

1. クリック **[!UICONTROL リモートサイトの設定]**.
1. （条件付き） [!DNL Workfront] URL が **[!UICONTROL すべてのリモートサイト]** リスト、クリック **[!UICONTROL 新しいリモートサイト]**.

1. （条件付き）サイトを追加する場合は、 **[!UICONTROL リモートサイト名]**.
例： *[!DNL Workfront]*.

1. （条件付き）サイトを追加する場合は、 **[!UICONTROL リモートサイトの URL]**.
例： *yourDomain.my.workfront.com*.

1. 「**[!UICONTROL 保存]**」をクリックします。

   The [!DNL Workfront] アプリが [!DNL Salesforce] インスタンス、および **[!DNL Workfront]** コンポーネントが環境に追加されました。

   [!UICONTROL Salesforce] ユーザーは、 [!DNL Workfront] 追加後のアプリ [!DNL Workfront] セクションに [!UICONTROL 商談] または [!UICONTROL アカウント] ページレイアウト。\
   の設定に関する情報 [!DNL Workfront] のセクションを参照してください。 [を設定します。 [!DNL Adobe Workfront] のセクション [!DNL Salesforce] ユーザー](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
