---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: インストール [!DNL Adobe Workfront] 対象 [!DNL Salesforce]
description: アプリがで使用可能になる前にインストールするには [!DNL Salesforce] AppExchange：インストールを参照 [!DNL Workfront] Salesforce の製品を Sales Marketplace で利用できるようにする前にAppExchange。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: 254ffae14b21dbef19b8f6b66a1c11e348c85c85
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# インストール [!DNL Adobe Workfront for Salesforce]

アプリがで使用可能になる前にインストールするには [!DNL Salesforce AppExchange]を参照してください。 [インストール [!DNL Workfront for Salesforce] 次で使用可能になる前に： [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

As a [!DNL Salesforce] および [!DNL Adobe Workfront] 管理者、インストール可能 [!DNL Workfront for Salesforce] を許可する [!DNL Salesforce] 送信するユーザー [!DNL Workfront] 要求を行い、Salesforce から離れることなくプロジェクトを自動的に作成します。

インストールによって何が期待されるかに関する一般的な理解 [!DNL Workfront for Salesforce]を参照してください。 [[!DNL Adobe Workfront for Salesforce] 概要](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [インストールおよび使用の前提条件 [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [インストール [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

## アクセス要件

この記事で説明する機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]</p> </td> 
  </tr>  </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## インストールおよび使用の前提条件 [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* 次をお持ちの場合は、 [!DNL Salesforce] インスタンスをインストールして、システム管理者アカウントにアクセスできるようにします。
* 次をお持ちの場合は、 [!DNL Workfront] 統合を設定するために、システム管理者アカウントにアクセスできるインスタンス。
* [!UICONTROL Salesforce] ユーザーが [!DNL Workfront] ～するために説明する

   * 作成 [!DNL Workfront] からのリクエスト [!DNL Salesforce] または
   * 表示 [!DNL Workfront] Salesforce のリクエストまたはプロジェクト。

## インストール [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

次の条件を満たす必要があります。 [!DNL Salesforce] および [!DNL Workfront] インストールと設定を行うシステム管理者 [!DNL Workfront for Salesforce].

次のサブセクションでは、をインストールする方法について説明します。 [!DNL Workfront] の [!DNL Salesforce] 実稼動環境。 同じ手順に従って、 [!DNL Workfront] の [!DNL Salesforce] サンドボックス環境。

* [インストール [!DNL Workfront for Salesforce] 次で使用可能になる前に： [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [インストール [!DNL Workfront for Salesforce] 内 [!DNL Salesforce Classic] フレームワーク](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [インストール [!DNL Workfront for Salesforce] 内 [!DNL Salesforce Lightning Experience] フレームワーク](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### インストール [!DNL Workfront for Salesforce] 次で使用可能になる前に： [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] が [!DNL Salesforce AppExchange] すぐに。

使用可能になる前にアプリをインストールするには：

1. 実稼動環境で、に移動します。

   `https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002eRjb`

   サンドボックス環境で、に移動します。

   `https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002eRjb`

1. 次を確認します。 **[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]** ボックス

   読み込み画面が表示され、インストールに時間がかかる場合があります。

1. クリック **[!UICONTROL 完了]** インストールが完了したら、

1. に移動します。 **[!UICONTROL [ 設定 ]>[ セキュリティコントロール ]>[ リモートサイトの設定 ]]**.
1. （条件付き） [!DNL Workfront] URL が **[!UICONTROL すべてのリモートサイト]** リスト、クリック **[!UICONTROL 新規リモートサイト]**.

1. 次を指定： **[!UICONTROL リモートサイト名]**.

   例： *[!DNL Workfront]*.

1. 次を指定： **[!UICONTROL リモートサイトの URL]**.

   例： *yourDomain.my.workfront.com*.

1. 「**[!UICONTROL 保存]**」をクリックします。

   この [!DNL Workfront] アプリが [!DNL Salesforce] インスタンスと **[!UICONTROL WorkfrontOpportunity]** および **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] ページがお使いの環境で作成されました。

   [!DNL Salesforce] ユーザーは、 [!DNL Workfront] セクションに [!UICONTROL 商談] または [!UICONTROL アカウント] ページレイアウト。\
   ユーザー向けのWorkfrontの設定について詳しくは、 [Salesforce ユーザー用のAdobe Workfrontセクションの設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### インストール [!DNL Workfront] 対象 [!DNL Salesforce] 内 [!DNL Salesforce Classic] フレームワーク

1. にログインします。 [!DNL Salesforce] をシステム管理者として設定します。
1. に移動します。 **設定。**
1. 内 **ビルド** セクションで、 **AppExchange市場**.

1. 内 **検索AppExchangeアプリ** ボックス、タイプ **Workfront**.

1. アプリが見つかったら、アプリをクリックし、 **すぐに入手**.
1. クリック **[!UICONTROL 実稼動環境にインストール]** をインストールするには、 [!DNL Workfront] アプリ内 [!DNL Salesforce] 実稼動環境。 （推奨）
1. を選択します。 **[!UICONTROL 利用条件を読み、同意しました]** フィールドに入力されます。
1. クリック **[!UICONTROL 確認してインストール]**.
1. 選択 **[!UICONTROL すべてのユーザーにインストール]** （推奨）」をクリックし、「 **[!UICONTROL インストール]**.

1. （条件付き）サードパーティへのアクセスを承認するかどうかを尋ねられた場合、 **[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]**&#x200B;を選択し、「 **[!UICONTROL 続行]**.

1. クリック **[!UICONTROL 完了]** インストールが完了したら、

   この [!DNL Workfront] アプリは、以下のリストに表示されます。 **[!UICONTROL インストール済みパッケージ]**.


1. に移動します。 **[!UICONTROL [ 設定 ]>[ セキュリティコントロール ]>[ リモートサイトの設定 ]]**.
1. （条件付き） [!DNL Workfront] URL が **[!UICONTROL すべてのリモートサイト]** リスト、クリック **[!UICONTROL 新規リモートサイト]**.\

1. 次を指定： **[!UICONTROL リモートサイト名]**.\
   例： *[!DNL Workfront]*.

1. 次を指定： **[!UICONTROL リモートサイトの URL]**.\
   例： *yourDomain.my.workfront.com*.

1. 「**[!UICONTROL 保存]**」をクリックします。\
   この [!DNL Workfront] アプリが [!DNL Salesforce] インスタンスと **[!UICONTROL WorkfrontOpportunity]** および **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] ページがお使いの環境で作成されました。\
   [!DNL Salesforce] ユーザーは、 [!DNL Workfront] セクションに [!UICONTROL 商談] または [!UICONTROL アカウント] ページレイアウト。\
   設定に関する情報 [!DNL Workfront] のセクションを参照してください。 [の設定 [!DNL Adobe Workfront] セクション [!DNL Salesforce] ユーザー](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### インストール [!DNL Workfront for Salesforce] 内 [!DNL Salesforce Lightning Experience] フレームワーク

1. にログインします。 [!DNL Salesforce] をシステム管理者として設定します。
1. 次をクリック： **[!UICONTROL 設定] アイコン**&#x200B;を選択し、「 **[!UICONTROL 設定]**.

1. 内 **[!UICONTROL PLATFORM ツール]** セクション、展開 **[!UICONTROL アプリ].**

1. クリック **[!DNL AppExchange Marketplace]**.
1. 内 **[!UICONTROL 検索 [!DNL AppExchange] アプリ]** ボックス、タイプ **[!DNL Workfront]**.

1. アプリが見つかったら、アプリをクリックし、 **[!UICONTROL すぐに入手]**.
1. クリック **[!UICONTROL ログイン画面を開く]**.\
   ログインする必要があります [!DNL Workfront] の管理者アカウント [!DNL Salesforce].

1. クリック **[!UICONTROL 許可]**.
1. 内 **[!UICONTROL この組織にインストール]** ボックス、 **[!UICONTROL ここにインストール]** インストール [!DNL Workfront] の [!DNL Salesforce] 実稼動環境。 （推奨）

1. を選択します。 **[!UICONTROL 利用条件を読み、同意しました]** フィールドに入力されます。
1. クリック **[!UICONTROL 確認してインストール]**.
1. 選択 **[!UICONTROL すべてのユーザーにインストール]** （推奨）」をクリックし、「 **[!UICONTROL インストール]**.

1. （条件付き）サードパーティへのアクセスを承認するかどうかを尋ねられた場合、 **[!UICONTROL はい、これらのサードパーティ Web サイトへのアクセス権を付与します]**&#x200B;を選択し、「 **[!UICONTROL 続行]**.

1. クリック **[!UICONTROL 完了]** インストールが完了したら、

   この [!DNL Workfront] アプリは、以下のリストに表示されます。 **[!UICONTROL インストール済みパッケージ]**.

1. に移動します。 **[!UICONTROL 設定].**
1. 内 **[!UICONTROL 設定]** セクション、展開&#x200B;**[!UICONTROL セキュリティ].**

1. クリック **[!UICONTROL リモートサイト設定]**.
1. （条件付き） [!DNL Workfront] URL が **[!UICONTROL すべてのリモートサイト]** リスト、クリック **[!UICONTROL 新規リモートサイト]**.

1. 次を指定： **[!UICONTROL リモートサイト名]**.

   例： *[!DNL Workfront]*.

1. 次を指定： **[!UICONTROL リモートサイトの URL]**.

   例： *yourDomain.my.workfront.com*.

1. 「**[!UICONTROL 保存]**」をクリックします。

   この [!DNL Workfront] アプリが [!DNL Salesforce] インスタンス、および **[!DNL Workfront]** コンポーネントが環境に追加されました。

   [!UICONTROL Salesforce] ユーザーは、 [!DNL Workfront] 追加後のアプリ [!DNL Workfront] セクションに [!UICONTROL 商談] または [!UICONTROL アカウント] ページレイアウト。\
   設定に関する情報 [!DNL Workfront] のセクションを参照してください。 [の設定 [!DNL Adobe Workfront] セクション [!DNL Salesforce] ユーザー](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
