---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの進捗状況の概要
description: Adobe Workfront では、タイムライン全体でプロジェクトの進行状況を確認することで、プロジェクトの進捗ステータスを決定します。 タスクの進捗ステータスの値に基づいて、プロジェクトの状況を決定するように Workfront を設定できます。 この記事では、プロジェクトの進捗ステータスについて説明します。
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
TQID: https://experienceleague.adobe.com/V9eyzkoYIREb4zUuDxmyDhnQa54YQaYTv2woNTOhq24
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 375
ht-degree: 80%

---

# プロジェクト進捗ステータスの概要

<!--Audited: 12/2023-->

Adobe Workfront では、タイムライン全体でプロジェクトの進行状況を確認することで、プロジェクトの進捗ステータスを決定します。 タスクの進捗ステータスの値に基づいて、プロジェクトの状況を決定するように Workfront を設定できます。 プロジェクト状況の設定について詳しくは、[プロジェクト状況と状況タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)の記事を参照してください。

Workfront におけるプロジェクトの進捗ステータスは次のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>予定通り</td> 
   <td> 次の場合、プロジェクトの進捗ステータスは<strong>予定通り</strong>です。<ul><li>プロジェクトの予定完了日以前の予定日と予定完了日の両方が指定されている場合 <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>リスクあり</td> 
   <td> 次の<strong>すべて</strong>が当てはまる場合、プロジェクトの進捗ステータスは<strong>危険あり</strong>です。<ul><li>推定完了日と見込み完了日の両方が未来の日付である</li><li> 予定完了日と予定完了日の両方よりも後の日付が指定されています <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul> </td> 
  </tr> 
  <tr> 
   <td>遅れ</td> 
   <td> 次の<strong>すべて</strong>が当てはまる場合、プロジェクトの進捗ステータスは<strong>遅れ</strong>です。<ul><li>推定完了日と見込み完了日の両方が未来の日付である</li><li> 推定完了日と見込み完了日の両方が、プロジェクトの予定完了日より後である</li><li> 推定完了日が予定完了日より後ではありません
   <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p></li></ul>  </td> 
  </tr> 
  <tr> 
   <td>遅延</td> 
   <td> 
     次の<strong>どちらか</strong>が当てはまる場合、プロジェクトの進捗ステータスは<strong>遅延</strong>です。<ul><li>プロジェクトが完了し、実際の完了日が予定完了日より後である <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>プロジェクトが完了しておらず、プロジェクトの予定完了日が過去の日付である <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

次の点に注意してください。

* プロジェクトの見込み完了日は、最新の見込み完了日を持つクリティカルパス上のタスクによって決まります。
* プロジェクトの推定納期は、最新の推定納期を持つクリティカルパス上のタスクによって決定されます。

プロジェクトのクリティカルパスについては、[プロジェクトのクリティカルパスの概要](../../../manage-work/tasks/manage-tasks/critical-path.md)を参照してください。

見込み完了日については、[プロジェクト、タスクおよびイシューの見込み完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。
