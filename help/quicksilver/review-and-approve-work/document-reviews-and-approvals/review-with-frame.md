---
product-area: documents
navigation-topic: approvals
title: Frame.io ビューアでのレビューと承認
description: Frame.io ビューアを使用してドキュメントをレビューおよび承認する方法について説明します。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 3190ad18-180e-42e5-aa10-bdad74303d3d
source-git-commit: a3edfadc447a763c638cc926b386272890697f81
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 1%

---

# Frame.io ビューアでのレビューと承認

Frame.io ビューアを使用して、Workfrontでドキュメントをレビューし、承認できます。

Frame.io ビューアを使用してWorkfront ドキュメントをレビューすると、コメントを残したり、ドキュメント、画像、ビデオの特定のセクションをマークアップしたりして、チームとの効率的な共同作業を行い、フィードバックが明確で実用的であることを確認できます。

Workfrontとの Frame.io 統合について詳しくは、「[Frame.io 統合の概要 ](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md)」を参照してください。


<!--## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Request or higher</p>
   <p>Contributor or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Documents</p>  </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit access to the object associated with the document</p>  </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ -->

## 前提条件

* Workfront インスタンスでWorkfrontと Frame.io の統合を設定する必要があります。 詳しくは、[Frame.io 統合の概要 ](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md#integration-requirements) を参照してください。

## ドキュメントのレビュー

レビュー担当者は、にコメントを追加したり、アセットをマークアップしたりできます。 完了したら、Workfrontでレビューを完了済みとしてマークできます。 アセットを承認プロセスで先に進めるために、レビューを完了とマークする必要はありません。

1. レビューメール通知に移動し、「**レビューに移動**」をクリックします。
または
Workfrontのホームページに移動して、「自分の承認」ウィジェットを見つけ、「**レビューを開く**」をクリックします。

   >[!NOTE]
   > 
   >のホームページに自分の承認ウィジェットを追加する必要がある場合があります。 詳しくは、[ ホームでのウィジェットの追加、編集、削除 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md) を参照してください。

1. Frame.io では、コメント ツールを使用して、フィードバックを残したり質問したりします。
コメントとアセットのマークアップは、Frame.io ビューアでのみ表示されます。 コメントがWorkfrontに表示されません。 Frame.io ビューアの使用について詳しくは、[ メディアへのコメント ](https://help.frame.io/en/articles/9105251-commenting-on-your-media) を参照してください。
1. ドキュメントの設定が完了したら、Workfrontのドキュメントの詳細ページに戻って、レビューを完了としてマークします。

   ![ レビュー完了のマーク ](assets/mark-review-complete.png)

## ドキュメントを承認

承認者は、コメントを追加し、アセットにマークアップできます。 承認プロセスを先に進めるための決定を行う必要があります。

割り当てられたすべての承認者が「承認済み」を選択するまで、ドキュメントは承認済みステータスに移動しません。

ドキュメントに対して決定を行うには：

1. レビューメール通知に移動し、「**レビューに移動**」をクリックします。
または
Workfrontのホームページに移動して、「自分の承認」ウィジェットを見つけ、「**レビューを開く**」をクリックします。

   >[!NOTE]
   > 
   >のホームページに自分の承認ウィジェットを追加する必要がある場合があります。 詳しくは、[ ホームでのウィジェットの追加、編集、削除 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md) を参照してください。


1. Frame.io では、コメント ツールを使用して、フィードバックを残したり質問したりします。 コメントとアセットのマークアップは Frame.io ビューアでのみ表示されます。 Frame.io ビューアの使用について詳しくは、[ メディアへのコメント ](https://help.frame.io/en/articles/9105251-commenting-on-your-media) を参照してください。
1. ドキュメントの設定が完了したら、Frame.io ビューアで次のいずれかの決定を選択できます。

   * **承認**：アセットは変更する必要がなく、使用できる状態になっています。
   * **作業が必要**：アセットに変更が必要ですが、使用する準備ができていません。 指定した変更を行ったら、アセットを新しいバージョンとしてアップロードし、別の承認を行う必要があります。 詳しくは、[ 新しいドキュメントバージョンをアップロードし、承認をリクエストする ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md) を参照してください。<!--do they need to tell someone it was uploaded via comment tagging?-->

   決定を行うと、ドキュメント所有者にメールで通知されます。

   Workfrontの決定について詳しくは、[ 決定ステータスの概要のドキュメント ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md) を参照してください。

   ![ フレームビューアと決定 ](assets/make-decision-frame.png)



<!--is document owner the correct term?-->
