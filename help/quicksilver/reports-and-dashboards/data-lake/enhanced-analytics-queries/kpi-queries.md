---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: KPI クエリ
description: Analytics クエリの強化機能
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: eccecaece64b78aa19444407b182ea80b2115a63
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 73%

---


# KPI クエリ

この記事のクエリを使用して、Enhanced Analytics と同様のデータビジュアライゼーションを作成できます。

>[!IMPORTANT]
>
>クエリは、Enhanced Analytics で表示される結果と同様の結果を生成しますが、完全には一致しない場合があります。


## 前提条件

開始する前に、

1. Business Intelligence（BI）ツールとの接続を確立します。
   1. [Snowflakeのリーダーアカウントまたは接続を作成する](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [Workfront Data Connect への接続の確立](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

接続を確立したら、この記事のクエリを使用してデータを抽出および視覚化できます。

## 完了したプロジェクト

「完了したプロジェクト」KPI は、フィルターした期間内に完了したプロジェクトの数と、前の期間以降に増加または減少した割合を示します。これらの数値の下に、前の期間に完了したプロジェクトの数と、前の期間の日数が表示されます。

![KPI プロジェクト完了 ](assets/kpi-projects-completed-350x182.png)

### クエリ

```
WITH completedProjectsInRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2025-01-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2025-01-31' 
), completedProjectsPreviousRange as ( 
SELECT COUNT(t0.PROJECTID) as PROJECT_COUNT FROM PROJECTS_CURRENT t0 
WHERE t0.ACTUALCOMPLETIONDATE >= '2024-12-01' 
AND t0.ACTUALCOMPLETIONDATE <= '2024-12-31' 
), rawChange as ( 
SELECT (a.PROJECT_COUNT - b.PROJECT_COUNT) as CHANGE_FROM_PREVIOUS_PERIOD FROM completedProjectsInRange a, completedProjectsPreviousRange b 
), percentChange as ( 
SELECT  
CASE 
WHEN a.PROJECT_COUNT = b.PROJECT_COUNT THEN 0.00 
WHEN b.PROJECT_COUNT > 0 THEN ((a.PROJECT_COUNT - b.PROJECT_COUNT) / b.PROJECT_COUNT * 100) 
END AS PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b 
) 
SELECT 
a.PROJECT_COUNT, 
b.PROJECT_COUNT as PREVIOUS_PROJECT_COUNT, 
c.CHANGE_FROM_PREVIOUS_PERIOD, 
d.PERCENT_CHANGE_FROM_PREVIOUS_PERIOD 
FROM completedProjectsInRange a, completedProjectsPreviousRange b, rawChange c, 
percentChange d
```

## 時間どおりに完了したプロジェクト

「時間どおりに完了したプロジェクト」KPI は、フィルターした期間内に時間どおり完了したプロジェクトの数と、前の期間以降に増加または減少した割合を示します。これらの数値の下に、前の期間で時間通りに完了したプロジェクトの割合と、前の期間の日数が表示されます。

![KPI プロジェクトが時間通りに完了しました ](assets/kpi-projects-completed-on-time-350x180.png)

## 平均プロジェクト期間

平均プロジェクト期間 KPI は、フィルターした期間内に実際の終了日があるプロジェクトの平均完了時間（日、週、または年）と、前の期間からの割合の増減を示します。これらの数値の下に、前の期間の実際の終了日を持つプロジェクトの平均完了時間と、前の期間の日数が表示されます。

![KPI 平均プロジェクト期間 ](assets/kpi-avg.-project-duration-350x168.png)

## プロジェクト当たりの平均タスク数

プロジェクトごとの平均タスク数 KPI は、フィルターした期間内にプロジェクトに割り当てられたタスクの平均数と、前の期間以降に増加または減少した割合を示します。これらの数値の下に、前の期間のプロジェクトに割り当てられたタスクの平均数と、前の期間の日数が表示されます。

![ プロジェクトあたりの KPI 平均タスク数 ](assets/kpi-average-tasks-per-project-350x179.png)