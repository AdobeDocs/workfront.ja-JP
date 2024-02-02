---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 従来のコネクタから拡張コネクタへの移行
description: 次のプロセスでは、Adobe Experience Manager の従来のコネクタから、Adobe Workfront と AEM Assets を統合できる拡張コネクタに移行するためのベストプラクティスの概要を説明します。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: ht
source-wordcount: '347'
ht-degree: 100%

---

# 従来のコネクタから拡張コネクタへの移行

次のプロセスでは、Adobe Experience Manager の従来のコネクタから、Adobe Workfront と AEM Assets を統合できる拡張コネクタに移行するためのベストプラクティスの概要を説明します。

>[!IMPORTANT]
>
>このドキュメントは、Adobe Experience Manager Assets をオンプレミス環境またはマネージドサービス環境で使用しているお客様にのみ適用されます。


Adobe Experience Manager Assets as a Cloud Service をご利用のお客様は、従来のコネクタから Workfront 内の新しいネイティブ統合への移行パスが適用されます。この移行プロセスの詳細については、[従来のコネクタまたは拡張コネクタから Adobe Experience Manager as a Cloud Service の Workfront 統合への移行](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md)を参照してください。

## 拡張コネクタの実装

>[!IMPORTANT]
>
>拡張コネクタの実装には、認定パートナーまたは Adobe コンサルティングサービスが必要です。
>
> パートナーが拡張コネクタで認定を希望する場合は、[Workfront for Experience Manager 拡張コネクタエキスパートシリーズ](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=ja)の記事を参照してください。

拡張コネクタを実装するには、[Workfront for Experience Manager 拡張コネクタの設定](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=ja)を参照してください。


## 既存アセットの移動

環境を設定したら、リンクされた既存のアセットとフォルダーを Adobe Experience Manager に移動できます。これはオプションの手順ですが、従来のコネクタをアンインストールした後も、従来のコネクタを介して以前にリンクされたフォルダーとアセットに引き続きアクセスできます。

アセットの移動について詳しくは、[リンクされたフォルダーとドキュメントの移行](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md)を参照してください。

## 使用予定のすべての重要なユースケースの検証

従来のコネクタをアンインストールする前に、拡張コネクタを介して使用する予定の重要なユースケースをすべて検証することが重要です。

## 従来のコネクターのアンインストール

最後に、従来のコネクタをアンインストールする必要があります。従来のコネクタは、拡張コネクタと併用することはできません。

アンインストールするには、[Adobe Experience Manager レガシーコネクタを使用した Workfront のアンインストール](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md)を参照してください。
