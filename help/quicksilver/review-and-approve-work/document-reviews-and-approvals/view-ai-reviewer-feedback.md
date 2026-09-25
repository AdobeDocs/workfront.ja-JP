---
product-area: documents
navigation-topic: approvals
title: AI レビュアーのスコアとフィードバックの表示
description: 承認リクエストを送信してから数秒後、AI レビュアーのスコアとフィードバックをドキュメントの概要パネルで表示できます。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 838e8f3d-0ea6-4844-a261-ef7b0e78a755
TQID: 'https://experienceleague.adobe.com/iPlcSTaPI-zhmWvRvO81RKFYnIzUoJqzM70mNcxrVbs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 3%
---
# AI レビュアーのスコアとフィードバックの表示

レビューと承認リクエストを送信してから数秒後、ドキュメントの概要パネルでAI レビュアーのスコアとフィードバックを表示できます。

AI レビュアーは、レビューと承認ワークフローの意思決定者となるように設計されていません。 指定されたブランド要件に合致するスコアとレコメンデーションのみが提供されます。

![AI レビュー担当者からのフィードバック ](assets/ai-reviewer-output.png)

## スコアの計算方法の理解

AI レビュアーは、レビュータイプに応じてスコアを異なる方法で計算します。

* 画像レビュー：このスコアは、合格したガイドラインと失敗したガイドラインの比率を反映しています。
* レビューをコピー：このスコアは、主観的な結果と客観的な結果のバランスのとれた重み付けを使用します。 目的のガイドライン（「修正」に表示）は、主観的なガイドライン（「検討」に表示）の3倍の重み付けになります。

客観的なガイドラインは、コピーレビューに重きを置くため、具体的で測定可能なガイドラインを作成することをお勧めします。 詳しくは、AI レビュアーのブランドの作成と管理の記事の「[ ブランドガイドラインの作成に関するベストプラクティス ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md#best-practices-for-writing-brand-guidelines)」の節を参照してください。

## スコアとフィードバックの表示

AI レビュアーのスコアとフィードバックは、ドキュメントの概要パネルまたはドキュメントの詳細ページの「承認」タブで表示できます。

1. Workfrontの通知メールで、**レビューに移動**&#x200B;をクリックします。

   または

   ドキュメントをアップロードするドキュメント領域に移動し、ドキュメントの概要パネルを開きます。
1. 「**スコア**」をクリックします。
   ![ ドキュメントのスコアを表示](assets/view-score.png)

スコアとフィードバックウィンドウで、AI レビュアーは、アセットが指定されたガイドラインを満たさない方法を説明します。
![AI レビュー担当者のフィードバックには注意が必要](assets/ai-reviewer-needs-attention.png)

## 新しいバージョンをアップロードし、AI レビュアーをもう一度追加します

AI レビュアーのフィードバックに基づいてアセットを調整する必要がある場合は、新しいバージョンをアップロードして新しいレビューを開始できます。

詳しくは、[新しいドキュメントのバージョンをアップロードし、承認をリクエスト ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md)するを参照してください。
