---
title: 23.3 統合の強化
description: 23.3 統合の強化
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d24ddc8a-fe96-4e9b-8186-0b54ab9ab213
TQID: https://experienceleague.adobe.com/dbwl44iOJoBWysGDsJYaFmjdMqoo-wL5sHiRxNqc4qQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: bbf3fe51-0066-4980-9062-f8005585ee10
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 700
ht-degree: 86%

---

# 23.3 統合の強化

このページでは、23.3 リリースで行われたすべての統合の機能強化について説明します。 これらの機能強化は、2023年7月20日（PT）および 2023年7月21日（PT）の 23.3 リリースで本番環境で使用可能になりました。

23.3 リリースサイクルのこの時点で使用可能なすべての変更点のリストについて詳しくは、[23.3 リリースの概要](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md)を参照してください。

## Google Workspaceの新しい統合機能が利用可能になりました

Google Workspaceの新しい統合機能が、Google Marketplaceで利用できるようになりました。 新しい統合は OAuth2 を使用して認証され、以前の統合から置き換わります。

以前のGoogle Workspace統合は非推奨（廃止予定）となり、自動的にアンインストールされます。

新しい統合のインストール方法については、[インストール [!DNL Adobe Workfront for Google Workspace]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)を参照してください。

Google Workspace用Workfrontについて詳しくは、[Google Workspace用Workfront](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md)を参照してください。

## Adobe Creative Cloud 統合で、複数の割り当て済みユーザーをサポートするようになりました。

Adobe Creative Cloud 統合では、タスクまたはイシューに複数のユーザーが割り当てられている場合に「担当部分は完了」と「完了」（または「解決済み」）のどちらかを選択できるようになりました。

以前は、統合により、「自分の担当部分を完了」または「完了」／「解決済み」を指定せずに、タスクを完了済みとしてマークできました。

この機能を活用するには、Creative Cloud プラグイン用の最新の Workfront をダウンロードしてインストールします。

この機能について詳しくは、[Adobe Workfront プラグインを使用して作業アイテムを完了とマーク](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md)を参照してください。

Creative Cloud プラグイン用の Workfront のインストールについて詳しくは、[Creative Cloud アプリケーション用 Adobe Workfront プラグインをインストール](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md)を参照してください。

## Creative Cloud プラグイン用 Workfront からの Workfront 通知を表示および管理する

必要な通知を簡単に受け取れるように、Adobe Creative Cloud を離れることなく、Workfront 通知を表示および管理できるようになりました。 これで、Creative Cloud アプリケーション内の Workfront プラグインウィンドウから直接、通知を表示したり、これらの通知に関連する作業アイテムやコメントにアクセスしたりできるようになりました。

以前は、Workfront 内およびメール経由でのみ通知を使用できました。

この機能を活用するには、Creative Cloud プラグイン用の最新の Workfront をダウンロードしてインストールします。

詳しくは、[Adobe Creative Cloudから  [!DNL Adobe Workfront]  通知を表示および管理](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md)を参照してください。

Creative Cloud プラグイン用の Workfront のインストールについて詳しくは、[Creative Cloud アプリケーション用 Adobe Workfront プラグインをインストール](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md)を参照してください。

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## プロジェクトの作成時に Adobe Experience Manager Assets にリンクされたフォルダーを自動的に作成する

Adobe Experience Manager 統合用の新しい「リンクされたフォルダーを作成ワークフロー」を使用して、Adobe Experience Manager Assets フォルダーのパスで統合を設定できます。 統合がプロジェクトテンプレートに追加されると、そのテンプレートから作成されたプロジェクトによって、指定したフォルダー内の Experience Manager Assets 内にリンクされたサブフォルダーが自動的に作成されます。

以前は、リンクされたフォルダーを作成するには、ユーザー側でアクションが必要でした。

この機能は、Workfront 内の Adobe Experience Manager as a Cloud Service 統合でのみ使用できます。 これは、Adobe Experience Manager 拡張コネクタでは使用できません。

詳しくは、[Experience Manager Assets 統合でワークフローを使用](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md)を参照してください。

## Experience Manager Assets で Workfront フィールド値をタグにマッピングする

これで、Workfront のデータに基づき、アセットを分類してすばやく見つけられるようになりました。 Experience Manager Assets の統合で、Workfront でこのデータをメタデータ設定の一部としてマッピングできます。

以前は、Workfront データを Experience Manager Assets タグにマッピングすることはできませんでした。

Experience Manager Assets as a Cloud Serviceのこの機能について詳しくは、[Experience Manager Assets as a Cloud Service]統合(/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)の設定を参照してください。
Experience Manager Assets Essentialsのこの機能について詳しくは、[Experience Manager Assets Essentials統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)を参照してください。

## Workfront フィールドをカスタム Experience Manager Assets メタデータフィールドにマッピングする

ネイティブ統合により、ネイティブとビルトインの Workfront フィールドの両方を、Experience Manager Assets as a Cloud Service のカスタムメタデータスキーマフィールドにマッピングできるようになりました。

Experience Manager Assets as a Cloud Serviceのこの機能について詳しくは、[Experience Manager Assets as a Cloud Service]統合(/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)の設定を参照してください。
Experience Manager Assets Essentialsのこの機能について詳しくは、[Experience Manager Assets Essentials統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)を参照してください。

## Creative Cloud 向け Adobe Workfront を使用して自動プルーフワークフローテンプレート設定を調整する

既存の自動ワークフローテンプレート設定を Creative Cloud で直接調整できるようになりました。 既存の自動ワークフローテンプレートを選択すると、次の操作を実行できます。

* ステージの無効化
* 受信者を追加する
* プルーフの役割を変更する
* 期限を調整する
* メール通知を更新する
* その他

詳しくは、[&#x200B; [!DNL Creative Cloud]  アプリケーション用  [!DNL Adobe Workfront]  プラグインを使用してドキュメントとプルーフをアップロード](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md)を参照してください。

以下の機能強化は、次の Creative Cloud アプリで利用できます。

* Photoshop
* XD
* InDesign
* Illustrator
