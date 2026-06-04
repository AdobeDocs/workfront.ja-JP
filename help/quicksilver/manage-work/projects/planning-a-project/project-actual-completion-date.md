---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの実際の完了日の概要
description: プロジェクト、タスクおよびイシューには、Adobe Workfront の実際の完了日が表示されます。 この日付は、プロジェクト、タスクまたはイシューが完了としてマークされた日付です。
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
TQID: https://experienceleague.adobe.com/MoATj74YM1zoW2SsIGrpKY0gc9dHRKjlDvnPfT-kk2s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 490
ht-degree: 88%

---

# プロジェクトの実際の完了日の概要

プロジェクト、タスクおよびイシューには、Adobe Workfront の実際の完了日が表示されます。 この日付は、プロジェクト、タスクまたはイシューが完了としてマークされた日付です。

## 実際の完了日

実際の完了日は、作業が完了した実際の日時を表します。 タスクまたはイシューが完了としてマークされると、Workfront は項目のステータスが変更された日付を、タスクまたはイシューの実際の完了日として自動的に設定します。 タスクまたはイシューが実際に完了した日付が正確に反映されていない場合は、実際の完了日を手動で編集できます。

例えば、月曜日に完了としてマークされたタスクまたはイシューの実際の完了日が、前の金曜日だったとします。 タスクまたはイシューが完了としてマークされた後で、タスクまたはイシューの実際の完了日を前の金曜日に手動で更新し、実際の完了を反映させることができます。

プロジェクトの実際の完了日を手動で編集することはできませんが、プロジェクトのステータスを手動で変更すると、プロジェクトの実際の完了日の変更をトリガーできます。

プロジェクトの実際の完了日は、次の方法で設定します。

* プロジェクトのステータスを手動で更新する：プロジェクトの「完了モード」が「手動」に設定され、プロジェクトのステータスを「完了」に手動で変更した場合、これにより、プロジェクトの実際の完了日が最後に完了したタスクの日時にトリガーされます。
* プロジェクトの最後のタスクの完了時に自動的に更新：プロジェクトの完了モードを自動に設定し、最後のタスクを完了としてマークするか、最後のタスクの実際の完了日を更新すると、プロジェクトの実際の完了日もその日付に更新されます。

  プロジェクトの完了モードの設定について詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)の記事を参照してください。

  >[!NOTE]
  >
  >Workfront では、最後に完了したプロジェクトのタスクの実際の完了日が、プロジェクト全体の実際の完了日として使用されます。

Workfront 管理者やグループ管理者は、タスクまたはイシューが完了またはクローズに設定されている場合に、Workfront で今日の日付と予定完了日のどちらを使用するかを決定します。 タスクとイシューの環境設定について詳しくは、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## 実際の完了日の検索

実際の完了日は、Workfront の次の領域で確認できます。

* プロジェクト、タスク、イシューの詳細領域
* プロジェクト、タスク、イシューを編集ボックス
* システム更新としてのプロジェクト、タスク、イシューの更新領域。
* プロジェクト、タスク、イシューのリストまたはレポート。

レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)の記事を参照してください。
