---
product-area: documents
navigation-topic: approvals
title: ドキュメント承認ワークフローへの承認者またはレビュー担当者の追加
description: 既に承認待ちのドキュメントに、追加の承認者またはレビュアーを追加できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jo3N878hmvHRqo6kCepxPDk2-zlalLvqQbMjHHB8aGE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 13%

---

# ドキュメント承認ワークフローへの承認者またはレビュー担当者の追加

保留中の承認が既にあるドキュメント承認ワークフローに、さらに承認者またはレビュー担当者を追加できます。

>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。 標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>従来のWorkfrontストレージを使用して承認を管理する、あらゆるWorkfrontパッケージ</p>
<p>Adobeのクラウドストレージを使用して承認を管理する任意のワークフローパッケージ</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>コントリビューター以上</p>
   <p>レビュー以上</p> 
   <p>Frame.io統合を使用している場合は、承認ワークフローを作成するための標準ライセンスが必要です。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクト、タスク、イシュー、テンプレート、ポートフォリオ、プログラム、レポート、ダッシュボード、カレンダー、ドキュメントへの表示以上のアクセス</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストのアクセスまたは承認に関連付けられたオブジェクトへの表示以上のアクセス権 </p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++



<!--
## Add additional approvers or reviewers in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To add additional approvers or reviewers from the Document Summary:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document will open.

1. Select the version of the document you would like to add an approver or reviewer to in the version drop-down menu. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Edit workflow**.

   ![edit approval workflow](assets/edit-approval-in-legacy.png)

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## レガシードキュメント領域に承認者またはレビュー担当者を追加する

組織がWorkfront ストレージを使用している場合は、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Adobe クラウドストレージと従来のWorkfront ストレージの違い](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)を参照してください。

ドキュメントの概要から承認者またはレビュー担当者を追加するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックします。 そのドキュメントのドキュメント概要パネルが開きます。

1. バージョン ドロップダウンメニューで、承認者またはレビュー担当者を追加するドキュメントのバージョンを選択します。 デフォルトでは、最新バージョンが選択されています。

1. **承認** セクションまでスクロールし、**ワークフローの編集**&#x200B;をクリックします。 承認を依頼ダイアログが開きます。1段階の承認の場合は「基本」、複数段階の承認の場合は「詳細」と、並行パスを使用する承認の場合は「詳細」の順に選択します。

1. ユーザー、チーム、またはメールを追加します。

   * 基本モードで、**名前または電子メールを追加** フィールドに名前または電子メールを入力します。
   * 詳細モードで、更新するステージを含むパスを選択し、ステージの&#x200B;**名前またはメールを追加** フィールドに入力します。

1. 追加した各ユーザーについて、承認者かレビュアーかを選択します。

   ![承認者またはレビュー担当者のドロップダウン ](assets/choose-reviewer-or-approver.png)

1. 「**保存**」をクリックします。 追加した参加者には、文書に対する承認またはレビューが必要であることを知らせる電子メール通知が送信されます。

>[!TIP]
>
>基本モードの承認をマルチステージまたはマルチパスの承認に再構築するには、右上隅の「**詳細に移動**」をクリックします。 既存の参加者は、パス 1、ステージ 1として保存されます。 保存した後は、基本モードに戻すことはできません。 詳しくは、[ ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。

<!--
## Add additional approvers or reviewers in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).


1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page. 

   ![Add approvers in document summary](assets/approvals-icon-new.png)


1. Click **Edit workflow**.

1. Locate the stage you would like to add approvers or reviewers to, then add the user's name or email in the text box. You can also add an entire team if needed. 

1. Once their name is added, choose if they are an approver or reviewer. 

   ![approver or reviewer drop-down](assets/choose-approver-or-reviewer.png)

1. Repeat steps 5-6 to add additional approvers or reviewers.
 Once you save, the participants added receive an email notification that their approval or review is needed on the document.
-->

## 新しいドキュメント領域のドキュメント概要から、追加の承認者またはレビュー担当者を追加します

組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

ドキュメントの概要から承認者またはレビュー担当者を追加するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. ドキュメントをクリックし、ページの右側にある&#x200B;**承認** アイコンをクリックします。

   ![ ドキュメントの概要に承認者を追加](assets/approvals-icon-new.png)

1. 「**ワークフローを編集**」をクリックします。 承認を依頼ダイアログが開きます。1段階の承認の場合は「基本」、複数段階の承認の場合は「詳細」と、並行パスを使用する承認の場合は「詳細」の順に選択します。

1. ユーザー、チーム、またはメールを追加します。

   * 基本モードで、**名前または電子メールを追加** フィールドに名前または電子メールを入力します。
   * 詳細モードで、更新するステージを含むパスを選択し、ステージの&#x200B;**名前またはメールを追加** フィールドに入力します。

1. 追加した各ユーザーについて、承認者かレビュアーかを選択します。

   ![承認者またはレビュー担当者のドロップダウン ](assets/choose-reviewer-or-approver.png)

1. 「**保存**」をクリックします。 追加した参加者には、文書に対する承認またはレビューが必要であることを知らせる電子メール通知が送信されます。

>[!TIP]
>
>基本モードの承認をマルチステージまたはマルチパスの承認に再構築するには、右上隅の「**詳細に移動**」をクリックします。 既存の参加者は、パス 1、ステージ 1として保存されます。 保存した後は、基本モードに戻すことはできません。 詳しくは、[ ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。
