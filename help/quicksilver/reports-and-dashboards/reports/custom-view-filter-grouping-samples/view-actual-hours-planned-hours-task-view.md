---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：タスク・ビューの同じ列の「計画時間に対する実績時間」'
description: このタスクビューでは、各タスクに予定された時間に対して、タスクに記録された実際の時間数が表示されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 表示：タスクビューの同じ列の計画時間に対する実績時間

このタスクビューでは、各タスクに予定された時間に対して、タスクに記録された実際の時間数が表示されます。

![actual_vs_planned_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

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
   <td> <p>ビューの変更をリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスク・ビューでの計画時間に対する実績時間の表示

このビューを適用するには：

1. タスクのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. 内&#x200B;**列のプレビュー** 領域を選択し、1 つ以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、 **テキストモードに切り替え**.
1. テキストモード領域の上にマウスを移動し、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=assignments<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=実績/計画時間<br>column.2.linkedname=direct<br>column.2.namekey=actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=Hours 差異<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. クリック **ビューを保存**.
