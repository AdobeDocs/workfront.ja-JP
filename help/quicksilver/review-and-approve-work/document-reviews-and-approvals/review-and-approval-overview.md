---
product-area: documents
navigation-topic: approvals
title: アセットのレビューと承認の概要
description: Workfrontの正式なレビューおよび承認プロセスについて説明します。
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 959bd3cab0de8b76c94fad1be5b6b2b8b7ae904b
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 1%

---

# アセットのレビューと承認の概要

新しいアセットのレビューと承認のワークフローは、Workfrontと Frame.io の緊密な統合に基づいて構築されています。 この統合では、各製品が提供する機能を最大限に活用し、それを組み合わせてエクスペリエンスを作成します。コンテンツの作成に関与するすべてのペルソナが、選択したツールで作業しながら、コメント、ファイル、ステータス更新にアクセスできます。両方のシステムでリアルタイムに同期されます。

Frame.io の詳細については、を参照してください [Frame.io の基本を学ぶ](https://support.frame.io/en/collections/49298-getting-started).

## Workfrontでの作業の開始と計画

Workfront管理者は、設定エリアでデフォルトの Frame.io アカウントを設定し、Workfrontで Frame.io ユーザーを指定することで、Workfrontと Frame.io の統合を有効にします。 これにより、コーディネーターはWorkfront プロジェクトと正式なレビューおよび承認ワークフローを使用して、作業を計画および開始できます。

### デフォルトの Frame.io アカウントの設定

Workfront管理者は、Workfrontの設定領域にデフォルトの Frame.io アカウントを追加することで、Workfrontと Frame.io の統合を開始します。 デフォルトの Frame.io アカウントが設定されると、Workfrontで作成されたプロジェクトには、Frame.io で作成されたミラープロジェクトが含まれます。

詳しくは、[] を参照してください。

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Frame.io ユーザーの有効化

Frame.io を定期的に使用するWorkfront ユーザーは、Frame.io ユーザーとしてマークされる必要があります。 Workfront管理者は、Workfront ユーザープロファイルで Frame.io ユーザーを指定できます。

Workfrontでユーザーが Frame.io ユーザーとしてマークされ、プロジェクトに追加されると、

* Frame.io のコラボレーターとして追加されます
* 正式なレビューと承認のために、Frame.io からWorkfrontにアセットを送信できます
* Workfrontから一方向の同期フォルダーの情報を表示できます

>[!TIP]
>
>クリエイティブツールで定期的に作業し、Frame.io ユーザーとしてレビューおよび承認用のアセットをアップロードするユーザーを有効にすることをお勧めします。

詳しくは、[] を参照してください。

![](assets/Frame-enabled-user.png)


### Frame.io に接続したプロジェクトを作成する

デフォルトの Frame.io アカウントが追加され、Frame.io ユーザーが指定されると、プロジェクトコーディネーターは Frame.io に接続されたWorkfront プロジェクトを作成できます。 接続プロジェクトを作成すると、次の操作を実行できます

* **Frame.io ユーザーのタスクへの割り当て**:Frame.io が有効なユーザーは、タスクに割り当てられるとメールで通知され、完了する作業があることを示します。
* **Frame.io ユーザーとのプロジェクトの共有**:Frame.io 対応のユーザーと共有されたプロジェクトは、Frame.io 内のプロジェクトへのアクセス権をユーザーに付与します。
* **Frame.io とのクリエイティブマテリアルの共有**：一方向同期プロジェクトフォルダーを使用して、Workfrontから Frame.io のクリエイティブユーザーに指示や資料を直接送信できます。
* **タスクの進捗の追跡**: クリエイティブ担当者は、Frame.io を離れることなく、完成したアセットを送信し、タスクに完了のマークを付けることができます。

詳しくは、[] を参照してください。

<!--Preassign approval templates to tasks coming in the future-->


## Frame.io でのコンテンツ作成と共同作業

クリエイティブ担当者は、選択したツールを使用し続けることで、Frame.io 内で自由にピアレビューを作成、反復、実施することができます。

クリエイティブが接続されたプロジェクトに追加された場合、Frame.io を離れることなく、次の操作を行うことができます。

* プロジェクトコーディネーターから手順へのアクセス
* 非公式なピアレビューの実施
* 完成したアセットをWorkfrontに送信して、正式にレビューおよび承認する
* タスクの状態の変更または完了のマーク
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Frame.io でのアセットの確認について詳しくは、

## アセットのレビューと承認

クリエイティブが完成したアセットを Frame.io からWorkfrontに送信すると、プロジェクトコーディネーターはWorkfrontで正式なレビューと承認のプロセスを開始できます。

承認が作成されると、ユーザーは Frame.io に戻ってアセットにコメントし、マークアップします。 また、Frame.io ビューアで承認の決定を行うこともできます。

### Workfrontでの正式なレビューと承認の開始

プロジェクトコーディネーターは、Workfrontの設定エリアで、1 回限りのレビューと承認、または再利用可能な承認テンプレートを作成できます。 Frame.io で行われたレビューと承認のアクティビティはすべてWorkfrontにも記録されます。

#### レビュー担当者と承認者の追加

プロジェクトコーディネーターは、レビュー担当者、承認者、またはその両方を割り当てるオプションがあります。

* **Reviewers** アセットにコメントしたり、アセットをマークアップしたりできます。 完了したら、レビューを完了としてマークできます。 <!--example of when to add reviewers-->
* **承認者** アセットにコメントしたり、アセットをマークアップしたりできます。 承認プロセスを進めるための決定を行う必要があります。


#### レビューおよび承認ワークフローの作成

レビュー担当者と承認者は、1 回限りの承認ワークフローまたは承認テンプレートに追加できます。

<!--can also assign teams and set deadline-->
メール – 期限のメール 72、24、および期限に。

* **1 回限りの承認**：承認期限の設定

* **承認テンプレート**
Workfrontの「設定」領域で、Standard ライセンスを持つユーザーは、再利用可能な承認テンプレートを作成できます。 ユーザーはテンプレート内で期間を指定し、レビュー担当者と承認者を追加できます。 <!--do we want to mention any upcoming plans here? -->

  作成したテンプレートは、Frame.io から送信されるアセットに適用され、Workfrontでの正式なレビューおよび承認プロセスを開始できます。
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Workfrontからアセットをアップロードし、レビューおよび承認用にフレームに送信 – 近日公開しますか？

### Frame.io でのアセットの承認

関係者は、Frame.io ビューアを使用して、接続されたアセットを確認および承認できます。

#### Frame.io ビューアへのアクセス

ユーザーは、次の方法で Frame.io ビューアにアクセスできます。

* 新しいWorkfrontのホームエリアの「承認待ち」ウィジェット
* Workfrontのメール通知。

社外の Workfront ユーザーは、アセットをレビューおよび承認するために、Frame.io ログインを作成するよう求められます。

#### アセットに対するコメントとマークアップ

Frame.io ビューアで作成されたすべてのコメントは、「Workfrontの更新」タブにも記録されます。 Workfrontで行われた返信は、Frame.io には表示されません。 「チームのみ」とマークされたコメントは、「Workfrontの更新」タブには表示されません。

#### 決定を下す

承認者は、次のいずれかの決定を行う必要があります。

* 承認：これ
* 変更して承認
* 作業が必要

レビュー担当者は、Frame.io ビューア内でレビューを完了としてマークできます。

<!-- include screenshot from frame.io-->



<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### レビューおよび承認指標の追跡

ホームの承認速度レポートのウィジェット

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## キャンペーンアセット承認ワークフローの例

導入部の段落

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
