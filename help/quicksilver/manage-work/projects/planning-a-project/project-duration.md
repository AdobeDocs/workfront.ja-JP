---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクト期間の概要
description: Adobe Workfrontは、最も早いタスクの開始日と最も遅いタスクの完了日を考慮に入れてプロジェクトの期間を計算し、2 つの日付の間の日数をカウントします。
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 2%

---

# プロジェクト期間の概要

Adobe Workfrontは、最も早いタスクの開始日と最も遅いタスクの完了日を考慮に入れてプロジェクトの期間を計算し、2 つの日付の間の日数をカウントします。

## プロジェクト期間

プロジェクトの期間は、次の数式で計算されます。

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>プロジェクトの問題の期間は、プロジェクトの期間には影響しません。

プロジェクトの期間は、プロジェクトに関連付けられたスケジュールまたはタスクに割り当てられたユーザーに基づいて、2 つのタスクの日付の間の日数を数えます。 Workfrontが期間の計算に使用するスケジュールについて詳しくは、 [スケジュールの概要](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## プロジェクト期間のタイプ

プロジェクト期間には 2 種類があり、Workfrontがそれらを計算する数式があります。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **予定期間**: 

   ```
   Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
   ```

* **実際の期間**: 

   ```
   Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
   ```

## プロジェクト期間を見つけます。

Workfrontの次の領域で、計画期間と実際の期間を検索できます。

* .「プロジェクトの詳細」領域の「概要」セクション。

   プロジェクトの「概要」サブタブの詳細については、「 [プロジェクトの概要領域で情報を管理します。](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* プロジェクトレポートで、「期間」フィールドまたは「実際の期間」フィールドをレポートに含めます。

   レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
