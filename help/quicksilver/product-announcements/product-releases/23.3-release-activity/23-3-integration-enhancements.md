---
title: 23.3 統合の強化
description: 23.3 統合の強化
author: Lisa
feature: Product Announcements
source-git-commit: d8420930738102e64fbab2eecf91f2eb4429cb0e
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 0%

---

# 23.3 統合の強化

このページでは、プレビュー環境の 23.3 リリースでおこなわれたすべての統合の機能強化について説明します。 これらの機能強化は、23.3 リリースで実稼動環境で利用できるようになります。

23.3 リリースサイクルのこの時点で使用可能なすべての変更点のリストについては、 [23.3 リリースの概要](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## 新しい G Suite 統合が利用可能になりました

Google Marketplace で新しい G Suite 統合が利用できるようになりました。 新しい統合は、OAuth2 を使用して認証され、以前の統合に代わるものです。

以前の G Suite 統合は廃止され、自動的にアンインストールされます。

新しい統合のインストール方法については、 [インストール [!DNL Adobe Workfront for G Suite]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Workfront for G Suite について詳しくは、 [Workfront for G Suite](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Adobe Creative Cloud統合で、複数の割り当て済みユーザーをサポートするようになりました

Adobe Creative Cloud統合では、タスクまたはイシューに複数のユーザーが割り当てられている場合に、「自分の部分で完了」と「完了」（または「解決済み」）のどちらかを選択できるようになりました。

以前は、統合により、「自分の部分で完了」または「完了」/「解決済み」を指定せずに、タスクを完了済みとしてマークできました。

この機能を活用するには、Creative Cloudプラグイン用の最新のWorkfrontをダウンロードしてインストールします。

この機能について詳しくは、 [Adobe Workfrontプラグインを使用して作業項目を完了とマーク](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Creative Cloudプラグイン用のWorkfrontのインストールについて詳しくは、 [Adobe WorkfrontプラグインのCreative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## WorkfrontからのWorkfront通知のCreative Cloudプラグインの表示と管理

必要な通知を簡単に受け取れるように、Adobe Creative Cloudを離れることなく、Workfront通知を表示および管理できるようにしました。 これで、Creative Cloudアプリケーション内のWorkfrontプラグインウィンドウから直接、通知を表示し、これらの通知に関連する作業項目やコメントにアクセスできるようになりました。

以前は、Workfront内および E メール経由でのみ通知を使用できました。

この機能を活用するには、Creative Cloudプラグイン用の最新のWorkfrontをダウンロードしてインストールします。

詳しくは、 [表示と管理 [!DNL Adobe Workfront] Adobe Creative Cloudからの通知](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Creative Cloudプラグイン用のWorkfrontのインストールについて詳しくは、 [Adobe WorkfrontプラグインのCreative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## ドラッグ&amp;ドロップでリンクされたフォルダーにドキュメントを移動する際のエクスペリエンスを向上

ドキュメントをリンクされたフォルダーにドラッグ&amp;ドロップするプロセスに、いくつかの透明性が追加されました。 これで、リンクされたフォルダに移動したドキュメントは、完全に移動されるまでドキュメントリストに残ります。 ドキュメントのオプションは無効ですが、ドキュメントの移動中にドキュメントを開いて表示することはできます。 ドキュメントはリンクされたフォルダ内に完全に配置されるので、ドキュメントの転送が完了すると、ドキュメントリストから消えます。

以前は、ドキュメントは、リンクされたフォルダーへの移動が完了する前に、ドキュメントリストから直ちに消えていました。

詳しくは、 [外部アプリケーションからドキュメントをリンク](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## プロジェクトの作成時に、Adobe Experience Manager Assets にリンクされたフォルダーを自動的に作成する

Adobe Experience Manager統合用の新しいリンクされたフォルダーを作成ワークフローを使用して、Adobe Experience Manager Assets フォルダーのパスで統合を設定できます。 統合がプロジェクトテンプレートに追加されると、そのテンプレートから作成されたプロジェクトによって、指定したフォルダー内にExperience Manager Assets内にリンクされたサブフォルダーが自動的に作成されます。

以前は、リンクされたフォルダーを作成するには、ユーザー側でアクションが必要でした。

この機能は、Workfront内のAdobe Experience Manager as a Cloud Service統合でのみ使用できます。 これは、Adobe Experience Manager拡張コネクタでは使用できません。

詳しくは、 [Experience Manager Assets統合でのワークフローの使用](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Workfrontフィールド値のExperience Manager Assetsでのタグへのマッピング

これで、Workfrontのデータに基づいて、アセットを分類してすばやく見つけることができるようになりました。 WorkfrontとExperience Manager Assetsの統合で、このデータをメタデータ設定の一部としてマッピングできます。

以前は、WorkfrontデータをExperience Manager Assetsタグにマッピングすることはできませんでした。

Experience Manager Assets as a Cloud Serviceのこの機能について詳しくは、 [の設定 [!UICONTROL Experience Manager Assetsas a Cloud Service] 統合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Experience Manager Assets Essentials のこの機能について詳しくは、 [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## WorkfrontフィールドをカスタムExperience Manager Assetsメタデータフィールドにマッピングする

ネイティブ統合により、ネイティブと組み込みのWorkfrontフィールドの両方を、Experience Manager Assets as a Cloud Serviceのカスタムメタデータスキーマフィールドにマッピングできるようになりました。

Experience Manager Assets as a Cloud Serviceのこの機能について詳しくは、 [の設定 [!UICONTROL Experience Manager Assetsas a Cloud Service] 統合](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Experience Manager Assets Essentials のこの機能について詳しくは、 [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Creative CloudにAdobe Workfrontを使用して自動配達確認ワークフローテンプレート設定を調整

既存の自動ワークフローテンプレート設定をCreative Cloudで直接調整できるようになりました。 既存の自動ワークフローテンプレートを選択すると、次の操作を実行できます。

* ステージの無効化
* 受信者を追加
* 配達確認の役割を変更
* 期限を調整
* 電子メール通知を更新
* その他！

詳しくは、 [でドキュメントと配達確認をアップロード [!DNL Adobe Workfront] プラグイン [!DNL Creative Cloud] アプリ](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

以下の機能強化は、次のCreative Cloudアプリで利用できます。

* Photoshop
* XD
* InDesign
* Illustrator
