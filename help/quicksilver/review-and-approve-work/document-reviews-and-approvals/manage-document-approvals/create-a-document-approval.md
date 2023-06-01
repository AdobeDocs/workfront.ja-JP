---
product-area: documents
navigation-topic: approvals
title: ドキュメントの承認の作成
description: Adobe Workfrontのドキュメントに対して、他のユーザーの承認をリクエストできます。
author: Nolan
feature: Work Management
source-git-commit: 2ae69970ebf5c72d4c192f8158bdc412c084ce35
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---


# ドキュメント承認リクエストの作成

Adobe Workfront内のドキュメントに対して、他のユーザーやチームの承認をリクエストしたり、ドキュメントを承認する必要なく、ドキュメントのレビューをリクエストしたりできます。

>[!IMPORTANT]
>
>この記事の内容は、特定のアカウントでのみ使用できる更新済みのドキュメント承認機能を指します。 標準の承認プロセスについて詳しくは、 [作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクト、タスク、タスク、タスク、テンプレート、Portfolio、プログラム、レポート、ダッシュボード、およびカレンダー、ドキュメントへのアクセス権を表示または高く表示します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストのアクセスまたは承認に関連付けられたオブジェクトへのアクセスを管理します </p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## ドキュメントページからのドキュメントの承認の作成

1. ドキュメントページに移動するには、ドキュメントの名前をクリックしてから、バージョンドロップダウンで承認を作成するドキュメントのバージョンを選択します。 デフォルトでは、最新バージョンが選択されます。

1. 選択 **承認** をクリックします。

1. 承認者を追加するには、 **承認者** 「 」チェックボックスがオンになっている場合、 **レビュー担当者** テキストボックス Workfrontユーザーまたはチームは、名前で追加できます。 レビュー担当者を追加する場合は、「 **承認者** チェックボックスをオンにして入力します。

1. 前の手順を繰り返して、承認者またはレビュー担当者を追加します。

## ドキュメントの概要ウィンドウからドキュメントの承認を作成する

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「 」を選択します。 **ドキュメント**.

1. 必要なドキュメントをクリックすると、そのドキュメントの [ ドキュメントの概要 ] ウィンドウが開きます。

1. 承認を作成するドキュメントのバージョンを「バージョン」ドロップダウンで選択します。 デフォルトでは、最新バージョンが選択されます。

1. 下にスクロールして **承認** 「ドキュメントの概要」ウィンドウの「 」セクションをクリックします。 承認者を追加するには、 **承認者** 「 」チェックボックスがオンになっている場合、 **レビュー担当者** テキストボックス Workfrontユーザーまたはチームは、名前で追加できます。 レビュー担当者を追加する場合は、「 **承認者** チェックボックスをオンにして入力します。

1. 前の手順を繰り返して、承認者またはレビュー担当者を追加します。

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![](assets/nwe-resubmit-approval-350x149.png)
-->
