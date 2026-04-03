---
title: 2025年第3四半期プルーフとドキュメント管理の機能強化
description: 2025年第3四半期プルーフとドキュメント管理の機能強化
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4829d487-7041-447f-9a68-fb1acf467734
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 10%

---

# 2025年第3四半期プルーフとドキュメント管理の機能強化

このページでは、2025年第3四半期リリースでプレビュー環境に加えられたすべてのドキュメント管理の機能強化について説明します。 これらの機能強化は、前述のように本番環境で利用できるようになります。

2025年第3四半期のリリースサイクルで現時点で利用可能なすべての変更のリストについては、[2025年第3四半期のリリースの概要](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md)を参照してください。


## 統合承認の段階的な展開

>[!NOTE]
>
>お客様向け実稼動リリース：2025年7月17日から段階的に展開


「新しいドキュメントの承認」と呼ばれる統合承認を、段階的に展開しています。 この機能は、今後6か月間、Workfront インスタンスで自動的に有効になります。

統合承認は、従来の文書の承認に代わるもので、次の機能を文書に直接提供します。

* Workfront チーム全体をレビューアーまたは承認者に指定します
* レビューまたは承認の期限を設定する
* 承認テンプレートの作成と再利用
* 新しいバージョンの活用
* Workfrontのホームウィジェットで、承認の複数の主要業績評価指標を表示します
* Canvas ダッシュボードを使用して、統合承認に関するレポートの詳細を表示する

詳しくは、[統合承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)を参照してください。

## デスクトップ校正ビューアの更新

>[!NOTE]
>
>* すべてのお客様向けの本番リリース： 2025年6月16日（PT）

デスクトップ校正ビューアがバージョン 2.1.50に更新されました。

このアップデートには内部ツールのアップデートが含まれており、エンドユーザーの機能には影響しません。

このアップデートは、Mac と Windows の両方に対応しています。

## 新しいプルーフとGenStudio for Performance Marketingの統合

>[!NOTE]
>
>* すべてのお客様向けの本番リリース： 2025年6月12日（PT）

「プルーフとGenStudio for Performance Marketingを新たに連携します。 この統合により、次のことができるようになります。

* Workfrontの承認テンプレートを使用して、承認ワークフローを定義します

* Workfront プルーフビューアでのドラフトコンテンツのレビュー

* GenStudio for Performance Marketingでの最終承認と公開については、レビューの決定を参照してください

### 統合要件

Workfront と GenStudio for Performance Marketing は、同じ IMS 組織にデプロイする必要があります。

詳しくは、[GenStudio for Performance MarketingとWorkfront Proofの統合の基本を学ぶ](/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-genstudio.md)を参照してください。

## デスクトップ校正ビューアの更新

デスクトップ校正ビューアがバージョン 2.1.48に更新されました。

このアップデートは、Desktop ViewerとMac オペレーティングシステムの互換性を維持するための問題の修正です。 Electronは34.4.0、Chromiumは132に格下げされた。

このアップデートは、Mac と Windows の両方に対応しています。


## リンクされたGoogle フォルダー内のAssetsを個別に追加して、Workfrontに表示する必要があります

>[!NOTE]
>
>* プレビューリリース：2025年6月2日（PT）、すべての顧客向けの実稼動版リリース：2025年6月2日（PT）

Googleは、Google Driveにアクセスするサードパーティ製アプリケーションのセキュリティ制御を[強化します](https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps)。そのため、アプリケーションではユーザーごとの同意モデルを採用する必要があります。 そのため、Workfrontで表示するには、個々のアセットを一度に1つずつリンクする必要があります。 詳しくは、[&#x200B; ドキュメント統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md)を参照してください。

変更されない主な機能：

* Google Drive モーダル内からアセットとフォルダーを検索してフィルタリングします
* Google DriveからWorkfront オブジェクトへのアセットのリンク
* ドキュメントページの「送信先」ドロップダウンからGoogle ドライブにアセットをアップロードします
* ユーザーのマイドライブ領域でのフォルダー構造の表示とアクセス
* Google ドライブからWorkfrontの既存のドキュメントに新しいバージョンのアセットをリンクする
* Google ドライブからWorkfront オブジェクトへのフォルダーのリンク
* リンクされたフォルダーにドキュメントをドラッグ&amp;ドロップして、Google ドライブにアセットをアップロードする
* Workfront内から新しいGoogle Drive ドキュメントを作成する


## プルーフビューアで使用できる新しいドキュメント承認決定ボタン

>[!IMPORTANT]
>
>この機能は段階的リリースの一部であり、特定のお客様のみが利用できます。

>[!NOTE]
>
>* プレビューリリース：2025年4月10日（PT）、実稼動リリース：すべてのユーザー：2025年4月17日（PT）

新しいドキュメント承認決定ボタンがプルーフビューアに表示されるようになりました。 これで、簡単なプルーフを作成し、ドキュメントの概要から承認者とレビュー担当者を追加すると、プルーフビューア内で直接決定を行うことができます。

以前は、プルーフビューアを終了して決定を下す必要がありました。

このリリースより前に作成された承認では、プルーフビューアにボタンが表示されません。

詳しくは、[新しいドキュメントの承認とプルーフの併用](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)を参照してください。
