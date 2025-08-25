---
product-area: documents
navigation-topic: approvals
title: Workfront AI レビュアーの基本を学ぶ
description: Workfront AI レビュアー
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 7%

---

# Workfront AI レビュアーの基本を学ぶ

>[!NOTE]
>
>この機能は現在ベータ版です。

Workfront AI レビュアーを使用すると、レビューおよび承認ワークフローでコンテンツベロシティを向上させ、ブランドコンプライアンスを最適化することができます。 AI レビュー担当者は、Workfrontの承認テンプレートまたは個々のレビューおよび承認リクエストに追加できます。

## アクセス要件

Workfrontで AI レビュー担当者を設定するには、システム管理者である必要があります。

すべてのユーザーが、レビューおよび承認リクエストに AI レビュー担当者を追加できます。


## 前提条件

<!--DELETE THIS SECTION MARCH 2026-->

<!--* Your organization must have migrated to Adobe IMS (Identity Management System).-->
* Workfront インスタンスでは、統合承認が有効になっている必要があります。
* Adobeには、Adobe生成 AI 契約がファイルに署名済みである必要があります。
契約の署名について詳しくは、[Adobe Gen AI 契約への署名 ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) を参照してください。


## サポートされているファイルタイプ {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="サポートされていないファイルタイプ"
>abstract="この AI レビュアーは、選択されたファイルタイプをサポートしていません。サポートされているファイルタイプをアップロードするか、AI レビュアーを削除してリクエストを送信します。"

AI レビュー担当者は、次のファイルタイプをレビューできます。

* PNG （.png）
* JPEG（.jpeg、.jpg）
* WEBP （.webp）
* 非アニメーション GIF （.gif）

## ブランドガイドラインの設定

Workfront AI レビュー担当者は、コンテンツのレビュー時に、Performance Marketing 用に Genstudio で設定されたブランドガイドラインを使用します。 現在、画像のブランドガイドラインのみをセットアップできます。 詳しくは、[Adobe GenStudio for Performance Marketingの基本を学ぶ ](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started) を参照してください。


## AI レビュー担当者の作成

GenStudio Foundations に 1 つ以上のブランドが設定されたら、Workfront管理者は、設定エリアで AI レビュー担当者の作成を開始できます。 その後、これらの AI レビュー担当者を承認テンプレートや個々のレビューおよび承認リクエストに割り当てることができます。 現在、AI レビュー担当者がレビューできるのは画像ブランドガイドラインに対してのみです。

詳しくは、[AI レビュー担当者の作成 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/set-up-ai-reviewer.md) を参照してください。

## AI レビュー担当者を追加してリクエストをレビューおよび承認

ユーザーは、既存の承認テンプレートまたは個々のレビューリクエストおよび承認リクエストに AI レビュー担当者を追加できます。

### 承認テンプレート

レビューと承認のリクエストに同じユーザーを追加することが多い場合、標準ライセンスのユーザーは、Workfrontの設定エリアで承認テンプレートを作成できます。

ユーザーは、AI レビュー担当者を承認テンプレートに追加することにより、テンプレートを使用してリクエストを作成する際に、ブランドのコンプライアンスを自動的に確認できます。

作成した承認テンプレートは、プロジェクト、タスクまたはイシューのドキュメント エリアにあるアセットに適用できます。

詳しくは、[ アセットおよびドキュメントの承認テンプレートの作成 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) を参照してください。

![AI レビュアーを表示するテンプレートリスト ](assets/ai-review-templates.png)

### 個々のレビューおよび承認要求

ユーザーは、レビューおよび承認の個々のリクエストを作成する際、に AI レビュー担当者を追加するか、AI レビュー担当者のみとのリクエストを 1 つ作成して、ブランドのコンプライアンスをチェックできます。

詳しくは、[ドキュメントのレビューまたは承認リクエストの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。


![AI レビュー担当者が個々の承認リクエストに追加されました ](assets/ad-ai-reviewer-to-request.png)

## AI レビュー担当者のスコアとフィードバックを表示

AI レビュー担当者とのレビューおよび承認リクエストが送信された数秒後に、他の参加者がまだレビューや決定を行っている場合でも、AI レビュー担当者からのスコアとフィードバックがドキュメントの概要パネルで利用できるようになります。

承認所有者には、アセットのレビューが完了したことを知らせるメールも届きます。 メールで「**レビューに移動**」をクリックし、Workfrontでスコアとフィードバックを確認します。

AI レビュー担当者は、レビューおよび承認ワークフローの意思決定者となるようには設計されていません。 アセットを指定されたブランド要件に合わせるためのスコアと推奨事項のみが提供されます。

画像がブランドガイドラインを満たさない場合は、クリエイティブが新しいバージョンをアップロードし、承認所有者が AI レビュー担当者と 2 回目のレビューおよび承認リクエストを作成して、バージョンを切り替えてフィードバックを比較できます。

スコアとフィードバックの表示について詳しくは、「[AI レビュー担当者のスコアとフィードバックの表示 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md)」を参照してください。


![AI レビュアーのフィードバック ](assets/ai-reviewer-feedback.png)


## ビデオチュートリアル

>[!VIDEO](https://video.tv.adobe.com/v/3470847/)