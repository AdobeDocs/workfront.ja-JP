---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクの進捗ステータスの概要
description: Adobe Workfront は、タスクのタイムライン全体でのタスクの進行状況を確認することで、タスクの進捗ステータスを決定します。タスクの進捗ステータスの値に基づいて、プロジェクトの状況を決定するように Workfront を設定できます。プロジェクト状況の設定について詳しくは、「プロジェクト状況と状況タイプの概要」の記事を参照してください。
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: 70d173ca3781d8d143a66ce7e963dcaf66bece19
workflow-type: ht
source-wordcount: '777'
ht-degree: 100%

---

# タスクの進捗ステータスの概要

<!-- Audited: 1/2024 -->

Adobe Workfront は、タスクのタイムライン全体でのタスクの進行状況を確認することで、タスクの進捗ステータスを決定します。タスクの進捗ステータスの値に基づいて、プロジェクトの状況を決定するように Workfront を設定できます。プロジェクト状況の設定について詳しくは、[プロジェクト状況と状況タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)の記事を参照してください。

## タスクの進捗ステータスを決定する条件

プロジェクトの進捗ステータスについて詳しくは、[プロジェクトの進捗ステータスの概要](../../../manage-work/projects/planning-a-project/project-progress-status.md)を参照してください。

タスクの進行状況のトラッキングについて詳しくは、[タスクトラッキングモードの概要](../../../manage-work/tasks/task-information/task-tracking-mode.md)を参照してください。

タスクの進捗ステータスは、以下の条件に基づいて決定されます。

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>進捗ステータス</strong> </p> </th> 
   <th> <p><strong>条件の決定</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>予定通り</strong> </p> </td> 
   <td scope="col"> <p>すべての見込み日が予定日と一致する場合、タスクは<strong>予定通り</strong>と見なされます。また、この進捗ステータスは、プロジェクトが予定より早く、見込み日が予定日より前になる可能性もあります。</p> <p>見込み日について詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">プロジェクト、タスクおよびイシューに関する見込み完了日の概要</a>を参照してください。</p> <p>予定完了日のタスクについて詳しくは、次の記事を参照してください。</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">タスクの予定開始日の概要</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">タスクの予定完了日の概要</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>リスクあり</strong> </p> </td> 
   <td><p>推定完了日が予定完了日より後で、見込み完了日より後の場合、タスクは<strong>危険</strong>と見なされます。これは、タスクに<strong>指定日に終了</strong>または<strong>指定日に開始</strong>の制約がある場合、タスクの完了率または先行タスクとの関係において、指定した日付までに終了または開始できないことを示します。 </p><p> タスクの制約を<strong>指定日に終了</strong>に設定して、予定完了日を特定の日付に手動で設定します。この例の見込み完了日は、予定完了日と一致します。この制約の場合、Workfront はタスクを分析し、完了率に基づいて、タスクが終了するタイミングを計算します。この計算は、推定期限として保存されます。推定期限が見込み完了日より後の場合、タスクは遅延のリスクがあると見なされます。 </p> <p> タスクの制約を<strong>指定日に開始</strong>に設定して、予定開始日を特定の日付に手動で設定します。この例の見込み開始日は、予定開始日と一致します。この制約の場合、Workfront はタスクを分析し、先行タスクとの関係に基づいて開始するタイミングを計算します。この計算は、推定開始日として保存されます。指定した開始日にタスクを開始できない強制先行タスクがある場合、推定開始日は、見込み完了日より後になる場合があります。タスクが遅れるリスクがあると見なされます。 </p> <p>メモ：通常、<strong>指定日に開始</strong>または<strong>指定日に終了</strong>が使用されている場合を除き、推定日は見込み日と一致します。この場合、推定日は、完了率およびその他の要因（先行タスクとの関係）に基づいて引き続き計算されますが、予定日は、手動で設定された見込み日と強制的に一致します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>遅れ</strong> </p> </td> 
   <td> <p>推定完了日が予定完了日より後で、見込み完了日より後の場合、タスクは<strong>遅れ</strong>と見なされます。</p> <p>見込み完了日は、前の進捗状況に基づいてタスクが完了するタイミングをリアルタイムで表示します。タスクは遅れて開始されましたが、予定完了日と見込み完了日は未来の日付であり、タスクは予定通りに完了する可能性があるので、まだ遅れているとは見なされません。</p> <p>メモ：<strong>遅れ</strong>および<strong>リスク</strong>の進捗ステータスは、ほぼ同じです。しかし、<strong>リスク</strong>はいずれか、または両方の予定日に、強制的にタスクの制約（指定日に終了、指定日に開始、固定日付）が設定されていることを示します。タスクに強制制約がない場合、予測日は推定日と同じになり、現在のタスクの進捗状況に基づく完了日のシステム計算が反映されます。予定完了日と見込み完了日は未来の日付のままであり、タスクは予定通りに完了する可能性があるので、まだ遅延と見なされません。<br>見込み日および推定日について詳しくは、<a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">見込み日と推定日の区別</a>を参照してください。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>遅れ</strong> </p> </td> 
   <td> <p>予定完了日が今日の日付より前の場合、タスクは<strong>遅れ</strong>となります。<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![](assets/on-time-progress-status-350x233.png)

* At Risk

  ![](assets/at-risk-progress-status-350x233.png)

* Behind

  ![](assets/behind-progress-status-350x233.png)

* Late

  ![](assets/late-progress-status-350x233.png)

-->