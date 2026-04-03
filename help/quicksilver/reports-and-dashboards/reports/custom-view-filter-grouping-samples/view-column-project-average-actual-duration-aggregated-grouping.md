---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示とグループ化：グループ化の平均で集計されたプロジェクトの実際の期間を表示します
description: プロジェクトレポートに以下の列を追加して、グループ化内の平均として集計された実際の期間を表示できます。
author: Courtney
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 42%

---

# ビューおよびグループ化：プロジェクトの実際の期間をグループ内の平均値で集計して表示

<!--Audited: 11/2024-->

プロジェクトビューに次の列を追加すると、グループ化で集計された実際の期間を平均として表示できます。

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>コントリビューターまたはフィルターを変更するリクエスト </p>
   <p>レポートを修正する標準または計画</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループ化の平均で集計されたプロジェクトの実際の期間を表示します

この列をプロジェクトビューに追加するには、以下のように行います。

1. プロジェクトリストを見る。
1. （必須） プロジェクトの実際の期間の集計平均値を表示するには、グループ化をプロジェクトリストに追加する必要があります。\
   グループ化の作成について詳しくは、Adobe Workfront[の「](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md) グループ化の概要」を参照してください。
1. **ビュー** ドロップダウンメニューを展開し、**ビューをカスタマイズ**&#x200B;を選択します。
1. 「**列を追加**」をクリックします。
1. 「**テキストモードに切り替え**」をクリックし、「**テキストモードを編集**」をクリックします。
1. 「**テキストモードを編集**」ボックス内のすべてのテキストを削除し、次のコードに置き換えます。

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. 「**完了**」をクリックし、「**ビューを保存**」をクリックします。
1. （オプション）ビュー名を更新し、**ビューを保存**&#x200B;をクリックします。
