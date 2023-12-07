---
content-type: reference
product-area: reporting;projects
keywords: 計算済み，集計，詳細，表示
navigation-topic: custom-view-filter-and-grouping-samples
title: 'グループ化： 1 つのグループ内で複数の計算値を集計した結果を表示します'
description: 列でテキストモードを使用すると、レポートまたはリストのビューで 2 つのフィールド間の計算を表示できます。 各行には、レポートまたはリスト内の各オブジェクトの計算が表示されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# グループ化：グループ化での複数の計算値の集計結果の表示

列でテキストモードを使用すると、レポートまたはリストのビューで 2 つのフィールド間の計算を表示できます。 各行には、レポートまたはリスト内の各オブジェクトの計算が表示されます。

たとえば、タスクレポートの各タスクの実績時間と計画時間の差を、3 番目の列 (Work Balance) に表示できます。 計算データ式について詳しくは、 [計算データ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

グループの 1 つの列に複数の計算ビュー項目の集計値を表示するには、 `aggregator` 計算値を含む列の行。 たとえば、レポートのグループ化に含まれるすべてのタスクの [ 作業時間の合計 ] または [ 作業時間の合計 ] 列の一覧を集計（表示）できます。 この記事では、この方法について説明します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>グループ化を変更するリクエスト </p>
   <p>レポートを変更する計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してグループ化を変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## グループ化での複数の計算値の集計結果の表示

1. タスクレポートに移動し、 **レポートのアクション** > **編集**.
1. Adobe Analytics の **グループ化** タブ、クリック **グループを追加**&#x200B;入力を開始します。 **プロジェクト名** （内） **レポートをグループ化** > **最初のユーザー** フィールドに値を入力し、リストに表示されるときに選択します。

1. Adobe Analytics の **列（表示）** タブ、クリック **列を追加**&#x200B;その後、入力を開始 **予定時間** （内） **この列に表示** フィールドに値を入力し、リストに表示されるときに選択します。

   >[!TIP]
   >
   >テキストモードで情報を編集する前に、必ず標準インターフェイスを使用して情報の追加を開始してください。 計算に最も近い、または最も多くの情報を含むフィールドを追加します。

1. Adobe Analytics の **この列の要約基準** フィールド、選択 **合計**&#x200B;を選択し、次に **完了**.
1. クリック **テキストモードに切り替え** をクリックします。
1. テキストモード領域の上にマウスポインターを置いて、 **クリックしてテキストを編集**.
1. 次を `valuefield ` そして `aggregator.valuefield` 次のテキストモードの例でハイライト表示された行を含む行：

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
   >グループ化の集計値を取得して「計画時間」フィールドと「実績時間」フィールドの集計された差異を表示するには、同じ式を `aggregator.valuefield` 行。 The `aggregator.displayformat` 「Planned Hours」列にを使用すると、分が時間に変換されます。 「計画時間」フィールドはプレースホルダーとして使用されたので、この行を調整する必要はありません。
   >
   >
   >The `minutesAsHoursString` の定義 `aggregator.displayformat` 線は、各フィールドを `valueexpression` を参照してください。 この `aggregator.valuefield=workRequired` 次になります。 `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. クリック **保存して閉じる**.
