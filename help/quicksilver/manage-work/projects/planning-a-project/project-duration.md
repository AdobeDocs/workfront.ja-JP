---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクト期間の概要
description: Adobe Workfront は、最も早いタスクの開始日と最も遅いタスクの完了日を考慮に入れてプロジェクトの期間を計算し、この 2 つの日付の間の日数をカウントします。
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
TQID: https://experienceleague.adobe.com/1j0nj2W5f7FtgIk46G3ePFA-zwt7VAyV9fQWKm2kZJ4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 254
ht-degree: 96%

---

# プロジェクト期間の概要

Adobe Workfront は、最も早いタスクの開始日と最も遅いタスクの完了日を考慮に入れてプロジェクトの期間を計算し、この 2 つの日付の間の日数をカウントします。

## プロジェクト期間

プロジェクトの期間は、次の数式で計算されます。

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>プロジェクトのイシューの期間は、プロジェクトの期間には影響しません。

プロジェクトの期間は、プロジェクトに関連付けられたスケジュールや、タスクに割り当てられたユーザーに基づいた、タスクの 2 つの日付の間の日数をカウントします。 Workfront が期間の計算に使用するスケジュールについて詳しくは、[スケジュールの概要](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)を参照してください。

## プロジェクト期間のタイプ

プロジェクト期間には 2 種類があり、Workfront では次のような数式を使用して計算します。

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

## プロジェクト期間の検索

Workfront の次のエリアで、プロジェクトの予定期間と実際の期間を見つけることができます。

* . プロジェクト詳細エリアの「概要」セクション。

  プロジェクトの「概要」サブタブについて詳しくは、[プロジェクトの概要エリアで情報を管理](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)を参照してください。

* プロジェクトレポートで、「期間」フィールドまたは「実際の期間」フィールドをレポートに含めます。

  レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)の記事を参照してください。
