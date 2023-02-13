---
product-area: projects;user-management
navigation-topic: assign-tasks
title: タスクに対するユーザーまたはロールの割り当て率の管理
description: 割り当て率は、割り当てられたリソースが 1 日に 1 回のタスクで作業する予定の時間を表します。 タスクの期間中にリソースが割り当てられる（ユーザーまたはプロジェクトのスケジュールに従った）稼働日の割合です。
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 1%

---

# タスクに対するユーザーまたはロールの割り当て率の管理

割り当て率は、割り当てられたリソースが 1 日に 1 回のタスクで作業する予定の時間を表します。 タスクの期間中にリソースが割り当てられる（ユーザーまたはプロジェクトのスケジュールに従った）稼働日の割合です。

>[!NOTE]
>
>ユーザーを作業に割り当てる場合、スケジュールに従って使用できるかどうかは、タスクや問題の計画日と予定日に影響します。 スケジュールについて詳しくは、 [スケジュールの作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

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
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに権限を付与するか、それ以上の権限を付与する</p> <p>権限を編集して、「タスクの編集」ボックスで割り当て率を更新します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスクの割り当て率の変更に関する考慮事項

* デフォルトでは、ユーザーは、割り当てられているタスクに対して、同じ割合の時間が割り当てられます。
* タスクの「期間タイプ」が「計算作業」または「労力主導」の場合のみ、タスクに割り当てられたユーザーおよびジョブロールの割り当て率を手動で変更できます。

   詳しくは、 [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* タスクに割り当てられたチームの割合は変更できません。
* 問題に割り当てられたユーザーとジョブのロールの割合は変更できません。

## タスクのユーザーまたは役割の割り当て率を変更する

1. 割合配分を変更するリソースを持つタスクに移動します。
1. 次をクリック： **詳細** メニュー ![](assets/qs-more-icon-on-an-object.png) タスク名の横にあるをクリックし、 **編集**.

   または

   次をクリック： **割り当て** 領域を選択し、 **詳細**.

1. 次を確認します。 **期間のタイプ** タスクのは次のいずれかです。

   * 算出した作業
   * 作業優先

   >[!TIP]
   >
   >* 「計算された割り当て期間の種類」で、Workfrontは次の数式を使用して各担当者の割り当て率を計算します。 `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* 「シンプル期間」タイプでは、各リソースに割り当てられた時間を見積もることができ、割り当て率ではありません。


1. クリック **割り当て**&#x200B;を編集し、 **配分** タスクの担当者ごとに

   変更できるのは、ユーザーとジョブのロールの割り当てに対する割り当て率のみです。

   タスクに割り当てられたチームの割り当て率は変更できません。

   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. 「**保存**」をクリックします。
