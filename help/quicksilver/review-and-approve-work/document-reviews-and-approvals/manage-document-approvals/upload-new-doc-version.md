---
product-area: documents
navigation-topic: approvals
title: 新しいドキュメントバージョンのアップロードと承認のリクエスト
description: 新しいドキュメントのバージョンをアップロードして、Adobe Workfrontの他のユーザーに承認を依頼できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 66a134507a06c0ce0b4fd78bfa5e32bd95f8f08c
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 14%

---

# 新しいドキュメントバージョンのアップロードと承認のリクエスト

以前のレビューで「作業が必要」とマークされたドキュメントの場合は、新しいバージョンを元のドキュメントにアップロードして、別の承認ラウンドを開始できます。 新しいバージョンのドキュメントをアップロードすると、以前のバージョンはロックされます。

新しいバージョンのファイル名が以前のバージョンのファイル名と異なる場合、Workfront は新しいファイル名を持つドキュメントを表示します。

未承認の文書に新しいバージョンを追加すると、以前のバージョンの承認は「撤回」と表示されます。 一部の参加者がまだ決定を下していない場合でも、以前の承認プロセスは終了します。

最新バージョンのドキュメントが削除された場合、以前のバージョンはロックされたままになります。 以前のバージョンを編集する必要がある場合は、手動でロックを解除する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>従来のWorkfrontストレージを使用して承認を管理する、あらゆるWorkfrontパッケージ</p>
<p>Adobeのクラウドストレージを使用して承認を管理する任意のワークフローパッケージ</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>リクエスト以上</p>
   <p>コントリビューター以上</p>
   <p>Frame.io統合を使用している場合は、承認ワークフローを作成するための標準ライセンスが必要です。</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントに関連付けられたオブジェクトへの編集アクセス権</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++



<!--
## Use drag-and-drop to add a new version in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-drop does not work with Internet Explorer.


If you need another round of review and approval on a document, you can create a new document version in Workfront.

You can add the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page. 

To add a new version:

1. Navigate to the document in Workfront.
1. Drag and drop the new file on top of the previous document. This automatically creates a new version. 

1. Once the document finishes uploading, select the document to open the Document Summary panel. Here you'll see the version number at the top of the panel.


1. Scroll down to the **Approvals** section.

1. Click **Create workflow**, then fill in the following details:

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



1. (Optional) To add an existing approval template, select a template from the left side of the dialog.

   >[!TIP]
   >
   >   Users with a Standard license can create reusable Approval Templates from the Setup area. For more information, see [Create an approval workflow template for documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Once you have added all the stages and participants you need, click **Request approval**.

   The approval workflow starts and the approvers receive a notification that their approval is needed on the new document version. The previous document version is locked and any outstanding approvals on the previous version are withdrawn.

    ![request approval](assets/request-approval.png)
-->

<!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

## ドラッグ&amp;ドロップを使用して、従来のドキュメント領域に新しいバージョンを追加します

組織がWorkfront ストレージを使用している場合は、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Adobe クラウドストレージと従来のWorkfront ストレージの違い](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)を参照してください。

>[!NOTE]
>
>Internet Explorer ではドラッグ＆ドロップは機能しません。

ドキュメントのレビューと承認をもう1回行う必要がある場合は、Workfrontで新しいドキュメントのバージョンを作成できます。 以前の参加者、新しい参加者、またはその両方を追加できます。 以前のバージョンと参加者に関する情報は、ドキュメントの詳細ページで確認できます。

1段階の承認の場合は、デフォルトで基本モードで「承認を依頼」ダイアログが開きます。 詳細設定モードに切り替えて、多段階の承認または並列パスを設定します。

新しいバージョンを追加して承認をリクエストするには：

1. Workfrontでドキュメントに移動します。

1. 新しいファイルを前のドキュメントの上にドラッグ&amp;ドロップします。 Workfrontは、新しいバージョンを自動的に作成します。

1. ドキュメントのアップロードが完了したら、ドキュメントを選択してドキュメント概要パネルを開きます。 バージョン番号がパネルの上部に表示されます。

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。 **承認依頼** ダイアログが基本モードで開きます。

1. 承認ワークフローを設定します。 フィールドの説明、詳細モードの切り替え、および並列パスのフローについては、[ ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。

1. 同じレビュー担当者と承認者を以前のドキュメント バージョンからコピーするには、**コピー**&#x200B;をクリックします。
1. 「**承認を依頼**」をクリックします。

   承認ワークフローが開始され、新しいドキュメントのバージョンで承認が必要であることを示す通知が承認者に届きます。 以前のバージョンのドキュメントはロックされ、以前のバージョンで未承認の承認は取り消されます。

## ドラッグ&amp;ドロップを使用して、新しいドキュメント領域に新しいバージョンを追加します

組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

>[!NOTE]
>
>Internet Explorer ではドラッグ＆ドロップは機能しません。

ドキュメントのレビューと承認をもう1回行う必要がある場合は、Workfrontで新しいドキュメントのバージョンを作成できます。 新しいバージョンのドキュメントに承認ワークフローを追加できます。

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

1段階の承認の場合は、デフォルトで基本モードで「承認を依頼」ダイアログが開きます。 詳細設定モードに切り替えて、多段階の承認または並列パスを設定します。

新しいバージョンを追加して承認をリクエストするには：

1. Workfrontでドキュメントに移動します。

1. 新しいファイルを前のドキュメントの上にドラッグ&amp;ドロップします。 Workfrontは、新しいバージョンを自動的に作成します。

1. ドキュメントのアップロードが完了したら、ドキュメントを選択して概要パネルを開きます。 デフォルトでは、ドキュメントの最新バージョンが選択されています。

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。 **承認依頼** ダイアログが基本モードで開きます。

1. 承認ワークフローを設定します。 フィールドの説明、詳細モードの切り替え、および並列パスのフローについては、[ ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。

1. 同じレビュー担当者と承認者を以前のドキュメント バージョンからコピーするには、**コピー**&#x200B;をクリックします。
1. 「**承認を依頼**」をクリックします。

   承認ワークフローが開始され、新しいドキュメントのバージョンで承認が必要であることを示す通知が承認者に届きます。 以前のバージョンのドキュメントはロックされ、以前のバージョンで未承認の承認は取り消されます。
