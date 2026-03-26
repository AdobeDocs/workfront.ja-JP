---
product-area: documents
navigation-topic: approvals
title: レビューと承認の統合を始める
description: WorkfrontとFrame.ioが実現する統合レビューと承認の詳細
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b9a83bc2-4dd8-4c77-a2e7-385baa809b3b
source-git-commit: 86d5ed6f91bca0b68748a43476710028d34d6ad2
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 4%

---

# レビューと承認の統合を始める

WorkfrontとFrame.ioの統合レビューおよび承認機能を利用すれば、クリエイター、マーケター、ステークホルダーはシームレスなワークフローで作業の足並みを揃えることができます。 リアルタイムの更新にアクセスし、重複作業を回避して、アセットがリリース前に承認されるようにします。

Frame.ioについて詳しくは、[Frame.ioの概要](https://support.frame.io/en/collections/49298-getting-started)を参照してください。

Workfront インスタンスでWorkfrontとFrame.ioの連携を設定している必要があります。 詳しくは、[統一されたレビューと承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md#integration-requirements)を参照してください。

## 統合要件

* WorkfrontとFrame.ioは、同じIdentity Management システム（IMS）組織にデプロイする必要があります。

* ユーザーは、IMS組織内の1つのWorkfront インスタンスにのみ属することができます。

* Workfront インスタンスは、Adobe Unified ExperienceおよびAdobe エンタープライズストレージで有効にする必要があります。

* 統合は、Adobe Professional Servicesで設定する必要があります。

## Workfrontにおける作業の立ち上げと計画

プロジェクトコーディネーターは、Workfrontでプロジェクトを作成し、作業を計画できます。 Frame.io統合が有効になっているインスタンスで作成されたプロジェクトは、Adobe エンタープライズストレージを使用します。これにより、アセットをAdobe エコシステム内で保存および管理できます。

組織がFrame.io エンタープライズライセンスを所有している場合、Workfrontで作成されたプロジェクトはFrame.ioでも表示されるため、ユーザーはどちらかの製品でアセットを操作したりアップロードしたりできます。

Frame.ioのAdobe エンタープライズストレージまたはプロジェクトについて詳しくは、

* [Workspaceの概要：プロジェクト &#x200B;](https://help.frame.io/en/articles/9101001-workspace-overview#h_d9f8654895)
* [アドビのエンタープライズストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)

## アセットのレビューと承認

アセットが完成したら、プロジェクトコーディネーターはWorkfrontで正式なレビューと承認プロセスを開始できます。

承認ワークフローを作成した後、レビュー担当者と承認者はFrame.io ビューアを使用してコメントを追加したり、アセットにマークを付けたりできます。 Frame.io ビューアで承認決定を行うこともできます。

プロジェクトの設定について詳しくは、「

* [プロジェクトの作成](/help/quicksilver/manage-work/projects/create-projects/create-project.md)

### Workfrontでの正式なレビューと承認の開始

プロジェクトコーディネーターは、1回限りのレビューと承認、または再利用可能な承認テンプレートを作成できます。 レビュアー、承認者、またはその両方を割り当てることができます。

* **レビュー担当者**&#x200B;は、コメントを追加したり、アセットをマークアップしたりできます。 終了したら、レビューを「完了」としてマークすることができます。 アセットを承認プロセスで進めるために、レビューを「完了」とマークする必要はありません。
* **承認者**&#x200B;は、コメントを追加したり、アセットをマークアップしたりできます。 承認プロセスを前進させるための決定を下す必要があります。

#### レビューと承認のワークフローを作成

レビュー担当者と承認者は、1回限りの承認ワークフローまたは再利用可能な承認テンプレートに追加できます。

* **単回使用の承認**: アセットが格納されているプロジェクトまたはタスクで、プロジェクトコーディネーターはレビュー担当者と承認者を割り当てて、完了期限を設定できます。 レビュアーと承認者には、期限の72時間前、期限の24時間前、そして期限の後に電子メールで通知が送られます。

  詳しくは、[&#x200B; ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md#create-an-approval-workflow-from-the-summary-panel-in-the-new-document-area)を参照してください。

* **承認テンプレート**: Workfrontの設定領域で、プロジェクトコーディネーターは再利用可能な承認テンプレートを作成できます。 ユーザーはテンプレート内でレビュー担当者や承認者を追加し、完了期間を指定できます。 承認テンプレートがアセットに適用されると、指定された期間から期限が計算されます。

  テンプレートを作成したら、そのテンプレートをアセットに適用して、Workfrontでの正式なレビューおよび承認プロセスを開始できます。

  詳しくは、[&#x200B; ドキュメントの承認ワークフローテンプレートの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)を参照してください。

### Frame.io ビューアでのアセットのレビューと承認

Workfrontでレビューと承認のワークフローが開始されると、レビュー担当者や承認者はFrame.io ビューアにアクセスしてコメントの追加、アセットのマークアップ、意思決定をおこなうことができます。

詳しくは、[Frame.io ビューアを使用したレビューと承認](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)を参照してください。

#### Frame.io ビューアへのアクセス

ユーザーは次の方法でFrame.io ビューアにアクセスできます。

* Workfrontのメール通知
* WorkfrontのホームエリアにあるMy approval widget

>[!NOTE]
>
>Workfrontの外部ユーザーにはメールで通知が送られ、アセットをレビューして承認するためにFrame.io ログインを作成するよう求められます。

![&#x200B; ホームからフレームビューアを開く](assets/open-fio-viewwer.png)

#### コメントの追加とアセットのマークアップ

コメントとアセットマークアップはFrame.io ビューアで表示されます。 Frame.io ビューアの使用について詳しくは、[&#x200B; メディアに対するコメント &#x200B;](https://help.frame.io/en/articles/9105251-commenting-on-your-media)を参照してください。

#### 決定を下す

すべてのレビューアクティビティが完了したら、承認者は次のいずれかの決定を行う必要があります。

* **承認**: アセットは変更を必要とせず、使用する準備ができています。
* **変更を承認**: アセットは大部分が完了しましたが、使用する前に少し変更が必要です。 指定した変更が行われると、アセットの準備ができたので、別の承認ラウンドを実行する必要はありません。
* **作業が必要**: アセットは変更が必要で、使用する準備ができていません。 指定した変更が行われたら、アセットを新しいバージョンとしてアップロードし、別の承認ラウンドを実行する必要があります。<!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

レビュー担当者は、Workfront内でレビューを完了したことをマークできますが、承認プロセスでアセットを先に進めるために、このマークは必要ありません。

Workfrontでの決定について詳しくは、[&#x200B; ドキュメントの決定ステータスの概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)を参照してください。

![&#x200B; フレームビューアーと決定](assets/decision-fio.png)


### レビューと承認の指標を追跡する

プロジェクトコーディネーターは、Workfrontのホームエリアにあるすべての進行中の承認の進捗状況をモニターしたり、Canvas ダッシュボードでカスタマイズされたレポートを使用したりできます。

* **カスタムダッシュボード**: カンバスダッシュボード領域にレポートダッシュボードを作成し、統合承認機能を使用して、レビューと承認に関する詳細情報と詳細情報の両方を表示します。 開始方法について詳しくは、[&#x200B; レビューと承認用のレポートダッシュボードの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md)を参照してください。
* **ドキュメント承認指標ホーム ウィジェット**：平均承認時間と決定に関する情報、保留中および期限切れの承認のリスト ビューを含む2つのグラフを表示します。
  ![すべての承認](assets/all-approvals.png)

## 完成したアセットをAdobe Experience Managerに送る

[!DNL Experience Manager Assets]&rbrace;&#x200B;を使用して、レビューと承認サイクルを経たデジタルアセットを管理および保存できます。 この統合により、Adobe Experience Manager、Frame.io、Workfront の機能を活用して、コンテンツ管理や共同作業のプロセスを合理化できます。

詳しくは、[Frame.io 統合した Adobe Experience Manager の使用](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)を参照してください。