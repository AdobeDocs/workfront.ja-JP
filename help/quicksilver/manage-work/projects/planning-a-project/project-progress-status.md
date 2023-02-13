---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの進行状況ステータスの概要
description: Adobe Workfrontは、プロジェクトの進行状況をタイムライン全体で確認することで、プロジェクトの進行状況ステータスを決定します。 タスクの進捗状況ステータスの値に基づいて、プロジェクトの条件を決定するようにWorkfrontを設定できます。 プロジェクトの条件の設定の詳細については、「プロジェクトの条件と条件の種類の概要」を参照してください。
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# プロジェクトの進行状況ステータスの概要

Adobe Workfrontは、プロジェクトの進行状況をタイムライン全体で確認することで、プロジェクトの進行状況ステータスを決定します。 タスクの進捗状況ステータスの値に基づいて、プロジェクトの条件を決定するようにWorkfrontを設定できます。 プロジェクトの条件の設定について詳しくは、この記事を参照してください。 [プロジェクト条件と条件タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Workfrontのプロジェクトの進捗状況ステータスを次に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>オンタイム</td> 
   <td> <p>予想完了日と推定完了日の両方がプロジェクトの計画完了日以前の場合、プロジェクトの進捗状況ステータスは次のようになります。 <strong>オンタイム</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>リスクあり</td> 
   <td> <p>「予定完了日」と「予定完了日」の両方が未来で、プロジェクトの「計画完了日」より後で、「予定完了日」が「予定完了日」より後の場合、「プロジェクト進捗状況ステータス」は「 <strong>リスク</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>遅れ</td> 
   <td> <p>「予定完了日」と「予定完了日」の両方が、プロジェクトの「計画完了日」よりも後の将来の日付で、「予定完了日」が「予定完了日」よりも後の場合、プロジェクトの進捗状況ステータスは「 <strong>後ろ</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>遅延</td> 
   <td> 
    <ul> 
     <li> <p>プロジェクトが完了し、実績完了日が計画完了日より後の場合、プロジェクトの進捗状況ステータスは次のようになります。 <strong>遅延</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>プロジェクトが完了しておらず、プロジェクトの計画完了日が過去の場合、プロジェクトの進捗状況ステータスは「 <strong>遅延</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

次の点に注意してください。

* プロジェクトの予測完了日は、最新の予測完了日を持つクリティカルパス上のタスクによって決定されます。
* プロジェクトの完了予定日は、最新の完了予定日と共に、クリティカルパス上のタスクによって決定されます。

プロジェクトのクリティカルパスについては、 [プロジェクトの概要の重要なパス](../../../manage-work/tasks/manage-tasks/critical-path.md).

完了予定日については、 [プロジェクト、タスクおよび問題に関する予定完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
