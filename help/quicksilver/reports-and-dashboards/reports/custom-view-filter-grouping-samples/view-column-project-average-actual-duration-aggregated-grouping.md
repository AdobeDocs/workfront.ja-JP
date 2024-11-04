---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「表示とグループ化：グループ化の平均で集計したプロジェクトの実際の期間を表示する」
description: プロジェクトレポートに以下の列を追加して、グループ化内の平均として集計された実際の期間を表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 37%

---

# 表示とグループ化：グループ化の平均で集計したプロジェクトの実際の期間を表示します

<!--Audited: 11/2024-->

プロジェクト ビューで次の列を追加すると、グループの平均として集計された実際の期間を表示できます。

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
    <p>新規：</p>
   <ul><li><p>フィルターを変更するコントリビューター </p></li>
   <li><p>レポートを変更する場合は Standard</p></li> </ul>

<p>現在：</p>
   <ul><li><p>フィルターを変更する場合は「要求」 </p></li>
   <li><p>レポートを変更するためのプラン</p></li> </ul></td> 
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

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 平均で集計したプロジェクトの実際の期間をグループ化で表示します

この列をプロジェクトビューに追加するには、以下のように行います。

1. プロジェクトリストに移動します。
1. （必須） プロジェクトの実際の期間の集計平均値を表示するには、プロジェクトリストにグループ化を追加する必要があります。\
   グループ化の作成について詳しくは、[Adobe Workfrontのグループ化の概要 ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md) を参照してください。
1. **表示** ドロップダウンメニューを展開し、「**表示をカスタマイズ**」を選択します。
1. 「**列を追加**」をクリックします。
1. **テキストモードに切り替え** をクリックしてから、**テキストモードを編集** をクリックします。
1. 「**テキストモードを編集**」ボックスのすべてのテキストを削除し、次のコードに置き換えます。

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

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。
1. （オプション）ビュー名を更新し、「**ビューを保存**」をクリックします。
