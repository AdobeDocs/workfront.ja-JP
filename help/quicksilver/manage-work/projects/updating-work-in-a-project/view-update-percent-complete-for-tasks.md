---
product-area: projects
navigation-topic: update-work-in-a-project
title: タスクの完了率を表示および更新します
description: タスクの完了率を更新して、タスクを完了するための進捗を示すことができます。 イシューの完了率の更新は、タスクの完了率の更新と似ています。 この記事では、タスクの完了率を更新する方法について説明します。
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 34%

---

# タスクの完了率の表示と更新

<!--Audited: 05/2025-->

タスクの完了率を更新して、完了に向けたタスクの進捗状況を示すことができます。

イシューの完了率の更新は、タスクの完了率の更新と似ています。 この記事では、タスクの完了率を更新する方法について説明します。

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
   <p>Work またはそれ以上</p>
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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   Or
   <p>Current license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## タスクの完了率を更新できるエリア

タスクの完了率は、次のすべてのエリアで更新できます。

* **タスクリストの場合**：完了率列が表示されたら、タスクの完了率を更新できます。

  インライン編集について詳しくは、[Adobe Workfront のリスト内の項目のインライン編集](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)を参照してください。

* **マイルストーン ビューで**: プロジェクトリストまたはプロジェクトレポートでマイルストーン ビューを使用している場合、タスクの完了率を更新できます。

  >[!TIP]
  >
  >  マイルストーン ビューでは、問題の完了率を更新することはできません。


  詳しくは、[マイルストーンビューの使用](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md)を参照してください。

* **タスクヘッダー内**：タスクヘッダー内のタスクの完了率を更新できます。

  ![ ヘッダーの更新率 ](assets/nwe-updatetaskpercentinheader-350x54.png)

* **タスクの概要パネル内**：次のエリアでタスクを表示する際に、概要パネルの上部でタスクの完了率を更新できます。

   * タスクリストまたはレポート
   * タイムシート
   * ワークロードバランサー

  ![ ハイライト表示されたタスクの概要の更新率 ](assets/update-percent-complete-in-task-summary-highlighted.png)

  詳しくは、[概要について](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)を参照してください

* **ホーム**: ホーム領域の概要パネルまたはマイ作業ウィジェットから、タスクまたは問題の完了率を更新できます。

  詳しくは、[ ホームの概要 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md) を参照してください。

## タスクの完了率を更新する際の考慮事項

* タスクを 100% 完了としてマークすると、そのタスクの状態は [ 完了 ] に更新されます。 問題のステータスがクローズ済みに更新されます。
* タスクを完了すると、親およびプロジェクトの完了率も更新されます。
* 親タスクおよびプロジェクトには次のシナリオが存在します。
   * プロジェクトの「概要完了モード」が「自動」に設定され、サブタスクが完了していない場合、親タスクの完了率を 100％に更新できません。
   * プロジェクトの概要完了モードが「手動」に設定され、サブタスクが完了または未完了の場合は、親タスクまたはプロジェクトの完了率を 100% に更新できます。

  詳しくは、[プロジェクトの編集](../manage-projects/edit-projects.md)を参照してください。

## タスクの完了率を更新

1. タスクの完了率を更新する領域に移動します。

   詳しくは、この記事の [ タスクの完了率を更新できる領域 ](#areas-where-you-can-update-the-percent-complete-of-a-task) 節を参照してください。

1. 完了率を更新するタスクの「**完了率**」フィールドを見つけます。

   >[!TIP]
   >
   >「完了率」フィールドは、常に概要パネルの上部に表示されます。

1. **完了率** フィールド内をクリックし、0～100 の数字を入力します

   または

   **完了率** の青いバブルをクリックして必要な数にドラッグし、可能な場合は完了したタスクの量を示します。

   >[!NOTE]
   >
   >    * 完了率バブル内をクリックした場合は、小数値を入力できません。
   >    * 概要パネルの青い通芯記号をドラッグ&amp;ドロップすると、完了率が 1 点増分で更新されます。
   >
   >    * タスクヘッダーの青いバブルをドラッグ&amp;ドロップすると、完了率が 5 ポイント増分で更新されます。

1. キーボードの Enter キーを押して、完了率を保存します。

   プロジェクトまたは親タスクの完了率も自動的に更新される場合があります。

   タスクまたはイシューのステータスも更新されます。

