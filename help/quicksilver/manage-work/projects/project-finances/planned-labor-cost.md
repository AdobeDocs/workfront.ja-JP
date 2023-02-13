---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 計画労務費の計算
description: プロジェクトでの作業を計画する際、Adobe Workfrontは、「時間当たりの原価」の値に基づいて、この作業に割り当てられた役割およびユーザーの計画労務費を計算します。
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 計画労務費の計算

プロジェクトでの作業を計画する際、Adobe Workfrontは、「時間当たりの原価」の値に基づいて、この作業に割り当てられた役割およびユーザーの計画労務費を計算します。

プロジェクトの計画労務費は、ジョブの役割に関連付けられた原価、またはプロジェクトの作業を完了するために割り当てられたユーザーと、各役割またはユーザーが作業を完了するのに要する予定時間（計画時間）との間の計算です。

## 計画労務費の概要

この **計画労務費** プロジェクトの計算には、プロジェクトのすべてのタスクの計画労務費をすべて追加します。

>[!TIP]
>
>問題やプロジェクト自体に関連する計画労務費はありません。

Workfrontは、次の式を使用して、プロジェクトの計画労務費を計算します。

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

タスク計画労務費は、次の項目に基づいて計算されます。

* タスク上のリソースの数とタスクに対する個々の割り当て
* タスクのコストタイプ。

「タスク計画労務費」は、次の式を使用して計算されます。

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Workfrontがタスクの計画労務費を計算する方法の詳細は、タスクの割り当てとコスト・タイプに応じて、この記事の「個々のタスクの原価タイプの変更」の項を参照してください [コストの追跡](../../../manage-work/projects/project-finances/track-costs.md).

## 計画労務費の検索

プロジェクトの計画労務費は、Workfrontの次の領域にあります。

* プロジェクトレポート
* プロジェクトのリスト
* 時間の経過に伴って追跡できるベースラインレポート
* API を使用する

レポートの作成とWorkfront API の使用について詳しくは、次の記事を参照してください。

* [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API の基本](../../../wf-api/general/api-basics.md)
