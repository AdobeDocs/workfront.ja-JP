---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: ' [!DNL Adobe Workfront] for [!DNL Jira] のインストール'
description: ' [!DNL Adobe Workfront] for [!DNL Jira] を使用すると、お使いの [!DNL Jira] システムと [!DNL Workfront] システムを統合できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: b98a7fa48e60f1f2c2ea938b14b88e0c5a2ee418
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 91%

---

# [!DNL Adobe Workfront for Jira] のインストール

[!DNL Adobe Workfront for Jira] を使用すると、[!DNL Jira] システムと [!DNL Workfront] システムを統合できます。

このアドオンをインストールすると、[!DNL Workfront] 作業項目の作成時に [!DNL Jira] に関するイシューを自動的に作成するワークフローを定義できます。両方のアプリケーションの項目がリンクされるので、情報の一部を両方のシステムで自動的に更新できます。

[!DNL Workfront] および [!DNL Jira] のすべてのユーザーが、この統合の恩恵を受けることができます。最も頻繁に作業するシステムのライセンスのみ必要で、両方のシステムのライセンスが必要になるわけではありません。

このアドオンは、[!DNL Jira] ソフトウェアの[!UICONTROL サーバー]バージョンと[!UICONTROL オンデマンド]（または[!UICONTROL クラウド]）バージョンで利用できます。このアドオンは、[!DNL Jira] ソフトウェアの [!DNL Data Center] バージョンでは利用できません。

のリスト [!DNL Jira] のバージョン [!DNL Workfront for Jira] は現在、をサポートしています。 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) アトラシア市場で

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td> 
   <p>新規：任意</p>
   <p>現在： [!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] ライセンスの概要</td> 
   <td> 
   <p>新規：標準</p>
   <p>現在： [!UICONTROL プラン ]</p></td> 
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

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## [!DNL Workfront] for [!DNL Jira] のインストール

[!DNL Workfront] for [!DNL Jira] OnDemand のインストール方法は、[!DNL Jira] サーバーインスタンスにインストールする場合と同じです。

[!DNL Workfront] アドオンをインストールするには、[!DNL Jira] 管理者である必要があります。

[!DNL Jira] 管理者でない場合は、[!DNL Workfront] アドオンを参照して、そのインストールをリクエストできます。リクエストは [!DNL Jira] 管理者に送信されて、承認後にインストールが行われます。

[!DNL Jira] アプリケーションへのアドオンのインストールをリクエストする方法について詳しくは、[ユーザーのアドオンリクエストの管理](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)を参照してください。

[!DNL Workfront for Jira] をインストールするには、次の手順に従います。

1. [!DNL Jira] に [!DNL Jira] 管理者としてログインします。
1. [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) で **[!DNL Workfront for Jira]** アドオンを検索します。

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
