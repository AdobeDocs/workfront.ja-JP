---
title: 2024 年第 1 四半期の統合の強化
description: 2024 年第 1 四半期の統合の強化
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0d581f3c-2aaf-4ac1-97a5-df1b01627080
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# 2024 年第 1 四半期の統合の強化

このページでは、2024 年第 1 四半期リリースのプレビュー環境に対する統合の機能強化について説明します。 これらの機能強化は、2024 年第 1 四半期リリースの実稼動環境で利用できるようになります。

2024 年第 1 四半期のリリースサイクルで現時点で使用可能なすべての変更のリストについては、 [2024 年第 1 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).

## Experience Manager Assets Essentials でのメタデータのマッピングで、が使用されるようになりました `xcm:keywords` の代わりに `dc:subject`

Experience Manager Assets Essentials の統合を更新し、Experience Manager Assets as a Cloud Service統合のエクスペリエンスに合わせました。 現在は、複数の 1 行テキストフィールドをExperience Manager Assetsの 1 つのフィールドにマッピングする際に、両方のサービスで `xcm:keywords` フィールドに入力します。

以前は、これらのフィールドは `dc:subject` フィールドを使用して、Experience Manager Assets Essentials にアクセスできます。 Experience Manager Assetsのas a Cloud Service機能は変更されていません。

現在マッピングされているExperience Manager Assets Essentials のメタデータ `dc:subject` は、に再マッピングする必要があります `xcm:keywords`.

メタデータのExperience Manager Assets Essentials へのマッピングについて詳しくは、 [AEMキーワード](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md#aem-keyword).

## Adobe Experience Manager統合で Typeahead フィールドを使用できるようになりました

WorkfrontとAdobe Experience Managerの間でフィールドを簡単にリンクできるように、メタデータマッピングに typeahead フィールドのサポートが追加されました。 これで、Adobe Experience Managerで typeahead フィールドを対応するフィールドにマッピングできるようになりました。

ユーザーがWorkfrontのフィールドに別の値を選択した場合、この変更はAdobe Experience Managerに直ちに反映されます。 また、フィールド値のオプションが変更された場合（チームが名前を新しい名前に変更するなど）、この変更はAdobe Experience Managerにも反映されます。

Adobe Experience Manager統合でのメタデータのマッピングに関する情報と手順については、 [メタデータの設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-metadata-optional).

## Adobe Experience Managerでのアセットの自動公開

Adobe Experience Manager統合に別のワークフローを追加しました。 これで、Adobe Experience Managerに送信する際に、アセットを自動的に公開するように設定できます。 統合は、Adobe Experience ManagerパブリッシュサービスまたはAdobe Experience Manager Brand Portal に公開するように設定できます。

自動公開ワークフローは、Adobe Experience Manager統合で有効にし、設定できます。 有効にすると、ワークフローはプロジェクトテンプレートまたはプロジェクトレベルで編集できます。

詳しくは、 [アセットの公開](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#publishing-assets) in [Experience Manager Assets統合でのワークフローの使用](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).
