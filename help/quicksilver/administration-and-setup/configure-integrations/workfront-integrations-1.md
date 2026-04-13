---
title: Adobe Workfront の統合
user-type: administrator
content-type: reference;overview
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Adobe Workfront はサードパーティのアプリケーションや、他の  [!DNL Adobe]  製品と統合できます。統合により、Workfront のユーティリティを拡張し、組織のニーズに合わせて調整できます。この記事では、様々なタイプの統合について説明します。
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 50aca40a-f971-42f2-b20f-fa4fff22335e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: a1bf0e508d11089c0835f17daf6a9e17d1b6b161
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 100%

---

# [!DNL Adobe Workfront] 統合

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] をサードパーティのアプリケーションや他の [!DNL Adobe] 製品と統合できます。統合により、Workfront のユーティリティを拡張し、これを組織のニーズに合わせて調整できます。

[!DNL Workfront] 用の統合は、次のカテゴリに分類されます。

## ビルトインの（ネイティブ）統合

[!DNL Workfront] は、Workfront アプリケーションから直接設定できる、または Workfront アプリケーション用の [!DNL Workfront] アドインをインストールすることによって、他のアプリケーションから直接設定できる、様々な統合を提供します。

これらの統合の一部は追加のコストなしで利用できますが、他の統合では追加の購入が必要です。

* [ビルトインの（ネイティブ）統合の概要](#get-started-with-built-in-native-integrations)
* [追加のコストなしで利用可能な統合](#integrations-available-at-no-additional-cost)
* [追加の購入が必要な統合](#integrations-requiring-an-additional-purchase)

### ビルトインの（ネイティブ）統合の概要 {#get-started-with-built-in-native-integrations}

ビルトインの（ネイティブ）統合を開始するには、以下のワークフローに従います。

1. **ニーズに最適なネイティブ統合を決定**

   統合を選択する場合、人々が既に常用しているアプリケーションを選ぶことが重要です。[!DNL Workfront] を定期的または頻繁に使用するアプリケーションと統合すると、ユーザーの間での採用件数が増加します。

   使用可能な統合の一覧については、[追加のコストなしで利用可能な統合](#integrations-available-at-no-additional-cost)および[追加の購入が必要な統合](#integrations-requiring-an-additional-purchase)を参照してください。

1. **技術管理者の特定**

   [!DNL Workfront] と統合するアプリケーションについて、組織の技術管理者を特定します。例えば、[!DNL Slack] との統合を選択した場合、会社の [!DNL Slack] 管理者に連絡し、プラットフォーム内の設定ニーズに参加してもらいます。[!DNL Workfront] カスタマーサポートと行うすべての会話にも、この管理者を参加させる必要があります。

   管理者が作業を開始するには、その統合に関する具体的な手順を提供する必要があります。これらの手順へのリンクについては、[追加のコストなしで利用可能な統合](#integrations-available-at-no-additional-cost)を参照してください。

1. **[!DNL Workfront] カスタマーサポート**&#x200B;との連携

   管理者にネイティブ統合の設定に関して課題が発生した場合は、[!DNL Workfront] カスタマーサポートと連携して、ガイドやトラブルシューティングを支援してください。[!DNL Workfront] が統合を設定することはないため、アドビでは、お客様がご自身で設定を行うために必要なすべてのツールおよびリソースを提供することに尽力しています。カスタマーサポートに直接お問い合わせいただいてもよいですし、統合を簡単に設定するのに役立つ、広範なリソース記事を参照することもできます。

   カスタマーサポートへの連携については、[ カスタマーサポートに連絡](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)を参照してください。

   ヘルプ記事へのリンクについては、[追加のコストなしで利用可能な統合](#integrations-available-at-no-additional-cost)および[追加の購入が必要な統合](#integrations-requiring-an-additional-purchase)を参照してください。

   サポートケースの作成手順については、[カスタマーサポートに連絡](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)を参照してください。

   >[!NOTE]
   >
   >サポートケースを提出するには、組織の任命されたサポート担当者である必要があります。ケースが送信された後、他のシステムの技術管理者も会話に追加できます。他のシステムの技術管理者は直接サポートに連絡することはできません。

使用可能なビルトインの（ネイティブ）統合は、会社のニーズのすべては満たしていない可能性があることを、アドビは理解しています。その場合は、アカウント担当者に連絡して、カスタム統合についてご相談ください。

### 追加のコストなしで利用可能な統合 {#integrations-available-at-no-additional-cost}

[!DNL Workfront] は、追加のコストなしで、以下のビルトインの統合を提供します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>システム</th> 
   <th>概要</th> 
   <th>要件</th> 
   <th>インストールを実行できるユーザー</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Express</p> </td> 
   <td> 
    <ul> 
     <li>プルーフエクスペリエンスを Adobe Express と統合します。この統合により、次のことができるようになります。 
     <ul>
     <li>Workfront 承認テンプレートを使用して、承認ワークフローを定義する。 </li>
     <li>プルーフビューアーで Adobe Express ドラフトコンテンツをレビューする。 </li>
     <li>最終承認と公開方法について、Adobe Express のレビューの決定を確認する。 </li>
     </ul>
   </ul>
     <p>詳しくは、<a href="/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-express.md" class="MCXref xref">Adobe Express と Workfront Proof の統合の基本を学ぶ</a>を参照してください。</p> 
     </td>  <td><ul><li>Workfront と Adobe Express の両方のライセンスが必要です。</li><li>Workfront と Adobe Express は、同じ IMS 組織にデプロイする必要があります。</li></ul></td> 
   <td>アドビ製品チームが、お使いのアカウントでこの統合を有効にする必要があります。詳しくは、<a href="/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-express.md" class="MCXref xref">Adobe Express とWorkfront Proof の統合の基本を学ぶ</a>を参照してください。</td> 
  </tr>
 <tr> 
   <td role="rowheader"> <p>GenStudio for Performance Marketing </p> </td> 
   <td> 
    <ul> 
     <li>プルーフエクスペリエンスと GenStudio for Performance Marketing を統合します。この統合により、次のことができるようになります。 
     <ul>
     <li>Workfront 承認テンプレートを使用して、承認ワークフローを定義する。 </li>
     <li>プルーフビューアーで GenStudio ドラフトコンテンツをレビューする。 </li>
     <li>最終承認と公開について、GenStudio のレビューの決定を確認する。 </li>
     </ul>
   </ul>
     <p>詳しくは、<a href="/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-genstudio.md" class="MCXref xref">プルーフと GenStudio for Performance Marketing の統合の基本を学ぶ</a>を参照してください。</p> 
     </td>  <td><ul><li>Workfront と GenStudio for Performance Marketing の両方のライセンスが必要です。</li><li>Workfront インスタンスは、Adobe Unified Experience 上にある必要があります。</li><li>Workfront と GenStudio for Performance Marketing は、同じ IMS 組織にデプロイする必要があります。</li></ul></td> 
   <td>すべての要件が満たされたら、Workfront の設定エリアで統合をオンに切り替えることができます。詳しくは、<a href="/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-genstudio.md" class="MCXref xref">プルーフと GenStudio for Performance Marketing の統合の基本を学ぶ</a>を参照してください。 </td> 
  </tr>
  <tr> 
   <td role="rowheader"> <p>Adobe Creative Cloud </p> <p> <img src="assets/creative-cloud-logo.png"> </p> </td> 
   <td> 
    <ul> 
     <li>[!DNL Workfront] コメントと承認を以下の Adobe Creative Cloud アプリケーションと統合します。 
     <ul>
     <li>InDesign </li>
     <li>Illustrator </li>
     <li>Photoshop </li>
     <li>XD </li>
     <li>Premiere Pro </li>
     <li>After Effects </li>
     </ul>
     <li><p><a href="https://exchange.adobe.com/apps/browse/cc?page=1&amp;product=All&amp;q=workfront&amp;sort=RELEVANCE" class="MCXref xref">Adobe Exchange</a> からダウンロード／インストールします。</p></li></ul>
     <p>詳しい情報と手順については、<a href="https://experienceleague.adobe.com/ja/docs/workfront/using/adobe-workfront-integrations/workfront-for-creative-cloud/install-wf-cc/wf-cc-install-toc" class="MCXref xref">[!DNL Creative Cloud] アプリケーション向け [!DNL Adobe Workfront] プラグインのインストール</a>を参照してください。</p> 
     </td>  <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Experience Manager Assets と Assets Essentials </p>  </p> </td> 
   <td> 
    <ul> 
     <li>Workfront と Adobe Experience Manager 間でリンクされたフォルダーを自動的に作成 
      <li>既存のリンクされたアセットのメタデータを同期</p></li>
      <li>Workfront で変更されたときに、ポートフォリオ、プログラム、プロジェクト、タスク、イシュー、ドキュメントのメタデータを自動的に更新</li>
      <li>複数の Experience Manager Assets リポジトリを 1 つの Workfront 環境に、または複数の Workfront 環境を組織 ID をまたいで 1 つの Experience Manager Assets リポジトリにスムーズに接続します。</li></ul>
     <p>詳細と手順について詳しくは、<a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/aem-asset-integrations.md" class="MCXref xref">Adobe Experience Manager Assets 統合の概要</a>を参照してください。</p> 
     </td>
   <td><ul><li>Workfront は、割り当てられた組織 ID を持つ Admin Console に属している必要があります。</li><li>Workfront および Experience Manager Assets または Assets Essentials は、統合を設定するユーザーに製品として割り当てる必要があります。</li></ul></td>   <td></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Box]</p> <p> <img src="assets/box,-inc.-logo.png"> </p> </td> 
   <td> 
    <ul> 
     <li>ドキュメントとフォルダーのリンク先 [!DNL Workfront]</li> 
    </ul> <p>詳しくは、<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合の設定</a>を参照してください。</p> </td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Dropbox]</p> <p> <img src="assets/dropbox-1-logo-png-transparent.png"> </p> </td> 
   <td> 
    <ul> 
     <li>ドキュメントとフォルダーのリンク先 [!DNL Workfront]</li> 
    </ul> <p>詳しくは、<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合の設定</a>を参照してください。</p> </td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Google Drive]</p> <p> <img src="assets/google-drive-logo.png"> </p> </td> 
   <td> 
    <ul> 
     <li>ドキュメントとフォルダーのリンク先 [!DNL Workfront]</li> 
    </ul> <p>詳しくは、<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合の設定</a>を参照してください。</p> </td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Microsoft OneDrive]</p> <p> <img src="assets/microsoft-onedrive.png"> </p> </td> 
   <td> 
    <ul> 
     <li>ドキュメントとフォルダーのリンク先 [!DNL Workfront]</li> 
    </ul> <p>詳しくは、<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合の設定</a>を参照してください。</p> </td> 
   <td></td> 
   <td></td> 
   </tr> 
  <tr> 
   <td> <p>[!DNL Microsoft Teams]</p> <p> <img src="assets/msteamslogo.png" style="max-width: 80px;"> </p> </td> 
   <td> 
    <ul> 
     <li>[!DNL Microsoft] Teams で [!DNL Workfront] 通知を受け取る </li> 
     <li>承認決定を行う </li> 
     <li>[!DNL Workfront] プロジェクト、タスクおよびイシューを検索 </li> 
     <li>[!DNL Workfront] 個人タスクを作成 </li> 
     <li>[!DNL Workfront] リクエストを送信 </li> 
    </ul> <p>詳しくは、<a href="../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/use-workfront-with-ms-teams.md" class="MCXref xref">[!DNL Adobe Workfront for Microsoft Teams]：記事インデックス</a>を参照してください。</p><p><b>メモ</b>：Microsoft は、2025年7月1日（PT）をもって Classic Teams デスクトップアプリのサポートを終了します。この結果、Classic Teams デスクトップアプリが使用できなくなると、Workfront とMicrosoft Teams の統合もサポートされなくなります。 </p></td> 
   <td> 
    <ul> 
     <li>複数のチームが使用する場合は、組織の各チームが統合をインストールする必要があります</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>チーム所有者</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL SharePoint]</p> <p> <img src="assets/sharepoint.png"> </p> </td> 
   <td> 
    <ul> 
     <li>ドキュメントとフォルダーのリンク先 [!DNL Workfront]</li> 
    </ul> <p>詳しくは、<a href="../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md" class="MCXref xref">[!DNL SharePoint] 統合を設定</a>を参照してください。</p> </td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Slack]</p> <p> <img src="assets/slacklogo.png" style="max-width: 80px;"> </p> </td> 
   <td> 
    <ul> 
     <li>[!DNL Slack] で [!DNL Workfront] 通知を受信 </li> 
     <li>[!DNL Slack] で承認を管理 </li> 
     <li>[!DNL Slack] から [!DNL Workfront] タスクとイシューを作成 </li> 
     <li>プロジェクトまたはタスクに対するコメントの投稿 [!DNL Slack]</li> 
    </ul> <p>詳しくは、<a href="../../workfront-integrations-and-apps/using-workfront-with-slack/use-workfront-for-slack.md" class="MCXref xref">[!DNL Adobe Workfront for Slack]</a> を参照してください。</p> </td> 
   <td> 
    <ul> 
     <li>[!DNL Slack] 管理者は、すべての Slack ユーザーにインストールを許可する必要があります [!DNL Workfront for Slack]</li> 
     <li>[!DNL Slack] ユーザーは [!DNL Workfront] ライセンスが必要です </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>[!DNL Slack] 管理者</li> 
     <li>[!DNL Workfront] 管理者 </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Webdam]</p> <p> <img src="assets/webdam-logo.png"> </p> </td> 
   <td> 
    <ul> 
     <li>ドキュメントとフォルダーのリンク先 [!DNL Workfront]</li> 
    </ul> <p>詳しくは、<a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">ドキュメント統合の設定</a>を参照してください。</p> </td> 
   <td></td> 
   <td></td> 
  </tr> 
 </tbody> 
</table>

### 追加の購入が必要な統合 {#integrations-requiring-an-additional-purchase}

[!DNL Workfront] を使用すると、他のビルトインの統合および統合製品を追加費用で活用できます。価格の詳細について詳しくは、アカウント担当者にお問い合わせください。

* [!DNL Workfront Fusion]

  [!DNL Adobe Workfront Fusion] は、アプリ内やサービス内およびそれらの間でアクションをリンクして、データを自動的に転送および変換するシナリオを作成します。多くのアプリへの専用コネクタを備えていますが、公開 API を使用して任意のアプリケーションに接続できます。

  詳しくは、[[!DNL Adobe Workfront Fusion] 概要](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)を参照してください。

* [!DNL Adobe Experience Manager Assets]
* [!DNL Anaplan]（[!DNL Workfront Fusion] が必要）

Workfront と Experience Manager Assets、または Assets Essentials の統合により、組織は作業とデジタルアセット管理を本質的に結び付けることで、コンテンツの速度と市場投入までの時間を改善できます。

詳しくは、[Adobe Workfront for Experience Manager Assets 統合の概要](../../documents/adobe-workfront-for-experience-manager-assets-essentials/aem-asset-integrations.md)を参照してください。

## パートナー統合

Workfront には、Workfront のエクスペリエンスを強化する多くのパートナー統合があります。既存のパートナーサービスの例として、Claravine、RWS グループとの統合などがあります。

これらの統合およびその他のパートナー統合について詳しくは、[Exchange マーケットプレイス](https://exchange.adobe.com/jp/apps/browse/ec?page=1&partnerLevel=All&product=WRKFRNT&sort=RELEVANCE)を参照してください。

## [!DNL Workfront] API

[!DNL Workfront] API を使用すると、パブリック API を活用して [!DNL Workfront] エクスペリエンスを拡張し、向上させることができます。オープン API を使用して、独自の統合を作成できます。

[!DNL Workfront] API で利用可能なオブジェクトのリストについて詳しくは、[!DNL Workfront] [API エクスプローラー](../../wf-api/general/api-explorer.md)を参照してください。

