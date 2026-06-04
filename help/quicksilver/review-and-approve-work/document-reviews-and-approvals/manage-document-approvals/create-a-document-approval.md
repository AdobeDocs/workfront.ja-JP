---
product-area: documents
navigation-topic: approvals
title: ドキュメント承認ワークフローの作成
description: Adobe Workfront のドキュメントに対して、他のユーザーの承認をリクエストできます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OoGv4oNg6GkKeo-zoVi5lSxtPK3UE64-EYW21Mz7GRA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1473
ht-degree: 12%

---

# ドキュメント承認ワークフローの作成

{{highlighted-preview}}

Adobe Workfront のドキュメントに対して、他のユーザーやチームの承認をリクエストしたり、ドキュメントを承認する必要なく、ドキュメントのレビューをリクエストしたりできます。

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

## 実稼動環境のレガシードキュメント領域にある概要パネルから承認ワークフローを作成します

組織がWorkfront ストレージを使用している場合は、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Adobe クラウドストレージと従来のWorkfront ストレージの違い](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)を参照してください。

承認ワークフローを作成するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメント概要パネルが開きます。

1. 承認を作成するドキュメントのバージョンをバージョンのドロップダウンで選択します。 デフォルトでは、最新バージョンが選択されています。

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。


1. 次の詳細を入力します。

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、<em>初期審査</em>や<em>最終承認</em>などのより分かりやすいものに変更できます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 レビューアーしかいない場合は、通知が送信され、レビューを完了するオプションが表示されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1つの決定が必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期日（オプション）</strong></td>
   <td>承認の期日を設定します。 ユーザーとチームには、指定された期日の72時間、24時間前に電子メールで通知されます。</td>
   </tr>
   </table>

1. （オプション）前の手順を繰り返して、必要に応じてステージを追加します。

   >[!NOTE]
   >
   >複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で進みます。 必要な決定がすべて行われると、次のステージが始まり、前のステージがロックされます。

   ![ ドキュメントの詳細](assets/new-stage.png)


<div class="preview">

## プレビューのレガシードキュメント領域にある概要パネルから承認ワークフローを作成します

組織がWorkfront ストレージを使用している場合は、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Adobe クラウドストレージと従来のWorkfront ストレージの違い](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)を参照してください。

承認ワークフローを作成するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメント概要パネルが開きます。

1. バージョン ドロップダウンメニューで、承認を作成するドキュメントのバージョンを選択します。 デフォルトでは、最新バージョンが選択されています。

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。

1. 次の詳細を入力します。

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、<em>初期審査</em>や<em>最終承認</em>などのより分かりやすいものに変更できます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 レビューアーしかいない場合は、通知が送信され、レビューを完了するオプションが表示されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1つの決定のみが必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限（オプション）</strong></td>
   <td>承認の期日を設定します。 ユーザーとチームには、指定された期日の72時間、24時間前に電子メールで通知されます。</td>
   </tr>
   <tr>
   <td><strong>カスタムメッセージの追加（オプション）</strong></td>
   <td>「<strong> カスタムメッセージを追加</strong>」テキストボックスにメッセージを入力します。このメッセージは、Workfrontの承認電子メール通知および「承認」タブに表示されます。
   <p>2番目のステージを追加すると、<strong>すべてのステージでこのメッセージを表示</strong>がデフォルトで選択されます。 各段階で同じメッセージを使用するように選択したままにします。 各ステージに異なるメッセージを使用するには、<strong>すべてのステージでこのメッセージを表示</strong>をクリアし、必要に応じて各ステージの<strong> カスタムメッセージを追加</strong> テキストボックスにステージ固有のメッセージを入力します。</p></td>
   </tr>
   </table>

1. （オプション）前の手順を繰り返して、必要に応じてステージを追加します。

   >[!NOTE]
   >
   >* 複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で進みます。 必要な決定がすべて行われると、次のステージが始まり、前のステージがロックされます。
   >* 承認ワークフローの作成後にカスタムメッセージを編集すると、更新されたメール通知がすべての既存の参加者に送信されます。 後で参加者を追加すると、カスタムメッセージがメール通知に含まれます。

   ![ ステージにカスタムメッセージを追加](assets/add-custom-message.jpeg)

</div>


## 実稼動環境の新しいドキュメント領域にある概要パネルから承認ワークフローを作成します

組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

承認ワークフローを作成するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. ドキュメントをクリックし、ページの右側にある&#x200B;**承認** アイコンをクリックします。

   ![ ドキュメントの概要に承認者を追加](assets/approvals-icon-new.png)

1. 「**ワークフローを作成**」をクリックし、次の詳細を入力します。

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、<em>初期審査</em>や<em>最終承認</em>などのより分かりやすいものに変更できます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 レビューアーしかいない場合は、通知が送信され、レビューを完了するオプションが表示されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1つの決定が必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期日（オプション）</strong></td>
   <td>承認の期日を設定します。 ユーザーとチームには、指定された期日の72時間、24時間前に電子メールで通知されます。</td>
   </tr>
   </table>

1. （オプション）前の手順を繰り返して、必要に応じてステージを追加します。

   >[!NOTE]
   >
   >複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で進みます。 必要な決定がすべて行われると、次のステージが始まり、前のステージがロックされます。

   ![ ドキュメントの詳細](assets/new-stage.png)


<div class="preview">

## プレビューの新しいドキュメント領域にある概要パネルから承認ワークフローを作成します

組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

承認ワークフローを作成するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. ドキュメントをクリックし、ページの右側にある&#x200B;**承認** アイコンをクリックします。

   ![ ドキュメントの概要に承認者を追加](assets/approvals-icon-new.png)

1. 「**ワークフローを作成**」をクリックし、次の詳細を入力します。

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージ名を追加します。 名前は、<em>初期審査</em>や<em>最終承認</em>などのより分かりやすいものに変更できます。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 レビューアーしかいない場合は、通知が送信され、レビューを完了するオプションが表示されますが、決定は必要ありません。</td>
   </tr>
   <tr>
   <td><strong>1つの決定のみが必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限（オプション）</strong></td>
   <td>承認の期日を設定します。 ユーザーとチームには、指定された期日の72時間、24時間前に電子メールで通知されます。</td>
   </tr>
   <tr>
   <td><strong>カスタムメッセージの追加（オプション）</strong></td>
   <td>「<strong> カスタムメッセージを追加</strong>」テキストボックスにメッセージを入力します。このメッセージは、Workfrontの承認電子メール通知および「承認」タブに表示されます。
   <p>2番目のステージを追加すると、<strong>すべてのステージでこのメッセージを表示</strong>がデフォルトで選択されます。 各段階で同じメッセージを使用するように選択したままにします。 各ステージに異なるメッセージを使用するには、<strong>すべてのステージでこのメッセージを表示</strong>をクリアしてから、各ステージの<strong> カスタムメッセージを追加</strong> テキストボックスにステージ固有のメッセージを入力します。</p></td>
   </tr>
   </table>

1. （オプション）前の手順を繰り返して、必要に応じてステージを追加します。

   >[!NOTE]
   >
   >* 複数のステージを追加した場合、承認ワークフローはステージがリストされている順序で進みます。 必要な決定がすべて行われると、次のステージが始まり、前のステージがロックされます。
   >* 承認ワークフローの作成後にカスタムメッセージを編集すると、更新されたメール通知がすべての既存の参加者に送信されます。 後で参加者を追加すると、カスタムメッセージがメール通知に含まれます。

   ![ ステージにカスタムメッセージを追加](assets/add-custom-message.jpeg)

</div>



<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->
