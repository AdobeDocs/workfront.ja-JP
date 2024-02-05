---
product-area: documents
navigation-topic: approvals
title: ドキュメントに追加の承認者またはレビュアーを追加
description: 既に承認待ちのドキュメントに、追加の承認者またはレビュアーを追加できます。
author: Nolan
feature: Work Management, Digital Content and Documents
exl-id: f3d94dff-a855-44ae-9e85-1dcbc4d417a0
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 100%

---

# ドキュメントに追加の承認者またはレビュアーを追加

既に承認待ちのドキュメントに、追加の承認者またはレビュアーを追加できます。

>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクト、タスク、タスク、タスク、テンプレート、ポートフォリオ、プログラム、レポート、ダッシュボード、カレンダー、ドキュメントへの表示アクセス権、またはより高いレベルのアクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストのアクセスまたは承認に関連付けられたオブジェクトへの表示以上のアクセス権 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## ドキュメントページから追加の承認者またはレビュアーを追加

1. ドキュメントの名前をクリックしてドキュメントページに移動し、バージョンのドロップダウンで、承認者またはレビュアーを追加するドキュメントのバージョンを選択します。デフォルトでは最新バージョンが選択されます。

1. 左側のウィンドウで「**承認**」を選択します。既存のすべての承認者とレビュアーがここに表示されます。

1. 承認者を追加するには、「**承認者**」チェックボックスをオンにして、「**レビュアー**」テキストボックスで入力を開始することを確認します。Workfront ユーザーまたはチームは、名前で追加できます。レビュアーを追加する場合は、入力を行う前に「**承認者**」チェックボックスをオフにします。

1. 以前の手順を繰り返して、承認者またはレビュアーを追加します。

## ドキュメントの概要パネルから、追加の承認者またはレビュアーを追加

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、**ドキュメント**&#x200B;を選択します。

1. 必要なドキュメントをクリックすると、ドキュメントの概要パネルが開きます。

1. バージョンドロップダウンで、承認者またはレビュアーを追加するドキュメントのバージョンを選択します。デフォルトでは最新バージョンが選択されます。

1. 既存の承認者とレビュアーの全員が表示されるドキュメントの概要パネル内&#x200B;**承認**&#x200B;のセクションまで下にスクロールします。承認者を追加するには、「**承認者**」チェックボックスをオンにして、「**レビュアー**」テキストボックスで入力を開始することを確認します。Workfront ユーザーまたはチームは、名前で追加できます。レビュアーを追加する場合は、入力を行う前に「**承認者**」チェックボックスをオフにします。

1. 以前の手順を繰り返して、承認者またはレビュアーを追加します。

<!--
## Add additional approvers or reviewers from Home

1. Click the **Home** icon ![](assets/home-icon-30x29.png) in the upper-left corner of Adobe Workfront.

   >[!NOTE]
   >
   >Your Workfront administrator might make the following changes to the Home icon in your environment:
   >
   >* Replace it with an image customized to illustrate your organization. In this case, the icon will look different that shown in this article. 
   >* Replace the page linked to it with a different page. In this case, click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner of the page, then click **Home**.

1. In the **Work List** area, Go to the **Approvals I've Submitted** grouping.

1. Select a **Document** approval.  

1. Click **Manage Approvals**&nbsp;in the upper-right corner of the right panel.
1. In the **Have someone approve this document** box, type the name of the approver.

   If your Adobe Workfront administrator has enabled the capability to collaborate with people who don't use Workfront, as described in [Configure system security preferences](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), you can type their email addresses to include them.

1. Click **Save**.
-->
