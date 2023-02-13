---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 従来のコネクタから拡張コネクタへの移行
description: Adobe WorkfrontとAEM Assetsを統合するための、Adobe Experience Manager従来のコネクタを拡張コネクタに移行する際のベストプラクティスの概要を次に示します。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4a8d1e2b-9744-4f72-a337-5057448db4fb
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 従来のコネクタから拡張コネクタへの移行

Adobe WorkfrontとAEM Assetsを統合するための、Adobe Experience Manager従来のコネクタを拡張コネクタに移行する際のベストプラクティスの概要を次に示します。

>[!IMPORTANT]
>
>このドキュメントは、Adobe Experience Manager Assets オンプレミスまたはManaged Services環境を使用するお客様にのみ適用されます。


Adobe Experience Manager Assetsas a Cloud Serviceのお客様の場合、従来のコネクタからWorkfront内の新しいネイティブ統合への移行パスが使用されます。 この移行プロセスの詳細については、 [従来のまたは拡張されたコネクタからWorkfrontへのAdobe Experience Manager as a Cloud Service統合用の移行](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/migrate-from-legacy-enhanced-connectors.md).

## 拡張コネクタの実装

>[!IMPORTANT]
>
>拡張コネクタの実装には、認定済みのパートナーまたはAdobeコンサルティングサービスが必要です。
>
> パートナーが拡張コネクタで認定を希望する場合は、次の記事を参照してください。 [Workfront forExperience Manager強化コネクタ Expert シリーズ](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/workfront/enhanced-connector/aem-experts-series/overview.html?lang=en).

拡張コネクタを実装するには、 [Workfront forExperience Manager拡張コネクタの設定](https://experienceleague.adobe.com/docs/experience-manager-65/assets/integrations/workfront-connector-configure.html?lang=en).


## 既存のアセットの移動

環境を設定したら、リンクされた既存のアセットおよびフォルダーをAdobe Experience Managerに移動できます。 これはオプションの手順ですが、従来のコネクタをアンインストールした後も、従来のコネクタを介して以前にリンクされたフォルダーとアセットに引き続きアクセスできるようにします。

アセットの移動について詳しくは、 [リンクされたフォルダとドキュメントを移行する](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/workfront-document-link-updates.md).

## 使用を意図したすべての重要な使用例を検証

従来のコネクタをアンインストールする前に、拡張コネクタを通じて使用することを想定している重要な使用例をすべて検証することが重要です。

## 従来のコネクタのアンインストール

最後に、従来のコネクタをアンインストールする必要があります。 従来のコネクタは、拡張コネクタと並行して実行することを意図していません。

アンインストールするには、 [Adobe Experience ManagerレガシーコネクタでのWorkfrontのアンインストール](/help/quicksilver/documents/workfront-and-experience-manager-integrations/legacy-enhanced-connector-migration/uninstall-legacy-connector.md).
