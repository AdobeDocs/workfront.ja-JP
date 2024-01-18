---
title: 22.3 統合の強化
description: 22.3 統合の強化
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: caaef6a2-a554-4a2c-a86d-df3f19a4f40c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# 22.3 統合の強化

このページでは、プレビュー環境の 2.3 リリースでおこなわれた統合の機能強化について説明します。 これらの機能強化は、2022 年 7 月 11 日の週の 2022 年 1 月に実稼動環境で利用可能になる予定です。 22.3 リリースで使用可能なすべての変更点の一覧については、 [22.3 リリースの概要](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Adobe Workfront for Experience Manager Assetsの統合

Adobe Workfront Experience Manager Assetsの統合がCloud Service可能になりました。

また、Cloud ServiceとAssets Essentialsの両方に新しい機能が導入されました。この統合により、ユーザーは次の操作を実行できます。

* Workfront内から、リンクされたAEMフォルダーを自動的に作成する

* 既にリンクされているアセットのメタデータの更新をWorkfrontからAEMにプッシュします

* Workfront内の最新のAEMメタデータをリアルタイムで表示


この統合を使用するには、WorkfrontとAdobe Experience Manager Assets、またはAssets EssentialsがAdobe Admin Consoleの組織 ID に関連付けられている必要があります。 詳細については、Adobeの営業担当者にお問い合わせください。

統合の設定について詳しくは、

* [Experience Manager Assets as a Cloud Service統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)

* [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)


統合の使用について詳しくは、 Adobe Workfront for Experience Manager Assets Essentials を参照してください。

## 新しいSharePoint(Graph API) 統合が利用できるようになりました

よりシンプルな新しいSharePoint統合を作成しました。 今は、SharePoint統合を設定する必要はありません。 代わりに、新しいSharePoint統合は、他のドキュメント統合と同様に、単に選択できるオプションです。

従来のSharePoint統合を通じて現在リンクされているドキュメントへのアクセス権は失われません。 ただし、従来の統合を通じて新しいドキュメントをリンクすることはできません。

Workfront管理者は、組織のニーズに応じて、SharePointと従来のSharePointの統合を別々に有効化および無効化できます。

詳しくは、 [レガシーSharePoint統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

## 複数のファイルを 1 つの配達確認でCreative Cloudプラグインで結合

Workfrontで複数ファイルの配達確認を作成するために、Adobe Workfrontで作成したコンテンツを使用して、外部のファイルをアップロードできるようになりました。 外部のファイルは、Workfront内に追加の配達確認ページとして表示されます。 この機能強化により、配達確認作成エクスペリエンスのルックアンドフィールも更新しました。

詳しくは、

* [Adobe Photoshopから配達確認をアップロード](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-proofs-ps.md)

* [XDアートボードを配達確認としてWorkfrontにアップロード](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-proofs.md)
