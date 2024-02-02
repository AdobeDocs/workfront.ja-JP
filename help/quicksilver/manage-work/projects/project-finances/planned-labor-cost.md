---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 予定労力コストの計算
description: プロジェクトでの作業を計画する際、Adobe Workfront は、1 時間当たりのコストの値に基づいて、この作業に割り当てられた役割およびユーザーの予定労力コストを計算します。
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '309'
ht-degree: 100%

---

# 予定労力コストの計算

プロジェクトでの作業を計画する際、Adobe Workfront は、1 時間当たりのコストの値に基づいて、この作業に割り当てられた役割およびユーザーの予定労力コストを計算します。

プロジェクトの予定労力コストは、プロジェクトの作業を完了するために割り当てられた担当業務やユーザーに関連するコストと、それぞれの役割やユーザーがその作業を完了するためにかかると考えられる予定時間数との間の計算です。

## 予定労力コストの概要

プロジェクトの&#x200B;**予定労力コスト**&#x200B;は、プロジェクトのすべてのタスクの予定労力コストをすべて加算して計算されます。

>[!TIP]
>
>イシューやプロジェクト自体に関連する予定労力コストはありません。

Workfront は、次の式を使用してプロジェクトの予定労力コストを計算します。

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

タスクの予定労力コストは、次の項目に基づいて計算されます。

* タスク上のリソースの数およびタスクに対する個々の割り当て
* タスクのコストタイプ。

タスクの予定労力コストは、次の式を使用して計算されます。

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

Workfront がタスクの割り当てとコストタイプに応じて、タスクの予定労力コストを計算する方法について詳しくは、[コストの追跡](../../../manage-work/projects/project-finances/track-costs.md)の記事にある「個々のタスクのコストタイプの変更」の節を参照してください。

## 予定労力コストの検索

プロジェクトの予定労力コストは、Workfront の次のエリアに表示されます。

* プロジェクトレポート
* プロジェクトのリスト
* 時系列で追跡できるベースラインレポート
* API 経由

レポートの作成および Workfront API の使用について詳しくは、次の記事を参照してください。

* [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API の基本](../../../wf-api/general/api-basics.md)
