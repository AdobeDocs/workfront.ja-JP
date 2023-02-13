---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 従来のまたは拡張されたコネクタからWorkfrontへのAdobe Experience Manager as a Cloud Service統合用の移行
description: このページでは、WorkfrontとAdobe Experience Manager Assetsas a Cloud ServiceのExperience Cloudを接続する最新のネイティブ統合に、拡張または従来のコネクタをWorkfrontから移行する際のベストプラクティスについて説明します。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: af14f408-df39-473c-9e18-bb88022c96ed
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# 従来のまたは拡張されたコネクタからWorkfrontへのAdobe Experience Manager as a Cloud Service統合用の移行

このページでは、WorkfrontとAdobe Experience Manager Assetsas a Cloud ServiceのExperience Cloudを接続する最新のネイティブ統合に、拡張または従来のコネクタをWorkfrontから移行する際のベストプラクティスについて説明します。

>[!IMPORTANT]
>
>この情報は、Adobe Experience Manager Assets オンプレミスまたはManaged Services環境を使用しているお客様には適用されません。

## WorkfrontインスタンスをAdmin Consoleに移動

WorkfrontとAdobe Experience Manager Assetsas a Cloud Serviceの新しいネイティブ統合を使用するお客様は、Workfront環境がAdobe Admin Consoleに結び付けられていることを確認する必要があります。 既存のWorkfront環境の場合、接続されているAdobe Admin Consoleに環境を移行する必要が生じる可能性があります。 この移行と関連するチェックリストについて詳しくは、 [組織をAdobe Admin Consoleにオンボーディングする準備](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md).

Adobeは、この移行の実行に役立つ必要があります。 ヘルプをリクエストするには、次のいずれかの操作を行います。

* Workfront Hub にアクセスできる場合は、 [Adobe Admin ConsoleへのWorkfront移行](https://hub.workfront.com/requests/new?activeTab=tab-new-helpRequest&amp;projectID=629674d500054a38133cf26e01d06a97&amp;path=).
* Workfront Hub へのアクセス権がない場合は、 [WorkfrontからAdobe Admin Consoleへの早期移行リクエストキュー](https://workfront.az1.qualtrics.com/jfe/form/SV_9T5LuHf05JUOPAi).

## 新しいWorkfrontをAdobe Experience Manager Assetsas a Cloud Service統合用に設定

Workfront環境をAdobe Admin Consoleに移行した後、Workfrontの管理者は、新しいネイティブ統合を設定できます。 設定のヘルプについては、 [Experience Manager Assets統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## 既存のアセットをWorkfrontに移動して、Adobe Experience Manager Assetsas a Cloud Service統合を実行する

環境を設定したら、リンクされた既存のアセットおよびフォルダーをAdobe Experience Managerに移動できます。 これはオプションの手順ですが、従来のコネクタまたは拡張コネクタを使用して以前にリンクしたフォルダーとアセットを、コネクタをアンインストールした後も引き続きアクセスできるようにします。

アセットの移動について詳しくは、 [リンクされたフォルダとドキュメントを移行する](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## 使用を意図したすべての重要な使用例を検証

従来のコネクタや拡張コネクタをアンインストールする前に、ネイティブ統合を通じて使用することを想定している重要な使用例をすべて検証することが重要です。

## 従来のコネクタまたは拡張コネクタのアンインストール

最後に、従来のコネクタまたは拡張コネクタをアンインストールする必要があります。 ネイティブ統合は、どちらのコネクタとも並行して実行することを意図していません。

アンインストールするには、

* 従来のコネクタのアンインストール手順： [Adobe Experience ManagerレガシーコネクタでのWorkfrontのアンインストール](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
* コネクタのアンインストール手順の強化： [Adobe Experience Manager拡張コネクタ付きWorkfrontのアンインストール](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-enhanced-connector.md).
