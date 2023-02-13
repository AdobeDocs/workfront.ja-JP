---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの概要実績完了日
description: プロジェクト、タスクおよびタスクは、Adobe Workfrontで実際の完了日が設定されます。 この日付は、プロジェクト、タスク、または問題が完了済みとマークされた日付です。
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: 3a3dc541219706e3f6a4700889db344c110838bb
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# プロジェクトの概要実績完了日

プロジェクト、タスクおよびタスクは、Adobe Workfrontで実際の完了日が設定されます。 この日付は、プロジェクト、タスク、または問題が完了済みとマークされた日付です。

## 実際の完了日

「実際の完了日」は、作業が完了した実際の日時を表します。 タスクまたはイシューが「完了」または「完了」とマークされると、Workfrontはアイテムのステータスが変更された日付をタスクまたはイシューの実際の完了日として自動的に設定します。 タスクまたはイシューが実際に完了した日時を反映した正確な日付でない場合は、実際の完了日を手動で編集できます。

例えば、タスクや問題を月曜日に「完了」とマークすることはできますが、作業が前の金曜日に完了したことがわかります。 タスクまたはイシューを「完了」としてマークした後、タスクまたはイシューの実際の完了日を前の金曜日の日付に手動で更新し、実際の完了を反映させることができます。

プロジェクトの実績完了日は手動で編集できませんが、プロジェクトのステータスを手動で変更して、プロジェクトの実績完了日に変更をトリガーできます。

プロジェクトの実際の完了日は、次の方法で設定します。

* 手動でプロジェクトのステータスを更新する場合：プロジェクトの「完了トリガー」が「手動」に設定され、プロジェクトのステータスを手動で「完了」に変更した場合、プロジェクトの実際の完了日が、ステータスを変更した日時に更新されます。
* プロジェクトの最後のタスクが完了したときに、自動的に次の操作を実行します。プロジェクトの [ 完了モード ] が [ 自動 ] に設定され、最後のタスクを [ 完了 ] または [ 最終タスクの実績完了日 ] に設定した場合、プロジェクトの実績完了日もその日に更新されます。

   プロジェクトの完了モードの設定については、この記事を参照してください。 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!NOTE]
   >
   >Workfrontは、最後に完了したプロジェクトのタスクの実績完了日を、プロジェクト全体の実績完了日として使用します。

Workfrontまたはグループ管理者は、Workfrontがタスクの今日の日付と計画完了日のどちらを使用するか、またはタスクが「完了」または「クローズ」に設定されている場合にタスクの計画完了日を使用するかを決定します。 タスクと問題の環境設定について詳しくは、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## 実際の完了日の検索

実際の完了日は、Workfrontの次の領域にあります。

* 「プロジェクト」、「タスク」、「問題の詳細」領域
* 「プロジェクト」、「タスク」および「タスク」ボックスを編集します
* システム更新としてのプロジェクト、タスク、問題の更新領域。
* プロジェクト、タスク、またはタスクのリストまたはレポート。

レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
