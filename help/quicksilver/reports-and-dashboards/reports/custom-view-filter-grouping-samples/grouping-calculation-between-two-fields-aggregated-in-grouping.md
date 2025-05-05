---
content-type: reference
product-area: reporting;projects
keywords: 計算済み,集計,詳細,表示
navigation-topic: custom-view-filter-and-grouping-samples
title: 「グループ化：グループ化で複数の計算値を集計した結果を表示」
description: 列でテキストモードを使用すると、レポートまたはリストのビューで 2 つのフィールド間の計算を表示できます。各行には、レポートまたはリスト内の各オブジェクトの計算が表示されます。
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 81%

---

# グループ化：グループ化での複数の計算済みの値の集計結果を表示する

<!--Audited: 10/2024-->

列でテキストモードを使用すると、レポートまたはリストのビューで 2 つのフィールド間の計算を表示できます。各行には、レポートまたはリスト内の各オブジェクトの計算が表示されます。

例えば、タスクレポートの各タスクの実際の時間数と予定時間数の差を、ワークバランスと呼ばれる 3 番目の列に表示できます。計算されたデータ式について詳しくは、[計算されたデータ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)を参照してください。

複数の計算ビュー項目の集計値をグループ内の同じ列に表示するには、計算値を含む列の `aggregator` 行に計算を追加します。例えば、レポートのグループまたはワークバランス列のリストにあるすべてのタスクのワークバランス時間を集計（合計表示）できます。この記事では、この方法について説明します。

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

## グループでの複数の計算値の集計結果を表示

1. タスクレポートに移動し、**アクションをレポート**／**編集**&#x200B;をクリックします。
1. 「**グループ化**」タブで「**グループ化を追加**」をクリックし、「**グループ化の条件**」フィールドに **プロジェクト名** と入力し始めると、リストに表示される **プロジェクト > 名前** が選択されます。

1. 「**列（表示）**」タブで、「**列を追加**」をクリックして、「**この列に表示**」フィールドに&#x200B;**予定時間数**&#x200B;を入力し始め、リストに表示されたら選択します。

   >[!TIP]
   >
   >常に、テキストモードで情報を編集する前に、標準インターフェイスを使用して、できるだけ多くの情報を追加してください。計算に最も近い、または最も多くの情報を含むフィールドを追加します。

1. **この列の集計基準** フィールドで、&lbrack; 合計 **を選択し** す。
1. 追加した列の「**テキストモードに切り替え**」をクリックし、「**テキストモードを編集**」をクリックします。
1. ボックス内のテキストを次のテキストモードの例に置き換えます。

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >グループの集計値を取得して「予定時間数」フィールドと「実際の時間数」フィールドの集計された差異を表示するには、同じ式を `aggregator.valuefield` 行に入力します。予定時間数の列に `aggregator.displayformat` を使用すると、分が時間に変換されます。「予定時間数」フィールドはプレースホルダーとして使用されたので、この行を調整する必要はありません。
   >
   >
   >`aggregator.displayformat` 行の `minutesAsHoursString` 定義は、`valueexpression` で行われたように各フィールドを 60 で割って結果を出す必要がないことを意味します。ここでは、`aggregator.valuefield=workRequired` は `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2` になります。
1. 「**完了**」をクリックします。
1. 「**保存して閉じる**」をクリックします。
