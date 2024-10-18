---
product-area: projects
navigation-topic: update-work-in-a-project
title: タスクの完了率を表示および更新します
description: タスクの完了率を更新して、完了に向けたタスクの進捗状況を示すことができます。
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: e68972f7334a93f7fbd3db29919a2f2746ce64fe
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 84%

---

# タスクの完了率の表示と更新

<!--Audited:01/2024-->

タスクの完了率を更新して、完了に向けたタスクの進捗状況を示すことができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

タスクを手動で更新するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>新規のライセンス：標準</p> 
   または
   <p>現在のライセンス：ワーク以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する管理権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## タスクの完了率を更新できるエリア

タスクの完了率は、次のすべてのエリアで更新できます。

* **タスクリスト内**：「完了率」列が表示されている場合に、タスクの完了率を更新できます。\
  インライン編集について詳しくは、[Adobe Workfront のリスト内の項目のインライン編集](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)を参照してください。

* **マイルストーンビュー内**：プロジェクトリストやプロジェクトレポートでマイルストーンビューを使用する際に、タスクの完了率を更新できます。詳しくは、[マイルストーンビューを使用](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md)を参照してください。

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **タスクヘッダー内**：タスクヘッダーで、タスクの完了率を更新できます。詳しくは、[タスクを編集](../../tasks/manage-tasks/edit-tasks.md)を参照してください。

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **タスクの概要パネル内**：次のエリアでタスクを表示する際に、概要パネルの上部でタスクの完了率を更新できます。

   * タスクリストまたはレポート
   * タイムシート
   * ワークロードバランサー

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  詳しくは、[概要について](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)を参照してください

* **ホーム**: ホーム領域の概要パネルまたはマイ作業ウィジェットから、タスクまたは問題の完了率を更新できます。

詳しくは、[ 新しいホームの概要 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md) を参照してください。

## タスクの完了率を更新する際の考慮事項

* タスクを「100% 完了」とマークすると、タスクのステータスが「完了」に更新されます。
* 親タスクには、次のシナリオが存在します。
   * プロジェクトの「概要完了モード」が「自動」に設定され、サブタスクが完了していない場合、親タスクの完了率を 100％に更新できません。
   * プロジェクトの「概要完了モード」が「手動」に設定され、サブタスクが完了または完了していない場合、親タスクの完了率を 100％に更新できます。

  詳しくは、[プロジェクトの編集](../manage-projects/edit-projects.md)を参照してください。

## タスクの完了率を更新

1. Workfront の次のいずれかのエリアに移動します。

   * タスクリスト
   * プロジェクトリスト（マイルストーンビューを適用）
   * タスク（タスクページにアクセス）
1. 完了率を更新するタスクの「**完了率**」フィールドを見つけます。

   >[!TIP]
   >
   >  「完了率」フィールドは、常に概要パネルの上部に表示されます。


1. **完了率** フィールド内をクリックし、0～100 の数字を入力します

   または

   タスクがどの程度完了しているかを表示するには、「**完了率**」バーをクリックして必要な数までドラッグします。

   >[!NOTE]
   >
   >タスクの 100％ が完了したと示すと、タスクのステータスも「完了」に更新されます。


1. 完了率を保存するには、キーボードの Enter キーを押します。

プロジェクトの完了率も自動的に更新されます。

