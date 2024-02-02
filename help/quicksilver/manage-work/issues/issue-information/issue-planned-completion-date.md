---
product-area: projects
navigation-topic: issue-information
title: イシューの予定完了日の概要
description: イシューの予定完了日とは、イシューが完了する予定の日付です。
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '580'
ht-degree: 100%

---

# イシューの予定完了日の概要

イシューの予定完了日とは、イシューが完了する予定の日付です。

イシューの予定完了日を指定することも、Workfront に任せて、特定の基準に基づいて計算することもできます。 

イシューの予定完了日は、プロジェクトの予定完了日には影響しません。タスクの予定完了日のみが、プロジェクトの予定完了日に影響を与えます。プロジェクトの予定完了日について詳しくは、[プロジェクトの予定完了日の設定](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)を参照してください。

>[!NOTE]
>
>イシューの予定完了日は、次の方法で、イシューのコミット日またはイシューの見込み完了日と異なります。
>
>* コミット日は、イシューに割り当てられたユーザーがイシューの完了を手動で推定した日付です。詳しくは、次の記事を参照してください。
>
* [コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [コミット日と予定完了日の間のインタラクション](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md)。
>
* 見込み完了日とは、Workfront によって計算された日付で、外部の要因を考慮して、イシューを現実的に完了できる実際の日付を決定します。詳しくは、[プロジェクト、タスクおよびイシューの見込み完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。
>

## イシューの予定完了日を手動で設定する

イシューの予定完了日を更新できるようにするには、イシューに対する編集権限と管理権限が必要です。

イシューの予定完了日は、Workfront の次のエリアで手動で設定できます。

* イシューを作成または編集するときに、「タスクの編集」ボックスまたはイシューの詳細エリアを使用。詳しくは、[イシューを編集](../../../manage-work/issues/manage-issues/edit-issues.md)を参照してください。
* ホームエリアで、イシューの表示時に予定完了日が表示される場合。詳しくは、[ホームエリアの作業アイテムを更新または編集](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)を参照してください。
* イシューのヘッダー内。詳しくは、[新しいオブジェクトヘッダー](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)を参照してください。
* イシューリストまたはレポートで、「予定完了日」フィールドがビューに表示される場合。

  詳しくは、[リスト内のイシューを編集](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md)を参照してください。

## Workfront でイシューの予定完了日が自動的に計算される方法

Workfront がイシューの予定完了日を自動的に計算する場合、次のことが日付に影響を与える可能性があります。

* 予定開始日

  イシューを最初に作成したときのイシューのエントリ日と予定開始日が一致する必要があります。

* プロジェクトの「キューの詳細」セクションで設定されたデフォルトの期間。詳しくは、[リクエストキューを作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

  デフォルト期間が 0 日の場合、予定完了日はイシューの予定開始日と一致します。

* プロジェクトスケジュール

自動的に設定された場合、予定完了日は次の計算に基づいて決定されます。

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**例：**&#x200B;例えば、タスクの開始日が 1月14日金曜日で、デフォルト期間が 5 日の場合、プロジェクトスケジュールが月曜日から金曜日で 1 日 8 時間とすると、予定完了日は 1月21日金曜日になります。

次の状況が存在します。

* プロジェクトにスケジュールがない場合、Workfront システムのデフォルトスケジュールが考慮されます。詳しくは、[スケジュールの概要](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)を参照してください。
* スケジュールが月曜日から金曜日の午前 9 時から午後 1 時（1 日あたり 4 時間）で、Workfront システムの 1 日あたりの標準労働時間が 8 時間の場合、予定完了日は 1月27日になります。

>[!TIP]
>
Workfront では、予定完了日を計算する場合に、休日や週末などスケジュールの例外が考慮されます。

 
