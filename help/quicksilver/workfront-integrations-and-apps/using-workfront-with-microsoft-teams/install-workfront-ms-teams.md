---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Adobe Workfront]  for Microsoft Teams をインストール'
description: ' [!DNL Adobe Workfront for Microsoft Teams]  アプリを使用すると、 [!DNL Microsoft Teams]  チャットチャネルから移動しなくても  [!DNL Workfront]  で基本的な操作を実行できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
source-git-commit: 940cbfb34f12eacd5ba698f60fb7a3e67eb62b22
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 70%

---

# [!DNL Adobe Workfront] for Microsoft Teams をインストール

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>[Microsoftが新しい Teams クライアント &#x200B;](https://learn.microsoft.com/en-us/microsoftteams/teams-classic-client-end-of-availability) に移行すると、Classic Teams クライアントは 2025 年 7 月 1 日（PT）以降は使用できなくなります。 Microsoft TeamsとWorkfrontなどの統合アプリを引き続き使用するには、この日付までに New Teams クライアントに移行する必要があります。
>
>更新されたWorkfront統合が利用できるようになり、新しい Teams エクスペリエンスと完全に互換性があります。 ほとんどの場合、ユーザーが移行すると、Workfrontが自動的に表示されます。 そうでない場合は、Microsoft Teams App Storeから手動で統合をインストールできます。


[!DNL Adobe Workfront for Microsoft Teams] アプリを使用すると、[!DNL Microsoft Teams] チャットチャネルから移動しなくても [!DNL Workfront] で基本的な操作を実行できます。

>[!NOTE]
>
>[!DNL Microsoft Teams] は、[!DNL Internet Explorer] のサポートを終了しました。[!DNL Adobe Workfront for Microsoft Teams integration] を使用する場合は、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。


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
   <td><p>新規：標準</p>
    <p>現在：[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

[!DNL Workfront] for [!DNL Microsoft Teams] をインストールするには、[!DNL Microsoft Teams] のチーム所有者である必要があります。

## [!DNL Workfront for Microsoft Teams] をインストール

[!DNL Microsoft Teams] のチーム所有者は、[!DNL Microsoft] ストアまたは [!DNL Workfront] によって提供されるファイルから、各チームの [!DNL Workfront for Microsoft Teams] アプリをインストールできます。

### [!DNL Microsoft] ストアから [!DNL Workfront for Microsoft Teams] をインストール

1. チーム所有者として [!DNL Microsoft Teams] にログインします。
1. [!DNL Workfront for Microsoft Teams] アプリをインストールするチームを選択します。
1. Workfront for Microsoft Teams統合をインストールするチームの **[!UICONTROL 詳細]** アイコンをクリックします
1. 「**[!UICONTROL アプリ]**」タブをクリックします。
1. 「**[!UICONTROL アプリなどを検索]**」ボックスに *[!DNL Workfront]* と入力します。
1. 「**追加**」をクリックします。
1. 開いたダイアログで「**追加**」をクリックします。
1. 「チャンネルを選択」セクションで、Workfront アプリを追加するチームを選択し、「**移動**」をクリックします。

   ![&#x200B; チームの選択 &#x200B;](assets/select-a-team.png)
1. Workfrontに **ログイン**」をクリックして、Microsoft TeamsのWorkfrontにアクセスします。

   [!DNL Workfront] へのログインの詳細については、この記事の [Microsoft Teams から Workfront にログイン](#log-in-to-workfront-from-microsoft-teams)の節を参照してください。

### プライベートファイルから [!DNL Workfront for Microsoft Teams] をインストール

組織が [!DNL Microsoft] ストアからのアプリのダウンロードへのアクセスを制限している場合は、サポートチームに連絡し、[!DNL Workfront for Microsoft Teams] アプリのプライベートファイルをリクエストしてアプリをインストールする必要があります。

サポートチームへのお問い合わせについては、[カスタマーサポートへのお問い合わせ](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)を参照してください。

[!DNL Workfront for Microsoft Teams] をプライベートファイルからインストールするには、次の手順を実行します。

1. [!DNL Workfront] から受け取ったプライベートファイルをコンピューターに保存します。
1. [!DNL Microsoft] チーム所有者として [!DNL Microsoft Teams] にログインします。
1. [!DNL Workfront for Microsoft Teams] をインストールするチームの&#x200B;**[!UICONTROL その他]**&#x200B;アイコンをクリックします。

1. 「**[!UICONTROL チームの管理]**」をクリックします。
1. 「アプリ」タブを選択し、画面の左上隅にある「アプリをアップロード」をクリックします。
1. コンピューターに保存したプライベートファイルを参照し、インストール手順に従って [!DNL Workfront for Microsoft Teams] をインストールします。
1. インストールが完了すると、インストールが成功したことを示す通知が、選択したチームの一般チャネルに表示されます。チームのメンバー全員がこの通知を見ることができます。

## [!DNL Microsoft] Teams から [!DNL Workfront] にログイン

[!DNL Microsoft Teams] チームの所有者は、自分またはチームの誰かが [!DNL Workfront from Microsoft Teams] にログインする前に、チームの [!DNL Workfront for Microsoft Teams] アプリをインストールする必要があります。

[!DNL Microsoft Teams] から [!DNL Workfront] にログインすると、[!DNL Workfront] ボットチャネルで [!DNL Workfront] 通知を受信したり、[!DNL Microsoft Teams] から [!DNL Workfront] で特定のアクションを実行したりすることができます。

[!DNL Workfront] アプリのインストールについて詳しくは、[&#x200B; [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams) をインストールの節を参照してください。

特定のアクションを実行するための [!DNL Microsoft Teams] から [!DNL Workfront] へのアクセスについて詳しくは、[&#x200B; [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md) から  [!DNL Adobe Workfront]  にアクセスを参照してください。

[!DNL Microsoft Teams] から [!DNL Workfront] にログインするには、次の手順を実行します。

1. [!DNL Workfront for Microsoft Teams] アプリがインストールされているチームの&#x200B;**[!UICONTROL 一般]**&#x200B;チャネルに移動して、「**[!UICONTROL Workfront にログイン]**」をクリックします。

   [!DNL Microsoft Teams] チャットチャネルに、[!DNL Workfront] ボットチャットチャネルが追加されました。

1. [!DNL Microsoft Teams] の [!DNL Workfront] ボットチャットチャネルに移動し、「*[!UICONTROL 質問をここに入力]*」または **[!UICONTROL メッセージを入力]** フィールドに **ログイン** と入力します。

   または

   「**[!UICONTROL ログイン]**」をクリックします。

   新しいブラウザータブが開きます。

1. 拡張認証 OAuth 2.0 または Security Assertion Markup Language（SAML）URL を使用し、画面の指示に従って、[!DNL Workfront] にログインします。

   >[!NOTE]
   >
   >* [!DNL Workfront] アカウントのドメインを入力するよう求められたら、*yourCompany&#39;sDomain.my.workfront.com* の形式で入力します。会社のドメインは通常、会社の名前です。
   >* 拡張認証は、[!DNL Workfront] 管理者が拡張認証をこの統合に対して有効にするまで使用できません。
   >* Microsoft Teams用Workfrontは、Workfront サンドボックス環境との互換性がありません。


1. ログインに使用したブラウザータブを閉じ、[!DNL Microsoft Teams] に戻ります。

   [!DNL Workfront] ボットチャットチャネルに通知が表示され、[!DNL Workfront] へのログインが完了したことを確認します。
