---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：前任者詳細'
description: このタスクビューは、コレクションビューを使用してタスクの先行タスクの詳細を表示します。 コレクションビューでは、「1 対多」関係にあるオブジェクトに関する情報を表示できます。 この場合、各タスク（1 つ）に複数の先行タスク（多数）を設定できます。 タスクの名前と、先行タスクの名前、先行タスクのプロジェクト名、先行タスクの計画完了日、先行タスクのステータスが表示されます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# 表示：先行者の詳細

このタスクビューは、コレクションビューを使用してタスクの先行タスクの詳細を表示します。 コレクションビューでは、「1 対多」関係にあるオブジェクトに関する情報を表示できます。 この場合、各タスク（1 つ）に複数の先行タスク（多数）を設定できます。 タスクの名前と、先行タスクの名前、先行タスクのプロジェクト名、先行タスクの計画完了日、先行タスクのステータスが表示されます。

レポートでコレクションを参照する方法について詳しくは、 [レポート内のコレクションの参照](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## 先行タスクの詳細を表示

1. タスクのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. 内&#x200B;**列のプレビュー** 領域を選択し、1 つ以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、 **テキストモードに切り替え**.
1. テキストモード領域の上にマウスを移動し、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Predecessors の番号と名前<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(predecessors).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({predecoder}.{taskNumber}、' - ',{predecessor}。{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Predecessors プロジェクト名<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(predecessors).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={predecoder}。{プロジェクト}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Predecessors 完了日<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(predecessors).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={predecoder}。{plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Predecessors ステータス<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(predecessors).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecoder}。{status}<br>column.4.valueformat=HTML</pre>

1. クリック **ビューを保存**.
