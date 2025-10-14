---
product-area: workfront-integrations;user-management
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: Google Workspaceへのログイ  [!DNL Adobe Workfront]  とログアウト
description: この記事では、 [!DNL Adobe Workfront for] Google Workspace統合にログインする方法と統合からログアウトする方法について説明します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 8a91f1d9-bc67-4c27-a6c0-2482488c670b
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 50%

---

# [!DNL Adobe Workfront for Google Workspace] にログインおよびログアウトする

>[!IMPORTANT]
>
>より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、Google Workspaceの次のWorkfront機能は、**2026 年 2 月 28 日** 以降は使用できなくなります。
>
>* Workfront内からのGoogle Workspace機能へのアクセス
>
>* Gmail またはWorkfrontのカレンダーサイトパネルからのGoogle タスクの表示と管理
>
>Google Workspaceを使用した組織の統合のニーズに対しては、Workfront Automation and Integration を使用することをお勧めします。
>
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>Google WorkspaceのWorkfront Automation and Integration モジュールの具体的な機能については、{Gmail モジュール [&#x200B; および &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)2}Google カレンダーモジュール [&#x200B; を参照してください。](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)

## アクセス要件

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
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
   </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!DNL Workfront for Google Workspace] にログインまたはログアウトする前に、以下を行う必要があります

* [!DNL Workfront for Google Workspace] をインストール\
   手順については、[インストール [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)を参照してください。

## [!DNL Adobe Workfront for Google Workspace] にログインする

1. [!DNL Workfront]、![&#x200B; または &#x200B;](assets/wf-lion-icon.png) の右端にある [!DNL Google Workspace] アドオンサイドバーの [!DNL Gmail] アイコン [!DNL Google Calendar]1&rbrace;Workfront アイコン &rbrace; をクリックします。[!DNL Google Drive]

   [!DNL Workfront for Google Workspace] アドオンをインストールしたばかりで、このアイコンが表示されない場合は、ブラウザーページを更新してみてください。

1. [!DNL Workfront for Google Workspace] アドオンの「**[!UICONTROL ログイン]**」をクリックします。
1. [!DNL Workfront] ドメイン アドレス（*companyname.my.workfront.com* など）を入力します。
1. 画面の指示に従って、[!DNL Workfront] にログインします。

   >[!NOTE]
   >
   >* [!DNL Workfront] と [!DNL Google Workspace] との接続には OAuth 2.0 を使用します。これはほとんどの Web ベースの統合で、ユーザーの認証と承認に使用される安全な規格です。
   >* [!DNL Workfront] アカウントの [ ドメインまたはホスト ] を入力するよう求められた場合は、*yourCompany&#39;sDomain.my.workfront.com* の形式で入力します。会社のドメインは通常、会社の名前です。


## [!DNL Workfront for Google Workspace] からログアウトする

1. Google Workspaceの [!UICONTROL Workfront] パネルが表示されない場合は、ページの右端にあるア [!DNL Workfront] オンサイドバーの ![&#x200B; アイコン &#x200B;](assets/wf-lion-icon.png)3&rbrace;Workfront アイコン &rbrace; をクリックします。[!DNL Google Workspace]
1. [!DNL Workfront for Google Workspace] パネルの上部にある「**[!UICONTROL その他]**」アイコンをクリックします。

1. 表示されるメニューで「**[!UICONTROL ログアウト]**」をクリックします。

   これによって、[!DNL Google Workspace] からログアウトされるわけではありません。
