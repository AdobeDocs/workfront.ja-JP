---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 従来のコネクタまたは拡張コネクタから Adobe Experience Manager as a Cloud Service 統合向け Workfront への移行
description: このページでは、Workfront for Experience Cloud の拡張コネクタまたは従来のコネクタから、Workfront と Adobe Experience Manager Assets as a Cloud Service を接続する最新のネイティブ統合に移行するためのベストプラクティスについて説明します。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: ht
source-wordcount: '502'
ht-degree: 100%

---

# 従来のコネクタまたは拡張コネクタから Adobe Experience Manager as a Cloud Service 統合向け Workfront への移行

このページでは、Workfront for Experience Cloud の拡張コネクタまたは従来のコネクタから、Workfront と Adobe Experience Manager Assets as a Cloud Service を接続する最新のネイティブ統合に移行するためのベストプラクティスについて説明します。

>[!IMPORTANT]
>
>この情報は、Adobe Experience Manager Assets オンプレミスまたは Managed Services 環境を使用しているお客様には適用されません。

## Workfront インスタンスを Admin Console に移動する

Workfront と Adobe Experience Manager Assetsas a Cloud Service の間で新しいネイティブ統合を使用するお客様は、Workfront 環境が Adobe Admin Console に結び付けられていることを確認する必要があります。既存の Workfront 環境の場合、接続済みの Adobe Admin Console に環境を移行する必要が生じる可能性があります。この移行と関連するチェックリストについて詳しくは、[組織の Adobe Admin Console 導入の準備](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)を参照してください。

アドビは、この移行を支援する必要があります。サポートをリクエストするには、次のいずれかを行います。

* Workfront Hub にアクセスできる場合は、[Workfront の Adobe Admin Console への移行](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=)へリクエストを送信します。
* Workfront Hub へのアクセスできない場合は、[Workfront から Adobe Admin Console への早期移行リクエストキュー](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi)へリクエストを送信します。

## 新しい Workfront を Adobe Experience Manager Assets as a Cloud Service 統合のために設定する

Workfront 管理者は、Workfront 環境を Adobe Admin Console に移行した後、新しいネイティブ統合を設定できます。設定のヘルプについては、[Experience Manager Assets as a Cloud Service 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)を参照してください。

## 既存のアセットを Adobe Experience Manager Assets as a Cloud Service 統合のために Workfront に移動する

環境を設定したら、リンクされた既存のアセットとフォルダーを Adobe Experience Manager に移動できます。これはオプションの手順ですが、従来のコネクタまたは拡張コネクタを使用して以前にリンクしたフォルダーとアセットに、コネクタをアンインストールした後も引き続きアクセスできるようにします。

アセットの移動について詳しくは、[リンクされたフォルダーとドキュメントの移行](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)を参照してください。

## 使用予定のすべての重要なユースケースの検証

従来のコネクタや拡張コネクタをアンインストールする前に、ネイティブ統合を通じて使用することを想定している重要なユースケースをすべて検証することが重要です。

## 従来のコネクタまたは拡張コネクタのアンインストール

最後に、従来のコネクタまたは拡張コネクタをアンインストールする必要があります。ネイティブ統合は、いずれかのコネクタと併せて実行することを意図していません。

アンインストールについて詳しくは、以下を参照してください。

* 従来のコネクタのアンインストール手順：[Adobe Experience Manager の従来のコネクタを使用した Workfront のアンインストール](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md)
* 拡張コネクタのアンインストール手順：[Adobe Experience Manager の拡張コネクタを使用した Workfront のアンインストール](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md)
