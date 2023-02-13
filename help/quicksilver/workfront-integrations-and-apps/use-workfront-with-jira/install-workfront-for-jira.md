---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: インストール [!DNL Adobe Workfront] 対象 [!DNL Jira]
description: 以下を使用できます。 [!DNL Adobe Workfront] 対象 [!DNL Jira] を [!DNL Jira] および [!DNL Workfront] システム。
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# インストール [!DNL Adobe Workfront for Jira]

以下を使用できます。 [!DNL Adobe Workfront for Jira] を [!DNL Jira] および [!DNL Workfront] システム。

アドオンをインストールした後、 [!DNL Jira] が [!DNL Workfront] 作業項目が作成されます。 両方のアプリケーションの項目がリンクされ、両方のシステムで情報の一部を自動的に更新できます。

のすべてのユーザー [!DNL Workfront] および [!DNL Jira] は、この統合のメリットを受けることができます。 彼らが最も多く機能するシステムのライセンスを必要とするだけで、両方のシステムに対しては必要ありません。

このアドオンは、 [!UICONTROL サーバー] および [!UICONTROL OnDemand] ( または [!UICONTROL クラウド]) のバージョン [!DNL Jira] ソフトウェア。 このアドオンは、 [!DNL Data Center] のバージョン [!DNL Jira] ソフトウェア。

のリスト [!DNL Jira] バージョン [!DNL Workfront for Jira] は現在、をサポートしています。 [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) アトラシア市場で

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 計画</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] ライセンスの概要</a>*</td> 
   <td> <p>[!UICONTROL プラン ]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p>重要：で別々のシステム管理者アカウントを作成することをお勧めします。 [!DNL Jira] および [!DNL Workfront] ユーザーに付随する可能性のある既存の統合を使用するのではなく、この統合専用にする場合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## インストール [!DNL Workfront] 対象 [!DNL Jira]

インストール [!DNL Workfront] 対象 [!DNL Jira] OnDemand は、 [!DNL Jira] サーバーインスタンス。

次の条件を満たす必要があります。 [!DNL Jira] インストールする管理者 [!DNL Workfront] アドオン。

次の場合、 [!DNL Jira] 管理者は、 [!DNL Workfront] アドオンを追加し、インストールをリクエストします。 リクエストが [!DNL Jira] 承認およびインストールの管理者。

にアドオンをインストールするようリクエストする方法の詳細 [!DNL Jira] アプリケーションについては、 [アドオンに対するユーザーリクエストの管理。](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

をインストールするには [!DNL Workfront for Jira]:

1. にログインします。 [!DNL Jira] as a [!DNL Jira] 管理者。
1. 次を検索： **[!DNL Workfront for Jira]** アドオン [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. クリック **[!UICONTROL 今すぐ入手]** をクリックしてインストールします。

   インストールが完了したら、にログインできます。 [!DNL Workfront] から [!DNL Jira] 統合を設定します。
   [!DNL ]
詳しくは、 [Jira 用Adobe Workfrontの設定](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## の考慮事項 [!DNL Jira Server] インストール

>[!NOTE]
>
>これらの要件は、 [!UICONTROL OnDemand] ([!UICONTROL クラウド]) バージョン [!DNL Jira] ソフトウェア。

ただし、 [!DNL Workfront] 二つのアドオン [!DNL Jira] 環境は似ていますが、 [!DNL Jira Server] インストール：

* アドオンを [!DNL Jira]の場合、 **[!DNL JIRA Base URL]** フィールドに、アクセスに使用する URL が同じでない可能性があります [!DNL Jira] をプライベートサーバーに設定します。 この **[!DNL JIRA Base URL]** は、NAT またはリバースプロキシプロトコルを使用してプライベートサーバに接続された、公にアクセス可能なアドレスである必要があります。そのため、 [!DNL Workfront] にアクセスして、サーバーにリクエストを送信できます。

* SSL 暗号化を使用して、 [!DNL Jira] および [!DNL Workfront]. SSL を有効にする場合は、認証局から完全な SSL 証明書スタックを取得する必要があります。 自己署名証明書はサポートされていません。
* 必ず [!DNL jira.workfront.com] ドメインは、会社のサーバーからアクセスできます。 A と B の間のミドルウェア環境として機能します。 [!DNL Workfront] および [!DNL Jira] とは、アドオンが動作するために必要です。

   また、送信接続と受信接続用に、次の静的 IP アドレスをファ許可リストイアウォール上のに追加する必要があります。

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   を使用して最適な機能を実現するためのファイアウォールの設定に関する詳細 [!DNL Workfront]を参照してください。 [ファイアウォールの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
