---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクト進捗ステータスの概要
description: Adobe Workfront では、タイムライン全体でプロジェクトの進行状況を確認することで、プロジェクトの進捗ステータスを決定します。タスクの進捗ステータスの値に基づいて、プロジェクトの状況を決定するように Workfront を設定できます。この記事では、プロジェクトの進捗ステータスについて説明します。
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: d85ccb9dbef343ecc8808412e89264b3ea6ab25e
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 95%

---

# プロジェクト進捗ステータスの概要

<!--Audited: 12/2023-->

Adobe Workfront では、タイムライン全体でプロジェクトの進行状況を確認することで、プロジェクトの進捗ステータスを決定します。タスクの進捗ステータスの値に基づいて、プロジェクトの状況を決定するように Workfront を設定できます。プロジェクト状況の設定について詳しくは、[プロジェクト状況と状況タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)の記事を参照してください。

Workfront におけるプロジェクトの進捗ステータスは次のとおりです。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>予定通り</td> 
   <td> 次の場合、プロジェクトの進捗ステータスは<strong>予定通り</strong>です。<ul><li>見込み完了日と推定完了日の両方が、プロジェクトの予定完了日と同じかそれより前の場合</li></ul> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>リスクあり</td> 
   <td> 次の<strong>すべて</strong>が当てはまる場合、プロジェクトの進捗ステータスは<strong>危険あり</strong>です。<ul><li>推定完了日と見込み完了日の両方が未来の日付である</li><li> 見込完了日が見込完了日および見込完了日の両方より後です </li></ul><p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>遅れ</td> 
   <td> 次の<strong>すべて</strong>が当てはまる場合、プロジェクトの進捗ステータスは<strong>遅れ</strong>です。<ul><li>推定完了日と見込み完了日の両方が未来の日付である</li><li> 推定完了日と見込み完了日の両方が、プロジェクトの予定完了日より後である</li><li> 推定完了日が見込み完了日より後でない</li></ul> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
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
* プロジェクトの推定完了日は、最新の推定完了日を持つクリティカルパス上のタスクによって決まります。

プロジェクトのクリティカルパスについては、[プロジェクトのクリティカルパスの概要](../../../manage-work/tasks/manage-tasks/critical-path.md)を参照してください。

見込み完了日については、[プロジェクト、タスクおよびイシューの見込み完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。
