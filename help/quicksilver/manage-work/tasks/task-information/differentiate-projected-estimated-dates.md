---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 予定日と推定日の概要
description: 開始可能なタイミングと完了可能なタイミングの間のタスクのタイムラインを表示する日付には、複数のタイプがあります。
author: Alina
feature: Work Management
exl-id: 7cc68fc4-5f79-4ce6-a404-737ea8959ec3
TQID: https://experienceleague.adobe.com/H-lO-an4TrEuwNx-l76JFpACJfyM22g36F3pa3aP6EY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 925
ht-degree: 89%

---

# 予定日と推定日の概要

<!--Audited: 07/2024-->

タスクの開始可能なタイミングと完了可能なタイミングの間のタイムラインを表示する日付には、複数のタイプがあります。 次に、タスクのタイムラインを表示する一部の日付を示します。

* 予定開始日と予定完了日
* 見込み開始日と見込み完了日
* 推定開始日と推定期限
* 実際の開始日と実際の完了日

この記事では、プロジェクトの予定日と見込日の違いについて説明します。

タスクを最初に作成する際は、通常、予定日、見込日、および推測日を一致させる必要があります。 例外がいくつかあります。

Adobe Workfrontのプロジェクト、タスク、イシューの日付について詳しくは、[Workfrontのプロジェクト、タスク、イシューの日付の概要](../../../workfront-basics/navigate-workfront/workfront-navigation/definitions-pti-dates.md)を参照してください。

## 予定日の概要

予定日は、プロジェクト所有者がタスクの開始日と終了日として定義する日付です。 自分またはプロジェクト所有者は、タスクの予定日を手動で変更できます。

## 実際の日付の概要

タスクを最初に作成したときは、まだ開始も完了もしていないので、実際の日付は表示されません。

## 予定日と推定日の概要

プロジェクトの期間中、見込日と推測日は、タスクの実際の開始と終了に影響を与える要因を考慮に入れるため、プロジェクトの実際の状況に合わせて設定されます。 これにより、予定日から変更されます。

タスクの見込日と推測日を使用する際は、次の点に注意してください。

* タスクの見込日も推定日も、手動で変更することはできません。 どちらも Adobe Workfront で計算されます。
* タスクを作成する場合、見込日と推測日は一致させる必要があり、タスクを開始または終了できる実際の時間が示されます。\
  タスクに対して行った一部の更新は、見込日および推測日の値に直接影響します。

  例えば、ユーザーがタスクを開始または完了した場合、タスクには実際の開始日と完了日が表示され、タスクの見込日と推測日に影響を与えます。 また、タスクの担当者がコミット日を変更すると、この日付はタスクの見込日に影響します。

## 見込日と推測日の違い

見込日と推測日の違いは次のとおりです。

* 見込日は、ユーザーがタスクを次のようにアップデートした場合に影響を受けます。

   * 固定タスクの制約を追加して制約の指定日を追加する
   * コミット日の追加

* 推測日では、特定の時点でのタスクの実際の進捗状況のみが考慮されます。

**例：**&#x200B;予定開始日が9月20日、予定完了日が9月24日で、制約の指定日に完了する必要があるタスクの場合、見込み完了日は9月24日です。 このタスクの期間は 4 日です。

推定完了日は、タスクに関する作業の現在の進捗状況に基づいて計算されます。 したがって、今日が 9月23日で、タスクがまだ開始されていない場合、推定完了日は 9月27日（今日作業が開始されると仮定して、4 日後に完了する）になります。

タスクの完了率が今日 50％の場合、推定完了日は 9月25日です（タスクの期間の半分となる 2 日後に完了する）。


### タスクで見込日がいつ更新されるかを把握する {#understand-when-projected-dates-update-on-tasks}

予測日は、他のタスク日と一致するか、タスクの実際の進捗状況を考慮したWorkfrontによる計算です。

次のリストには、タスクの実際の状況に応じて、プロジェクトの期間中にタスクの見込日が変更された場合のシナリオが表示されています。

* タスクが「完了」とマークされた場合：

  `Projected Dates = Estimated Dates = Actual Dates`

* タスクの開始日が実際の日付の場合：

  `Projected Start Date = Estimated Start Date = Actual Start Date`

* タスクに実際の開始日が設定されていないが、将来の予定開始日に対して強制的に制約が適用される（指定日に開始）場合：

  `Projected Start Date = Constraint Date`

  制約の指定日について詳しくは、[Adobe Workfront の用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

* タスクに実際の開始日が設定されておらず、タスクに強制された制約の指定日が設定されていない場合：

  `Projected Start Date = the next available date in the future that falls within working schedule`

* 担当者がコミット日を更新した場合：

  `Projected Completion Date = Commit Date`

  コミット日に関して詳しくは、[コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)を参照してください。

* タスクに更新されたコミット日がなく、タスクに将来の予定完了日に対する強制された制約（指定日に終了）がある場合：

  `Projected Completion Date = Constraint Date`

* タスクに更新されたコミット日や将来の日付で強制された制約の指定日がない、または、過去の日付で制約の指定日がある場合：

  `Projected Completion Date = system calculation for the Completion Date based on the current progress and the work left to be done`

### タスクで推定日が更新されるタイミングについて {#understand-when-the-estimated-dates-update-on-tasks}

見込み日に関する前述のシナリオと比較すると、推定日は、制約やコミット日に関係なく、タスクが開始または完了するタイミングを Workfront が実際に分析した結果を反映します。

## タスクのタイムラインに影響を与えるもの

次に、タスクの実際のタイムラインに影響を与える可能性のあるものの例を示します。

* 予定日と現在の日付に関するタスク進行状況
* 今までのタスクの完了率
* 先行タスクの関係
* 先行タスクの進行状況
* ユーザー割り当て

  >[!NOTE]
  >
  >ユーザー割り当てが、タスクを完了できるスピードに影響を与える場合、タスクの予定完了日に影響を与える可能性があります。 例えば、タスクの期間タイプが「残存作業時間の優先」の場合は、担当者を追加することで、タスクを早い段階で完了させることができます。 その結果、見込完了日が変更されます。
