---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: 設定 [!DNL Adobe Workfront] Slack
description: 統合 [!DNL Adobe Workfront] Slackを使用すると、にアクセスして [!DNL Workfront] 作業項目、承認、お気に入り、Slackの最近の項目
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# 設定 [!DNL Adobe Workfront for Slack]

統合 [!DNL Adobe Workfront] と [!DNL Slack] では、次の操作を実行できます。

* 次にアクセス： [!DNL Workfront] 作業項目、承認、お気に入り、最近使用した項目 [!DNL Slack].
* 購読、承認、作業の割り当て [!DNL Slack].
* タスクとタスクの作成元 [!DNL Slack].
* いくつか受信 [!DNL Workfront] 通知 [!DNL Slack].

使用する [!DNL Slack] 環境を設定する場合は、 [!DNL Workfront for Slack] あなた自身、またはあなた自身 [!DNL Workfront] 管理者が自分で設定する前に、管理者が最初にインストールして設定する必要があります。

を統合する場合、 [!DNL Slack] インスタンスと [!DNL Workfront] ユーザーが [!DNL Workfront] 彼らの中で協力しながら [!DNL Slack] チャネル。 統合は、任意の [!DNL Slack] 環境 ( [!DNL Slack] モバイルアプリを使用します。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 計画]</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。\

## 使用の前提条件 [!DNL Workfront] と [!DNL Slack]

* 次をお持ちの場合は、 [!DNL Slack] インスタンス。
* お使いの [!DNL Slack] システム管理者は、 [!DNL Slack] インストールするユーザー [!DNL Workfront for Slack].
* 次をお持ちの場合は、 [!DNL Workfront] の統合機能を使用するためのライセンス [!DNL Workfront].

   >[!NOTE]
   >
   >任意の [!DNL Workfront] ライセンスタイプがアクセス可能 [!DNL Workfront] から [!DNL Slack]. 実行できるアクション [!DNL Slack] は、 [!DNL Workfront] ライセンスレベルと権限レベル。

でのアプリ管理について詳しくは、 [!DNL Slack]を参照してください。 [ワークスペースのアプリを管理します。](https://get.slack.help/hc/en-us/articles/222386767-Manage-apps-for-your-workspace)

## インストール [!DNL Workfront for Slack]

各 [!DNL Slack] ユーザーは、をインストールする必要があります。 [!DNL Workfront] 使用するためにアプリ自体を使用する [!DNL Workfront] から [!DNL Slack].

デスクトップアプリケーションは、次の方法でインストールできます。

* [のインストール [!DNL Workfront] 外のアプリ [!DNL Slack]](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [のインストール [!DNL Workfront] 内のアプリ [!DNL Slack]](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### のインストール [!DNL Workfront] 外のアプリ [!DNL Slack] {#install-the-workfront-app-outside-slack}

以下の手順に従って、インストールプロセスを実行し、認証します。 [!DNL Workfront for Slack] を [!DNL Slack] インスタンス。

>[!IMPORTANT]
>
>の新しいバージョンが [!DNL Workfront] Slackがリリースされた場合、アプリを引き続き使用するには、アプリを再認証する必要があります。

1. を [!DNL Adobe Workfront] アドオン [[!DNL Slack] ストア](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info).

1. クリック **[!UICONTROL 次で開く：[!DNL Slack]]**.

1. 次の項目を指定して、ワークスペースにサインイン [!DNL Slack] URL とクリック **[!UICONTROL 続行]**.\

1. アクセス権を確認します。 [!DNL Slack] がリクエストしています。 このアクセスに同意する場合は、 **[!UICONTROL アクセスを許可]** 認証する [!DNL Workfront] アプリを使用します。

これで、 [!DNL Workfront] から [!DNL Slack]( [アクセス [!DNL Workfront] から [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] から [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

### のインストール [!DNL Workfront] 内のアプリ [!DNL Slack] {#install-the-workfront-app-within-slack}

次をインストールできます： [!DNL Workfront] アプリを [!DNL Slack] アプリケーション：

1. 次の場所に移動： [!DNL Slack] URL。

   例： *`<YourTeamName>`.slack.com/apps*.

   または

   次をクリック： **[!UICONTROL アプリを追加]** アイコン [!DNL Slack] インスタンス。

1. 入力を開始 *[!DNL Workfront]* 」と入力します。
1. Enter キーを押します。
1. を選択します。 **[!DNL Workfront]** アプリを使用します。
1. クリック **[!UICONTROL 設定]**.

   アプリディレクトリページが表示されます。

1. クリック **[!UICONTROL アプリサイトにアクセス]**.
1. クリック **[!UICONTROL 追加先[!DNL Slack]]**.
1. 手順に従って、インストールを完了します。
1. インストールが完了したら、 [!DNL Workfront] から [!DNL Slack]( [[!UICONTROL アクセス [!DNL Workfront] から [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] から [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).
