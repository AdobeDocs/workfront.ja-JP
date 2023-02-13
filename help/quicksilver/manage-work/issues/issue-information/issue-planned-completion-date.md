---
product-area: projects
navigation-topic: issue-information
title: 問題の概要計画完了日
description: 問題の「計画完了日」は、問題の完了が予想される日です。
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# 問題の概要計画完了日

問題の「計画完了日」は、問題の完了が予想される日です。

イシューの「計画完了日」を指定するか、特定の条件に応じてAdobe Workfrontまで計算できます。 

問題の計画完了日は、プロジェクトの計画完了日には影響しません。 タスクの計画完了日のみが、プロジェクトの計画完了日に影響を与えます。 プロジェクトの計画完了日の詳細は、 [プロジェクトの完了予定日を設定](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md).

>[!NOTE]
>
>問題の計画完了日は、次の点で、問題のコミット日または計画完了日と異なります。
>
>* 「コミット日」は、問題に割り当てられた人が手動で問題を完了したと推定する日付です。 詳しくは、次の記事を参照してください。
   * [コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
   * [コミット日と計画完了日の間のインタラクション](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md).
* 完了予定日とは、問題が現実的に完了できる実際の日付を決定する外部要因を考慮に入れて、Workfrontが計算した日付です。 詳しくは、 [プロジェクト、タスクおよび問題に関する予定完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
>


## 問題の計画完了日を手動で設定

問題の計画完了日を更新するには、問題に対する編集アクセス権と管理権限が必要です。

問題の計画完了日は、Workfrontの次の領域で手動で設定できます。

* イシューを作成または編集する際に、「Edit Issue」ボックスまたは「Issue Details」領域で、以下の操作を実行します。 詳しくは、 [問題の編集](../../../manage-work/issues/manage-issues/edit-issues.md).
* 問題の表示時に計画完了日が表示される場合は、「ホーム」領域で 詳しくは、 [ホーム領域の作業項目を更新または編集する](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md).
* イシューのヘッダー。 詳しくは、 [新しいオブジェクトヘッダー](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).
* 発行リストまたはレポートで、「計画完了日」フィールドがビューに表示されるとき。

   詳しくは、 [リスト内の問題の編集](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Workfrontが問題の計画完了日を自動的に計算する方法

Workfrontが問題の計画完了日を自動的に計算する場合、次のような影響が日付に及ぶ可能性があります。

* 計画開始日

   イシューを最初に作成したときのイシューの「入口日」と「計画開始日」が一致する必要があります。

* プロジェクトの「キューの詳細」セクションで設定されたデフォルト期間。 詳しくは、 [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   デフォルト期間が 0 日の場合、計画完了日は問題の計画開始日と一致します。

* プロジェクトスケジュール

自動的に設定された場合、計画完了日は次の計算に基づいて決定されます。 

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**例：** 例えば、タスクの開始日が 1 月 14 日（金）で、デフォルト期間が 5 日の場合、計画完了日は 1 月 21 日（プロジェクトスケジュールが月～金）で、1 日 8 時間は 1 日（金）です。

次の状況が存在します。

* プロジェクトにスケジュールがない場合、Workfrontシステムのデフォルトスケジュールが考慮されます。 詳しくは、 [スケジュールの概要](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).
* スケジュールが月曜日～金曜日の午前 9 時～午後 1 時（1 日 4 時間）で、Workfrontシステムの通常の 1 作業時間が 8 時間の場合、完了予定日は 1 月 27 日です。

>[!TIP]
Workfrontでは、計画完了日を計算する際に、休日や週末などの計画例外が考慮されます。

 
