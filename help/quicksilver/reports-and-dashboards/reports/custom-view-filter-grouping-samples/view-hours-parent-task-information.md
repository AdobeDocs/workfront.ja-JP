---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「表示：親タスク情報を含む時間」
description: この時間ビューには、時間が記録されたタスク名とその親タスク名が表示されます。
author: Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 76%

---

# 表示：親タスクの情報とともに時間数を表示

<!--Audited: 11/2024-->

この時間ビューには、時間が記録されたタスク名とその親タスク名が表示されます。

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：<ul><li>ビューを変更する場合は Contributor</li><li>レポートを変更する場合は Standard</li></ul></p><p>または</p>現在：<ul><li>表示の変更をリクエスト</li><li>レポートを変更するためのプラン</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 親タスクの情報とともに時間数を表示

1. 時間のリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューから、**新規表示**&#x200B;を選択します。

1. **列プレビュー** 領域で、1 列以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、「**テキストモードに切り替え**」をクリックします。
1. **テキストモードを編集** をクリックします。
1. 「**テキストモードを編集**」ボックスで検索したテキストを削除し、次のコードに置き換えます。



   ```
   column.0.aggregator.displayformat=doubleAsString
   column.0.aggregator.function=SUM
   column.0.aggregator.namekey=hours
   column.0.aggregator.valuefield=hours
   column.0.aggregator.valueformat=doubleAsDouble
   column.0.descriptionkey=hours
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=doubleAsDouble(hours)
   column.0.namekey=hours.abbr
   column.0.querysort=hours
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=hours
   column.0.valueformat=doubleAsString
   column.0.width=150
   column.1.descriptionkey=task
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=task:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=task:objCode
   column.1.link.valueformat=val
   column.1.linkedname=task
   column.1.listsort=nested(task).string(name)
   column.1.namekey=task
   column.1.querysort=task:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=task:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Parent Task Name
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=task:parent:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=task:objCode
   column.2.link.valueformat=val
   column.2.linkedname=task
   column.2.listsort=nested(task:parent).string(name)
   column.2.name=Parent Task Name
   column.2.querysort=task:parent:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=task:parent:name
   column.2.valueformat=HTML
   column.2.width=150
   ```

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。

