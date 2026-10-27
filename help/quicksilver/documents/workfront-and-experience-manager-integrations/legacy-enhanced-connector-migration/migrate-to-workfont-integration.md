---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 従来のコネクタまたは拡張コネクタから Adobe Experience Manager as a Cloud Service 統合向け Workfront への移行
description: このページでは、Workfront for Experience Cloud の拡張コネクタまたは従来のコネクタから、Workfront と Adobe Experience Manager Assets as a Cloud Service を接続する最新のネイティブ統合に移行するためのベストプラクティスについて説明します。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
TQID: 'https://experienceleague.adobe.com/0pAHfS7cDqv1tV4TBdx9WqvJA1-zySGsPHVXI8EG7Hc'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: e7123179a59cd7ed9c76f4718b3b8019854cbfe1
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 100%
---
# 従来のコネクタまたは拡張コネクタから Adobe Experience Manager as a Cloud Service 統合向け Workfront への移行

このページでは、Workfront for Experience Cloud の拡張コネクタまたは従来のコネクタから、Workfront と Adobe Experience Manager Assets as a Cloud Service を接続する最新のネイティブ統合に移行するためのベストプラクティスについて説明します。

>[!IMPORTANT]
>
>この情報は、Adobe Experience Manager Assets オンプレミスまたは Managed Services 環境を使用しているお客様には適用されません。

<!--

## Move your Workfront instance to the Admin Console

Customers that intend to use the new native integration between Workfront and Adobe Experience Manager Assets as a Cloud Service must ensure their Workfront environment is tied to an Adobe Admin Console. For existing Workfront environments, this will likely require a migration of the environment to a connected Adobe Admin Console. For more details regarding this migration and the associated checklist, see [Prepare to onboard your organization to the Adobe Admin Console](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md). 

 Adobe must help carry out this migration. To request help, do one of the following:

* If you have Workfront Hub access, submit your request to the [Workfront Migration to Adobe Admin Console](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=629674d500054a38133cf26e01d06a97&path=).
* If you do not have Workfront Hub access, you can submit your request to the [Workfront to Adobe Admin Console Early Migration Request Queue](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

-->

## 新しい Workfront を Adobe Experience Manager Assets as a Cloud Service 統合のために設定する

Workfront 管理者は、Workfront 環境を Adobe Admin Console に移行した後、新しいネイティブ統合を設定できます。 設定のヘルプについては、[Experience Manager Assets as a Cloud Service 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)を参照してください。

## 既存のアセットを Adobe Experience Manager Assets as a Cloud Service 統合のために Workfront に移動する

環境を設定したら、リンクされた既存のアセットとフォルダーを Adobe Experience Manager に移動できます。 これはオプションの手順ですが、従来のコネクタまたは拡張コネクタを使用して以前にリンクしたフォルダーとアセットに、コネクタをアンインストールした後も引き続きアクセスできるようにします。

アセットの移動について詳しくは、[リンクされたフォルダーとドキュメントの移行](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)を参照してください。

## 使用予定のすべての重要なユースケースの検証

従来のコネクタや拡張コネクタをアンインストールする前に、ネイティブ統合を通じて使用することを想定している重要なユースケースをすべて検証することが重要です。

## 従来のコネクタまたは拡張コネクタのアンインストール

最後に、従来のコネクタまたは拡張コネクタをアンインストールする必要があります。 ネイティブ統合は、いずれかのコネクタと併せて実行することを意図していません。

アンインストールについて詳しくは、以下を参照してください。

* 従来のコネクタのアンインストール手順：[Adobe Experience Manager の従来のコネクタを使用した Workfront のアンインストール](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md)
* 拡張コネクタのアンインストール手順：[Adobe Experience Manager の拡張コネクタを使用した Workfront のアンインストール](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md)
