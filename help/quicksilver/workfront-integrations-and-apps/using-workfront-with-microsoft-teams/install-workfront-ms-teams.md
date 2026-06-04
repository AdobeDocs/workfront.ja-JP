---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Adobe Workfront]  for Microsoft Teams をインストール'
description: ' [!DNL Adobe Workfront for Microsoft Teams]  アプリを使用すると、 [!DNL Microsoft Teams]  チャットチャネルから移動しなくても  [!DNL Workfront]  で基本的な操作を実行できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
TQID: https://experienceleague.adobe.com/6bVoPpO5kyn202DJrUZ8lEmwzz6-V0wVEY8D9F42jFo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: a7ef0b24-c866-4849-a368-53678af2dfe5
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 719
ht-degree: 83%

---

# [!DNL Adobe Workfront] for Microsoft Teams をインストール

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>[Microsoft が New Teams クライアントに移行すると](https://learn.microsoft.com/ja-jp/microsoftteams/teams-classic-client-end-of-availability)、Classic Teams クライアントは 2025年7月1日（PT）以降は使用できなくなります。 Microsoft Teams や Workfront などの統合アプリを引き続き使用するには、この日付までに New Teams クライアントに移行する必要があります。
>
>アップデートされた Workfront 統合が利用可能になりました。この統合には、New Teams エクスペリエンスとの完全な互換性があります。 ほとんどの場合、ユーザーが移行すると、Workfront が自動的に表示されます。 表示されない場合は、Microsoft Teams App Store から手動で統合をインストールできます。


[!DNL Adobe Workfront for Microsoft Teams] アプリを使用すると、[!DNL Microsoft Teams] チャットチャネルから移動しなくても [!DNL Workfront] で基本的な操作を実行できます。

>[!NOTE]
>
>[!DNL Microsoft Teams] は、[!DNL Internet Explorer] のサポートを終了しました。 [!DNL Adobe Workfront for Microsoft Teams integration] を使用する場合は、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。




## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>Work またはそれ以上</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

[!DNL Workfront] for [!DNL Microsoft Teams] をインストールするには、[!DNL Microsoft Teams] のチーム所有者である必要があります。

## [!DNL Workfront for Microsoft Teams] をインストール

[!DNL Microsoft Teams] のチーム所有者は、[!DNL Microsoft] ストアまたは [!DNL Workfront] によって提供されるファイルから、各チームの [!DNL Workfront for Microsoft Teams] アプリをインストールできます。

### [!DNL Microsoft] ストアから [!DNL Workfront for Microsoft Teams] をインストール

1. チーム所有者として [!DNL Microsoft Teams] にログインします。
1. [!DNL Workfront for Microsoft Teams] アプリをインストールするチームを選択します。
1. Workfront for Microsoft Teams統合をインストールするチームの&#x200B;**[!UICONTROL 詳細]** アイコンをクリックします
1. 「**[!UICONTROL アプリ]**」タブをクリックします。
1. **[!UICONTROL アプリおよび詳細]** ボックスに「*[!DNL Workfront]*」と入力します。
1. 「**追加**」をクリックします。
1. 開いたダイアログで「**追加**」をクリックします。
1. 「チャネルを選択」セクションで、Workfront アプリを追加するチームを選択し、**Go**&#x200B;をクリックします。

   ![&#x200B; チームを選択](assets/select-a-team.png)
1. 「**Workfrontに** ログインしてMicrosoft Teams用Workfrontにアクセスします。

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
1. インストールが完了すると、インストールが成功したことを示す通知が、選択したチームの一般チャネルに表示されます。 チームのメンバー全員がこの通知を見ることができます。

## [!DNL Microsoft] Teams から [!DNL Workfront] にログイン

[!DNL Microsoft Teams] チームの所有者は、自分またはチームの誰かが [!DNL Workfront from Microsoft Teams] にログインする前に、チームの [!DNL Workfront for Microsoft Teams] アプリをインストールする必要があります。

[!DNL Microsoft Teams] から [!DNL Workfront] にログインすると、[!DNL Workfront] ボットチャネルで [!DNL Workfront] 通知を受信したり、[!DNL Microsoft Teams] から [!DNL Workfront] で特定のアクションを実行したりすることができます。

[!DNL Workfront] アプリのインストールについて詳しくは、[&#x200B; [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams) をインストールの節を参照してください。

特定のアクションを実行するための [!DNL Microsoft Teams] から [!DNL Workfront] へのアクセスについて詳しくは、[&#x200B; [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md) から  [!DNL Adobe Workfront]  にアクセスを参照してください。

[!DNL Microsoft Teams] から [!DNL Workfront] にログインするには、次の手順を実行します。

1. [!DNL Workfront for Microsoft Teams] アプリがインストールされているチームの&#x200B;**[!UICONTROL 一般]**&#x200B;チャネルに移動して、「**[!UICONTROL Workfront にログイン]**」をクリックします。

   [!DNL Microsoft Teams] チャットチャネルに、[!DNL Workfront] ボットチャットチャネルが追加されました。

1. [!DNL Microsoft Teams]の[!DNL Workfront] ボットチャットチャネルに移動し、**[!UICONTROL 質問をここに入力]**&#x200B;または&#x200B;**メッセージを入力** フィールドに&#x200B;*[!UICONTROL ログイン]*&#x200B;と入力します。

   または

   「**[!UICONTROL ログイン]**」をクリックします。

   新しいブラウザータブが開きます。

1. 拡張認証 OAuth 2.0 または Security Assertion Markup Language（SAML）URL を使用し、画面のプロンプトに従って、[!DNL Workfront] にログインします。

   >[!NOTE]
   >
   >* [!DNL Workfront] アカウントのドメインを入力するよう求められたら、*yourCompany&#39;sDomain.my.workfront.com* の形式で入力します。 会社のドメインは通常、会社の名前です。
   >* 拡張認証は、[!DNL Workfront] 管理者が拡張認証をこの統合に対して有効にするまで使用できません。
   >* Workfront for Microsoft Teamsは、Workfront サンドボックス環境と互換性がありません。


1. ログインに使用したブラウザータブを閉じ、[!DNL Microsoft Teams] に戻ります。

   [!DNL Workfront] ボットチャットチャネルに通知が表示され、[!DNL Workfront] へのログインが完了したことを確認します。
