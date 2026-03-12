---
product-area: documents
navigation-topic: approvals
title: ドキュメント承認ワークフローの作成
description: Adobe Workfront のドキュメントに対して、他のユーザーの承認をリクエストできます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: 149c8adcf886f837bc94ac78f8a3ea54c47e375c
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 32%

---

# ドキュメント承認ワークフローの作成

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。プレビューサンドボックス環境でのみ使用できます。</span>

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
   <p>コントリビューター以上</p>
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


## 実稼動環境のドキュメントページから、ドキュメントレビューまたは承認リクエストを作成します

1. ドキュメントにポインタを合わせ、「ドキュメントの詳細」をクリックします。
   ![ ドキュメントの詳細 ](assets/doc-details.png)

1. ドキュメント名の近くにあるバージョンのドロップダウンで、承認を作成するドキュメントのバージョンを選択します。デフォルトでは、最新バージョンが選択されています。

1. 左パネルの「**承認**」をクリックします。

1. （任意）承認の期限を設定します。 ユーザーとチームには、指定した期限の 72 時間前と 24 時間前にメールで通知が届きます。

1. 承認者を追加するには、[ 承認者 **をクリックし** ユーザー名またはチーム名を入力します。

1. レビュアーを追加するには、「**レビュアー**」チェックボックスをオンにして、ユーザー名またはチーム名を入力していきます。

   ![ 承認者と期限を追加 ](assets/add-approver-and-deadline.png)

1. 以前の手順を繰り返して、承認者またはレビュアーを追加します。

## 実稼動環境のドキュメントの概要パネルから、ドキュメントレビューまたは承認リクエストを作成します

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメントの概要左パネルが開きます。

1. 承認を作成するドキュメントのバージョンをバージョンのドロップダウンで選択します。デフォルトでは、最新バージョンが選択されています。

1. ドキュメントの概要ウィンドウの「**承認**」セクションにスクロールして、「**追加**」をクリックします。

![ ドキュメントの概要に承認者を追加 ](assets/doc-summary-add-approvers.png)

1. （任意）承認の期限を設定します。 ユーザーとチームには、指定した期限の 72 時間前と 24 時間前にメールで通知が届きます。

1. 承認者を追加するには、[ 承認者 **をクリックし** ユーザー名またはチーム名を入力します。

1. レビュアーを追加するには、「**レビュアー**」チェックボックスをオンにして、ユーザー名またはチーム名を入力していきます。

   ![ 承認者と期限を追加 ](assets/add-approver-and-deadline.png)

1. 以前の手順を繰り返して、承認者またはレビュアーを追加します。

<div class="preview">

## レガシードキュメント領域のプレビュー環境の概要パネルで承認ワークフローを作成します

組織がWorkfront ストレージ上にある場合、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Workfront ストレージとAdobe エンタープライズストレージの比較 ](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage) を参照してください。

承認ワークフローを作成するには：

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、左パネルで **ドキュメント** を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメント概要パネルが開きます。

1. 承認を作成するドキュメントのバージョンをバージョンのドロップダウンで選択します。デフォルトでは、最新バージョンが選択されています。

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。


1. 次の詳細を入力します。

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、「最初のレビュー」や「<em> 最終承認 </em> など、よりわかりやすい名前 <em> 変更 </em> きます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>ユーザー名またはチーム名の入力を開始して、承認者またはレビュアーとして追加します。 レビュー担当者のみが存在する場合、レビュー担当者に通知され、レビューを完了するオプションが提供されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1 つの決定が必要（オプション）</strong></td>
   <td>最初に決定を行ったユーザーがステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限（オプション）</strong></td>
   <td>承認期限を設定します。 ユーザーとチームには、指定した期日の 72 時間前、つまり 24 時間前にメールで通知が届きます。</td>
   </tr>
   </table>

1. （オプション）必要に応じて、前の手順を繰り返して追加のステージを追加します。

   >[!NOTE]
   >
   >複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で続行されます。 必要な決定がすべて行われると、次のステージが開始され、前のステージがロックされます。

   ![ ドキュメントの詳細 ](assets/new-stage.png)

</div>

## 新しいドキュメント領域の概要パネルから承認ワークフローを作成する

エンタープライズストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 エンタープライズストレージについて詳しくは、[ エンタープライズストレージの概要 ](/help/quicksilver/review-and-approve-work/esm-overview.md) を参照してください。

承認ワークフローを作成するには：

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、左パネルで **ドキュメント** を選択します。

1. ドキュメントをクリックしてから、ページの右側にある「承認」アイコンをクリックします。

   ![ ドキュメントの概要に承認者を追加 ](assets/approvals-icon-new.png)

1. **ワークフローを作成** をクリックし、次の詳細を入力します。

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、「最初のレビュー」や「<em> 最終承認 </em> など、よりわかりやすい名前 <em> 変更 </em> きます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>ユーザー名またはチーム名の入力を開始して、承認者またはレビュアーとして追加します。 レビュー担当者のみが存在する場合、レビュー担当者に通知され、レビューを完了するオプションが提供されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1 つの決定が必要（オプション）</strong></td>
   <td>最初に決定を行ったユーザーがステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限（オプション）</strong></td>
   <td>承認期限を設定します。 ユーザーとチームには、指定した期日の 72 時間前、つまり 24 時間前にメールで通知が届きます。</td>
   </tr>
   </table>

1. （オプション）必要に応じて、前の手順を繰り返して追加のステージを追加します。

   >[!NOTE]
   >
   >複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で続行されます。 必要な決定がすべて行われると、次のステージが開始され、前のステージがロックされます。

   ![ ドキュメントの詳細 ](assets/new-stage.png)



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
