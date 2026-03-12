---
product-area: documents
navigation-topic: approvals
title: ドキュメント承認ワークフローへの承認者またはレビュー担当者の追加
description: 既に承認待ちのドキュメントに、追加の承認者またはレビュアーを追加できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 25%

---

# ドキュメント承認ワークフローへの承認者またはレビュー担当者の追加

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

既に承認待ちになっているドキュメント承認ワークフローに、別の承認者またはレビュー担当者を追加できます。

>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>コントリビューター以上</p>
   <p>レビュー以上</p> 
   <p>Frame.io 統合を使用している場合、承認ワークフローを作成するには Standard ライセンスが必要です。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクト、タスク、問題、テンプレート、ポートフォリオ、プログラム、報告書、ダッシュボード、カレンダー、およびドキュメントへの表示以上のアクセス</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストのアクセスまたは承認に関連付けられたオブジェクトへの表示以上のアクセス権 </p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 実稼動環境のドキュメントの詳細ページから、追加の承認者またはレビュー担当者を追加します

1. ドキュメントの名前をクリックしてドキュメントページに移動し、承認者またはレビュアーを追加するドキュメントのバージョンを「バージョン」ドロップダウンメニューで選択します。 デフォルトでは、最新バージョンが選択されています。

1. 左側のパネルで **承認** を選択します。 既存のすべての承認者とレビュアーがここに表示されます。

1. 承認者を追加するには、「承認者 **のチェックボックスがオンになっている** とを確認し、「レビュー担当者 **テキストボックスに入力し** す。 Workfront ユーザーまたはチームは、名前で追加できます。レビュアーを追加する場合は、入力を行う前に「**承認者**」チェックボックスをオフにします。

1. 以前の手順を繰り返して、承認者またはレビュアーを追加します。

## 実稼動環境のドキュメントの概要から、追加の承認者またはレビュー担当者を追加します

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、ドキュメントの概要パネルが開きます。

1. 承認者またはレビュアーを追加するドキュメントのバージョンをバージョン ドロップダウン メニューで選択します。 デフォルトでは、最新バージョンが選択されています。

1. ドキュメントの概要パネルの「**承認**」セクションまでスクロールします。このセクションには、既存の承認者とレビュー担当者がすべて表示されます。 承認者を追加するには、「承認者 **のチェックボックスがオンになっている** とを確認し、「レビュー担当者 **テキストボックスに入力し** す。 Workfront ユーザーまたはチームは、名前で追加できます。レビュアーを追加する場合は、入力を行う前に「**承認者**」チェックボックスをオフにします。

1. 以前の手順を繰り返して、承認者またはレビュアーを追加します。

<div class="preview">

## レガシードキュメント領域のプレビュー環境のドキュメントの概要から、追加の承認者またはレビュー担当者を追加します

組織がWorkfront ストレージ上にある場合、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Workfront ストレージとAdobe エンタープライズストレージの比較 ](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage) を参照してください。

ドキュメントの概要から追加の承認者またはレビュー担当者を追加するには：

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、左パネルで **ドキュメント** を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメント概要パネルが開きます。

1. 承認者またはレビュアーを追加するドキュメントのバージョンをバージョン ドロップダウン メニューで選択します。 デフォルトでは、最新バージョンが選択されています。

1. 「**承認**」セクションまでスクロールし、「**ワークフローを編集**」をクリックします。

   ![ 承認ワークフローを編集 ](assets/edit-approval-in-legacy.png)

1. 承認者またはレビュー担当者を追加するステージを見つけ、テキストボックスにユーザーの名前またはメールを追加します。 必要に応じて、チーム全体を追加することもできます。

1. 名前を追加したら、承認者かレビュアーかを選択します。

   ![ 承認者またはレビュアードロップダウン ](assets/choose-approver-or-reviewer.png)

1. 手順 5～6 を繰り返して、承認者またはレビュー担当者を追加します。
保存すると、追加された参加者には、ドキュメントで承認またはレビューが必要であることを通知するメール通知が届きます。

</div>


## 新しいドキュメント領域のドキュメントの概要からさらに承認者またはレビュー担当者を追加します

エンタープライズストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 エンタープライズストレージについて詳しくは、[ エンタープライズストレージの概要 ](/help/quicksilver/review-and-approve-work/esm-overview.md) を参照してください。


1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、左パネルで **ドキュメント** を選択します。

1. ドキュメントをクリックしてから、ページの右側にある **承認** アイコンをクリックします。

   ![ ドキュメントの概要に承認者を追加 ](assets/approvals-icon-new.png)


1. **ワークフローを編集** をクリックします。

1. 承認者またはレビュー担当者を追加するステージを見つけ、テキストボックスにユーザーの名前またはメールを追加します。 必要に応じて、チーム全体を追加することもできます。

1. 名前を追加したら、承認者かレビュアーかを選択します。

   ![ 承認者またはレビュアードロップダウン ](assets/choose-approver-or-reviewer.png)

1. 手順 5～6 を繰り返して、承認者またはレビュー担当者を追加します。
保存すると、追加された参加者には、ドキュメントで承認またはレビューが必要であることを通知するメール通知が届きます。







<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![Home icon](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
