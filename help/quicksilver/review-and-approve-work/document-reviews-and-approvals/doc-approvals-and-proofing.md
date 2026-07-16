---
product-area: documents
navigation-topic: approvals
title: 統合承認とプルーフの併用
description: プルーフで統合承認を使用できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 678
ht-degree: 10%

---

# 統合承認とプルーフの併用

Workfrontの統合承認には、ドキュメントのレビューと承認に役立つ新しい機能セットが導入されています。 既存のプルーフビューアで統合承認ワークフローを使用して、レビュー中のドキュメントにコメントやマークアップを追加できます。

統合承認とプルーフを一緒に使用する場合のワークフローには、いくつかの重要な違いがあります。

* 参加者は、プルーフワークフローではなく、ドキュメントの概要に表示されます。

* ドキュメント リストの送信済み、開封、コメント、決定（SOCD）の詳細はプルーフに関連しており、ドキュメントの決定ステータスを反映していません。

## ドキュメントのアップロードとプルーフの作成

1. 新しいドキュメントを追加するプロジェクト、タスク、またはイシューに移動します。
1. 「**ドキュメント**」タブをクリックし、**新規追加**&#x200B;ドロップダウンメニューをクリックします。
または
ドキュメントをドキュメントリストにドラッグ&amp;ドロップします。

   >[!NOTE]
   >
   >ユーザープロファイルで&#x200B;**ドキュメントのアップロード時にプルーフを自動的に生成**&#x200B;を有効にしている場合、システムはシンプルなプルーフを自動的に作成します。

1. ドキュメントにカーソルを合わせ、ドキュメント名の下に表示される「**プルーフを作成**」リンクをクリックし、「**シンプルなプルーフ**」を選択します。 承認にプルーフワークフローを使用しないため、シンプルなプルーフを作成する必要があります。

参加者として割り当てられたユーザーは、プルーフビューアを使用して、ドキュメントにコメントやマークアップを追加できます。 次の節に進んで、レビュー参加者を追加する方法を説明します。

<!--
## Open the document Summary and assign participants in Production

You have the option to assign reviewers, approvers, or a mix of both:

* **Reviewers** can add comments and mark up assets. Once finished, they can mark their review as complete. Marking the review as complete is not required for the document to move forward in the approval process.
* **Approvers** can add comments and mark up assets. They must make a decision to move the approval process forward. 

To assign participants:

1. Select the document you uploaded and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## ドキュメント概要を開き、参加者を割り当てます

1段階の承認の場合は、デフォルトで基本モードで「承認を依頼」ダイアログが開きます。 詳細設定モードに切り替えて、多段階の承認または並列パスを設定します。

参加者を割り当てるには：

1. アップロードしたドキュメントを選択し、ドキュメントの概要を開きます。

   ![&#x200B; ドキュメントの概要を開く](assets/open-doc-summary.png)

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。 **承認依頼** ダイアログが基本モードで開きます。

1. 承認ワークフローを設定します。 フィールドの説明、詳細モードの切り替え、および並列パスのフローについては、[&#x200B; ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。

1. 「**承認を依頼**」をクリックします。 参加者にはメールで通知されます。

<!--
## Create a new version as needed in Production

If you need another round of review and approval, you can create a new proof version and add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants in the document Summary.

To add a new version:

1. Drag and drop the new file on top of the previous document in Workfront. This automatically creates a new version. 

1. Once the document finishes uploading, select the document, then click **Create proof** > **Simple proof**. 

1. Select the document again, and open the document Summary.
    ![Open document summary](assets/open-doc-summary.png)

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![new stage](assets/new-stage.png)

1. Once you've added all reviewers and approvers, click **Request approvals**. Participants are notified via email.
-->

## 必要に応じて新しいバージョンを作成し

レビューと承認が必要な場合は、新しいプルーフバージョンを作成し、以前の参加者、新しい参加者、またはその両方を追加できます。 ドキュメントの概要で、以前のバージョンと参加者に関する情報を表示できます。

1段階の承認の場合は、デフォルトで基本モードで「承認を依頼」ダイアログが開きます。 詳細設定モードに切り替えて、多段階の承認または並列パスを設定します。

新しいバージョンを追加するには：

1. 新しいファイルをWorkfrontの前のドキュメントの上にドラッグ&amp;ドロップします。 Workfrontは、新しいバージョンを自動的に作成します。

1. ドキュメントのアップロードが完了したら、ドキュメントを選択し、**プルーフを作成** > **シンプル プルーフ**&#x200B;をクリックします。

1. 文書をもう一度選択してから、文書の概要を開きます。

   ![&#x200B; ドキュメントの概要を開く](assets/open-doc-summary.png)

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。 **承認依頼** ダイアログが基本モードで開きます。

1. 承認ワークフローを設定します。 フィールドの説明、詳細モードの切り替え、および並列パスのフローについては、[&#x200B; ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。

1. 「**承認を依頼**」をクリックします。 参加者にはメールで通知されます。

## プルーフを確認して決定する

割り当てられたすべての承認者が「承認済み」を選択するまで、文書は承認済みステータスに移動しません。

ドキュメントをレビューして承認するには：

1. レビューメール通知に移動し、**レビューに移動**&#x200B;をクリックします。

1. Workfrontにアクセスしたら、**プルーフに移動**&#x200B;をクリックします。

1. コンテンツを確認し、コメントやマークアップを追加します。 プルーフビューアの使用方法について詳しくは、[Adobe Workfront内のプルーフのレビュー：記事インデックス &#x200B;](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)を参照してください。

1. 次のいずれかの決定を選択します。

   * **承認**: ドキュメントは変更が必要なく、使用する準備ができています。
   * **変更を加えて承認**：文書は変更が必要で、作成したら使用できる状態になります。 追加の承認は必要ありません。
   * **作業が必要**：文書は変更が必要で、使用する準備ができていません。 指定した変更が行われたら、ドキュメントを新しいバージョンとしてアップロードし、別の承認ラウンドを実行する必要があります。 新しいバージョンのアップロードについて詳しくは、この記事の「[必要に応じて新しいバージョンを作成する](#create-a-new-version-as-needed)」を参照してください。

決定を下すと、ドキュメント所有者にメールで通知されます。