---
product-area: projects
navigation-topic: update-work-in-a-project
title: タスク状態の更新
description: タスクのステータスを更新すると、タスクの場所（およびプロジェクト全体）と進行状況を他のユーザーに通知できます。
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 66%

---

# タスクステータスの更新

<!--Audited: 10/2024-->

タスクのステータスを更新すると、タスクの場所（およびプロジェクト全体）と進行状況を他のユーザーに通知できます。

デフォルトのステータスは、「新規」、「処理中」および「完了」です。Adobe Workfront 管理者は、組織のカスタムステータスを追加できます。詳しくは、[ステータスの作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

タスクのステータスは、手動で更新することも、特定のアクションが実行されたときに Workfront で自動的に更新することもできます。

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
   <td> <p>標準</p> 
   <p>ワークまたはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクへのアクセスを編集</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する管理権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p> 
   Or
   <p>Current: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## タスクのステータスの更新に関する考慮事項

* タスクを完了としてマークすると、タスクの完了率は 100％に更新されます。
* 親タスクには、次のシナリオが存在します。
   * プロジェクトの概要完了モードが [ 自動 ] に設定され、サブタスクが完了していない場合、親タスクの状態を [ 完了 ] に更新することはできません。
   * プロジェクトの概要完了モードを「手動」に設定し、サブタスクが完了または未完了の場合、親タスクのステータスを「完了」に更新できます。

  詳しくは、[プロジェクトの編集](../manage-projects/edit-projects.md)を参照してください。

## タスクのステータスを手動で更新

次の領域でタスクステータスを更新できます。

* タスクページのタスクヘッダー。
* タスクの編集時の「タスクを編集」ボックス。
* タスクページの「タスクの詳細」セクション。
* タスク リストまたは報告書で、[ 状態 ] フィールドがビューに表示されている場合。
* タスクの概要パネル内。

タスクヘッダーのタスクステータスを手動で更新するには：

1. 状態を更新するタスクに移動します。
1. タスクヘッダーで「**ステータス**」フィールドをクリックし、新しいステータスを選択します。
1. タスクの完了を視覚的に示すには、タスクのヘッダーにある **完了率** の下のバブルをドラッグします。

   または

   **完了率** バブル内をダブルクリックして、新しいパーセンテージを手動で入力します。

   ![](assets/percent-complete-status-widgets-task-header.png)

1. （オプション）更新に関する追加情報を指定するには、次のいずれかの操作を行います。

   * 更新に関するメモを追加するには、「**更新**」セクションに移動し、「**新しいコメント**」をクリックして、メモを入力します。

     ![&#x200B; タスクへの更新の追加 &#x200B;](assets/add-update-to-task.png)

   * 特定のユーザーに更新について通知するには、コメントを入力した際に表示される「**人物またはチームにタグ付け**」フィールドにユーザーの名前を入力します。詳しくは、[更新時の他のユーザーへのタグ付け](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。
   * タスクのコミット日を更新するには、「**タスクの詳細**」をクリックし、「**コミット日**」フィールドを編集します。 詳しくは、[タスクを編集](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。


   >[!IMPORTANT]
   >
   >  コミット日を更新できるのは、タスクの担当者のみです。

<!--old functionality in old commenting: 

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![](assets/drag-the-progress-bar-350x155.png)-->

## タスクのステータスを自動的に更新

Workfront は、以下の表に示すアクションが発生すると、タスクの既存のステータスを別のステータスに自動的に更新します。

>[!NOTE]
>
>以下の表のステータスは、デフォルトのシステムステータスです。Workfront 管理者またはグループ管理者は、Workfront のインスタンスでステータスの名前を変更できます。Workfront でのステータスの作成と管理について詳しくは、[ステータスを作成または編集](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>アクション</b></td> 
   <td><b>元のステータス</b></td> 
   <td><b>新しいステータス</b></td> 
  </tr> 
  <tr> 
   <td>タスクの完了率を 100％に更新</td> 
   <td>新規または進行中</td> 
   <td>完了</td> 
  </tr> 
  <tr> 
   <td>タスクの完了率を 100％から低い数値に更新</td> 
   <td>完了</td> 
   <td>処理中</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>「タスクを開始」ボタンをクリックして割り当てられたタスクの作業を開始</span> </td> 
   <td><span>新規</span> </td> 
   <td> <p>ホームチーム設定の「タスクを開始」ボタンに関連付けられたステータス。</p> <p>「作業をする」ボタンを「タスクを開始」ボタンに置き換える方法については、<span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業をする」ボタンを「開始」ボタンに置き換える</a></span>を参照してください。</p> <p>ヒント：<span> タスクを開始 </span> をクリックした後、<span data-mc-conditions="QuicksilverOrClassic.Quicksilver"> クリック </span> 取り消しボタンをクリックすると、ステータスが「新規」に戻ります。 </p> </td> 
  </tr> 
 </tbody> 
</table>
