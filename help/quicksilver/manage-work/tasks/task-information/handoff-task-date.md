---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクハンドオフ日の概要
description: ハンドオフ日とは、タスクが作業可能になる日付です。これは、通常、先行タスクが解決済みで、タスクの担当者が作業を開始できることを意味します。
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: b774a74863bb35e3477a69ff11189c40a6d66437
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 60%

---

# タスクハンドオフ日の概要

ハンドオフ日とは、タスクが作業可能になる日付です。これは、通常、先行タスクが解決済みで、タスクの担当者が作業を開始できることを意味します。

>[!TIP]
>
>イシューおよびプロジェクトにはハンドオフ日は存在しません。

## Adobe Workfront でのハンドオフ日の計算方法

>[!NOTE]
>
>ハンドオフ日は、プロジェクトのステータスが次のステータスと等しい場合にのみ計算されます。
>
>* 保留中
>* 現在
>* 完了
>* 停止
>

Workfront では、タスクのハンドオフ日の計算に次のルールを使用します。

* **タスクに未完了の先行タスクがある場合**：タスクのハンドオフ日は null です。
* **タスクに完全な先行タスクがある場合**：ハンドオフ日は、先行タスクの実際の完了日と同じです。先行タスクに遅延がある場合、Workfront は次の式を使用して後続タスクのハンドオフ日を計算します。

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  ラグタイムについて詳しくは、[ラグタイプの概要](../use-prdcssrs/lag-types.md)を参照してください。

  後続タスクに複数の先行タスクがある場合、先行タスクの最新の実際の完了日に基づいて、ハンドオフ日が計算されます。 例えば、2 つの先行タスクの実際の完了日が 2022年11月8日と 2022年11月20日の場合、後続タスクのハンドオフ日は 2022年11月20日になります。

  >[!NOTE]
  >
  >   実際の完了日または先行タスクに基づく後続タスクのハンドオフ日の計算は、先行タスクが実行されるかどうかに関係なく同じです。強制的な先行タスクについて詳しくは、[先行タスクの実行](../use-prdcssrs/enforced-predecessors.md)を参照してください。


* **タスクに先行タスクがない場合**：

   * **計画開始日が過去の日付です**：タスクに強制的な制約が設定されていない場合、引き渡し日は、プロジェクトの計画開始日と同じです。 タスクに強制制約がある場合は、以下の「計画日に対して強制制約がタスクに含まれている場合」を参照してください。
   * **計画開始日が将来の日付です（現在の日付より後の任意の日付）**：タスクに強制的な制約が設定されていない場合、ハンドオフ日は、タスクの計画開始日と同じです。 タスクに強制制約がある場合は、以下の「計画日に対して強制制約がタスクに含まれている場合」を参照してください。

>[!NOTE]
>
>タスクにプロジェクト間の先行タスクがある場合、後続タスクのハンドオフ日は、次のいずれかが発生した場合にのみ再計算されます。
>
>* 後続のプロジェクトのタイムラインを手動で再計算します。タイムラインを再計算するには、プロジェクトに対する管理権限が必要です。
>* 後続プロジェクトのタイムラインは、夜間に自動的に再計算されます。
>
>プロジェクトのタイムラインの再計算について詳しくは、[プロジェクトタイムラインの再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)を参照してください。

* **タスクに予定日に対する強制制約がある場合**：ハンドオフ日は、制約のタイプと、タスクに実際の開始日が設定されているかどうかによって異なります。\
  次に、タスクに対する強制制約を示します。

   * 指定日に開始
   * 指定日に終了
   * 指定日以降に開始
   * 指定日までに開始
   * 固定日付

  次のシナリオが存在します。

   * **タスクに「次の日に開始する」または「次の日に開始する」という制約がある場合**：タスクの制約日が過去で、タスクに実際の開始日がない（タスクがまだ開始されていない）場合、「ハンドオフ日」は、タスクの実行を開始できる最も近い日付です。 タスクが開始した場合、「引き渡し日」はプロジェクトの開始日と同じになります。
   * **タスクに [ 終了日 ] または [ 次の日までに開始 ] という制約がある場合**：タスク制約の日付が将来の日付で、タスクに実際の開始日がない（タスクがまだ開始されていない）場合、引き渡し日はタスクの計画開始日になります。 タスクに実際の開始日が設定されている場合は、引き渡し日がプロジェクトの開始日になります。
   * **タスクに固定日付の制約がある場合**:「ハンドオフ日」は、タスクに先行タスクがあるかどうか、および先行タスクが完了したかどうかに関係なく、タスクの計画開始日です。

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## ハンドオフ日を見つける

タスクのハンドオフ日をタスクレポートまたはタスクリストの表示に表示できます。\
レポートの作成に関して詳しくは、[カスタムレポートを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。
