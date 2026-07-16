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
source-git-commit: 632c8690acc30121fe72338326ec8ab58c0fd3a6
workflow-type: tm+mt
source-wordcount: 2231
ht-degree: 6%

---

# ドキュメント承認ワークフローの作成

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

<!--

## Create an approval workflow in the legacy documents area in Production

If your organization is on Workfront storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront storage, see [Differences between Adobe cloud storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document you need and the Document Summary panel for that document opens.

1. Select the version of the document you would like to create an approval for in the version dropdown. The latest version is selected by default.

1. Scroll down to the **Approvals** section, then click **Create workflow**.


1. Fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)

-->

## レガシードキュメント領域での承認ワークフローの作成

組織がWorkfront ストレージを使用している場合は、Workfrontでドキュメントにアクセスすると、従来のドキュメント領域が表示されます。 Workfront ストレージについて詳しくは、[Adobe クラウドストレージと従来のWorkfront ストレージの違い](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage)を参照してください。

### 基本的な承認ワークフローの作成

1段階の承認ワークフローを作成するには、次の手順に従います。

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメント概要パネルが開きます。

1. バージョン ドロップダウンメニューで、承認を作成するドキュメントのバージョンを選択します。 デフォルトでは、最新バージョンが選択されています。

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。 **承認依頼** ダイアログが基本モードで開きます。

1. 次の詳細を入力します。

   <table>
   <tr>
   <td><strong>承認テンプレートの使用（オプション）</strong></td>
   <td>ドロップダウンメニューからテンプレートを選択します。 テンプレートに1つのパスと1つのステージがある場合は、基本モードで適用されます。 テンプレートに複数のステージまたは複数のパスがある場合、ダイアログは自動的に詳細モードに切り替わり、基本モードで入力した入力は、テンプレートのコンテンツに置き換えられます。</td>
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
   <td>「<strong> カスタムメッセージを追加</strong>」テキストボックスにメッセージを入力します。 このメッセージは、Workfrontの承認電子メール通知および「承認」タブに表示されます。
   <p>注意：承認ワークフローの作成後にカスタムメッセージを編集すると、更新されたメール通知がすべての既存の参加者に送信されます。 後で参加者を追加すると、カスタムメッセージがメール通知に含まれます。</p>
   </td>
   </tr>
   </table>

1. 「**承認を依頼**」をクリックします。

   ![基本モードで承認を要求](assets/request-approval-basic.jpeg)

### 高度な承認ワークフローの作成

高度なモードでは、複数のステージと並行パスをサポートしています。 各パスは独立して実行され、1つ以上のシーケンシャルステージを含みます。 ステージで必要なすべての意思決定が行われると、そのパスの次のステージが開始され、前のステージがロックされ、新しいステージのレビュー担当者と承認者にメール通知が送信されます。

「作業が必要です」という決定は、そのパスを停止しますが、他のパスの承認ワークフローには影響しません。 最大30個のパスと合計100個のステージを設定できます。

高度な承認ワークフローを作成するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. 必要なドキュメントをクリックすると、そのドキュメントのドキュメント概要パネルが開きます。

1. バージョン ドロップダウンメニューで、承認を作成するドキュメントのバージョンを選択します。 デフォルトでは、最新バージョンが選択されています。

1. 「**承認**」セクションまでスクロールし、「**ワークフローを作成**」をクリックします。

1. **承認を依頼** ダイアログの右上にある「**詳細に移動**」をクリックします。 基本モードで入力した入力はすべて保持され、**パス 1**、**ステージ 1**&#x200B;に適用されます。

   >[!TIP]
   >
   >承認の作成中に、右上の「**基本に移動**」をクリックして基本モードに戻ることができます。 **承認を依頼**&#x200B;をクリックすると、**基本に移動** オプションは使用できなくなります。

1. パス 1のステージ 1の詳細を入力：

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージには、デフォルトで<em> ステージ 1</em>、<em> ステージ 2</em>などの名前が付けられます。 ステージの名前を、<em>初期審査</em>や<em>最終承認</em>などのより記述的な名前に変更します。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 レビューアーしかいない場合は、通知が送信され、レビューを完了するオプションが表示されますが、決定は必要ありません。<p>注意：レビュアーまたは承認者は、同じアセットで一度に1つのオープンステージにのみ割り当てることができます。 複数の並行ステージが同時に開いている場合、同じ人物を複数に追加することはできません。</p></td>
   </tr>
   <tr>
   <td><strong>1つの決定のみが必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限（オプション）</strong></td>
   <td>各パスの最初のステージでは、絶対期日をサポートします。 パス内の後続の各ステージは、相対的な期日（そのステージが開くまでの日数）をサポートします。 ユーザーとチームには、期日の72時間、24時間前にメールで通知されます。</td>
   </tr>
   <tr>
   <td><strong>カスタムメッセージの追加（オプション）</strong></td>
   <td>「<strong> カスタムメッセージを追加</strong>」テキストボックスにメッセージを入力します。 このメッセージは、Workfrontの承認電子メール通知および「承認」タブに表示されます。<p>2番目のステージを追加すると、<strong>すべてのステージでこのメッセージを表示</strong>がデフォルトで選択されます。 各段階で同じメッセージを使用するように選択したままにします。 各ステージに異なるメッセージを使用するには、<strong>すべてのステージでこのメッセージを表示</strong>をクリアしてから、各ステージの<strong> カスタムメッセージを追加</strong> テキストボックスにステージ固有のメッセージを入力します。</p></td>
   </tr>
   </table>

1. （オプション）「**ステージを追加**」をクリックして、パスに別のステージを追加します。 パス内のステージは、リストされている順序で順次実行されます。 パス内のステージを並べ替えることはできますが、あるパスから別のパスにステージを移動することはできません。 各パスには異なる数のステージを設定できます。

1. （オプション）「**並列パス**」で、「**パスを追加**」をクリックして別のパスを追加します。 新しいパスは、1つの空のステージから始まり、選択したパスになります。 パスの名前を変更するには、パスのラベルにカーソルを合わせて鉛筆アイコンをクリックし、新しい名前を入力します。

1. （オプション）パスを削除するには、パスラベルにカーソルを合わせて、ごみ箱アイコンをクリックします。 **パス 1**&#x200B;を削除できません。パスを並べ替えることはできません。 その他のパスは、パス内のステージがロックまたは完了していない場合にのみ削除できます。

   ![並列パスを使用した詳細設定モード &#x200B;](assets/request-approval-parallel-paths.jpeg)

1. （オプション）すべてのパスとステージをクリアして最初からやり直すには、右上の「**リセット**」をクリックします。

1. 「**承認を依頼**」をクリックします。


<!--

## Create an approval workflow in the new Documents area in Production

If your organization uses Adobe cloud storage, you will see the new Documents area when you access documents in Workfront. For more information about Adobe cloud storage, see [Adobe cloud storage overview](/help/quicksilver/review-and-approve-work/esm-overview.md).

To create an approval workflow:

1. Go to the project, task, or issue that contains the document, then select **Documents** in the left panel.

1. Click on the document, then click the **Approvals** icon on the right side of the page.

   ![Add approvers in document summary](assets/approvals-icon-new.png)

1. Click **Create workflow**, then fill in the following details:

   <table>
   <tr>
   <td><strong>Stage name</strong></td>
   <td>Add a stage name. You can change the name to something more descriptive, such as <em>Initial Review</em> or <em>Final Approval</em>.</td>
   </tr>
   <tr>
   <td><strong>Add names or emails</strong></td>
   <td>Begin typing a user or team name to add as an approver or reviewer. If you only have reviewers, they will be notified and have the option to complete the review but no decision will be required or made.</td>
   </tr>
   <tr>
   <td><strong>One decision required (optional)</strong></td>
   <td>The first person who makes a decision completes the stage.</td>
   </tr>
   <tr>
   <td><strong>Due date (optional)</strong></td>
   <td>Set a due date for the approval. Users and teams are notified by email 72 hours, then 24 hours before the specified due date.</td>
   </tr>
   </table>

1. (Optional) Repeat the previous step to add additional stages as needed.

   >[!NOTE]
   >
   >If you add multiple stages, the approval workflow proceeds in the order the stages are listed. When all required decisions are made, the next stage begins and the previous stage is locked.

   ![Document details](assets/new-stage.png)
   
-->

## 新しいドキュメント領域での承認ワークフローの作成

組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

**承認依頼** ダイアログは、デフォルトで&#x200B;**基本** モードで開きます。 基本モードは、承認者またはレビュー担当者のセットを持つ単一のステージです。 **詳細** モードに切り替えて、多段階の承認または並列パスを設定します。

### 基本的な承認ワークフローの作成

1段階の承認ワークフローを作成するには、次の手順に従います。

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. ドキュメントをクリックし、ページの右側にある&#x200B;**承認** アイコンをクリックします。

   ![&#x200B; ドキュメントの概要に承認者を追加](assets/approvals-icon-new.png)

1. 「**ワークフローを作成**」をクリックします。 **承認依頼** ダイアログが基本モードで開きます。

1. 次の詳細を入力します。

   <table>
   <tr>
   <td><strong>承認テンプレートの使用（オプション）</strong></td>
   <td>デフォルトでは、「テンプレート」フィールドは折りたたまれています。 フィールドをクリックして展開し、ドロップダウンメニューからテンプレートを選択します。 テンプレートに1つのパスと1つのステージがある場合は、基本モードで適用されます。 テンプレートに複数のステージまたは複数のパスがある場合、ダイアログは自動的に詳細モードに切り替わり、基本モードで入力した入力は、テンプレートのコンテンツに置き換えられます。</td>
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
   <td>「<strong> カスタムメッセージを追加</strong>」テキストボックスにメッセージを入力します。 このメッセージは、Workfrontの承認電子メール通知および「承認」タブに表示されます。</td>
   </tr>
   </table>

1. 「**承認を依頼**」をクリックします。

   ![基本モードで承認を要求](assets/request-approval-basic.jpeg)

>[!NOTE]
>
>* 以前のセッションに関係なく、毎回&#x200B;**承認依頼** ダイアログが基本モードで開きます。
>* 承認ワークフローの作成後にカスタムメッセージを編集すると、更新されたメール通知がすべての既存の参加者に送信されます。 後で参加者を追加すると、カスタムメッセージがメール通知に含まれます。
>* 承認を保存した後は、基本モードに戻すことはできません。 進行中の承認は、承認がロックされていないか完了していない限り、「基本」から「詳細」に切り替えることができます。

### 高度な承認ワークフローの作成

高度なモードは並列パスをサポートしています。 各パスは独立して実行され、1つ以上のシーケンシャルステージを含みます。 ステージで必要なすべての意思決定が行われると、そのパスの次のステージが開始され、前のステージがロックされ、新しいステージのレビュー担当者と承認者にメール通知が送信されます。

「作業が必要です」という決定は、そのパスを停止しますが、他のパスの承認ワークフローには影響しません。 最大30個のパスと合計100個のステージを設定できます。

高度な承認ワークフローを作成するには：

1. ドキュメントを含むプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。

1. ドキュメントをクリックし、ページの右側にある&#x200B;**承認** アイコンをクリックします。

   ![&#x200B; ドキュメントの概要に承認者を追加](assets/approvals-icon-new.png)

1. 「**ワークフローを作成**」をクリックします。

1. **承認を依頼** ダイアログの右上にある「**詳細に移動**」をクリックします。 基本モードで入力した入力はすべて保持され、**パス 1**、**ステージ 1**&#x200B;に適用されます。

   >[!TIP]
   >
   >承認の作成中に、右上の「**基本に移動**」をクリックして基本モードに戻ることができます。 **承認を依頼**&#x200B;をクリックすると、**基本に移動** オプションは使用できなくなります。

1. パス 1のステージ 1の詳細を入力：

   <table>
   <tr>
   <td><strong>ステージ名</strong></td>
   <td>ステージには、デフォルトで<em> ステージ 1</em>、<em> ステージ 2</em>などの名前が付けられます。 ステージの名前を、<em>初期審査</em>や<em>最終承認</em>などのより記述的な名前に変更します。</td>
   </tr>
   <tr>
   <td><strong>名前またはメールを追加</strong></td>
   <td>承認者またはレビュアーとして追加するユーザー名またはチーム名の入力を開始します。 レビューアーしかいない場合は、通知が送信され、レビューを完了するオプションが表示されますが、決定は必要ありません。<p>注意：レビュアーまたは承認者は、同じアセットで一度に1つのオープンステージにのみ割り当てることができます。 複数の並行ステージが同時に開いている場合、同じ人物を複数に追加することはできません。</p></td>
   </tr>
   <tr>
   <td><strong>1つの決定のみが必要です（オプション）</strong></td>
   <td>最初に決定を下した人がステージを完了します。</td>
   </tr>
   <tr>
   <td><strong>期限（オプション）</strong></td>
   <td>各パスの最初のステージでは、絶対期日をサポートします。 パス内の後続の各ステージは、相対的な期日（そのステージが開くまでの日数）をサポートします。 ユーザーとチームには、期日の72時間、24時間前にメールで通知されます。</td>
   </tr>
   <tr>
   <td><strong>カスタムメッセージの追加（オプション）</strong></td>
   <td>「<strong> カスタムメッセージを追加</strong>」テキストボックスにメッセージを入力します。 このメッセージは、Workfrontの承認電子メール通知および「承認」タブに表示されます。<p>2番目のステージを追加すると、<strong>すべてのステージでこのメッセージを表示</strong>がデフォルトで選択されます。 各段階で同じメッセージを使用するように選択したままにします。 各ステージに異なるメッセージを使用するには、<strong>すべてのステージでこのメッセージを表示</strong>をクリアしてから、各ステージの<strong> カスタムメッセージを追加</strong> テキストボックスにステージ固有のメッセージを入力します。</p></td>
   </tr>
   </table>

1. （オプション）「**ステージを追加**」をクリックして、パスに別のステージを追加します。 パス内のステージは、リストされている順序で順次実行されます。 パス内のステージを並べ替えることはできますが、あるパスから別のパスにステージを移動することはできません。 各パスには異なる数のステージを設定できます。


1. （オプション）「**並列パス**」で、「**パスを追加**」をクリックして別のパスを追加します。 新しいパスは、1つの空のステージから始まり、選択したパスになります。 パスの名前を変更するには、パスのラベルにカーソルを合わせて鉛筆アイコンをクリックし、新しい名前を入力します。

1. （オプション）パスを削除するには、パスラベルにカーソルを合わせて、ごみ箱アイコンをクリックします。 **パス 1**&#x200B;を削除できません。パスを並べ替えることはできません。 その他のパスは、パス内のステージがロックまたは完了していない場合にのみ削除できます。

   ![並列パスを使用した詳細設定モード &#x200B;](assets/request-approval-advanced.jpeg)

1. （オプション）すべてのパスとステージをクリアして最初からやり直すには、右上の「**リセット**」をクリックします。

1. 「**承認を依頼**」をクリックします。

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![Resubmit approval](assets/nwe-resubmit-approval-350x149.png)
-->