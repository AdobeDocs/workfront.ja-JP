---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: 自動ワークフローステージの概要
description: 配達確認ステージは、様々なユーザーが配達確認を確認する期間のセグメントです。 配達確認がある段階から次の段階に移ると、Adobe Workfrontはレビュー担当者に対し、作業するタイミングを通知するよう通知します。
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---

# 自動ワークフローステージの概要

配達確認ステージは、様々なユーザーが配達確認を確認する期間のセグメントです。 配達確認がある段階から次の段階に移ると、Adobe Workfrontはレビュー担当者に対し、作業するタイミングを通知するよう通知します。

![stages_diagram.png](assets/stages-diagram-350x63.png)

ステージは、次の 2 つの異なる状況で発生します。

* [自動ワークフローでの配達確認の作成](#create-a-proof-with-an-automated-workflow)
* [配達確認の異なるレビュー担当者に期限を割り当てる](#assign-deadlines-for-different-reviewers-on-a-proof)

## 自動ワークフローでの配達確認の作成 {#create-a-proof-with-an-automated-workflow}

配達確認に自動ワークフローを追加する場合は、実行するレビュー作業のステージを設定します。

自動ワークフローを使用して配達確認のステージを設定する場合：

* ステージを連続または同時に実行するように設定できます。
* 一部のステージは、前のステージが完了した後にのみアクティブになるように設定できます。
* いくつかのステージを非公開にすることができます。 これは、例えば、クライアントと共有する前に配達確認をレビューし、結果のコメントをクライアントに表示したくない代理店で役立ちます。

自動ワークフローを使用して配達確認のステージを作成する手順については、 [自動ワークフローを使用した高度な配達確認の作成](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>ユーザーがどのステージにも含まれず、ドキュメントへのアクセス権を持ち、配達確認を開いた場合、と呼ばれるステージが作成されます。 *Workfront*.
>
>配達確認を開いたユーザーには、ドキュメント配達確認を開く受信者以外のユーザーの設定/レビューと承認/役割で指定した役割が割り当てられます。

## 配達確認の異なるレビュー担当者に期限を割り当てる {#assign-deadlines-for-different-reviewers-on-a-proof}

配達確認のレビュー担当者に異なる検証期限を割り当てると、各期限のステージが作成され、各期限のレビュー担当者が対応するステージにグループ化されます。 

**例：** 例えば、4 人のレビュー担当者を含む配達確認を作成する場合は、次のようになります。

* Olivia と Tony のレビュー担当者の方は、今から数日後に 14:00 の締め切りを指定してください。
* Aaron と Amy の場合は、数日後に 17:00 の期限を指定します。
* 自分に期限を指定していません。

システムは、次の 3 つの「グループ」レビュー担当者のそれぞれにステージを作成します。

![stages.png](assets/stages-350x239.png)

別のレビュー担当者と配達確認を共有し、期限を指定しない場合、Workfrontは期限がないステージ 3 にユーザーを追加します。 
