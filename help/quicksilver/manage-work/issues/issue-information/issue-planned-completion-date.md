---
product-area: projects
navigation-topic: issue-information
title: イシュー予定完了日の概要
description: イシューの予定完了日とは、イシューが完了する予定の日付です。
author: Alina
feature: Work Management
exl-id: bdb206dc-18f8-4f8a-862b-e881408a8408
TQID: https://experienceleague.adobe.com/WodCHwmu7JYCZKdoqoJ6W88AP0xzlZ-Jglj5zxD8-6g
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 595
ht-degree: 50%

---

# イシューの予定完了日の概要

<!--Audited: 08/2025-->

イシューの予定完了日とは、イシューが完了する予定の日付です。

イシューの予定完了日を指定することも、Workfront に任せて、特定の基準に基づいて計算することもできます。

問題の予定完了日は、プロジェクトの予定完了日には影響しません。 タスクの予定完了日のみが、プロジェクトの予定完了日に影響します。 プロジェクトの予定完了日について詳しくは、[ プロジェクトの予定完了日の設定](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)を参照してください。

>[!NOTE]
>
>イシューの予定完了日は、次の方法で、イシューのコミット日またはイシューの見込み完了日と異なります。
>
>* コミット日とは、イシューに割り当てられたユーザーが手動でイシューを完了したと見積もる日付です。 詳しくは、次の記事を参照してください。
>
>   * [コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
>   * [コミット日と予定完了日の間のインタラクション](../../../manage-work/projects/updating-work-in-a-project/interactions-between-commit-and-planned-completion-dates.md)。
>
>* 見込み完了日とは、Workfront によって計算された日付で、外部の要因を考慮して、イシューを現実的に完了できる実際の日付を決定します。 詳しくは、[プロジェクト、タスクおよびイシューの見込み完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。
>

## イシューの予定完了日を手動で設定する

イシューの予定完了日を更新できるようにするには、イシューに対する編集権限と管理権限が必要です。

Workfrontの次の領域で、イシューの予定完了日を手動で設定できます。

* イシューを作成または編集する際は、「イシューを編集」ボックスまたは「イシューの詳細」エリアでイシューを編集します。 詳しくは、[イシューを編集](../../../manage-work/issues/manage-issues/edit-issues.md)を参照してください。
* イシューの概要パネルに「予定完了日」が表示されている場合は、ホーム領域に表示されます。 詳しくは、[ホームエリアの作業アイテムを更新または編集](../../../workfront-basics/using-home/using-the-home-area/update-and-edit-work-item-home.md)を参照してください。
* イシューのヘッダー内。 詳しくは、[新しいオブジェクトヘッダー](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md)を参照してください。
* イシューリストまたはレポートで、「予定完了日」フィールドがビューに表示される場合。

  詳しくは、[リスト内のイシューを編集](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md)を参照してください。

## Workfront でイシューの予定完了日が自動的に計算される方法

Workfrontが問題の予定完了日を自動的に計算する場合、次の影響を受ける可能性があります。

* 予定開始日

  最初にイシューを作成する際に、イシューのエントリ日と予定開始日を一致させる必要があります。

* プロジェクトの「キューの詳細」セクションで設定されたデフォルト期間。 詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

  デフォルト期間が0日の場合、予定完了日はイシューの予定開始日と一致します。

* プロジェクトスケジュール

自動設定の場合、予定完了日は次の計算に基づいて決定されます。

```
Planned Completion Date = Planned Start Date (or Entry Date + Default Duration
```

**例：**&#x200B;例えば、タスクの開始日が1月14日（金）で、デフォルト期間が5日の場合、プロジェクト スケジュールが1日8時間、月曜日から金曜日の場合、予定完了日は1月21日（金）になります。

次の状況が存在します。

* プロジェクトにスケジュールがない場合、Workfront システムのデフォルトスケジュールが考慮されます。 詳しくは、[スケジュールの概要](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)を参照してください。
* スケジュールが月曜日から金曜日の午前9時から午後1時（1日4時間）で、Workfrontシステムの1日あたりの標準時間が8時間の場合、予定完了日は1月27日になります。

>[!TIP]
>
>Workfrontでは、予定完了日を計算する際に、休日や週末などのスケジュールの例外を考慮しています。


