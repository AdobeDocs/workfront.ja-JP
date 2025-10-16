---
product-area: documents
navigation-topic: approvals
title: ドキュメントのレビューおよび承認リクエストの作成
description: Adobe Workfront のドキュメントに対して、他のユーザーの承認をリクエストできます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 76%

---

# ドキュメントのレビューおよび承認リクエストの作成

Adobe Workfront のドキュメントに対して、他のユーザーやチームの承認をリクエストしたり、ドキュメントを承認する必要なく、ドキュメントのレビューをリクエストしたりできます。

>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

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
   <td>
   <p>投稿者以上</p>
   <p>レビュー以上</p>
   <p>Frame.io 統合を使用している場合、承認ワークフローを作成するには Standard ライセンスが必要です。</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクト、タスク、タスク、タスク、テンプレート、ポートフォリオ、プログラム、レポート、ダッシュボード、カレンダー、ドキュメントへの表示アクセス権、またはより高いレベルのアクセス権</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストのアクセスまたは承認に関連付けられたオブジェクトへのアクセス管理 </p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ドキュメントページからのドキュメントレビューまたは承認リクエストの作成

1. ドキュメントにポインタを合わせ、「ドキュメントの詳細」をクリックします。
   ![ ドキュメントの詳細 ](assets/doc-details.png)

1. ドキュメント名の近くにあるバージョンのドロップダウンで、承認を作成するドキュメントのバージョンを選択します。デフォルトでは最新バージョンが選択されます。

1. 左パネルの「**承認**」をクリックします。

1. （任意）承認の期限を設定します。 ユーザーとチームには、指定した期限の 72 時間前と 24 時間前にメールで通知が届きます。

1. 承認者を追加するには、「**承認者**」をクリックし、ユーザー名またはチーム名を入力していきます。

1. レビュアーを追加するには、「**レビュアー**」チェックボックスをオンにして、ユーザー名またはチーム名を入力していきます。

   ![ 承認者と期限を追加 ](assets/add-approver-and-deadline.png)

1. 以前の手順を繰り返して、承認者またはレビュアーを追加します。

## ドキュメントの概要パネルからのドキュメントレビューまたは承認リクエストの作成

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメントの概要ウィンドウが開きます。

1. 承認を作成するドキュメントのバージョンをバージョンのドロップダウンで選択します。デフォルトでは最新バージョンが選択されます。

1. ドキュメントの概要ウィンドウの「**承認**」セクションにスクロールして、「**追加**」をクリックします。

![ ドキュメントの概要に承認者を追加 ](assets/doc-summary-add-approvers.png)

1. （任意）承認の期限を設定します。 ユーザーとチームには、指定した期限の 72 時間前と 24 時間前にメールで通知が届きます。

1. 承認者を追加するには、「**承認者**」をクリックし、ユーザー名またはチーム名を入力していきます。

1. レビュアーを追加するには、「**レビュアー**」チェックボックスをオンにして、ユーザー名またはチーム名を入力していきます。

   ![ 承認者と期限を追加 ](assets/add-approver-and-deadline.png)

1. 以前の手順を繰り返して、承認者またはレビュアーを追加します。





<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
