---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: ' [!DNL Adobe Workfront] for [!DNL Jira] のインストール'
description: ' [!DNL Adobe Workfront] for [!DNL Jira] を使用すると、お使いの [!DNL Jira] システムと [!DNL Workfront] システムを統合できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 83%

---

# [!DNL Adobe Workfront for Jira] のインストール

>[!IMPORTANT]
>
>より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、Workfront for Jira の統合は **2026 年 2 月 28 日** 以降は利用できなくなります。
>
>Jira を使用する場合は、組織の統合のニーズに合わせてWorkfront Automation and Integration を使用することをお勧めします。
>
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>Jira 用のWorkfront Automation and Integration Modules の具体的な機能については、「[Jira ソフトウェアモジュール ](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)」を参照してください。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

[!DNL Adobe Workfront for Jira] を使用すると、[!DNL Jira] システムと [!DNL Workfront] システムを統合できます。

このアドオンをインストールすると、[!DNL Workfront] 作業項目の作成時に [!DNL Jira] に関するイシューを自動的に作成するワークフローを定義できます。両方のアプリケーションの項目がリンクされるので、情報の一部を両方のシステムで自動的に更新できます。

[!DNL Workfront] および [!DNL Jira] のすべてのユーザーが、この統合の恩恵を受けることができます。最も頻繁に作業するシステムのライセンスのみ必要で、両方のシステムのライセンスが必要になるわけではありません。

このアドオンは、[!DNL Jira] ソフトウェアの[!UICONTROL サーバー]バージョンと[!UICONTROL オンデマンド]（または[!UICONTROL クラウド]）バージョンで利用できます。このアドオンは、[!DNL Jira] ソフトウェアの [!DNL Data Center] バージョンでは利用できません。

[!DNL Workfront for Jira] で現在サポートされている [!DNL Jira] バージョンのリストについては、Atlassian Marketplace の [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> 
   <p>新規：任意</p>
   <p>現在：[!UICONTROL Pro] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] ライセンスの概要</td> 
   <td> 
   <p>新規：標準</p>
   <p>現在：[!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p>重要：ユーザーに関連付けられている既存のアカウントを使用するのではなく、この統合専用のシステム管理者アカウントを [!DNL Jira] と [!DNL Workfront] に個別に作成することをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td><p>[!DNL Workfront] 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront] for [!DNL Jira] のインストール

[!DNL Workfront] for [!DNL Jira] OnDemand のインストール方法は、[!DNL Jira] サーバーインスタンスにインストールする場合と同じです。

[!DNL Workfront] アドオンをインストールするには、[!DNL Jira] 管理者である必要があります。

[!DNL Jira] 管理者でない場合は、[!DNL Workfront] アドオンを参照して、そのインストールをリクエストできます。リクエストは [!DNL Jira] 管理者に送信されて、承認後にインストールが行われます。

[!DNL Jira] アプリケーションへのアドオンのインストールをリクエストする方法について詳しくは、[ユーザーのアドオンリクエストの管理](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)を参照してください。

[!DNL Workfront for Jira] をインストールするには、次の手順に従います。

1. [!DNL Jira] に [!DNL Jira] 管理者としてログインします。
1. [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) で **[!DNL Workfront for Jira]** アドオンを検索します。

1. 「**[!UICONTROL 今すぐ入手]**」をクリックしてインストールします。

   インストールが完了したら、[!DNL Jira] から [!DNL Workfront] にログインし統合を設定できます。

   詳しくは、[Adobe Workfront の Jira 向け設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)を参照してください。

## [!DNL Jira Server] インストールの考慮事項

>[!NOTE]
>
>これらの要件は、[!DNL Jira] ソフトウェアの[!UICONTROL オンデマンド]（[!UICONTROL クラウド]）バージョンには当てはまりません。

2 つの [!DNL Jira] 環境への [!DNL Workfront] アドオンのインストールは似ていますが、[!DNL Jira Server] インストールを扱う際には次の点を考慮する必要があります。

* [!DNL Jira] でアドオンを設定する場合、**[!DNL JIRA Base URL]** フィールドに指定されたアドレスは、プライベートサーバー上の [!DNL Jira] へのアクセスに使用する URL と同じでない可能性があります。[!DNL Workfront] からアクセスしてサーバーにリクエストを送信できるように、**[!DNL JIRA Base URL]** は、NAT またはリバースプロキシプロトコルを使用してプライベートサーバに接続されたパブリックにアクセス可能なアドレスにする必要があります。

* SSL 暗号化を使用して、[!DNL Jira] と [!DNL Workfront] の間の通信を保護する必要があります。SSL を有効にする場合は、認証局から完全な SSL 証明書スタックを取得する必要があります。自己署名証明書はサポートされていません。
* [!DNL jira.workfront.com] ドメインが企業サーバーからアクセスできることを確認する必要があります。これは、[!DNL Workfront] と [!DNL Jira] の間のミドルウェア環境として機能し、アドオンが動作するために必要です。

  また、アウトバウンドおよびインバウンド接続用に、以下の静的 IP アドレスをファイアウォールの許可リストに追加する必要があります。

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  ファイアウォールが最適に機能するように設定する方法については、[!DNL Workfront][ファイアウォールの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。
