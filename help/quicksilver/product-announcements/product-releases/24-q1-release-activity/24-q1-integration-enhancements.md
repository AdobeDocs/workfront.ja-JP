---
title: 2024年第 1 四半期の統合の機能強化
description: 2024年第 1 四半期の統合の機能強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
TQID: https://experienceleague.adobe.com/ZPt9H-R2eSNNha-gjfwkgnUOQqvU5tzAQPE5fMA-9uA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 385
ht-degree: 100%

---

# 2024年第 1 四半期の統合の機能強化

このページでは、プレビュー環境の 2024年第 1 四半期リリースで行われた統合の機能強化について説明します。 この機能強化は、2024年第 1 四半期のリリースにおいて本番環境で利用できるようになります。

2024年第 1 四半期リリースサイクルの現時点で利用可能なすべての変更のリストについて詳しくは、[2024年第 1 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md)を参照してください。

## Experience Manager Assets Essentials でのメタデータのマッピングで、`dc:subject` の代わりに `xcm:keywords` が使用されるようになりました。

Experience Manager Assets Essentials の統合を更新し、Experience Manager Assets as a Cloud Service 統合のエクスペリエンスに合わせました。 複数の 1 行テキストフィールドを Experience Manager Assets の 1 つのフィールドにマッピングする際に、両方のサービスで `xcm:keywords` フィールドを使用するようになりました。

以前は、これらのフィールドは Experience Manager Assets Essentials の `dc:subject` フィールドにマッピングされていました。 Experience Manager Assets as a Cloud Service の機能は変更されていません。

現在 `dc:subject` にマッピングされている Experience Manager Assets Essentials のメタデータは、`xcm:keywords` にマッピングし直す必要があります。

Experience Manager Assets Essentials へのメタデータのマッピングについて詳しくは、[AEM キーワード](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword)を参照してください。

## Adobe Experience Manager 統合で先行入力フィールドを使用できるようになりました。

Workfront と Adobe Experience Manager の間でフィールドを簡単にリンクできるように、メタデータマッピングにおける先行入力フィールドへのサポートが追加されました。 これで、Adobe Experience Manager の対応するフィールドに先行入力フィールドをマッピングできるようになりました。

ユーザーが Workfront のフィールドに別の値を選択した場合、この変更は Adobe Experience Manager に直ちに反映されます。 また、フィールド値のオプションが変更された場合（チーム名を新しい名前に変更するなど）、この変更は Adobe Experience Manager にも反映されます。

Adobe Experience Manager 統合でのメタデータのマッピングに関する情報と手順について詳しくは、[メタデータの設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional)を参照してください。

## Adobe Experience Manager のアセットの自動公開

Adobe Experience Manager 統合に別のワークフローを追加しました。 これで、Adobe Experience Manager に送信する際に、アセットを自動的に公開するように設定できます。 統合は、Adobe Experience Manager パブリッシュサービスまたは Adobe Experience Manager Brand Portal に公開するように設定できます。

Adobe Experience Manager 統合で自動公開ワークフローを有効にして設定できます。 有効にすると、ワークフローはプロジェクトテンプレートまたはプロジェクトレベルで編集できます。

詳しくは、[Experience Manager Assets 統合でのワークフローの使用](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md)の[アセットの公開](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets)を参照してください。
