---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-slack
title: ' [!DNL Adobe Workfront]  を Slack 向けに設定'
description: ' [!DNL Adobe Workfront]  を Slack と統合すると、Slack から  [!DNL Workfront]  作業アイテム、承認、お気に入り、最近使用した項目にアクセスして作成できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: cac75a81-26e8-4713-a6be-453943b431ab
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# 設定 [!DNL Adobe Workfront for Slack]

[!DNL Adobe Workfront] を [!DNL Slack] と統合すると、次の操作を実行できます。

* [!DNL Workfront] 作業アイテム、承認、お気に入り、最近使用した項目に [!DNL Slack] からアクセスします。
* [!DNL Slack] から登録、承認、作業の割り当てを行います。
* [!DNL Slack] からタスクおよびイシューを作成します。
* [!DNL Slack] で [!DNL Workfront] 通知を受信します。

[!DNL Slack] 環境の設定に応じて、[!DNL Workfront for Slack] を自身でインストールして設定するか、またはユーザーが設定を行う前に [!DNL Workfront] 管理者が最初にインストールして設定する必要があります。

[!DNL Slack] インスタンスを [!DNL Workfront] と統合する場合、[!DNL Slack] チャネル内で共同に作業を行いながら、ユーザーは [!DNL Workfront] を使用できます。[!DNL Slack] モバイルアプリを含め、任意の [!DNL Slack] 環境から統合を使用できます。

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

&#42;ご利用のプラン、ライセンスタイプ、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!DNL Slack] で [!DNL Workfront] を使用する際の前提条件

* [!DNL Slack] インスタンスが必要です。
* [!DNL Slack] システム管理者は、すべての [!DNL Slack] ユーザーに [!DNL Workfront for Slack] のインストールを許可する必要があります。
* [!DNL Workfront] の統合機能を使用するには、[!DNL Workfront] ライセンスが必要です。

  >[!NOTE]
  >
  >任意の [!DNL Workfront] ライセンスタイプを持つユーザーは、[!DNL Slack] から [!DNL Workfront] をアクセスできます。[!DNL Slack] から実行できるアクションは、[!DNL Workfront] ライセンスレベルおよび権限レベルに限定されます。

[!DNL Slack] でのアプリ管理について詳しくは、[ワークスペースでのアプリ管理](https://get.slack.help/hc/ja-jp/articles/222386767-Manage-apps-for-your-workspace)を参照してください。

## [!DNL Workfront for Slack] をインストール

各 [!DNL Slack] ユーザーは、[!DNL Slack] から [!DNL Workfront] を使用するには、[!DNL Workfront] アプリを自身でインストールする必要があります。

アプリは、次の方法でインストールできます。

* [ [!DNL Slack] 外で  [!DNL Workfront]  アプリをインストールする](#install-the-workfront-app-outside-slack-install-the-workfront-app-outside-slack)
* [ [!DNL Slack] 内に  [!DNL Workfront]  アプリをインストールする](#install-the-workfront-app-within-slack-install-the-workfront-app-within-slack)

### [!DNL Slack] 外に [!DNL Workfront] アプリをインストールする {#install-the-workfront-app-outside-slack}

以下の手順に従って、インストールプロセスを実行し、[!DNL Workfront for Slack] を [!DNL Slack] インスタンスで認証します。

>[!IMPORTANT]
>
>Slack の [!DNL Workfront] の新しいバージョンがリリースされた場合、アプリを引き続き使用するには、アプリを再認証する必要があります。

1. [[!DNL Slack]  ストア](https://workfront.slack.com/apps/A7CLAMVNW-adobe-workfront?tab=more_info)で [!DNL Adobe Workfront] アドオンを見つけます。

1. **[!UICONTROL をクリックして、[!DNL Slack]]** で開きます。

1. [!DNL Slack] URL を指定し、「**[!UICONTROL 続行]**」をクリックして、ワークスペースにログインします。

1. [!DNL Slack] がリクエストするアクセス権を確認します。このアクセスに許可する場合は、「**[!UICONTROL アクセスを許可]**」をクリックして、[!DNL Workfront] アプリを認証します。

これで、[!DNL Slack] から [!DNL Workfront] をアクセスできます（[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) で [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] から [!DNL Workfront] へのアクセスを参照）。

### [!DNL Slack] 内に [!DNL Workfront] アプリをインストールする {#install-the-workfront-app-within-slack}

[!DNL Slack] アプリケーションから直接 [!DNL Workfront] アプリをインストールできます。

1. [!DNL Slack] URL に移動します。

   例：*`<YourTeamName>`.slack.com/apps*。

   または

   [!DNL Slack] インスタンスで&#x200B;**[!UICONTROL アプリを追加]**&#x200B;アイコンをクリックします。

1. 検索フィールドに *[!DNL Workfront]* を入力開始します。
1. Enter キーを押します。
1. **[!DNL Workfront]** アプリを選択します。
1. 「**[!UICONTROL 設定]**」をクリックします。

   アプリディレクトリページが表示されます。

1. 「**[!UICONTROL アプリサイトにアクセス]**」をクリックします。
1. 「**[!UICONTROL [!DNL Slack]]** に追加」をクリックします。
1. 手順に従って、インストールを完了します。
1. インストールが完了したら、[!DNL Slack] から [!DNL Workfront] にアクセスできます（[ [!UICONTROL Access [!DNL Workfront] from [!DNL Slack]]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#viewing-all-available-commands) section in [Access [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)] を参照）。
