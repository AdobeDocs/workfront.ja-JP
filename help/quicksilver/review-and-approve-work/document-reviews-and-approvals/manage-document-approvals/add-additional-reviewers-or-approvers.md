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
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 532
ht-degree: 18%

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



## レガシードキュメント領域のドキュメント概要から、追加の承認者またはレビュー担当者を追加します

組織がWorkfront ストレージを使用している場合は、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Adobe クラウドストレージと従来のWorkfront ストレージの違い](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)を参照してください。

ドキュメントの概要から承認者またはレビュー担当者を追加するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメント概要パネルが開きます。

1. バージョン ドロップダウンメニューで、承認者またはレビュー担当者を追加するドキュメントのバージョンを選択します。 デフォルトでは、最新バージョンが選択されています。

1. **承認** セクションまでスクロールし、**ワークフローの編集**&#x200B;をクリックします。

   ![承認ワークフローの編集](assets/edit-approval-in-legacy.png)

1. 承認者またはレビュー担当者を追加するステージを見つけ、テキストボックスにユーザーの名前またはメールを追加します。 必要に応じて、チーム全体を追加することもできます。

1. 名前が追加されたら、承認者またはレビュアーのどちらかであるかを選択します。

   ![承認者またはレビュー担当者のドロップダウン &#x200B;](assets/choose-approver-or-reviewer.png)

1. 手順5～6を繰り返して、承認者またはレビュー担当者を追加します。
保存すると、追加された参加者には、文書に対する承認またはレビューが必要であることを知らせる電子メール通知が送信されます。



## 新しいドキュメント領域のドキュメント概要から、追加の承認者またはレビュー担当者を追加します

組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。


1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. ドキュメントをクリックし、ページの右側にある&#x200B;**承認** アイコンをクリックします。

   ![&#x200B; ドキュメントの概要に承認者を追加](assets/approvals-icon-new.png)


1. 「**ワークフローを編集**」をクリックします。

1. 承認者またはレビュー担当者を追加するステージを見つけ、テキストボックスにユーザーの名前またはメールを追加します。 必要に応じて、チーム全体を追加することもできます。

1. 名前が追加されたら、承認者またはレビュアーのどちらかであるかを選択します。

   ![承認者またはレビュー担当者のドロップダウン &#x200B;](assets/choose-approver-or-reviewer.png)

1. 手順5～6を繰り返して、承認者またはレビュー担当者を追加します。
保存すると、追加された参加者には、文書に対する承認またはレビューが必要であることを知らせる電子メール通知が送信されます。







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
