---
product-area: projects
navigation-topic: update-work-in-a-project
title: タスクの完了率の表示と更新
description: タスクの完了率を更新して、タスクを完了するためのタスクの進捗状況を示すことができます。
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# タスクの完了率の表示と更新

<!--Audited:01/2024-->

タスクの完了率を更新して、タスクを完了するためのタスクの進捗状況を示すことができます。

## アクセス要件

タスクを手動で更新するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>新しいライセンス：標準</p> 
   または
   <p>現在のライセンス：作業中以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>タスクに対する権限の管理</p>  </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## タスクの完了率を更新できる領域

タスクの完了率は、次のいずれかの領域で更新できます。

* **タスクリスト内**:「完了の割合」列が表示されている場合に、タスクの完了率を更新できます。\
  インライン編集について詳しくは、 [Adobe Workfrontのリスト内の項目をインライン編集する](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **マイルストーン表示で**：タスクの完了率は、プロジェクトリストまたはプロジェクトレポートでマイルストーンビューを使用する際に更新できます。 詳しくは、 [マイルストーンビューの使用](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **タスクヘッダー内**：タスクヘッダーでタスクの完了率を更新できます。 詳しくは、 [タスクを編集](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## タスクの完了率を更新する際の考慮事項

* タスクを「100%完了」とマークすると、タスクの「ステータス」が「完了」に更新されます。
* 親タスクには、次のシナリオが存在します。
   * プロジェクトの [ サマリー完了モード ] が [ 自動 ] に設定され、サブタスクが完了していない場合は、親タスクの完了率を 100%に更新することはできません。
   * プロジェクトの [ サマリー完了モード ] が [ 手動 ] に設定され、サブタスクが完了または不完全になっている場合は、親タスクの完了率を 100%に更新できます。

  詳しくは、 [プロジェクトを編集](../manage-projects/edit-projects.md).

## タスクの完了率の更新

1. Workfrontの次のいずれかの領域に移動します。

   * タスクリスト
   * プロジェクトのリストとマイルストーンビューの適用
   * タスク（タスクページにアクセスする）
1. 次を見つけます。 **完了率** 達成率を更新するタスクのフィールド。
1. 「完了率」フィールド内をクリックし、0 ～ 100 の数値を入力します

   または

   をクリックし、 **完了率** 必要な数のバーをクリックして、完了したタスクの時間（使用可能な場合）を示します。

   >[!NOTE]
   >
   >タスクの 100%が完了したと示すと、タスクのステータスも「完了」に更新されます。


1. 完了率を保存するには、キーボードの Enter キーを押します。

プロジェクトの「完了率」も自動的に更新されます。

