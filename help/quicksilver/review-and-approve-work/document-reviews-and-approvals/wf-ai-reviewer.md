---
product-area: documents
navigation-topic: approvals
title: Workfront AI レビュアーを始める
description: WorkfrontのAI レビュアーを使用して、レビューや承認のワークフロー中に、コンテンツとブランドガイドラインを比較して評価できます。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5nwapHAbb8wRWqen7a49QfpsAMLPZNEfJUJ2vm4R7SA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 3%
---
# Workfront AI レビュアーを始める

AI レビュアーはAI コラボレーターの一種で、プロジェクト、タスク、ドキュメントに追加できます。 AI共同作業者は、設定エリアで設定し、ユーザーと同じように割り当てることができます。

WorkfrontのAI Reviewerは、レビューと承認のプロセス全体を通じてコンテンツ制作をスピードアップし、ブランドコンプライアンスを向上させるのに役立ちます。 AI レビュー担当者を承認テンプレートに追加したり、個別のレビューや承認のリクエストに含めたりすることができます。

## アクセス要件

WorkfrontでAI レビューアーを設定するには、システム管理者である必要があります。

誰でもAI レビュー担当者をレビューおよび承認リクエストに追加できます。

## 要件

* Workfront インスタンスでは、統合承認が有効になっている必要があります。
* 組織にはGenStudio Foundationが必要です。
  * WORKFRONTのAI Reviewerは、GenStudio Foundationでアセットのレビューと承認ワークフローに使用できる機能を提供します。 作業を完了するためにGenStudio Foundationに直接アクセスする必要はありません。 AI ReviewerによるGenStudio Foundation機能へのアクセスは、Workfront契約の条件に該当します。
* Adobeには、署名済みのAdobe Gen AI契約書がファイルに登録されている必要があります。
契約書への署名について詳しくは、[Adobe Gen AI契約書への署名](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)を参照してください。
* AI Reviewerはサンドボックス環境では使用できません。


## サポートされているファイルタイプ {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="サポートされていないファイルタイプ"
>abstract="この AI レビュアーは、選択されたファイルタイプをサポートしていません。 サポートされているファイルタイプをアップロードするか、AI レビュアーを削除してリクエストを送信します。"

AI レビュアーは、次のファイルタイプを確認できます。

* PNG （.png）
* JPEG （.jpeg、.jpg）
* WEBP （.webp）
* GIF以外（.gif）
* PDF （.pdf）
* PPT （.ppt, .pptx）
* DOC （.doc, .docx）

サポートされていないファイルタイプをアップロードした場合、承認ワークフローの作成時にAI レビューアーオプションは使用できません。

## ブランドガイドラインの設定

Workfront AI Reviewerは、コンテンツをレビューする際にブランドガイドラインを使用します。 Workfront管理者は、Workfrontの設定領域でブランドガイドラインを設定できます。 GenStudio Foundationで作成されたブランドは、Workfrontでも利用できます。

ブランドガイドラインを設定するには、システム管理者は次の手順に従う必要があります。

1. [ブランド権限へのアクセス権の付与](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [AI レビュアー](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)のブランドを作成および管理します。


## AI レビュアーの作成

少なくとも1つのブランドを設定すると、Workfront管理者は設定領域でAI レビューアーの作成を開始できます。 異なるガイドラインに焦点を当てた複数のAI レビューアーを作成することができます。

* **画像**：このAI レビュアーは、Workfrontで設定した画像ブランドガイドラインに照らし合わせてアセットをレビューします。 [!BADGE ベータ版]{type=Positive tooltip="この機能は現在ベータ版です。"}
  * この機能を有効にするには、システム管理者がベータ版の契約書に署名する必要があります。
* **ブランドボイス**: AI レビュアーは、Workfrontで設定したブランドボイスのガイドラインに照らし合わせてアセットをレビューします。

AI レビュー担当者は、承認テンプレートや個々のレビューおよび承認リクエストに割り当てることができます。

詳しくは、[AI コラボレーターの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)を参照してください。

## AI レビュアーによる評価 {#what-ai-reviewer-evaluates}

AI レビュアーによるコンテンツの評価は、ガイドラインの種類（画像またはブランドボイス）によって異なります。

### 画像

AI レビュアーは次の項目を評価します。

* **構図**：焦点、背景、切り抜き、クリエイティブな構図
* **照明とムード**：光、鮮やかさ、楽観主義の使用
* **多様性とインクルージョン**：人物像（人種、性別、年齢、能力）

AI Reviewerは次の項目を評価しません。

* **ロゴの使用状況**：配置、空き領域、サイズ、正しいロゴバージョン
* **カラーパレット**：ブランドの色のコンプライアンス、未承認の色の回避
* **タイポグラフィ**: フォントファミリー、重み、間隔、整列
* **イラストスタイル**：ブランドのイラストアプローチとの一貫性
* **アクセシビリティ**: コントラストコンプライアンス、読みやすさ

### ブランドボイス

AI レビュアーは次の項目を評価します。

* **声のトーン**：会話形式で、明確で、人間味があり、ブランドパーソナリティに沿っている
* **言葉遣い/形式**：流行語、エリティズム、過剰な形式の回避
* **メッセージ**：奨励、正直、責任あるポジショニング（AI トピックなど）

AI Reviewerは次の項目を評価しません。

* **法律/コンプライアンス**：商標の使用、免責事項、ローカライゼーションルール

AI レビュアーが評価する内容に沿ったブランドガイドラインの作成に関するガイダンスについては、[AI レビュアーのブランドの作成と管理](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)を参照してください。

## AI レビュー担当者のレビューおよび承認リクエストへの追加

ユーザーは、AI レビュー担当者を既存の承認テンプレートや個々のレビューおよび承認要求に追加できます。

### 承認テンプレート

同じユーザーが同じユーザーをレビューリクエストと承認リクエストに追加することが多い場合、Standard ライセンスユーザーはWorkfrontの設定領域で承認テンプレートを作成できます。

ユーザーは、AI レビューアーを承認テンプレートに追加することで、テンプレートを使用してリクエストを作成する際に、ブランドコンプライアンスを自動的にチェックできます。

作成した承認テンプレートは、プロジェクト、タスク、イシューの「ドキュメント」エリアのアセットに適用できます。

詳しくは、[ ドキュメントの承認ワークフローテンプレートの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)を参照してください。

AI レビューアーを表示する![ テンプレートリスト ](assets/ai-review-templates.png)

### 個人のレビューと承認のリクエスト

ユーザーが個別のレビューと承認のリクエストを作成する場合、AI レビュアーを他の参加者と追加したり、AI レビュアーのみで1つのリクエストを作成してブランドコンプライアンスをチェックしたりできます。

詳しくは、[ ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。


![AI レビュアーが個別の承認リクエストに追加されました](assets/new-stage.png)

## AI レビュアーのスコアとフィードバックの表示

AI レビュアーによるレビューと承認のリクエストが送信された数秒後、他の参加者がまだレビューと意思決定を行っている場合でも、AI レビュアーからのスコアとフィードバックはドキュメントの概要パネルで確認できます。

また、承認担当者には、アセットのレビューが完了したことを知らせるメールが送信されます。 メールから、**レビューに移動**&#x200B;をクリックし、Workfrontでスコアとフィードバックを確認します。

AI レビュアーは、レビューと承認ワークフローの意思決定者となるように設計されていません。 指定されたブランド要件に合致するスコアとレコメンデーションのみが提供されます。

アセットがブランドガイドラインを満たしていない場合、クリエイターは新しいバージョンをアップロードでき、承認オーナーはAI レビュアーで2回目のレビューと承認リクエストを作成できます。

スコアとフィードバックの表示について詳しくは、[AI Reviewerのスコアとフィードバックの表示](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md)を参照してください。

