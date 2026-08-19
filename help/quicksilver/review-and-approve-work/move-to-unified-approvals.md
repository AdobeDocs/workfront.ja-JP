---
product-area: documents
navigation-topic: approvals
title: 従来のドキュメント承認から統合承認への移行
description: 統合承認をサポートするバージョンのWorkfrontに移行すると、既存のドキュメント承認ワークフローはどうなるかを把握します。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: b612a50b7445732f90b7de2a216f4bca499fd96b
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
| 承認のステージとパス | ひとつの承認ステージで並行するパスはない | [複数の承認ステージと並行したレビューパス &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| 承認テンプレート | 各承認をゼロから設定 | Workfront セットアップで利用できる[再利用可能なテンプレート &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) |
| レビューとマークアップ | プルーフビューアー | レガシーWorkfront ストレージオブジェクトの[&#x200B; プルーフビューア &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)、またはAdobe クラウドストレージオブジェクトの[Frame.io ビューア &#x200B;](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) |
| AIを活用したレビュー | 利用不可 | [Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)による自動ブランドコンプライアンス確認 |
| レポート | レガシーレポート | ホーム KPI ウィジェットと[Canvas ダッシュボード &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |



### 進行中の承認はどうなるか

従来のドキュメント承認で作成された実行中の承認は、アップグレード前と同様に機能し続けます。 ただし、アップグレード後に作成された新しい承認は、統合承認を使用します。


## アップグレードの準備

* [統一されたレビューと承認を開始する](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)記事をエンドユーザーと共有します。
* 既存のWorkfront Fusionのシナリオを確認します。 プルーフで従来のドキュメントの承認を使用する場合は、組織をアップグレードする前に、[統一されたレビューと承認のためのWorkfront Fusion シナリオの更新](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md)を参照してください。
* Canvas ダッシュボードでレビューと承認ダッシュボードを設定して、従来の承認レポートを置き換えます。 詳しくは、[&#x200B; レビューと承認ダッシュボードの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)を参照してください。


### エンドユーザー向けのヘルプ記事

* [レビューと承認の統合を始める](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [ドキュメント承認で利用可能な機能](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [統一されたレビューと承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Frame.io ビューアでのレビューと承認](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [統合承認とプルーフの併用](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [ドキュメントの決定ステータスの概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Workfront Content Reviewerの基本を学ぶ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
