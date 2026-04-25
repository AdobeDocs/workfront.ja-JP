---
product-area: documents
navigation-topic: approvals
title: ドキュメント承認ワークフローから承認者またはレビュー担当者を削除する
description: ドキュメントから個々の承認者またはレビュアーを削除できます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 33%

---

# ドキュメント承認ワークフローから承認者またはレビュー担当者を削除する

アセットまたはドキュメントが割り当てられた後、個々の承認者またはレビュー担当者をアセットまたはドキュメントから削除できます。

>[!IMPORTANT]
>
>この記事では、特定のアカウントでのみ利用できる更新済みのドキュメントの承認機能について説明します。 標準の承認プロセスについて詳しくは、[作業承認](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md)にリストされている記事を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>従来のWorkfrontストレージを使用して承認を管理する、あらゆるWorkfrontパッケージ</p>
<p>Adobeのエンタープライズストレージを使用して、承認を管理するあらゆるワークフローパッケージ</p>  </td> 
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
   <td> <p>プロジェクト、タスク、タスク、タスク、テンプレート、ポートフォリオ、プログラム、レポート、ダッシュボード、カレンダー、ドキュメントへの表示アクセス権、またはより高いレベルのアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストのアクセスまたは承認に関連付けられたオブジェクトへのアクセス管理 </p>  </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## レガシードキュメント領域の承認ワークフローから承認者またはレビュー担当者を削除する

組織がWorkfront ストレージを使用している場合は、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Workfront ストレージとAdobe エンタープライズストレージ &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage)の比較を参照してください。

承認ワークフローから承認者またはレビュー担当者を削除するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメント概要パネルが開きます。

1. ドキュメントの概要パネルの&#x200B;**承認** セクションまで下にスクロールします。

1. 「**ワークフローを編集**」をクリックします。

1. 削除する参加者を見つけ、名前の横にある&#x200B;**削除** アイコンをクリックします。

   承認またはレビューリクエストが削除され、承認者は、承認が不要になったという通知を受け取ります。 承認関連の共有アクセスも削除されます。

   ![承認ワークフローの編集](assets/edit-approval-in-legacy.png)

1. （オプション）承認者の役割をレビュアーに変更する場合、またはその逆の場合は、ユーザー名の横にあるドロップダウンメニューをクリックし、新しい役割を選択します。

1. 上記の手順を繰り返して、その他の承認者またはレビュアーを削除します。

</div>


## 新しいドキュメント領域の承認ワークフローへの承認者またはレビュー担当者の削除

組織でエンタープライズストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント領域が表示されます。 エンタープライズストレージについて詳しくは、[&#x200B; エンタープライズストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

承認ワークフローを作成するには、次の手順に従います。

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. ドキュメントをクリックし、ページの右側にある&#x200B;**承認** アイコンをクリックします。

   ![&#x200B; ドキュメントの概要に承認者を追加](assets/approvals-icon-new.png)


1. 「**ワークフローを編集**」をクリックします。

1. 削除する参加者を見つけ、名前の横にある&#x200B;**削除** アイコンをクリックします。

   承認またはレビューリクエストが削除され、承認者は、承認が不要になったという通知を受け取ります。

1. （オプション）承認者の役割をレビュアーに変更する場合、またはその逆の場合は、ユーザー名の横にあるドロップダウンメニューをクリックし、新しい役割を選択します。

1. 上記の手順を繰り返して、その他の承認者またはレビュアーを削除します。

   ![&#x200B; ステージから参加者を削除](assets/add-or-remove-participants.png)

1. 「**保存**」をクリックします。