---
title: 2025 年第 3 四半期のプルーフとドキュメント管理の機能強化
description: 2025 年第 3 四半期のプルーフとドキュメント管理の機能強化
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4829d487-7041-447f-9a68-fb1acf467734
source-git-commit: 9948927b4f61e0bafd815951bfaede0da064ef91
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 3%

---

# 2025 年第 3 四半期のプルーフとドキュメント管理の機能強化

このページでは、2025 年第 3 四半期リリースで行われた、プレビュー環境に対するすべてのドキュメント管理の機能強化について説明します。 これらの機能強化は、前述のように実稼動環境で利用できるようになります。

2025 年第 3 四半期のリリースサイクルのこの時点で利用できるすべての変更のリストについては、[2025 年第 3 四半期のリリースの概要 ](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md) を参照してください。

<!--## Adobe Express and Workfront Proof integration

We are excited to announce a new integration between Adobe Express and Workfront Proof.

With this integration, you can 

* Streamline collaboration between creative, legal, and compliance teams to reduce time-to-publish while maintaining oversight  

* Conduct for deep reviews using drawing markups, annotations, and commenting with the Workfront proofing viewer 

* Meet enterprise compliance standards with electronic signatures and full audit logs 

* Require approval on any remixed files from an Express branded template  

* Map an Express template to a multi-stage review and approval workflow using advanced proof templates

Note: The integration must be enabled for your accounts by the Adobe Product Team.

For more information, see [Get started with the Adobe Express and Workfront Proof integration](/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-express.md).
-->

## 統合承認の段階的なロールアウト

>[!NOTE]
>
>お客様向けの実稼動リリース：2025 年 7 月 17 日（PT）から段階的にロールアウトを開始


以前は新規ドキュメント承認と呼ばれていた統合承認を、段階的にロールアウトして有効にしています。 この機能は、今後 6 か月間にWorkfront インスタンスで自動的に有効になります。

統合承認は、従来のドキュメント承認に代わるもので、ドキュメントに直接次の機能を提供します。

* レビュアーまたは承認者として、Workfront チーム全体を指定します
* レビューまたは承認の期限を設定
* 承認テンプレートの作成と再利用
* 新しいバージョンの使用
* Workfrontのホームウィジェットで、承認に関する複数の主要業績評価指標を表示します
* キャンバスダッシュボードを使用すると、統合承認に関するレポートの詳細を表示できます

詳しくは、[ 統合承認の概要 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md) を参照してください。

## デスクトッププルーフビューアの更新

>[!NOTE]
>
>* すべてのお客様向けの本番リリース： 2025年6月16日（PT）

デスクトッププルーフビューアがバージョン 2.1.50 に更新されました。

この更新には、内部ツールの更新が含まれており、エンドユーザーの機能には影響しません。

このアップデートは、Macと Windows の両方に対応しています。

## 新規プルーフとGenStudio for Performance Marketingの統合

>[!NOTE]
>
>* すべてのお客様向けの本番リリース： 2025年6月12日（PT）

プルーフとGenStudio for Performance Marketingの新しい統合を導入できることを非常に嬉しく思います。 この統合を使用すると、次のことができます

* Workfront承認テンプレートを使用した承認ワークフローの定義

* Workfront プルーフビューアでのドラフトコンテンツのレビュー

* GenStudio for Performance Marketingでの最終承認と公開に関する決定のレビューを参照してください

### 統合要件

WorkfrontとGenStudio for Performance Marketingは、同じ IMS 組織にデプロイする必要があります。

詳しくは、[GenStudio for Performance MarketingとWorkfront Proofの統合の基本を学ぶ ](/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-genstudio.md) を参照してください。

## デスクトッププルーフビューアの更新

デスクトッププルーフビューアがバージョン 2.1.48 に更新されました。

このアップデートは、デスクトップビューアとMac オペレーティングシステムとの互換性を維持するための問題修正です。 電子は 34.4.0 に、クロムは 132 にダウングレードされた。

このアップデートは、Macと Windows の両方に対応しています。


## リンクされたGoogle フォルダー内のAssetsがWorkfrontに表示されるようにするには、そのを個別に追加する必要があります

>[!NOTE]
>
>* プレビューリリース：2025 年 6 月 2 日（PT）、すべてのお客様向けの実稼動リリース：2025 年 6 月 2 日（PT）

Googleは、Google Drive にアクセスするサードパーティアプリケーション向けに [ セキュリティ制御の強化 ](https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps) を行っており、アプリケーションにはユーザーごとの同意モデルを採用する必要があります。 その結果、Workfrontに表示するには、個々のアセットを 1 つずつリンクする必要があります。 詳しくは、[ ドキュメント統合の設定 ](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md) を参照してください。

変更されていない主な機能は次のとおりです。

* Google ドライブモーダル内からアセットやフォルダーを検索してフィルタリングします
* Google ドライブからWorkfront オブジェクトへのアセットのリンク
* ドキュメントページの「送信先」ドロップダウンを使用して、Google Drive にアセットをアップロードします
* ユーザーのマイドライブ領域のフォルダー構造を表示してアクセスする
* Google Drive にあるアセットの新しいバージョンをWorkfrontの既存のドキュメントにリンクする
* Google Drive からのWorkfront オブジェクトへのフォルダーのリンク
* リンクされたフォルダーにドキュメントをドラッグ&amp;ドロップして、Google Drive にアセットをアップロードする
* Workfront内から新しいGoogle Drive ドキュメントを作成する


## プルーフビューアで使用できる新しいドキュメント承認決定ボタン

>[!IMPORTANT]
>
>この機能は段階的なリリースの一部であり、特定のお客様のみが使用できます。

>[!NOTE]
>
>* プレビューリリース：2025 年 4 月 10 日（PT）、すべてのお客様向けの実稼動リリース：2025 年 4 月 17 日（PT）

新しいドキュメント承認決定ボタンがプルーフビューアに表示されます。 これで、単純なプルーフを作成してから、ドキュメントの概要から承認者とレビュー担当者を追加すると、プルーフビューア内で直接決定できるようになります。

以前は、決定を行うためにプルーフビューアを終了する必要がありました。

このリリースより前に作成された承認では、プルーフビューアにボタンは表示されません。

詳しくは、[ 新規ドキュメントの承認とプルーフの併用 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) を参照してください。
