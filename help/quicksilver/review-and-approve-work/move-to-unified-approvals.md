---
product-area: documents
navigation-topic: approvals
title: 従来のドキュメント承認から統合承認への移行
description: 統合承認をサポートするバージョンのWorkfrontに移行すると、既存のドキュメント承認ワークフローはどうなるかを把握します。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%
---
# 従来のドキュメント承認から統合承認への移行

AdobeクラウドストレージをサポートするWorkfrontのバージョンに移行すると、組織も従来のドキュメント承認から統合承認に移行します。 この記事では、統合承認で使用できる機能に関する情報と、Workfront管理者が従来のドキュメント承認からユーザーを移行する際の推奨事項について説明します。


>[!IMPORTANT]
>
>この変更は、Adobe クラウドストレージをサポートするバージョンのWorkfrontに移行すると、組織全体に適用されます。 従来のドキュメント承認から統合承認に移行する際に、パイロットグループや段階的なロールアウトオプションはありません。<br>
>Adobe クラウドストレージの変更点について詳しくは、[Adobe クラウドストレージ上のWorkfrontへの移行](/help/quicksilver/review-and-approve-work/workfront-storage.md)を参照してください。

## 従来のドキュメント承認から統合承認への変化を理解する

|  | レガシードキュメントの承認 | 統合承認 |
| --- | --- | --- |
| 承認者とレビュアー | 個々のユーザーのみが承認 | 個々のユーザーまたはチームによる承認またはレビュー |
| 期限とリマインダー | 自動リマインダーなし | 72時間切れ、24時間切れ、期限内の自動リマインダー |
| 承認のステージとパス | ひとつの承認ステージで並行するパスはない | [複数の承認ステージと並行したレビューパス ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| 承認テンプレート | 各承認をゼロから設定 | Workfront セットアップで利用できる[再利用可能なテンプレート ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) |
| レビューとマークアップ | プルーフビューアー | レガシーWorkfront ストレージオブジェクトの[ プルーフビューア ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)、またはAdobe クラウドストレージオブジェクトの[Frame.io ビューア ](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) |
| AIを活用したレビュー | 利用不可 | [AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)による自動ブランドコンプライアンスチェック |
| レポート | レガシーレポート | ホーム KPI ウィジェットと[Canvas ダッシュボード ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### 進行中の承認はどうなるか

従来のドキュメント承認で作成された実行中の承認は、アップグレード前と同様に機能し続けます。 ただし、アップグレード後に作成された新しい承認は、統合承認を使用します。


## アップグレードの準備

* [統一されたレビューと承認を開始する](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)記事をエンドユーザーと共有します。
* 既存のWorkfront Fusionのシナリオを確認します。 プルーフで従来のドキュメントの承認を使用する場合は、組織をアップグレードする前に、[統一されたレビューと承認のためのWorkfront Fusion シナリオの更新](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)を参照してください。
* Canvas ダッシュボードでレビューと承認ダッシュボードを設定して、従来の承認レポートを置き換えます。 詳しくは、[ レビューと承認ダッシュボードの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)を参照してください。


### エンドユーザー向けのヘルプ記事

* [レビューと承認の統合を始める](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [ドキュメント承認で利用可能な機能](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [統一されたレビューと承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Frame.io ビューアでのレビューと承認](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [統合承認とプルーフの併用](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [ドキュメントの決定ステータスの概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Workfront AI レビュアーを始める](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)