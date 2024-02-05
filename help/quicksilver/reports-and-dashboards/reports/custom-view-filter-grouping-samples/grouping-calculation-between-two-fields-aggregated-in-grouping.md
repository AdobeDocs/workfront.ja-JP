---
content-type: reference
product-area: reporting;projects
keywords: 計算済み,集計,詳細,表示
navigation-topic: custom-view-filter-and-grouping-samples
title: 「グループ化：1 つのグループ内で複数の計算値を集計した結果を表示します」
description: 列でテキストモードを使用すると、レポートまたはリストのビューで 2 つのフィールド間の計算を表示できます。各行には、レポートまたはリスト内の各オブジェクトの計算が表示されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 97%

---

# グループ化：グループ化での複数の計算済みの値の集計結果を表示する

列でテキストモードを使用すると、レポートまたはリストのビューで 2 つのフィールド間の計算を表示できます。各行には、レポートまたはリスト内の各オブジェクトの計算が表示されます。

例えば、タスクレポートの各タスクの実際の時間数と予定時間数の差を、ワークバランスと呼ばれる 3 番目の列に表示できます。計算データ式について詳しくは、 [計算データ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

複数の計算ビュー項目の集計値をグループ内の同じ列に表示するには、計算値を含む列の `aggregator` 行に計算を追加します。例えば、レポートのグループまたはワークバランス列のリストにあるすべてのタスクのワークバランス時間を集計（合計表示）できます。この記事では、この方法について説明します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>グループ化を変更するためのリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、ビュー、グループ化へのアクセス権を編集して、グループ化を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## グループでの複数の計算値の集計結果を表示

1. タスクレポートに移動し、**アクションをレポート**／**編集**&#x200B;をクリックします。
1. 「**グループ化**」タブで、「**グループを追加**」をクリックし、**レポートをグループ化**／**最初の基準**&#x200B;フィールドに、**プロジェクト名**&#x200B;を入力し始め、リストに表示されたら選択します。

1. 「**列（表示）**」タブで、「**列を追加**」をクリックして、「**この列に表示**」フィールドに&#x200B;**予定時間数**&#x200B;を入力し始め、リストに表示されたら選択します。

   >[!TIP]
   >
   >常に、テキストモードで情報を編集する前に、標準インターフェイスを使用して、できるだけ多くの情報を追加してください。計算に最も近い、または最も多くの情報を含むフィールドを追加します。

1. 「**このカラムの集計方法**」フィールドで、「**SUM**」を選択し、次に「**完了**」をクリックします。
1. 追加した列で「**テキストモードに切り替える**」をクリックします。
1. テキストモードエリアの上にポインタを合わせ、「**クリックしてテキストを編集**」をクリックします。
1. `valuefield ` 行と `aggregator.valuefield` 行を、次のテキストモードの例のようにハイライト表示された行で置き換えます。

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

1. 「**保存して閉じる**」をクリックします。
