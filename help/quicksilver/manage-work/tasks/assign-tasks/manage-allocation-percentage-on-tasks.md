---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクのユーザーまたは役割の割り当て率を管理します
description: 配分率は、割り当てられたリソースが 1 日に 1 回のタスクで作業する予定の時間を表します。タスクの期間中にリソースが配分される、（ユーザーまたはプロジェクトのスケジュールに従った）作業日の割合です。
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 798e9ee9862b34653730c07acc9c48b901b98e63
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 70%

---

# タスクに対するユーザーまたは役割の配分率の管理

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<div class="preview">

このページで強調表示されている情報は、まだ一般公開されていない機能を示しています。 すべてのお客様が、プレビュー環境でのみ使用できます。 プレビューリリースから 1 週間後に、すべてのお客様の実稼動環境でも同じ機能が使用できるようになります。

詳しくは、[&#x200B; インターフェイスの最新化 &#x200B;](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md) を参照してください。

</div>


配分率は、割り当てられたリソースが 1 日に 1 回のタスクで作業する予定の時間を表します。タスクの期間中にリソースが配分される、（ユーザーまたはプロジェクトのスケジュールに従った）作業日の割合です。

タスクに対して高度な割り当てを行う際に、割り当て率を変更できます。

>[!NOTE]
>
>ユーザーを作業に割り当てる場合、ユーザーのスケジュールに応じた空き時間は、タスクやイシューの予定日と見込日に影響します。スケジュールについて詳しくは、[スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>ワークまたはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>タスクへのアクセスを編集</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td>
   <td><p>タスクに対する参加以上の権限</p>
   <p>古いエクスペリエンスを使用してタスクを編集する際に、「タスクを編集」ボックスで割り当て率を更新する権限を編集し <span class="preview"> す。 新しいエクスペリエンスでタスクを編集する際に、「タスクを編集」ボックスで割り当ての割合を管理できなくなりました。</span></p> <p>詳しくは、<a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md"> タスクの編集 </a> を参照してください</p>.</td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

## タスクの配分率の変更に関する考慮事項

* デフォルトでは、ユーザーは、割り当てられているタスクに対して同じ割合の時間が配分されます。
* タスクの「期間タイプ」が「予定作業」または「残存作業時間の優先」の場合のみ、タスクに割り当てられたユーザーおよび担当業務の配分率を手動で変更できます。

  詳しくは、[タスク期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

* タスクに割り当てられたチームの配分率は変更できません。
* イシューに割り当てられたユーザーと担当業務の配分率は変更できません。

## タスクに対するユーザーまたは役割の配分率を変更

1. 配分率を変更するリソースを持つタスクに移動します。
1. タスクヘッダーの **割り当て** エリアをクリックし、**詳細** をクリックします。

1. タスクの&#x200B;**期間タイプ**&#x200B;が次のいずれかであることを確認します。

   * 予定作業
   * 残存作業時間の優先

   >[!TIP]
   >
   >* 期間タイプが予定割り当て時間の場合、Workfront は次の数式を使用して各担当者の配分率を計算します。`Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`
   >* 期間タイプがシンプルの場合、配分率ではなく、各リソースに割り当てられた時間を見積もることができます。

1. 各タスク担当者の **割り当て** フィールドを変更します。

   変更できるのは、ユーザーと担当業務の割り当てに関する配分率のみです。

   タスクに割り当てられたチームの配分率は変更できません。

   ![&#x200B; 配分率の変更 &#x200B;](assets/advanced-assignments-allocation-percentage.png)

1. 「**保存**」をクリックします。
