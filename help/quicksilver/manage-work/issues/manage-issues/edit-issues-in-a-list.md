---
product-area: projects
navigation-topic: manage-issues
title: リストでイシューを編集
description: 個々のイシューを編集することも、イシューリストまたはレポート内のイシューを編集することもできます。この記事では、リスト内のイシューを編集する方法について説明します。
author: Alina
feature: Work Management
exl-id: a3276d83-c08f-4480-9092-aa47ba76d794
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 81%

---

# リスト内のイシューの編集

<!--Audited: 08/2025-->

個々のイシューを編集することも、イシューリストまたはレポート内のイシューを編集することもできます。この記事では、リスト内のイシューを編集する方法について説明します。

個々のイシューの編集について詳しくは、[イシューの編集](../../../manage-work/issues/manage-issues/edit-issues.md)を参照してください。

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

<ul><li><p>投稿者以上</p> </li>
   <li><p>プロジェクトの「イシュー」セクションでイシューを編集するためのライト以上のライセンス</p></li></ul> 
    または
   <ul><li><p>要求者以上</p> </li>
   <li><p>プロジェクトの「イシュー」セクションでイシューを編集するためのレビュアー以上のライセンス</p></li></ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>イシューに対する参加以上の権限</p> <p> イシューに関する権限の付与については、<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">イシューの共有</a>を参照してください。</p> <p>追加権限の要求については、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権の要求</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to edit issues in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the issue</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## イシューのインライン編集

リストのビューに表示されるインライン編集フィールドを使用して、イシューのリスト内のイシュー情報を編集できます。

リスト内のイシューを編集する際は、次の点を考慮してください。

* リストに表示され、更新する権限を持つイシューフィールドを編集できます。
* 以下のリスト内にあるイシューを編集できます。

   * プロジェクトまたはタスクの「イシュー」セクション
   * イシューレポート

イシューをインライン編集するには：

1. プロジェクトまたはタスク内のイシューのリストに移動します。
1. 手動で更新する権限を持つフィールド内をクリックします。フィールドが編集可能になり、変更を加えることができます。

   ![&#x200B; 問題をインラインで編集 &#x200B;](assets/edit-issues-inline-350x34.png)

1. 変更を受け入れる場合は、Enter キーを押します。変更は直ちに保存されます。

   オブジェクトのインライン編集について詳しくは、[Adobe Workfront のリスト内の項目のインライン編集](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)を参照してください。

## リストからイシューを編集

1. プロジェクトまたはタスク内のイシューのリストに移動します。
1. 次のいずれかの操作を行います。

   * リストでイシューを選択し、ツールバーの **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/qs-edit-icon.png) をクリックします。
   * イシューの名前をクリックし、「**編集**」をクリックします。

     これらのアクションのいずれかを実行すると、「**イシューを編集** ボックスが開きます。

     **イシューを編集** ボックスでのイシューの編集について詳しくは、[&#x200B; イシューの編集 &#x200B;](../../../manage-work/issues/manage-issues/edit-issues.md) を参照してください。

## 概要を使用してイシューを編集

概要パネルを使用して、リストのイシューを編集できます。

1. 編集するイシューを含むプロジェクトに移動します。
1. 左側のパネルで「**イシュー**」をクリックします。

   プロジェクトのイシューのリストが表示されます。

1. 編集するイシューを選択し、イシューリストの右上隅にある **概要を開く** アイコン ![&#x200B; 概要を開くアイコン &#x200B;](assets/qs-open-summary-icon-in-new-toolbar-small.png) をクリックします。

   **概要**&#x200B;が開きます。

1. （オプション）**更新**&#x200B;エリアでイシューの更新を入力し始めます。
1. 次のアイコンまたはエリアのいずれかをクリックしてイシューに移動し、次のイシューのレベルで情報を編集します。

   | アイコン | アクション |
   |---|---|
   | ドキュメント ![&#x200B; ドキュメントアイコン &#x200B;](assets/documents-icon-in-summary.png) | 「**ここをクリックして追加**」をクリックして、イシューにドキュメントを追加します。 |
   | 詳細 ![&#x200B; 詳細アイコン &#x200B;](assets/details-icon-in-summary.png) | クリックして、イシューに関する情報を更新します。 |
   | 時間 ![&#x200B; 時間を記録 &#x200B;](assets/log-time-icon-in-summary.png) | クリックして時間を記録します。 |
   | 承認 ![&#x200B; 承認アイコン &#x200B;](assets/approvals-icon-in-summary.png) | クリックして、イシューの承認を追加します。 |

1. （オプション）**概要を開く**&#x200B;アイコンを再びクリックするか、概要の右上にある&#x200B;**X アイコン**&#x200B;をクリックしてパネルを閉じ、イシューをインラインで編集します。

## イシューを一括で編集

イシューを一括で編集し、そのすべての情報を同時に更新できます。

イシューを一括で編集するには、次の手順に従います。

1. **メインメニュー**&#x200B;に移動します。
1. 「**プロジェクト**」をクリックします。
1. プロジェクト名をクリックして、プロジェクトにアクセスします。
1. 左側のパネルで「**イシュー**」をクリックします。
1. リストから複数のイシューを選択します。
1. **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックします。

   **イシューを編集**&#x200B;ダイアログボックスが開きます。

1. 選択したすべてのイシューに関する情報を指定します。

   すべてのイシューに関する情報を編集するのは、次のエリアを編集する際に、1 つのイシューに関する情報を編集する場合と同じです。

   * 概要
   * 設定
   * 割り当て
   * コメント

   イシューの編集について詳しくは、[イシューの編集](../../../manage-work/issues/manage-issues/edit-issues.md)を参照してください。

   >[!NOTE]
   >
   >「**割り当て**」フィールドを除き、選択したすべてのイシューについて変更する情報は、個々のイシューに関する既存の情報を上書きします。一括編集で新しい担当者を追加すると、その担当者は選択したすべてのイシューに追加されます。選択したイシューに他の担当者が割り当てられている場合、一括編集で追加されたイシューに加えて、割り当てられたままになります。

1. 「**カスタムフォーム**」をクリックして、選択したすべてのイシューに添付されているカスタムフォームを編集します。

   選択したイシューに共通するカスタムフォームがない場合、このセクションにはフォームが表示されません。

   選択したすべてのイシューに添付され、編集権限を持つフォーム上のフィールドのみを編集できます。

1. （オプション）**カスタムフォーム**&#x200B;エリアで、「**カスタム式を再計算**」オプションを使用して、選択したイシューに関連付けられているカスタムフォーム上の計算カスタムフィールドをすべて最新の状態に保つことができます。

   >[!IMPORTANT]
   >
   >カスタム式を再計算する場合は、一度に 500 件を超えるイシューを選択しないことをお勧めします。

1. 「**変更を保存**」をクリックします。

   選択したすべてのイシューに対して、行った変更がすべて表示されます。
