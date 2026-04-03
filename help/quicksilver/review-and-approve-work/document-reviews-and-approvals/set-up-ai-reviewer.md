---
product-area: documents
navigation-topic: approvals
title: AI レビュアーの作成
description: Workfrontで少なくとも1つのブランドを設定したら、複数のAI レビューアーを作成して、承認テンプレートや個々のレビューおよび承認リクエストに割り当てることができます。
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 551f316bcfd5e0a1390e7be4679e06cd6808e969
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 19%

---

# AI レビュアーの作成

>[!NOTE]
>
>この機能は現在ベータ版です。

Workfrontで少なくとも1つのブランドを設定したら、複数のAI レビューアーを作成して、承認テンプレートや個々のレビューおよび承認リクエストに割り当てることができます。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>あなたはシステム管理者でなければなりません。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

開始する前に、Workfrontで画像ブランドガイドラインを設定する必要があります。 詳しくは、「[&#x200B; コンテンツレビュー担当者のブランドの作成と管理](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md)」を参照してください。

## AI レビュアーの追加

>[!NOTE]
>
>AI レビュアーは、レビューと承認ワークフローの意思決定者となるように設計されていません。 指定されたブランド要件に合致するスコアとレコメンデーションのみが提供されます。

コンテンツレビュアーを追加するには：

{{step-1-to-setup}}

1. 左側のパネルで、**レビューと承認** > **AI レビューアー**&#x200B;に移動します。
1. 「**新規追加**」をクリックします。
1. レビュアーに名前を付けます。
1. **ブランド**&#x200B;を選択します。
1. 「**ガイドラインの種類**」ドロップダウンメニューで、次のいずれかを選択します。
   * **画像**: AI レビュアーは、Workfrontで設定した画像ブランドガイドラインに照らし合わせてアセットをレビューします。
   * **ブランドボイス**: AI レビュアーは、Workfrontで設定したブランドボイスのガイドラインに照らし合わせてアセットをレビューします。
1. 「**作成**」をクリックします。

   AI レビュー担当者が作成されたら、ユーザーはAI レビュー担当者を承認テンプレートや個人承認に追加できます。

   詳しくは、次を参照してください。

   * [ドキュメントの承認ワークフローテンプレートの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
