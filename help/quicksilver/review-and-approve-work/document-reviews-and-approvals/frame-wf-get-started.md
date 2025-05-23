---
product-area: documents
navigation-topic: approvals
title: Frame.io を使用したアセットのレビューと承認の概要
description: Workfrontと Frame.io を使用した正式なレビューおよび承認プロセスについて説明します。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Frame.io を使用したアセットのレビューと承認の概要

新しいアセットのレビューと承認のワークフローは、Workfrontと Frame.io の緊密な統合に基づいて構築されています。 この統合では、各製品の機能を最大限に活用し、それらを組み合わせてエクスペリエンスを作成します。これにより、コンテンツの作成に関与しているすべてのユーザーが選択したツールを使用しながら、コメント、ファイル、ステータスの更新にアクセスできるようになります。これらはすべて、両方のシステム間でリアルタイムに同期されます。

Frame.io について詳しくは、[Frame.io の概要 ](https://support.frame.io/en/collections/49298-getting-started) を参照してください。

## Workfrontでの作業の開始と計画

Workfront管理者は、設定エリアでデフォルトの Frame.io アカウントを設定し、Workfrontで Frame.io ユーザーを指定することで、Workfrontと Frame.io の統合を有効にします。 これにより、コーディネーターはWorkfront プロジェクトと正式なレビューおよび承認ワークフローを使用して、作業を計画および開始できます。

### デフォルトの Frame.io アカウントを設定 [!BADGE &#x200B; 近日公開 &#x200B;]{type=Informative}

Workfront管理者は、Workfrontの設定領域にデフォルトの Frame.io アカウントを追加することで、Workfrontと Frame.io の統合を開始します。 デフォルトの Frame.io アカウントが設定されると、Workfrontで作成されたプロジェクトには、Frame.io で作成されたミラープロジェクトが含まれます。

>[!IMPORTANT]
>
>この機能は、近日公開予定です。 現時点では、Workfront チームが Frame.io アカウントを手動で追加します。 Adobe アカウント担当者にお問い合わせください。

<!--For more information, see [Configure the [!DNL Workfront] and [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

 in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Frame.io ユーザーの有効化が利用可能になりました

Frame.io を定期的に使用するWorkfront ユーザーは、Frame.io ユーザーとしてマークされる必要があります。 Workfront管理者は、Workfront ユーザープロファイルで Frame.io ユーザーを指定できます。

>[!TIP]
>
>クリエイティブツールで定期的に作業し、Frame.io ユーザーとしてレビューおよび承認用のアセットをアップロードするユーザーを有効にすることをお勧めします。

ユーザーがWorkfrontで Frame.io ユーザーとしてマークされ、プロジェクトに追加された場合：

* Frame.io のコラボレーターとして追加されます。
* Frame.io からWorkfrontにアセットを送信して、正式なレビューと承認を受けることができます。
* Workfrontから一方向の同期フォルダーの情報を表示できます。 [!BADGE &#x200B; 準備中 &#x200B;]{type=Informative}

詳しくは、「[and [!DNL Workfront] integration の設定 ](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md) を参照  [!DNL Frame.io]  てください。

![ フレーム対応ユーザー ](assets/Frame-enabled-user.png)


### Frame.io に接続したプロジェクトを作成する

デフォルトの Frame.io アカウントが追加され、Frame.io ユーザーが指定されると、プロジェクトコーディネーターは Frame.io に接続されたWorkfront プロジェクトを作成できます。 接続プロジェクトを作成すると、次の操作を実行できます

* **Frame.io ユーザーをタスクに割り当て**:Frame.io が有効なユーザーは、Workfront タスクに割り当てられると、完了すべき作業があることを示すメールで通知されます。
* **Frame.io ユーザーとプロジェクトを共有**：プロジェクトを Frame.io 対応ユーザーと共有すると、Workfrontと Frame.io の両方の内部のプロジェクトにアクセスできます。
* **Frame.io でクリエイティブマテリアルを共有**: プロジェクトコーディネーターは、一方向の同期プロジェクトフォルダーを使用して、Workfrontから Frame.io のクリエイティブユーザーに指示やマテリアルを直接送信できます。 [!BADGE &#x200B; 準備中 &#x200B;]{type=Informative}
* **タスクの進捗の追跡**：クリエイティブ担当者は、Frame.io を離れることなく、完了したアセットを送信し、タスクを完了としてマークすることができます。

詳しくは、[Frame.io に接続したプロジェクトの作成 ](/help/quicksilver/manage-work/projects/create-projects/create-frame-connected-project.md) を参照してください。


## Frame.io でのコンテンツ作成と共同作業

クリエイティブ担当者は、選択したツールを使用し続けることで、Frame.io 内で自由にピアレビューを作成、反復、実施することができます。

クリエイティブを接続されたプロジェクトに追加すると、Frame.io で次の操作を実行できます。

<!--* Access instructions from the project coordinator -->
* 非公式なピアレビューの実施
* 完成したアセットをWorkfrontに送信して、正式にレビューおよび承認する
* タスクの状態の変更または完了のマーク
* 新しいバージョンをアップロードしてから、承認 <!--do they have to send to frame.io again?--> に再送信してください

Frame.io の詳細については、[ プロジェクトでの共同作業に招待されました ](https://support.frame.io/ja/articles/11125-i-ve-been-invited-to-collaborate-on-a-project) を参照してください。

## アセットのレビューと承認

クリエイティブが完成したアセットを Frame.io からWorkfrontに送信すると、プロジェクトコーディネーターはWorkfrontで正式なレビューと承認のプロセスを開始できます。

承認ワークフローが作成されると、レビュー担当者と承認者は Frame.io に戻ってコメントを追加し、アセットをマークアップします。 また、Frame.io ビューアで承認の決定を行うこともできます。

### Workfrontでの正式なレビューと承認の開始

プロジェクトコーディネーターは、1 回限りのレビューと承認、または再利用可能な承認テンプレートを作成できます。 Frame.io におけるすべてのレビューと承認のアクティビティもWorkfrontに記録されます。

プロジェクトコーディネーターは、レビュー担当者、承認者、またはその両方を割り当てるオプションがあります。

* **レビュー担当者** は、コメントを追加したり、アセットをマークアップしたりできます。 完了したら、レビューを完了としてマークできます。 アセットを承認プロセスで先に進めるために、レビューを完了とマークする必要はありません。
* **承認者** は、コメントを追加し、アセットをマークアップできます。 承認プロセスを進めるための決定を行う必要があります。


#### レビューおよび承認ワークフローの作成

レビュー担当者と承認者は、1 回限りの承認ワークフローまたは再利用可能な承認テンプレートに追加できます。

* **1 回限りの承認**：プロジェクトコーディネーターは、アセットが存在するプロジェクトまたはタスクで、レビュー担当者と承認者を割り当て、完了期限を設定できます。 レビュー担当者と承認者には、期限の 72 時間前と 24 時間前に、および期限自体にメールで通知が送信されます。

  詳しくは、* [Frame.io アセットのレビューリクエストまたは承認リクエストの作成 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-request-for-frame-asset.md) を参照してください。

* **承認テンプレート**:Workfrontの「設定」エリアで、プロジェクトコーディネーターは作成可能な承認テンプレートを作成できます。 ユーザーはテンプレート内で、レビュー担当者と承認者を追加し、完了期間を指定できます。 承認テンプレートがアセットに適用されると、期限が指定された期間から計算されます。

  作成したテンプレートは、Frame.io から送信されるアセットに適用され、Workfrontでの正式なレビューおよび承認プロセスを開始できます。

  詳しくは、[ 承認テンプレートの作成 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) を参照してください


![ テンプレートを割り当て ](assets/assign-template.png)


#### Frame.io ビューアへのアクセス

ユーザーは、次の方法で Frame.io ビューアにアクセスできます。

* Workfrontのメール通知
* 新しいWorkfrontのホームエリアの「自分の承認」ウィジェット
  ![マイ承認待ち](assets/awaiting-my-approval.png)

>[!NOTE]
>
>Workfrontの社外ユーザーにはメールで通知され、アセットをレビューおよび承認するために Frame.io ログインを作成するよう求められます。

#### コメントの追加とアセットのマークアップ

Frame.io ビューアで作成されたすべてのコメントは、「Workfrontの更新」タブにも記録されます。 Workfrontで行われた返信は、Frame.io には表示されません。 コメントが Frame.io ビューアで「チームのみ」とマークされている場合、「Workfrontの更新」タブには表示されません。

#### 決定を下す

すべてのレビューアクティビティが完了したら、承認者は次のいずれかの決定を行う必要があります。

* **承認**：アセットは変更する必要がなく、使用できる状態になっています。
* **変更を加えて承認**：アセットには変更が必要です。変更が行われると使用できるようになります。 追加の承認は必要ありません。
* **作業が必要**：アセットに変更が必要ですが、使用する準備ができていません。 指定した変更を行ったら、アセットを新しいバージョンとしてアップロードし、別の承認を行う必要があります。<!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

レビュー担当者は、Frame.io ビューア内でレビューを完了とマークできますが、アセットが承認プロセスを進めるためにレビューを完了する必要はありません。

Workfrontの決定について詳しくは、[ 決定ステータスの概要のドキュメント ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md) を参照してください。

![ フレームビューアと決定 ](assets/frame-viewer-and-decision.png)


<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### レビューおよび承認指標の追跡

プロジェクトコーディネーターは、次のウィジェットを使用して、Workfrontのホームエリアにあるすべての進行中の承認の進行状況を監視できます。

* **すべての承認**：平均承認時間と決定に関する情報を含む 2 つのグラフと、保留中および期限切れの承認のリストビューを表示します。
  ![すべての承認](assets/all-approvals.png)
