---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Jira のアクティビティログの表示
description: ' [!DNL Jira]  管理者は、  [!DNL Adobe Workfront]  と  [!DNL Jira]  の間の同期中またはチケットの作成中に発生した例外やエラーをアクティビティログで参照できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 66%

---

# [!UICONTROL [!DNL Jira]アクティビティログ]の表示

>[!IMPORTANT]
>
>より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、Workfront for Jira の統合は **2026 年 2 月 28 日** 以降は利用できなくなります。
>
>Jira を使用する場合は、組織の統合のニーズに合わせてWorkfront Automation and Integration を使用することをお勧めします。
>
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>Jira 用のWorkfront Automation and Integration Modules の具体的な機能については、「[Jira ソフトウェアモジュール &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new)」を参照してください。

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

[!DNL Jira] 管理者は、[!DNL Adobe Workfront] と [!DNL Jira] の間の同期中またはチケットの作成中に発生した例外やエラーを[!UICONTROL アクティビティログ]で参照できます。

アクティビティログには、最大 500 個の項目が新しい順に表示されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準 </p>
       <p>プラン </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira アクセス</td> 
   <td> <p>システム管理者のアクセス権</p> <p>重要：ユーザーに関連付けられた既存のシステム管理者アカウントを使用するのではなく、Jira とWorkfrontで個別のシステム管理者アカウントを作成して、この統合専用にすることをお勧めします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

[!DNL Workfront] と [!DNL Jira] 間の項目をリンクするには、まず以下が必要です

* [!DNL Workfront for Jira] をインストールする

  [!DNL Workfront for Jira] をインストールする手順については、[インストール [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)を参照してください。

## [!UICONTROL [!DNL Jira]アクティビティログ]にアクセスする

1. システム管理者として Jira にログインします。
1. [!DNL Jira] のメインメニューで「**[!UICONTROL 設定]**」をクリックします。
1. 「**[!UICONTROL アドオン]**」、「**[!UICONTROL アドオンを管理]**」の順にクリックします。

1. **[!DNL Workfront]** アドオンを展開します。
1. 「**[!UICONTROL 設定]**」をクリックします。
1. システム管理者として [!DNL Workfront] にログインします。
1. 「**[!UICONTROL アクティビティログ]**」タブを選択します。

   アイテムの作成中、または 2 つのアプリケーションのフィールドの同期中に発生した例外およびエラーに関する情報が表示されます。

   ログには、次のフィールドが含まれます。

   * 発生日
   * Jira のユーザーの名前
   * Jira のイシュー番号
   * 発生したエラーの簡単な説明。
